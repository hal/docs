# 2.8.19.Final 

- Target WildFly 10.0.0.Final
- Release Stream [2.8.19.Final](https://github.com/hal/release-stream/tree/2.8.19.Final)
- Core Console [2.8.19.Final](https://github.com/hal/core/tree/2.8.19.Final)
- Tracking Issue [WFLY-6065](https://issues.jboss.org/browse/WFLY-6065)

## New & Improved Features

- New homepage
- Support for suspend and graceful shutdown
- Replaced HornetQ with ActiveMQ Artemis
- Request Controller subsystem
- Deployment Scanner subsystem

## Bugfixes

- [HAL-1039](https://issues.jboss.org/browse/HAL-1039): Move test connection button to its own page
- [HAL-1034](https://issues.jboss.org/browse/HAL-1034): Add logo image for new product name
- [HAL-1031](https://issues.jboss.org/browse/HAL-1031): Fix confirmation messages in TX log view
- [HAL-1017](https://issues.jboss.org/browse/HAL-1017): JMSMetricPresenter always uses "default" as part of operation address even if name is changed.
- [HAL-1016](https://issues.jboss.org/browse/HAL-1016): Webconsole should require to have set 'use journal store' as true when changing value 'Journal store enable async io' to true
- [HAL-1013](https://issues.jboss.org/browse/HAL-1013): Rely on new DoubleFormItem in ModelNodeFormBuilder; Tweak the double parsing
- [HAL-1012](https://issues.jboss.org/browse/HAL-1012): Infinispan cache screens are not cleared when a resource is removed
- [HAL-1003](https://issues.jboss.org/browse/HAL-1003): High memory consumption by Firefox when configuring Infinispan subsystem
- [HAL-993](https://issues.jboss.org/browse/HAL-993): Show effective port offset for running servers in preview
- [HAL-992](https://issues.jboss.org/browse/HAL-992): Socket binding group remembers current page after changing selection
- [HAL-990](https://issues.jboss.org/browse/HAL-990): Broken layout when accepting to reload servers in domain mode
- [HAL-988](https://issues.jboss.org/browse/HAL-988): Update to ballroom 2.3.11-SNAPSHOT
- [HAL-987](https://issues.jboss.org/browse/HAL-987): Create socket binding groups and clone them
- [HAL-984](https://issues.jboss.org/browse/HAL-984): Add i18n for guided tour
- [HAL-983](https://issues.jboss.org/browse/HAL-983): Button to add server doesn't disappear after server group deletion
- [HAL-975](https://issues.jboss.org/browse/HAL-975): Fix zanata.sh; update Zanata documentation
- [HAL-973](https://issues.jboss.org/browse/HAL-973): Adding socket shouldn't allow user to select binding-group
- [HAL-972](https://issues.jboss.org/browse/HAL-972): Replace deployment shouldn't allow to specify name and runtime name
- [HAL-969](https://issues.jboss.org/browse/HAL-969): Broken layout for "related" link
- [HAL-968](https://issues.jboss.org/browse/HAL-968): Add link and instructions of adding JMS queue on homepage
- [HAL-966](https://issues.jboss.org/browse/HAL-966): Add explanation for unmanaged deployments
- [HAL-965](https://issues.jboss.org/browse/HAL-965): Change the label "Destinations" in messaging provider to "Topics/Queues"
- [HAL-964](https://issues.jboss.org/browse/HAL-964): Add preview for messaging provider
- [HAL-962](https://issues.jboss.org/browse/HAL-962): required fields get an asterix
- [HAL-961](https://issues.jboss.org/browse/HAL-961): Add h2 database template
- [HAL-960](https://issues.jboss.org/browse/HAL-960): Add help texts in add datasource wizard
- [HAL-959](https://issues.jboss.org/browse/HAL-959): Replace op at content repository level not server group level
- [HAL-956](https://issues.jboss.org/browse/HAL-956): Web Console shows different Infinispan Eviction Max Entries value for default value.
- [HAL-951](https://issues.jboss.org/browse/HAL-951): Fix i18n text on homepage
- [HAL-947](https://issues.jboss.org/browse/HAL-947): Problem with showing elements in table in messaging clustering.
- [HAL-946](https://issues.jboss.org/browse/HAL-946): Update jboss.as.console.bom.version to 2.8.15
- [HAL-943](https://issues.jboss.org/browse/HAL-943): Security domain module options not reading data from configuration
- [HAL-942](https://issues.jboss.org/browse/HAL-942): Validate changing transaction log store
- [HAL-934](https://issues.jboss.org/browse/HAL-934): Update ballroom to 2.3.10
- [HAL-931](https://issues.jboss.org/browse/HAL-931): Group reload operation runs into timeout
- [HAL-930](https://issues.jboss.org/browse/HAL-930): HAL's TransactionPresenter doesn't update underlying model upon successful save
- [HAL-929](https://issues.jboss.org/browse/HAL-929): Cleanup breadcrumb management
- [HAL-928](https://issues.jboss.org/browse/HAL-928): Wrong 'Access tutorials and quickstarts' link in Web Console homepage
- [HAL-926](https://issues.jboss.org/browse/HAL-926): server group reload does not work
- [HAL-925](https://issues.jboss.org/browse/HAL-925): IO subsystem not shown
- [HAL-923](https://issues.jboss.org/browse/HAL-923): Reimplement PicketLink extension
- [HAL-922](https://issues.jboss.org/browse/HAL-922): Picket link user interface (functional)
- [HAL-915](https://issues.jboss.org/browse/HAL-915): Fix RRD address resolution for root resources
- [HAL-914](https://issues.jboss.org/browse/HAL-914): Backt to finder based on place hierarchy, opposed to PM#navigateBack()
- [HAL-913](https://issues.jboss.org/browse/HAL-913): keepalive-time attribute of batch thread pool is not visible
- [HAL-910](https://issues.jboss.org/browse/HAL-910): Resource focus change after edit is confusing
- [HAL-909](https://issues.jboss.org/browse/HAL-909): Missing start and stop button for server in domain mode with operator roles
- [HAL-904](https://issues.jboss.org/browse/HAL-904): Followup fix
- [HAL-903](https://issues.jboss.org/browse/HAL-903): Cannot add discovery group to bridge attributes
- [HAL-903](https://issues.jboss.org/browse/HAL-903): Cannot add discovery group to bridge attributes
- [HAL-900](https://issues.jboss.org/browse/HAL-900): Log viewer can show logs of another server in domain mode
- [HAL-898](https://issues.jboss.org/browse/HAL-898): Webconsole - runtime - webservices - responses graph - zero value not shown, old one displayed
- [HAL-897](https://issues.jboss.org/browse/HAL-897): web service metrics not displayed
- [HAL-895](https://issues.jboss.org/browse/HAL-895): Detect error message when statistics are disabled
- [HAL-894](https://issues.jboss.org/browse/HAL-894): Reload required information should be stressed more
- [HAL-893](https://issues.jboss.org/browse/HAL-893): Impossible to disable usage data collection by web console.
- [HAL-892](https://issues.jboss.org/browse/HAL-892): Data Collection doesn't indicate if Google analytics are already enabled
- [HAL-891](https://issues.jboss.org/browse/HAL-891): server status is confusing
- [HAL-887](https://issues.jboss.org/browse/HAL-887): incorrect error message in transaction subsystem configuration
- [HAL-882](https://issues.jboss.org/browse/HAL-882): Missing JPA Statistics
- [HAL-880](https://issues.jboss.org/browse/HAL-880): Problem with creating bridge in messaging subsystem
- [HAL-879](https://issues.jboss.org/browse/HAL-879): Tour wizard can't be closed by Esc
- [HAL-878](https://issues.jboss.org/browse/HAL-878): Guided tour for standalone mode
- [HAL-877](https://issues.jboss.org/browse/HAL-877): added incrementer and decrementer suggestions
- [HAL-860](https://issues.jboss.org/browse/HAL-860): ServerStore shows incomplete data
- [HAL-858](https://issues.jboss.org/browse/HAL-858): Use manual reveal for  host and server group presenters
- [HAL-856](https://issues.jboss.org/browse/HAL-856): fix for runtime DS view
- [HAL-850](https://issues.jboss.org/browse/HAL-850): Disable AddressTemplate test
- [HAL-846](https://issues.jboss.org/browse/HAL-846): Reuse model browser to show deployment details
- [HAL-845](https://issues.jboss.org/browse/HAL-845): Unable to open 'Transport Settings' dialogue for any Infinispan cache container
- [HAL-844](https://issues.jboss.org/browse/HAL-844): Add '<disableClassMetadata>false</disableClassMetadata>' for EAP build profiles
- [HAL-837](https://issues.jboss.org/browse/HAL-837): Can not set thread pool max size to -1
- [HAL-836](https://issues.jboss.org/browse/HAL-836): No items present in EE subsystem -> services tables
- [HAL-835](https://issues.jboss.org/browse/HAL-835): Freeze of domain runtimem finder
- [HAL-834](https://issues.jboss.org/browse/HAL-834): New homepage
- [HAL-834](https://issues.jboss.org/browse/HAL-834): Fix i18n resources
- [HAL-832](https://issues.jboss.org/browse/HAL-832): Can not add messaging connection factory through web console
- [HAL-831](https://issues.jboss.org/browse/HAL-831): Fix resource address in new activemq msg impl
- [HAL-830](https://issues.jboss.org/browse/HAL-830): Fix typo in resource address
- [HAL-829](https://issues.jboss.org/browse/HAL-829): Equal signs in property lists
- [HAL-828](https://issues.jboss.org/browse/HAL-828): Can not set cluster connection attributes to null
- [HAL-827](https://issues.jboss.org/browse/HAL-827): Can not create messaging clustering connection
- [HAL-826](https://issues.jboss.org/browse/HAL-826): Increase page size for deployment finder columns to 999
- [HAL-824](https://issues.jboss.org/browse/HAL-824): missing help texts for broadcast groups
- [HAL-823](https://issues.jboss.org/browse/HAL-823): JBEAP-978 - Added scrollbar to deployment preview
- [HAL-822](https://issues.jboss.org/browse/HAL-822): Can't change cache attributes
- [HAL-820](https://issues.jboss.org/browse/HAL-820): Add support for new jberet-batch metrics
- [HAL-818](https://issues.jboss.org/browse/HAL-818): Cannot set initial-pool-size attribute of datasource from web console
- [HAL-817](https://issues.jboss.org/browse/HAL-817): Cannot set use-fast-fail attribute of datasource from web console
- [HAL-814](https://issues.jboss.org/browse/HAL-814): file attributes for log handlers
- [HAL-813](https://issues.jboss.org/browse/HAL-813): Port 0 in syslog handler config
- [HAL-812](https://issues.jboss.org/browse/HAL-812): Fix XHR2 / FormData uploads
- [HAL-809](https://issues.jboss.org/browse/HAL-809): Fix missing class metadata in EntityAdapter and production mode
- [HAL-804](https://issues.jboss.org/browse/HAL-804): Change undertow to web/http
- [HAL-801](https://issues.jboss.org/browse/HAL-801): Add support for new batch-jberet subsystem
- [HAL-798](https://issues.jboss.org/browse/HAL-798): Switch to XHR / FormData uploads using 'management-upload' for deployments and patching
- [HAL-796](https://issues.jboss.org/browse/HAL-796): Add ability to restart a server
- [HAL-795](https://issues.jboss.org/browse/HAL-795): ModelBrowser window size handling
- [HAL-788](https://issues.jboss.org/browse/HAL-788): Remote socket binding is not displayed if it's port uses a property expression
- [HAL-787](https://issues.jboss.org/browse/HAL-787): Adding new Logger category: remove the name attribute/field etc.
- [HAL-785](https://issues.jboss.org/browse/HAL-785): Fix requires resources to match new Infinispan management model
- [HAL-781](https://issues.jboss.org/browse/HAL-781): Removed deprecated tx properties; switch to MBUI forms
- [HAL-780](https://issues.jboss.org/browse/HAL-780): Datasource: Statement Cache Size, Min Pool Size, Max Pool Size should not be required fields
- [HAL-778](https://issues.jboss.org/browse/HAL-778): Some socket bindings group is not in table with all socket binding groups in web console
- [HAL-774](https://issues.jboss.org/browse/HAL-774): JVM attributes heapSize and maxHeapSize should be nillable.
- [HAL-769](https://issues.jboss.org/browse/HAL-769): left align application contents
- [HAL-766](https://issues.jboss.org/browse/HAL-766): Splitbutton on chrome and safari did not work properly
- [HAL-765](https://issues.jboss.org/browse/HAL-765): StandaloneRuntimeRefresh.java did reside in wrong module
- [HAL-764](https://issues.jboss.org/browse/HAL-764): Unable to unset wsdl-port and wsdl-secure-port via console
- [HAL-763](https://issues.jboss.org/browse/HAL-763): Run as Role dialog: web console is reloaded
- [HAL-762](https://issues.jboss.org/browse/HAL-762): CAnnot add http server resources
- [HAL-760](https://issues.jboss.org/browse/HAL-760): Server-group-scoped-roles not respected in Domain mode
- [HAL-758](https://issues.jboss.org/browse/HAL-758): Add color codes to the deployment previews
- [HAL-754](https://issues.jboss.org/browse/HAL-754): preview contents
- [HAL-754](https://issues.jboss.org/browse/HAL-754): Fix previews for included subsystems
- [HAL-753](https://issues.jboss.org/browse/HAL-753): Fix error after uploading and removing content from the content repository
- [HAL-750](https://issues.jboss.org/browse/HAL-750): Re-add deployment scanner
- [HAL-749](https://issues.jboss.org/browse/HAL-749): allow white space in profile names
- [HAL-747](https://issues.jboss.org/browse/HAL-747): Initialisation of finder contributions doesn't work reliably
- [HAL-745](https://issues.jboss.org/browse/HAL-745): Show progress bar for long running deployment actions
- [HAL-744](https://issues.jboss.org/browse/HAL-744): Add tooltips for deployments
- [HAL-743](https://issues.jboss.org/browse/HAL-743): Finder tooltip facilities
- [HAL-740](https://issues.jboss.org/browse/HAL-740): Button overlay for finder rows
- [HAL-739](https://issues.jboss.org/browse/HAL-739): Switch defaults in new deployment / choose
- [HAL-738](https://issues.jboss.org/browse/HAL-738): Finder context menus remain visible
- [HAL-737](https://issues.jboss.org/browse/HAL-737): Finder row hover color
- [HAL-736](https://issues.jboss.org/browse/HAL-736): Revisit deployment previews
- [HAL-734](https://issues.jboss.org/browse/HAL-734): Filter for deployments, servers and server groups
- [HAL-732](https://issues.jboss.org/browse/HAL-732): State dependent menu actions for deployments
- [HAL-731](https://issues.jboss.org/browse/HAL-731): Add unmanaged content to the content repository
- [HAL-730](https://issues.jboss.org/browse/HAL-730): Change label from 'Remove' to 'Unassign'
- [HAL-729](https://issues.jboss.org/browse/HAL-729): Allow users to assign deployments to server groups from Content Repository and Unassigned Content
- [HAL-725](https://issues.jboss.org/browse/HAL-725): Add notifications for deployment related actions
- [HAL-723](https://issues.jboss.org/browse/HAL-723): Add 'Unassign' context menu item to content column
- [HAL-722](https://issues.jboss.org/browse/HAL-722): Change default value for flag 'enabled'
- [HAL-720](https://issues.jboss.org/browse/HAL-720): ResourceAdapter become finder contributions
- [HAL-719](https://issues.jboss.org/browse/HAL-719): Datasources become finder contributions
- [HAL-718](https://issues.jboss.org/browse/HAL-718): HTTP metrics in standalone mode
- [HAL-716](https://issues.jboss.org/browse/HAL-716): Can't change cache store attributes back to false from true
- [HAL-712](https://issues.jboss.org/browse/HAL-712): Add preview for include / exclude columns
- [HAL-705](https://issues.jboss.org/browse/HAL-705): Mail server definitons and mail session attributes have been fixed (includes [HAL-706](https://issues.jboss.org/browse/HAL-706))
- [HAL-702](https://issues.jboss.org/browse/HAL-702): Fix deprecated links
- [HAL-701](https://issues.jboss.org/browse/HAL-701): Fix broken links on homepage
- [HAL-700](https://issues.jboss.org/browse/HAL-700): scrolling with nested presenters
- [HAL-699](https://issues.jboss.org/browse/HAL-699): Closong of notification messages
- [HAL-698](https://issues.jboss.org/browse/HAL-698): Reload standalone server, server and groups in domain
- [HAL-697](https://issues.jboss.org/browse/HAL-697): Scrolling in standalone mode
- [HAL-692](https://issues.jboss.org/browse/HAL-692): Web Console uses wrong JGroup stack transport address
- [HAL-690](https://issues.jboss.org/browse/HAL-690): Check and add missing subresource; reset finder column selection
- [HAL-685](https://issues.jboss.org/browse/HAL-685): Backlink for finder breadcrumb ( includes an update to the page views)
- [HAL-684](https://issues.jboss.org/browse/HAL-684): Add all resource adapter config options to console
- [HAL-683](https://issues.jboss.org/browse/HAL-683): Support for scoped roles (except host scopes)
- [HAL-679](https://issues.jboss.org/browse/HAL-679): RBAC for finder menu items
- [HAL-672](https://issues.jboss.org/browse/HAL-672): Replace old access control UI with finder based UI
- [HAL-658](https://issues.jboss.org/browse/HAL-658): Missing configuration options in Console for new attributes in webservices subsystem
- [HAL-649](https://issues.jboss.org/browse/HAL-649): suspend resume operations on groups and servers
- [HAL-641](https://issues.jboss.org/browse/HAL-641): Add content columns; remove old deployment classes
- [HAL-638](https://issues.jboss.org/browse/HAL-638): Upgrade Ballroom to 2.3.1
- [HAL-619](https://issues.jboss.org/browse/HAL-619): Tweak maven settings to use new extension archetypes
- [HAL-618](https://issues.jboss.org/browse/HAL-618): New ActiveMQ messaging subsystem
- [HAL-615](https://issues.jboss.org/browse/HAL-615): Support for profile inheritance
- [HAL-614](https://issues.jboss.org/browse/HAL-614): Support for cloning of profiles
- [HAL-610](https://issues.jboss.org/browse/HAL-610): Support capacity policies for JCA deployments
- [HAL-520](https://issues.jboss.org/browse/HAL-520): ported enhancements to master
- [HAL-297](https://issues.jboss.org/browse/HAL-297): Migrate datasource wizard to have back buttons

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
