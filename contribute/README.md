# Getting Started 

## Prerequisites

In order to work on the console you a need running [WildFly][1] instance on your local host. You can download it from the [Wildfly homepage][2].

You can run WildFly in either the 'domain' or 'standalone' mode.

## Introduction to GWT

If you are not familiar with GWT, I would recommend you read at least [the introduction documents][3].

## The GWTP Framework

The web console relies on the [GWTP framework][4] that provides the core design patterns (MVP), navigation handling and IOC support.

It's useful to understand the [building blocks][5] before you dive into the code base.

## Build and Deploy

### Running in hosted mode

1. Make sure WildFly is started
1. Make sure you build the top level module first (mvn -Pdev clean install).
1. cd 'build/app'

You need to add user with WildFly add-user.sh script.

Start the GWT shell with

    mvn gwt:<run|debug>

When the hosted browser is started, it's enough to hit the 'refresh' button to recompile and verify changes. You can get the OOPHM Plugin, required for attaching your browser to the hosted mode execution on the [GWT Plugin homepage][6].

### Running in web mode

    cd build/app
    mvn package

Produces a war file in target/*-resources.jar, which needs to be deployed as a WildFly Module.

### EAP Build Profile

To run a customised EAP build (L&amp;F) follow these steps:

1. Create a dedicated version number (i.e. 1.0.0.EAP.CR2) 
1. Rebuild with the EAP profile enabled:

        mvn -Peap clean install

### Development Profile

Due to the increased number of permutations (additional languages) the full compile times have increased quiet drastically. To work around this problem during development, we've added a development build profile that restricts the languages to english and the browser permutations to firefox:

1. Build

        mvn -Pdev clean install

1. Run hosted mode

        cd 'build/app' mvn -Pdev gwt:run

### Bind Address

In some cases you may want to bind both the AS and the hosted mode to a specific address. A typical scenario is running a different OS (i.e windows) in a virtual machine. To make such a setup work you need to bind the hosted mode environment and the application server to a specific inet address that can be access from the virtual machine:

1. start the AS on a specific address:

    ```sh
    ./bin/standalone.sh \
        -Djboss.bind.address=192.168.2.126 \
        -Djboss.bind.address.management=192.168.2.126
    
    ```

1. launch hosted mode on a specific address:

        mvn clean -Dgwt.bindAddress=192.168.2.126 gwt:run

[1]: http://www.wildfly.org/
[2]: http://www.wildfly.org/download/
[3]: http://www.gwtproject.org/gettingstarted.html
[4]: https://github.com/arcbees/gwtp/
[5]: https://github.com/arcbees/gwtp/wiki
[6]: http://gwt.google.com/samples/MissingPlugin/MissingPlugin.html
