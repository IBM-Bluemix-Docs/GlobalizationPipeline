---

copyright:
  years: 2016, 2019

lastupdated: "2019-03-20"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:codeblock: .codeblock}
{:tip: .tip}
{:download: .download}


# {{site.data.keyword.GlobalizationPipeline_short}} {{site.data.keyword.cloudaccesstrailshort}} events
{: #gpat_events}

Use the {{site.data.keyword.cloudaccesstrailfull}} service to track how users and applications interact with the IBM {{site.data.keyword.GlobalizationPipeline_short}} in the {{site.data.keyword.Bluemix}}.
{:shortdesc}

The {{site.data.keyword.cloudaccesstrailfull_notm}} service records user-initiated activities that change the state of a service in the {{site.data.keyword.Bluemix_notm}}. For more information, see [{{site.data.keyword.cloudaccesstrailfull_notm}}](/docs/services/Activity-Tracker-with-LogDNA?topic=logdnaat-getting-started).




## List of events: Bundle events
{: #gpevents_bundle}

The following table lists the actions that are related to bundles and generate an event:

|Action|Description|
|---|---|  
|g11n-pipeline.bundles.read|Gets a list of bundle IDs.|
|g11n-pipeline.bundle.create|Creates a new bundle.|
|g11n-pipeline.bundle.read|Gets the bundle's information.|
|g11n-pipeline.bundle.update|Updates the bundle's configuration.|
|g11n-pipeline.bundle.delete|Deletes the specified bundle.|
|g11n-pipeline.bundle-language.create|Uploads resource entries.|
|g11n-pipeline.bundle-language.read|Gets the resource strings (key/value pairs) for the language.|
|g11n-pipeline.bundle-language.update|Updates resource entries.|
|g11n-pipeline.bundle-language.read|Gets the resource entry information.|
|g11n-pipeline.bundle-language.update|Updates the resource entry.|

## List of events: Bundle Translation Request Events
{: #gpevents_bundle_tr_req}

The following table lists the actions that are related to bundle translation requests and generate an event:

|Action|Description|
|---|---|  
|g11n-pipeline.trs.read|Gets a list of translation requests.|
|g11n-pipeline.tr.read|Gets the specified translation request's information.|
|g11n-pipeline.tr.update|Updates the specified translation request's information.|
|g11n-pipeline.tr.delete|Deletes the specified translation request.|
|g11n-pipeline.tr-bundle.read|Gets the bundle's information.|
|g11n-pipeline.tr-bundle-language.read|Gets resource entries for the specified bundle and language.|
|g11n-pipeline.tr-bundle-language.read|Gets the resource entry information.|
|g11n-pipeline.trs.create|Creates a new translation request.|


## List of events: Bundle xliff events
{: #gpevents_bundle_xliff}

The following table lists the actions that are related to bundle xliff and generate an event:

|Action|Description|
|---|---|  
|g11n-pipeline.xliff-bundles.read|Gets resource data in the specified language from the bundles in XLIFF 2.0 format.|
|g11n-pipeline.xliff-bundles.update|Updates bundles in the service instance with the XLIFF data.|
|g11n-pipeline.xliff-tr-bundles.read|Gets resource data in the specified language in the translation request in XLIFF 2.0 format.|


## List of events: Partner events
{: #gpevents_partner}

The following table lists the actions that are related to partners and generate an event:

|Action|Description|
|---|---|  
|g11n-pipeline.partner.read|Gets the partner's information.|
|g11n-pipeline.partner.update|Updates the partner's information.|
|g11n-pipeline.partner-trs.read|Gets a list of translation requests assigned to the partner.|
|g11n-pipeline.partner-tr.read|Gets the specified translation request's information.|
|g11n-pipeline.partner-tr.update|Updates the specified translation request's information.|
|g11n-pipeline.partner-tr.delete|Deletes the specified translation request.|
|g11n-pipeline.partner-tr-bundle.read|Gets the bundle's information.|
|g11n-pipeline.partner-tr-bundle-language.read|Gets resource entries for the specified bundle and language.|
|g11n-pipeline.partner-tr-bundle-language.update|Updates resource entries for the specified bundle and language.|
|g11n-pipeline.partner-tr-bundle-language.read|Gets the resource entry information.|
|g11n-pipeline.partner-tr-bundle-language.update|Updates the resource entry.|
|g11n-pipeline.partner-users.read|Gets available users for this partner.|
|g11n-pipeline.partner-user.read|Gets the specified partner user's information.|
|g11n-pipeline.partner-user.update|Update a partner user's information.|
|g11n-pipeline.partner-user.delete|Deletes the specified partner user.|
|g11n-pipeline.partner-user.create|Creates a new partner user.|
|g11n-pipeline.partner-tr-xliff-bundles.update|Updates resource data in the translation request with the XLIFF data.|
|g11n-pipeline.partner-tr-xliff-bundles-language.read|Gets resource data in the specified language in the translation request in XLIFF 2.0 format.|



## List of events: admin events
{: #gpevents_admin}

The following table lists the actions that are related to administrator and generate an event:

|Action|Description|
|---|---|  
|g11n-pipeline.instances.read|Gets a list of service instances.|
|g11n-pipeline.instance.read|Gets the service instance's information.|
|g11n-pipeline.instance.update|Updates the service instance's configuration.|
|g11n-pipeline.instance.create|Creates a new service instance.|
|g11n-pipeline.instance.delete|Deletes the specified service instance.|
|g11n-pipeline.instance.create|Creates a new Cloud Foundry managed service instance.|
|g11n-pipeline.partners.read|Gets a list of partners.|
|g11n-pipeline.partner.create|Creates a new partner.|
|g11n-pipeline.partner.delete|Deletes the specified partner.|



## List of events: User events
{: #gpevents_user}

The following table lists the actions that are related to users and generate an event:

|Action|Description|
|---|---|  
|g11n-pipeline.instance-users.read|Gets users in this service instance.|
|g11n-pipeline.instance-user.read|Gets the specified user's information.|
|g11n-pipeline.instance-user.update|Update a user's information.|
|g11n-pipeline.instance-user.delete|Deletes the specified user.|
|g11n-pipeline.instance-users.create|Creates a new user.|


## List of events: Config events
{: #gpevents_config}

The following table lists the actions that are related to translation configuration and generate an event:

|Action|Description|
|---|---|  
|g11n-pipeline.config-mts.read|Gets all MT service bindings.|
|g11n-pipeline.config-mt.read|Gets the MT service binding data.|
|g11n-pipeline.config-translations.read|Gets all translation configurations.|
|g11n-pipeline.config-translation.read|Gets the translation configuration.|
|g11n-pipeline.config-mt.update|Puts the specified MT service binding data. If the specified binding data already exists, it is replaced by the specified MT service binding data.|
|g11n-pipeline.config-mt.delete|Deletes the specified MT service binding data.|
|g11n-pipeline.config-translation.update|Puts the translation configuration for the specified language pair. If the configuration for the pair already exists, it is replaced by the specified configuration.|
|g11n-pipeline.config-translation.delete|Deletes the translation configuration for the specified language pair.|


## List of events: Instance events
{: #gpevents_instance}

The following table lists the actions that are related to instances and generate an event:

|Action|Description|
|---|---|  
|g11n-pipeline.instance.read|Gets this translation service instance's information.|


## Where to look for the events
{: #gp_at_ui}

{{site.data.keyword.cloudaccesstrailshort}} events are available in the {{site.data.keyword.cloudaccesstrailshort}} **space domain** that is available in the {{site.data.keyword.Bluemix_notm}} region where the {{site.data.keyword.GlobalizationPipeline_short}} service is provisioned. The {{site.data.keyword.cloudaccesstrailshort}} service instance and the {{site.data.keyword.GlobalizationPipeline_short}} instance must be provisioned in the same CF space.

For RC instances of {{site.data.keyword.GlobalizationPipeline_short}}, the Activity Tracker events are available in the Activity Tracker **account** domain where the events are generated in the {{site.data.keyword.Bluemix_notm}} region.
