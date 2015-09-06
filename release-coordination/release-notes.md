# 2.7.4.Final

- Target: WildFly 9.0.0.Final
- Release Stream: [2.7.4.Final](https://github.com/hal/release-stream/tree/2.7.4.Final)  
- Core Console: [2.7.4.Final](https://github.com/hal/core/tree/2.7.4.Final) 
- Tracking Issue: [WFLY-4809](https://issues.jboss.org/browse/WFLY-4809) 

## New & Improved Features

- New finder based user interface
- Replaced JacORB with IIOP OpenJDK subsystem
- Remoting subsystem  
- Support for datasource templates.
- Provide all flush-* operations for connection pools
- Improved log viewer
- Enhanced model browser with support for singleton resources
- Get more details about applied patches
- Ability to launch the management console independently from WildFly

## Bugfixes

- [HAL-701](https://issues.jboss.org/browse/HAL-701): Fix broken links on homepage
- [HAL-700](https://issues.jboss.org/browse/HAL-700): Scrolling with nested presenters
- [HAL-699](https://issues.jboss.org/browse/HAL-699): Closing of notification messages
- [HAL-698](https://issues.jboss.org/browse/HAL-698): Reload standalone server, server and groups in domain
- [HAL-697](https://issues.jboss.org/browse/HAL-697): Scrolling in standalone mode
- [HAL-690](https://issues.jboss.org/browse/HAL-690), [HAL-691](https://issues.jboss.org/browse/HAL-691): Check and add missing subresource; reset finder column selection
- [HAL-678](https://issues.jboss.org/browse/HAL-678): Server config settings don't refresh after changes
- [HAL-674](https://issues.jboss.org/browse/HAL-674): Server groups settings don't refresh after changes
- [HAL-672](https://issues.jboss.org/browse/HAL-672): Replace old access control UI with finder based UI
- [HAL-665](https://issues.jboss.org/browse/HAL-665): Replace EJB subsystem with MBUI views
- [HAL-655](https://issues.jboss.org/browse/HAL-655): Add support for remaining servlet container settings (undertow)
- [HAL-644](https://issues.jboss.org/browse/HAL-644): Hornetq messaging finder contributions
- [HAL-643](https://issues.jboss.org/browse/HAL-643): Infinispan cache container become finder contributions
- [HAL-641](https://issues.jboss.org/browse/HAL-641): Deployment Finder
- [HAL-635](https://issues.jboss.org/browse/HAL-635): Runtime/Transaction typo fix.
- [HAL-634](https://issues.jboss.org/browse/HAL-634): Remove non-heap panel: meatspace has replaced permgen on JDK 8
- [HAL-633](https://issues.jboss.org/browse/HAL-633): Fix refreshing in deployment / content repository
- [HAL-630](https://issues.jboss.org/browse/HAL-630): Preview content i18n
- [HAL-621](https://issues.jboss.org/browse/HAL-621): Added 'module' attribute to security domain forms
- [HAL-609](https://issues.jboss.org/browse/HAL-609): Scrolling in finder views
- [HAL-607](https://issues.jboss.org/browse/HAL-607): Additional preview contents
- [HAL-606](https://issues.jboss.org/browse/HAL-606): Finder styles
- [HAL-599](https://issues.jboss.org/browse/HAL-599): JXM subsystem attributes have changed
- [HAL-598](https://issues.jboss.org/browse/HAL-598): Fix jGroups protocol and transport properties
- [HAL-598](https://issues.jboss.org/browse/HAL-598): Fix backport from master
- [HAL-597](https://issues.jboss.org/browse/HAL-597): Fix interface form validation
- [HAL-594](https://issues.jboss.org/browse/HAL-594): Removed check for 'transactions' flag in JacORB subsystem
- [HAL-594](https://issues.jboss.org/browse/HAL-594): Remove JacORB related form validation
- [HAL-593](https://issues.jboss.org/browse/HAL-593): Add new IIOP JDK ORB subsystem
- [HAL-592](https://issues.jboss.org/browse/HAL-592): Fix default table selection
- [HAL-591](https://issues.jboss.org/browse/HAL-591): Adjust to changed management model for jgroup protocols
- [HAL-588](https://issues.jboss.org/browse/HAL-588): Gracfully handle optional resource references
- [HAL-587](https://issues.jboss.org/browse/HAL-587): Revert to action parameter API in stores
- [HAL-585](https://issues.jboss.org/browse/HAL-585): Revisit resource adapter configuration
- [HAL-583](https://issues.jboss.org/browse/HAL-583): Revisit (xa) datasource configuration
- [HAL-582](https://issues.jboss.org/browse/HAL-582): Revisit JCA common configuration
- [HAL-580](https://issues.jboss.org/browse/HAL-580): Fix ReadRequiredResources (patch management for standalone is broken)
- [HAL-575](https://issues.jboss.org/browse/HAL-575): Upgrade GWT to 2.7.0; switch to Super DevMode
- [HAL-574](https://issues.jboss.org/browse/HAL-574): Update bootstrap process
- [HAL-573](https://issues.jboss.org/browse/HAL-573): Combine security context setup and r-r-d processing
- [HAL-572](https://issues.jboss.org/browse/HAL-572): Upgrade GWTP to 1.4
- [HAL-569](https://issues.jboss.org/browse/HAL-569): Expose all flush-* operations for datasources
- [HAL-565](https://issues.jboss.org/browse/HAL-565): Add datasource templates
- [HAL-564](https://issues.jboss.org/browse/HAL-564): Replace data-source=*:enable() / :disable() op
- [HAL-563](https://issues.jboss.org/browse/HAL-563): Add pager to datasource tables in #ds-metrics
- [HAL-562](https://issues.jboss.org/browse/HAL-562): Fix typo
- [HAL-561](https://issues.jboss.org/browse/HAL-561): Fix broken filter after removing deployment from content repository
- [HAL-560](https://issues.jboss.org/browse/HAL-560): :flush-all-connection-in-pool called
- [HAL-556](https://issues.jboss.org/browse/HAL-556), [HAL-640](https://issues.jboss.org/browse/HAL-640): server group and profile stores
- [HAL-554](https://issues.jboss.org/browse/HAL-554): Fix loading settings
- [HAL-553](https://issues.jboss.org/browse/HAL-553): Use '{selected.profile}' when saving model driven widgets in web presenter
- [HAL-544](https://issues.jboss.org/browse/HAL-544): UI for remoting subsystem
- [HAL-536](https://issues.jboss.org/browse/HAL-536): Changing the settings should force reload the browser window
- [HAL-533](https://issues.jboss.org/browse/HAL-533): Adjust section about latest applied patch
- [HAL-529](https://issues.jboss.org/browse/HAL-529): Fix hanging "download in progress" dialog
- [HAL-528](https://issues.jboss.org/browse/HAL-528): Fix search in concurrently opened log files
- [HAL-526](https://issues.jboss.org/browse/HAL-526): Fix add mail server dialog
- [HAL-523](https://issues.jboss.org/browse/HAL-523): Singleton resource metata, support for list and property attribute types in model browser
- [HAL-520](https://issues.jboss.org/browse/HAL-520): Ability to choose the available security module codes
- [HAL-473](https://issues.jboss.org/browse/HAL-473): provide http metrics view for undertow

# 2.5.5.Final

- Target: EAP 6.4.0.GA
- Release Stream: [2.5.5.Final](https://github.com/hal/release-stream/tree/2.5.5.Final) 
- Core Console: [2.5.5.Final](https://github.com/hal/core/tree/2.5.5.Final)
- Tracking Issue: [BZ1193523](https://bugzilla.redhat.com/show_bug.cgi?id=1193523)

## Bugfixes

- [BZ901260](https://bugzilla.redhat.com/show_bug.cgi?id=901260): Updated translations
- [BZ1176249](https://bugzilla.redhat.com/show_bug.cgi?id=1176249): Product logo depends on product name.
- [BZ1174732](https://bugzilla.redhat.com/show_bug.cgi?id=1174732): Use '{selected.profile}' when saving model driven widgets in web presenter
- [BZ1173031](https://bugzilla.redhat.com/show_bug.cgi?id=1173031): Fix loading settings
- [BZ1172168](https://bugzilla.redhat.com/show_bug.cgi?id=1172168): Fix match between subsystem key and related subsystem token
- [BZ1170538](https://bugzilla.redhat.com/show_bug.cgi?id=1170538): Fix in viewframework
- [BZ1167673](https://bugzilla.redhat.com/show_bug.cgi?id=1167673): Fix search in concurrently opened log files
- [BZ1167525](https://bugzilla.redhat.com/show_bug.cgi?id=1167525): Fix add mail server dialog
- [BZ1167362](https://bugzilla.redhat.com/show_bug.cgi?id=1167362): Fix hanging "download in progress" dialog
- [BZ1166749](https://bugzilla.redhat.com/show_bug.cgi?id=1166749) / [BZ1166737](https://bugzilla.redhat.com/show_bug.cgi?id=1166737): Visual adjustments for the homepage and the search
- [BZ1159771](https://bugzilla.redhat.com/show_bug.cgi?id=1159771): Wrong error message in New Connector wizard
- [BZ1026823](https://bugzilla.redhat.com/show_bug.cgi?id=1026823): run as dialog
- [BZ1017655](https://bugzilla.redhat.com/show_bug.cgi?id=1017655): Fix validation in WebServicePresenter#onSaveProvider
- [BZ1017059](https://bugzilla.redhat.com/show_bug.cgi?id=1017059): After :server-set-restart-required operation web console shows reload required message

# 2.4.9.Final

- Target: WildFly 8.2.0.Final
- Release Stream: [2.4.9.Final](https://github.com/hal/release-stream/tree/2.4.9.Final)  
- Core Console: [2.4.9.Final](https://github.com/hal/core/tree/2.4.9.Final) 
- Tracking Issue: [WFLY-4107](https://issues.jboss.org/browse/WFLY-4107) 

## New & Improved Features

- Updated look & feel. Now follows the Patternfly styles.
- Improved information architecture: Domain management, deployments and runtime views have been relocated / consolidated
- Extended / complete subsystem configuration: EE, Undertow, Messaging, IO and Batch
- Updated model browser: supports inline editing of resources
- Log Viewer: Tail log files from within the console
- Picketlink extension: The GUI now ships the picketlink management parts (enabled on demand)
- Improved runtime monitoring: The charts and data tables have been cleaned up
- See also http://hbraun.info/2014/10/updated-management-console-in-[wildfly-8](https://issues.jboss.org/browse/wildfly-8)-2/

## Bugfixes

- [HAL-514](https://issues.jboss.org/browse/HAL-514): Prepare double click handler on log file table
- [HAL-512](https://issues.jboss.org/browse/HAL-512): Display deployment "status" attribute on deployment list
- [HAL-508](https://issues.jboss.org/browse/HAL-508): Tools links leave wrong name token
- [HAL-507](https://issues.jboss.org/browse/HAL-507): Tab titles are no longer truncated by default
- [HAL-506](https://issues.jboss.org/browse/HAL-506): Add operation adresses to tool buttons in logviewer
- [HAL-503](https://issues.jboss.org/browse/HAL-503): Product and server name are displayed in the browser's title
- [HAL-501](https://issues.jboss.org/browse/HAL-501): relative-to for file based log handler is only required if path is relative
- [HAL-500](https://issues.jboss.org/browse/HAL-500): Navigation for RH Access
- [HAL-497](https://issues.jboss.org/browse/HAL-497): Entire layout of csp plugin falls apart after visiting different page
- [HAL-495](https://issues.jboss.org/browse/HAL-495): Fix tooltips in topology view
- [HAL-493](https://issues.jboss.org/browse/HAL-493): Apply patch wizard stuck on patch application step
- [HAL-492](https://issues.jboss.org/browse/HAL-492): Fix URL fragment problem
- [HAL-490](https://issues.jboss.org/browse/HAL-490): Distinguish community and product version
- [HAL-487](https://issues.jboss.org/browse/HAL-487): Fix handler reference bug which was introduced by [HAL-313](https://issues.jboss.org/browse/HAL-313)
- [HAL-486](https://issues.jboss.org/browse/HAL-486): Invalid default value for "Default Module" attribute of Virtual Server
- [HAL-484](https://issues.jboss.org/browse/HAL-484): Resource adapter names not visible
- [HAL-483](https://issues.jboss.org/browse/HAL-483): Switch back to 'StandaloneDriverStrategy' for standalpone mode
- [HAL-482](https://issues.jboss.org/browse/HAL-482): Application constraints for logging subsystem
- [HAL-481](https://issues.jboss.org/browse/HAL-481): Cache Containers doesn't refresh after save
- [HAL-477](https://issues.jboss.org/browse/HAL-477): Exclude attribute 'thread-factory' from 'ThreadPoolsView'
- [HAL-476](https://issues.jboss.org/browse/HAL-476): Update to CSP Plugin 0.9.4-SNAPSHOT
- [HAL-472](https://issues.jboss.org/browse/HAL-472): Highlight Standalone Runtime Nav
- [HAL-471](https://issues.jboss.org/browse/HAL-471): Introduce collapsible panel and cleanup left hand navigation
- [HAL-469](https://issues.jboss.org/browse/HAL-469): LHS navigation highlight is gone when using place requests that include parameters
- [HAL-468](https://issues.jboss.org/browse/HAL-468): Enable stats on data sources
- [HAL-467](https://issues.jboss.org/browse/HAL-467): Cleanup subsystem metrics
- [HAL-465](https://issues.jboss.org/browse/HAL-465): Unable to remove server config
- [HAL-463](https://issues.jboss.org/browse/HAL-463): ModelBrowser doesn't work for profiles on EAP 6.x
- [HAL-457](https://issues.jboss.org/browse/HAL-457): Provide a stripped down version of the GUI
- [HAL-455](https://issues.jboss.org/browse/HAL-455): Perspective presenter cause unnecessary onReset() calls
- [HAL-454](https://issues.jboss.org/browse/HAL-454): Add support for adding a periodic-size-rotating-file handler.
- [HAL-451](https://issues.jboss.org/browse/HAL-451): Extended configuration for the EE subsystem
- [HAL-425](https://issues.jboss.org/browse/HAL-425): Reorganize web subsystem attributes into 'global' and 'jsp'
- [HAL-397](https://issues.jboss.org/browse/HAL-397): JTA default not respected creating datasource
- [HAL-391](https://issues.jboss.org/browse/HAL-391): show timestamp when deployed applications are enabled/disabled.
- [HAL-389](https://issues.jboss.org/browse/HAL-389): Change flush operation from 'flush-all-connection-in-pool' to 'flush-idle-connection-in-pool'
- [HAL-388](https://issues.jboss.org/browse/HAL-388): Console uses hardcoded hornetq-server name as "default"
- [HAL-354](https://issues.jboss.org/browse/HAL-354): display jvm uptime on jvm rutime view
- [HAL-342](https://issues.jboss.org/browse/HAL-342): Remove unused class
- [HAL-342](https://issues.jboss.org/browse/HAL-342): After cancel the process to upload a deployment file, the content is added to data directory
- [HAL-311](https://issues.jboss.org/browse/HAL-311): Provide the ability to view server logs
- [HAL-303](https://issues.jboss.org/browse/HAL-303): Improve the question asked when enabling / disabling datasource
- [HAL-292](https://issues.jboss.org/browse/HAL-292): Add error message when unable to execute an operation

# 2.2.8.Final

- Target: EAP 6.3.0.GA
- Release Stream: [2.2.8.Final](https://github.com/hal/release-stream/tree/2.2.8.Final) 
- Core Console: [2.2.8.Final](https://github.com/hal/core/tree/2.2.8.Final)
- Tracking Issue: [BZ1104216](https://bugzilla.redhat.com/show_bug.cgi?id=1104216)

## New & Improved Features

- Role based access control (RBAC)
- Patching
- New top level navigation
- Home page

## Bugfixes

- [BZ901227](https://bugzilla.redhat.com/show_bug.cgi?id=901227): Allow -1 as default value for modcluster timeout attributes
- [BZ1092650](https://bugzilla.redhat.com/show_bug.cgi?id=1092650): Add pager to list of EE modules
- [BZ1088314](https://bugzilla.redhat.com/show_bug.cgi?id=1088314): Fix refresh in JacORB view
- [BZ1081990](https://bugzilla.redhat.com/show_bug.cgi?id=1081990): Add restart button; fix for one-off patches
- [BZ1081570](https://bugzilla.redhat.com/show_bug.cgi?id=1081570): Add check if running in domain mode
- [BZ1081186](https://bugzilla.redhat.com/show_bug.cgi?id=1081186): Change label and help text for GA
- [BZ1080767](https://bugzilla.redhat.com/show_bug.cgi?id=1080767): Home page string suggestions and corrections
- [BZ1075720](https://bugzilla.redhat.com/show_bug.cgi?id=1075720): Get rid of patch confirm step
- [BZ1075264](https://bugzilla.redhat.com/show_bug.cgi?id=1075264): Remove inline warning icon
- [BZ1075169](https://bugzilla.redhat.com/show_bug.cgi?id=1075169): Fix wizard title
- [BZ1075137](https://bugzilla.redhat.com/show_bug.cgi?id=1075137): Disable rollback button when no items are available
- [BZ1074675](https://bugzilla.redhat.com/show_bug.cgi?id=1074675): Modal patch wizard
- [BZ1074623](https://bugzilla.redhat.com/show_bug.cgi?id=1074623): Fix parsing error
- [BZ1073988](https://bugzilla.redhat.com/show_bug.cgi?id=1073988): Fix intro paragraph for homepage
- [BZ1073597](https://bugzilla.redhat.com/show_bug.cgi?id=1073597): Home page task containers show (empty) scrollbar.
- [BZ1072337](https://bugzilla.redhat.com/show_bug.cgi?id=1072337): Fix recovery from verify connection failed
- [BZ1071949](https://bugzilla.redhat.com/show_bug.cgi?id=1071949): Redirect when trying to access "Security Domains"
- [BZ1070130](https://bugzilla.redhat.com/show_bug.cgi?id=1070130): Postpone driver auto detection
- [EAP6-109](https://issues.jboss.org/browse/EAP6-109): New top-level navigation
- [EAP6-87](https://issues.jboss.org/browse/EAP6-87): Analytics is disabled in product version by default
- [EAP6-66](https://issues.jboss.org/browse/EAP6-66): Add ability to test the connection for new and existing datasources
- [EAP6-18](https://issues.jboss.org/browse/EAP6-18): Expose patch management in Console
- [EAP6-16](https://issues.jboss.org/browse/EAP6-16): Refactoring of the confirm step; apply success i18n

# 2.2.6.Final

- Target: WildFly 8.1.0.Final
- Release Stream: [2.2.6.Final](https://github.com/hal/release-stream/tree/2.2.6.Final) 
- Core Console: [2.2.6.Final](https://github.com/hal/core/tree/2.2.6.Final) 
- Tracking Issue: [WFLY-3332](https://issues.jboss.org/browse/WFLY-3332) 

## New & Improved Features

- Patching
- New top level navigation
- Home page

## Bugfixes

- [HAL-403](https://issues.jboss.org/browse/HAL-403): Fix index setup
- [HAL-402](https://issues.jboss.org/browse/HAL-402): Fix refresh when using view framework
- [HAL-385](https://issues.jboss.org/browse/HAL-385): Scrollbar for profile selector
- [HAL-384](https://issues.jboss.org/browse/HAL-384): Only servers which belong to the current profile are part of the verify operation
- [HAL-383](https://issues.jboss.org/browse/HAL-383): Homepage links don't work as expected
- [HAL-382](https://issues.jboss.org/browse/HAL-382): Prevent loading of google vis in web mode
- [HAL-381](https://issues.jboss.org/browse/HAL-381): Default build for community includes modern browsers and en. New profile 'full' for all browsers / locales
- [HAL-347](https://issues.jboss.org/browse/HAL-347): Queues are read-only after creation
- [HAL-312](https://issues.jboss.org/browse/HAL-312): Prevent duplicate mail server types
- [HAL-302](https://issues.jboss.org/browse/HAL-302): It is possible to use duplicate name or jdni in "New Datasource" wizard
- [HAL-301](https://issues.jboss.org/browse/HAL-301): Proper use of IDs and classes to enable better testability
- [HAL-295](https://issues.jboss.org/browse/HAL-295): Console responses are slow in case of larger domains
- [HAL-260](https://issues.jboss.org/browse/HAL-260): Facilities to reset policy decision on interaction units (post DOM creation)
- [HAL-259](https://issues.jboss.org/browse/HAL-259): Security child contexts for instance based meta data
- [HAL-238](https://issues.jboss.org/browse/HAL-238): Control element visibility for users with multiple scoped roles
- [HAL-226](https://issues.jboss.org/browse/HAL-226): Abbreviate long JNDI names for JMS endpoints

# 2.1.1.Final

- Target: WildFly 8.0.0.Final
- Release Stream: [2.1.1.Final](https://github.com/hal/release-stream/tree/2.1.1.Final) 
- Core Console: [2.1.1.Final](https://github.com/hal/core/tree/2.1.1.Final)
- Tracking Issue: [HAL-346](https://issues.jboss.org/browse/HAL-346)

## New & Improved Features

- Topology View
- Performance
- RBAC sensitive UI

## Bugfixes

- [HAL-337](https://issues.jboss.org/browse/HAL-337): Partly undo fix which was introduced by HAL-10
- [HAL-336](https://issues.jboss.org/browse/HAL-336): Show a warning and change default place to "Profiles" if there are no groups defined.
- [HAL-335](https://issues.jboss.org/browse/HAL-335): Workaround using include-aliases=true; more fail-safe RBACGatekeeper
- [HAL-331](https://issues.jboss.org/browse/HAL-331): Add horizontal scrolling to value table in properties table
- [HAL-329](https://issues.jboss.org/browse/HAL-329): Fix top level navigation for MBUI dialogs
- [HAL-328](https://issues.jboss.org/browse/HAL-328): Navigation not highlighted for MBUI dialogs
- [HAL-327](https://issues.jboss.org/browse/HAL-327): Add RBAC check for server reload button
- [HAL-326](https://issues.jboss.org/browse/HAL-326): remote repo in dev mode
- [HAL-321](https://issues.jboss.org/browse/HAL-321): properly clear and reset dialog state upon removal of resources
- [HAL-320](https://issues.jboss.org/browse/HAL-320): Progress bar for RBAC related r-r-d
- [HAL-319](https://issues.jboss.org/browse/HAL-319): Scope assignment and statement context resolution
- [HAL-317](https://issues.jboss.org/browse/HAL-317): Undefine attribute doesn't work
- [HAL-315](https://issues.jboss.org/browse/HAL-315): "Max Retry" -> "Max Retry Interval"
- [HAL-313](https://issues.jboss.org/browse/HAL-313): Async handlers don't provide handlers to subviews - ie no nesting allowed!
- [HAL-312](https://issues.jboss.org/browse/HAL-312): Prevent creation of duplicate mail server type per mail session
- [HAL-308](https://issues.jboss.org/browse/HAL-308): Fix error when no running server is present
- [HAL-296](https://issues.jboss.org/browse/HAL-296): Add progress element to footer
- [HAL-295](https://issues.jboss.org/browse/HAL-295): Read topology using async flow API and condensed composite operatiions
- [HAL-280](https://issues.jboss.org/browse/HAL-280): Read drivers for domain mode using async flow functions
- [HAL-266](https://issues.jboss.org/browse/HAL--26): Upgrade to ballroom 2.0.5.Final
- [HAL-265](https://issues.jboss.org/browse/HAL-265): Several GIU enhancements
- [WFLY-1921](https://issues.jboss.org/browse/WFLY-1921): Honor cancel button

# 2.0.6.Final

- Target: EAP 6.2.0.GA
- Release Stream: [2.0.6.Final](https://github.com/hal/release-stream/tree/2.0.6.Final) 
- Core Console: [2.0.6.Final](https://github.com/hal/core/tree/2.0.6.Final)
- Tracking Issue: [HAL-291](https://issues.jboss.org/browse/HAL-291)

## Release Notes

- [HAL-285](https://issues.jboss.org/browse/HAL-285): Syslog handler is missing in setting of Handlers in Management Console
- [HAL-284](https://issues.jboss.org/browse/HAL-284): Changing scope type of the role leads to "Failed to save" error
- [HAL-281](https://issues.jboss.org/browse/HAL-281): Unclear error message when trying to configure Auditor role as Administrator
- [HAL-280](https://issues.jboss.org/browse/HAL-280): Unable to List Driver during Datasource Creation via the management console
- [HAL-278](https://issues.jboss.org/browse/HAL-278): List attributes in "need help" in same order as in settings tabs
- [HAL-275](https://issues.jboss.org/browse/HAL-275): Improve error handling when operating on stopped server instances
- [HAL-274](https://issues.jboss.org/browse/HAL-274): RunAs after switching roles results in an error
- [HAL-264](https://issues.jboss.org/browse/HAL-264): Resource adapter inline editing problems
- [HAL-263](https://issues.jboss.org/browse/HAL-263): Modal windows are sized inconsistently
- [HAL-261](https://issues.jboss.org/browse/HAL-261): Role management mapping should be accessible for Auditor
- [HAL-256](https://issues.jboss.org/browse/HAL-256): Module and ClassName fields are disabled in new Custom handler dialog
- [HAL-255](https://issues.jboss.org/browse/HAL-255): Runtime name input disable in new Unmanaged Deployment dialog
- [HAL-253](https://issues.jboss.org/browse/HAL-253): Domain mode: kill an unresponsive JVM
- [HAL-250](https://issues.jboss.org/browse/HAL-250): Revert project name references
- [HAL-244](https://issues.jboss.org/browse/HAL-244): Unable to unset "Default From" attribute in Mail Session administration
- [HAL-241](https://issues.jboss.org/browse/HAL-241): Role names seem to be case insensitive but roles tab of the console assumes they are ALLCAPS
- [HAL-240](https://issues.jboss.org/browse/HAL-240): Push translations to translate.jboss.org
- [HAL-239](https://issues.jboss.org/browse/HAL-239): Removing role with "include-all"
- [HAL-221](https://issues.jboss.org/browse/HAL-221): Missing server controls in topology view for Server scoped roles
- [HAL-208](https://issues.jboss.org/browse/HAL-208): Add descriptions and help texts to the role assignment views
