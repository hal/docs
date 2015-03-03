# Distribution

This chapter describes the different distribution models for the HAL management console. Basically there are two ways to use the console:
   
## Bundled with WildFly

Each WildFly installation ships with a specific version of the HAL management console. To find out which version of HAL relates to which WildFly version, take a look at the [released versions](versions/index.html) page. 

## Standalone Console

Starting with HAL [2.6.5.Final](versions/2.6.5.Final.md) and WildFly 9 the console is also available as a standalone web application. These standalone consoles are served from the HAL build proxy living at http://access-halproject.rhcloud.com/. The HAL build proxy provides access to both released HAL versions and snapshots. 

When a standalone console starts, the user can manage a list of management interfaces and chooses the one he likes to connect to. The configuration is stored in the browsers local storage, so it's available the next time the console is launched. 

Using this kind of setup has several advantages:

- We can update the console independently from the rest of the WildFly code base
- We can have different console versions with different feature sets (nightly, beta, stable)
- Using one console you can connect to different server instances running different setups (development, staging, production)

In order to make this work, restrictions that come with the [same origin policy](http://en.wikipedia.org/wiki/Same_origin_policy) (SOP) need to be resolved. Such restrictions arise when the console is served from origin A, but talks to the management interface on origin B. Starting with WildFly 9, the http interface supports the configuration of so-called allowed origins. That is a list of URLs which are allowed to access to the http interface (see http://en.wikipedia.org/wiki/Cross-origin_resource_sharing for more details).

### Allowed Origins Setup

Use the following CLI commands to add `http://access-halproject.rhcloud.com` to the list of allowed origins:

- standalone mode: 

        /core-service=management/management-interface=http-interface:list-add(name=allowed-origins,value=http://access-halproject.rhcloud.com)
        reload
    
- domain mode:

        /host=master/core-service=management/management-interface=http-interface:list-add(name=allowed-origins,value=http://access-halproject.rhcloud.com)
        reload --host=master

Once you've setup the list of allowed origins, you can choose a console version from http://access-halproject.rhcloud.com to manage your WildFly instance. Say you want access your local WildFly instance with the HAL management console 2.6.5.Final. Follow these steps in order to do so:
 
1. Point your browser to https://access-halproject.rhcloud.com/release/2.6.5.Final
1. Click 'Add' to configure a management endpoint

  ![Connect to Management Interface](/assets/images/bootstrap_server_select_0.png)
