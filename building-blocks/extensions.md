# Compile Time Extensions 

## Extensions

The console provides a compile time extension mechanism. Extensions are regular GWT modules that implement the SPI and follow certain conventions. Extension are provided as maven dependencies and distributed through the [hal/release-stream build][1].

Any extension has access to the regular framework contract, all of it's services and the full dependency injection scope. In order the get an idea how extensions are setup, we provide a [maven archetype][3] to get started quickly. The archetype creates an extension with a presenter / view tuple to edit the top level attributes of a given subsystem. 

Normally an extension is a multi maven module which consists of the following sub modules:

- `gui`: Contains the GWT code for the extension
- `app`: Provides a GWT module to run and test the extension

The actual extension is developed in the `gui` module. You have access to all HAL APIs and can use the building blocks described in this chapter.
 
To launch the extension, switch to the `app` directory and execute one of the following:
 
- `mvn gwt:run` for GWT SuperDevMode
- `mvn gwt:run|debug -Dgwt.superDevMode=false` to use the old DevMode. Please note that you'll need [Firefox <= 26](http://ftp.mozilla.org/pub/mozilla.org/firefox/releases/26.0/) and the [GWT plugin](http://www.gwtproject.org/missing-plugin/) to use DevMode.

You'll need a running WildFly instance which is configured to allow access from http://localhost:8888. Use one of the following CLI commands to configure the management endpoint:

- standalone mode: 

        /core-service=management/management-interface=http-interface:list-add(name=allowed-origins,value=http://localhost:8888)
        reload
    
- domain mode:

        /host=master/core-service=management/management-interface=http-interface:list-add(name=allowed-origins,value=http://localhost:8888)
        reload --host=master

Please note that the extension will only show up in the UI if the subsystem is configured in standalone mode or is part of the selected profile in domain mode. 

## Contract

The extension itself must provide specific building blocks:

- Maven setup
- The extension point
- Gin mixin definitions

### Maven setup

The `gui` maven module which carries the actual extension must inherit from `org.jboss.as:jboss-as-console-extension`. To run the extension as part of the HAL management console, the `app` module must inherit from `org.jboss.as:jboss-as-console-build` and contain a specific configuration for the `build-helper-maven-plugin` and `maven-processor-plugin` plugin. Create a simple extension using the [archetype][3] and take a look at the generated maven modules for al details. 

### Extension Point

In order to provide an extension point you need to implement a presenter / view tuple. For the extension to be discovered you need to annotate the Presenter proxy with a `@SubsystemExtension` declaration. This instructs the annotation processors to include another place that represents your subsystem specific screen:

```java
@ProxyCodeSplit
@NameToken("request-controller")
@SubsystemExtension(name = "Request Controller", group = "Extensions", key = "request-controller")
public interface MyProxy extends ProxyPlace<ExtensionPresenter> {
}
```

The extension will be loaded, initialised and revealed automatically by the core framework according to the following criteria:

* `name` &amp; `group` declarations: The link name and the group for the navigation.
* `key`: the subsystem as it is referred to in the DMR model. If the subsystem doesn't exist, the extension will not show up.

### IOC Mixins

These mixins are needed to extend the dependency injection scope and wire up your presenters / view tuples and other utility classes (if needed). A mixin is declared both as a binding and model extension. The `@GinExtension` value refers the GWT module descriptor used with the extension.

The injection points:

```java
@GinExtension
public interface Extension {
    AsyncProvider<ExtensionPresenter> getExtensionPresenter();
}
```

The actual binding:

```java
@GinExtensionBinding
public class ExtensionBinding extends AbstractPresenterModule {

    @Override
    protected void configure() {
        install(new I18nModule());

        bindPresenter(ExtensionPresenter.class,
                ExtensionPresenter.MyView.class,
                ExtensionView.class,
                ExtensionPresenter.MyProxy.class);
    }
}
```

### Contributions

Extensions are currently used by the following projects to integrate with the management console:

- Switchyard: https://github.com/jboss-switchyard/console
- Teiid: https://github.com/teiid/teiid-web-console
- PicketLink: https://github.com/picketlink2/picketlink-console

[1]: https://github.com/hal/release-stream/
[2]: https://github.com/teiid/teiid-web-console/tree/teiid-console-parent-1.1.0.Final
[3]: https://github.com/hal/archetypes/tree/master/subsystem-extension
