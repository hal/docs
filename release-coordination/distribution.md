# Distribution

This chapter describes the different distribution models for the HAL management console. Basically there are two ways to use the console:
   
## Bundled with WildFly

Each WildFly installation ships with a specific version of the HAL management console. This model applies to all versions of HAL prior to [2.6.5.Final](versions/2.6.5.Final.md). To find out which version of HAL relates to which WildFly or EAP version, take a look at the [released versions](versions/index.html) page. 

## Standalone Console

Starting with HAL [2.6.5.Final](versions/2.6.5.Final.md) the console is available as a standalone web application. These standalone consoles are served from the HAL build proxy living at: http://access-halproject.rhcloud.com/. The HAL build proxy provides access to both released HAL versions and snapshots. 

When the standalone console starts, the user can manage a list of management interfaces and chooses the one he likes to connect to. The configuration is stored in the browsers local storage, so it's available the next time the console is launched. 

Using this kind of setup has several advantages:

- We can update the console independently from the rest of the WildFly code base
- We can deploy the console to various (web)app stores like Firefox Marketplace or Chrome Web Store
- We can have different console versions with different feature sets (nightly, beta, stable)
- Using one console you can connect to different server instances running different setups (development, staging, production)

In order to make this work, we need a way to solve restrictions that come with the [same origin policy](http://en.wikipedia.org/wiki/Same_origin_policy) (SOP). Such restrictions arise when the console is served from origin A, but talks to the management interface on origin B. Starting with WildFly 9, the http interface supports the configuration of so-called allowed origins. That is a list of URLs which are allowed to connect to the http interface (see http://en.wikipedia.org/wiki/Cross-origin_resource_sharing for more details).

### CORS Setup in WildFly 9

Use the following CLI commands to add `http://access-halproject.rhcloud.com` to the list of allowed origins:

- standalone mode: 

        /core-service=management/management-interface=http-interface:list-add(name=allowed-origins,value=http://access-halproject.rhcloud.com)
        reload
    
- domain mode:

        /host=master/core-service=management/management-interface=http-interface:list-add(name=allowed-origins,value=http://access-halproject.rhcloud.com)
        reload --host=master
