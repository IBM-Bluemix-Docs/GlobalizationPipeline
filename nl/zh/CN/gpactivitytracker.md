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


# {{site.data.keyword.GlobalizationPipeline_short}} {{site.data.keyword.cloudaccesstrailshort}} 事件
{: #gpat_events}

使用 {{site.data.keyword.cloudaccesstrailfull}} 服务可跟踪用户和应用程序如何与 {{site.data.keyword.Bluemix}} 中的 IBM {{site.data.keyword.GlobalizationPipeline_short}} 进行交互。
{:shortdesc}

{{site.data.keyword.cloudaccesstrailfull_notm}} 服务会记录哪些由用户发起的活动更改了 {{site.data.keyword.Bluemix_notm}} 中服务的状态。有关更多信息，请参阅 [{{site.data.keyword.cloudaccesstrailfull_notm}}](/docs/services/cloud-activity-tracker/index.html)。




## 事件列表：束事件
{: #gpevents_bundle}

下表列出了与束相关且生成事件的操作：

|操作|描述|
|---|---|  
|g11n-pipeline.bundles.read|获取束标识的列表。|
|g11n-pipeline.bundle.create|创建新束。|
|g11n-pipeline.bundle.read|获取束的信息。|
|g11n-pipeline.bundle.update|更新束的配置。|
|g11n-pipeline.bundle.delete|删除指定的束。|
|g11n-pipeline.bundle-language.create|上传资源条目。|
|g11n-pipeline.bundle-language.read|获取语言的资源字符串（键/值对）。|
|g11n-pipeline.bundle-language.update|更新资源条目。|
|g11n-pipeline.bundle-language.read|获取资源条目信息。|
|g11n-pipeline.bundle-language.update|更新资源条目。|

## 事件列表：束翻译请求事件
{: #gpevents_bundle_tr_req}

下表列出了与束翻译请求相关且生成事件的操作：

|操作|描述|
|---|---|  
|g11n-pipeline.trs.read|获取翻译请求的列表。|
|g11n-pipeline.tr.read|获取指定翻译请求的信息。|
|g11n-pipeline.tr.update|更新指定翻译请求的信息。|
|g11n-pipeline.tr.delete|删除指定的翻译请求。|
|g11n-pipeline.tr-bundle.read|获取束的信息。|
|g11n-pipeline.tr-bundle-language.read|获取指定束和语言的资源条目。|
|g11n-pipeline.tr-bundle-language.read|获取资源条目信息。|
|g11n-pipeline.trs.create|创建新的翻译请求。|


## 事件列表：束 XLIFF 事件
{: #gpevents_bundle_xliff}

下表列出了与束 XLIFF 相关且生成事件的操作：

|操作|描述|
|---|---|  
|g11n-pipeline.xliff-bundles.read|以 XLIFF 2.0 格式获取束中指定语言的资源数据。|
|g11n-pipeline.xliff-bundles.update|使用 XLIFF 数据更新服务实例中的束。|
|g11n-pipeline.xliff-tr-bundles.read|以 XLIFF 2.0 格式获取翻译请求中指定语言的资源数据。|


## 事件列表：合作伙伴事件
{: #gpevents_partner}

下表列出了与合作伙伴相关且生成事件的操作：

|操作|描述|
|---|---|  
|g11n-pipeline.partner.read|获取合作伙伴的信息。|
|g11n-pipeline.partner.update|更新合作伙伴的信息。|
|g11n-pipeline.partner-trs.read|获取分配给合作伙伴的翻译请求的列表。|
|g11n-pipeline.partner-tr.read|获取指定翻译请求的信息。|
|g11n-pipeline.partner-tr.update|更新指定翻译请求的信息。|
|g11n-pipeline.partner-tr.delete|删除指定的翻译请求。|
|g11n-pipeline.partner-tr-bundle.read|获取束的信息。|
|g11n-pipeline.partner-tr-bundle-language.read|获取指定束和语言的资源条目。|
|g11n-pipeline.partner-tr-bundle-language.update|更新指定束和语言的资源条目。|
|g11n-pipeline.partner-tr-bundle-language.read|获取资源条目信息。|
|g11n-pipeline.partner-tr-bundle-language.update|更新资源条目。|
|g11n-pipeline.partner-users.read|获取此合作伙伴的可用用户。|
|g11n-pipeline.partner-user.read|获取指定合作伙伴用户的信息。|
|g11n-pipeline.partner-user.update|更新合作伙伴用户的信息。|
|g11n-pipeline.partner-user.delete|删除指定的合作伙伴用户。|
|g11n-pipeline.partner-user.create|创建新的合作伙伴用户。|
|g11n-pipeline.partner-tr-xliff-bundles.update|使用 XLIFF 数据更新翻译请求中的资源数据。|
|g11n-pipeline.partner-tr-xliff-bundles-language.read|以 XLIFF 2.0 格式获取翻译请求中指定语言的资源数据。|



## 事件列表：管理员事件
{: #gpevents_admin}

下表列出了与管理员相关且生成事件的操作：

|操作|描述|
|---|---|  
|g11n-pipeline.instances.read|获取服务实例的列表。|
|g11n-pipeline.instance.read|获取服务实例的信息。|
|g11n-pipeline.instance.update|更新服务实例的配置。|
|g11n-pipeline.instance.create|创建新的服务实例。|
|g11n-pipeline.instance.delete|删除指定的服务实例。|
|g11n-pipeline.instance.create|创建新的 Cloud Foundry 受管服务实例。|
|g11n-pipeline.partners.read|获取合作伙伴的列表。|
|g11n-pipeline.partner.create|创建新的合作伙伴。|
|g11n-pipeline.partner.delete|删除指定的合作伙伴。|



## 事件列表：用户事件
{: #gpevents_user}

下表列出了与用户相关且生成事件的操作：

|操作|描述|
|---|---|  
|g11n-pipeline.instance-users.read|获取此服务实例中的用户。|
|g11n-pipeline.instance-user.read|获取指定用户的信息。|
|g11n-pipeline.instance-user.update|更新用户的信息。|
|g11n-pipeline.instance-user.delete|删除指定的用户。|
|g11n-pipeline.instance-users.create|创建新用户。|


## 事件列表：配置事件
{: #gpevents_config}

下表列出了与翻译配置相关且生成事件的操作：

|操作|描述|
|---|---|  
|g11n-pipeline.config-mts.read|获取所有 MT 服务绑定。|
|g11n-pipeline.config-mt.read|获取 MT 服务绑定数据。|
|g11n-pipeline.config-translations.read|获取所有翻译配置。|
|g11n-pipeline.config-translation.read|获取翻译配置。|
|g11n-pipeline.config-mt.update|放置指定的 MT 服务绑定数据。如果指定的绑定数据已存在，那么会将其替换为指定的 MT 服务绑定数据。|
|g11n-pipeline.config-mt.delete|删除指定的 MT 服务绑定数据。|
|g11n-pipeline.config-translation.update|放置指定语言对的翻译配置。如果该对的配置已存在，那么会将其替换为指定的配置。|
|g11n-pipeline.config-translation.delete|删除指定语言对的翻译配置。|


## 事件列表：实例事件
{: #gpevents_instance}

下表列出了与实例相关且生成事件的操作：

|操作|描述|
|---|---|  
|g11n-pipeline.instance.read|获取此翻译服务实例的信息。|


## 在何处查找事件
{: #gp_at_ui}

{{site.data.keyword.cloudaccesstrailshort}} 事件在 {{site.data.keyword.cloudaccesstrailshort}} **空间域**中提供，此域在供应 {{site.data.keyword.GlobalizationPipeline_short}} 服务的 {{site.data.keyword.Bluemix_notm}} 区域中可用。{{site.data.keyword.cloudaccesstrailshort}} 服务实例和 {{site.data.keyword.GlobalizationPipeline_short}} 实例必须在同一 CF 空间中进行供应。

对于 {{site.data.keyword.GlobalizationPipeline_short}} 的 RC 实例，Activity Tracker 事件在 {{site.data.keyword.Bluemix_notm}} 区域中生成这些事件的 Activity Tracker **帐户**域中提供。
