# Running a domain on a single machine

Sometimes it’s required to verify a domain setup with multiple hosts involved. But what if only a single machine is at your service? This document describes a simple setup that allows you to create a WildFly domain on a number of virtual hosts: Simply by binding the host controllers to virtual network interfaces.

## Create a host controller configuration

Create a copy of the domain directory that ships with the default distribution.

    cd $WILDFLY_HOME
    cp -R domain domain2

The slave controller configuration (domain2/configuration/host.xml) requires two significant changes:

1. assign a distinct host name
1. turn the host control into a slave

The first step requires you to chose a name that distinct across the domain. We are going to name it “slave.local”:

```xml
<host name="slave.local" xmlns="urn:jboss:domain:2.2">
```

The second step is as simple. Instead of declaring another master controller (element) we point the slave controller to a master it should connect to:

```xml
<remote host="${jboss.domain.master.address}" port="${jboss.domain.master.port:9999}" security-realm="ManagementRealm"/>
```

For our purposes we stick with the expressions (${foo.bar}), because it allows us to easily pass in arguments from the command line. But you could as well provide fixed values.

## Starting the domain controller

Bring up the domain by starting the domain controller:

    ./bin/domain.sh

Notice that we launch it without arguments. In this case it will refer to the default domain directory.

After a few seconds the domain controller should up and running and started it’s default servers:

    [Host Controller] 13:28:21,552 INFO  [org.jboss.as] (Controller Boot Thread) JBAS015874: WildFly 8.2.0.Final "Tweek" (Host Controller) started in 6683ms - Started 44 of 46 services (13 services are lazy, passive or on-demand)

## The virtual network interface

Before we can launch the host controller (slave) we need to create a virtual network interface (alias) for the second process to bind to. We’ll simply create an alias on loopback adapter:

    sudo ifconfig lo0 alias 172.16.123.1

Now we are ready to start the slave controller process, pointing it to the second directory:

    ./bin/domain.sh \
    -Djboss.domain.master.address=127.0.0.1 \
    -Djboss.bind.address=172.16.123.1 \
    -Djboss.bind.address.management=172.16.123.1 \
    -Djboss.domain.base.dir=./domain2

After a while the main controller registers it:

    [Host Controller] 13:52:12,494 INFO  [org.jboss.as.domain] (Host Controller Service Threads - 28) JBAS010918: Registered remote slave host "slave.local", WildFly 8.2.0.Final "Tweek"

This means the domain including both “hosts” (aka 'master' and 'slave.local') is up and running. The same steps would be necessary to create a domain with two physical distinct hosts.
