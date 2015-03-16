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

### BYO (Build Your Own)

Instead using the prebuilt proxy on OpenShift, you can also checkout the source code and run your own build proxy:
 
1. Clone the registry from https://github.com/hal/mvn-repo-server
1. Build the proxy with Maven: `mvn clean package` (requires Java 8)
1. Start the proxy: `java -jar target/server-jar-with-dependencies.jar` (by default port 8080 is used)
1. Open http://localhost:8080/

Don't forget to add http://localhost:8080 as allowed origin (see below).

### Allowed Origins Setup

Use the following CLI commands to add `http://access-halproject.rhcloud.com` to the list of allowed origins:

- standalone mode: 

        /core-service=management/management-interface=http-interface:list-add(name=allowed-origins,value=http://access-halproject.rhcloud.com)
        reload
    
- domain mode:

        /host=master/core-service=management/management-interface=http-interface:list-add(name=allowed-origins,value=http://access-halproject.rhcloud.com)
        reload --host=master

Once you've setup the list of allowed origins, you can choose a console version from http://access-halproject.rhcloud.com to manage your WildFly instance. Say you want access your local WildFly instance with the HAL management console 2.6.5.Final. Follow these steps to configure your local WildFly instance:
 
1. Point your browser to http://access-halproject.rhcloud.com/release/2.6.5.Final

1. Click 'Add' to configure a management endpoint.

  ![Connect to Management Interface](/assets/images/bootstrap_server_select_0.png)

1. Add the hostname and port of you local WildFly instance. You can verify your settings using 'Ping'.

  ![Connect to Management Interface](/assets/images/bootstrap_server_select_1.png)

1. Click 'Connect' to finish. 

  ![Connect to Management Interface](/assets/images/bootstrap_server_select_2.png)

You can use an existing configuration using the `connect` query parameter. For the above example this url is a shortcut and will skip the bootstrap dialogs: http://access-halproject.rhcloud.com/2.6.5.Final/App.html?connect=local

### Limitations and Known Problems

When using the standalone console there are some pitfalls and preconditions you should be aware of:
 
- The standalone console can only connect to WildFly 9.x and above.
- Make sure to configure the allowed origins before connecting from the standalone console.
- Don't use different schemes (https and http) for the standalone console and the WildFly instance you want to connect to.
- In rare cases it might be necessary to clear the cache or use the browser's private mode when switching between different WildFly instances. 
