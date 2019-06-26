---

copyright:
  years: 2016, 2019

lastupdated: "2019-06-26"

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

使用 {{site.data.keyword.cloudaccesstrailfull}} 服務可追蹤使用者和應用程式如何與 {{site.data.keyword.Bluemix}} 中的 IBM {{site.data.keyword.GlobalizationPipeline_short}} 進行交互。
{:shortdesc}

{{site.data.keyword.cloudaccesstrailfull_notm}} 服務會記錄由使用者起始，且會變更 {{site.data.keyword.Bluemix_notm}} 中服務狀態的活動。如需相關資訊，請參閱 [{{site.data.keyword.cloudaccesstrailfull_notm}}](/docs/services/Activity-Tracker-with-LogDNA?topic=logdnaat-getting-started)。




## 事件清單：組合事件
{: #gpevents_bundle}

下表列出了與組合相關且產生事件的動作：

|動作|說明|
|---|---|  
|g11n-pipeline.bundles.read|取得組合 ID 的清單。|
|g11n-pipeline.bundle.create|建立新組合。|
|g11n-pipeline.bundle.read|取得組合的資訊。|
|g11n-pipeline.bundle.update|更新組合的配置。|
|g11n-pipeline.bundle.delete|刪除指定的組合。|
|g11n-pipeline.bundle-language.create|上傳資源項目。|
|g11n-pipeline.bundle-language.read|取得語言的資源字串（鍵值組）。|
|g11n-pipeline.bundle-language.update|更新資源項目。|
|g11n-pipeline.bundle-language.read|取得資源項目資訊。|
|g11n-pipeline.bundle-language.update|更新資源項目。|

## 事件清單：組合翻譯要求事件
{: #gpevents_bundle_tr_req}

下表列出了與組合翻譯要求相關且產生事件的動作：

|動作|說明|
|---|---|  
|g11n-pipeline.trs.read|取得翻譯要求的清單。|
|g11n-pipeline.tr.read|取得指定翻譯要求的資訊。|
|g11n-pipeline.tr.update|更新指定翻譯要求的資訊。|
|g11n-pipeline.tr.delete|刪除指定的翻譯要求。|
|g11n-pipeline.tr-bundle.read|取得組合的資訊。|
|g11n-pipeline.tr-bundle-language.read|取得指定組合和語言的資源項目。|
|g11n-pipeline.tr-bundle-language.read|取得資源項目資訊。|
|g11n-pipeline.trs.create|建立新的翻譯要求。|


## 事件清單：組合 XLIFF 事件
{: #gpevents_bundle_xliff}

下表列出了與組合 XLIFF 相關且產生事件的動作：

|動作|說明|
|---|---|  
|g11n-pipeline.xliff-bundles.read|以 XLIFF 2.0 格式取得組合中指定語言的資源資料。|
|g11n-pipeline.xliff-bundles.update|使用 XLIFF 資料更新服務實例中的組合。|
|g11n-pipeline.xliff-tr-bundles.read|以 XLIFF 2.0 格式取得翻譯要求中指定語言的資源資料。|


## 事件清單：夥伴事件
{: #gpevents_partner}

下表列出了與夥伴相關且產生事件的動作：

|動作|說明|
|---|---|  
|g11n-pipeline.partner.read|取得夥伴的資訊。|
|g11n-pipeline.partner.update|更新夥伴的資訊。|
|g11n-pipeline.partner-trs.read|取得指派給夥伴的翻譯要求的清單。|
|g11n-pipeline.partner-tr.read|取得指定翻譯要求的資訊。|
|g11n-pipeline.partner-tr.update|更新指定翻譯要求的資訊。|
|g11n-pipeline.partner-tr.delete|刪除指定的翻譯要求。|
|g11n-pipeline.partner-tr-bundle.read|取得組合的資訊。|
|g11n-pipeline.partner-tr-bundle-language.read|取得指定組合和語言的資源項目。|
|g11n-pipeline.partner-tr-bundle-language.update|更新指定組合和語言的資源項目。|
|g11n-pipeline.partner-tr-bundle-language.read|取得資源項目資訊。|
|g11n-pipeline.partner-tr-bundle-language.update|更新資源項目。|
|g11n-pipeline.partner-users.read|取得此夥伴的可用使用者。|
|g11n-pipeline.partner-user.read|取得指定夥伴使用者的資訊。|
|g11n-pipeline.partner-user.update|更新夥伴使用者的資訊。|
|g11n-pipeline.partner-user.delete|刪除指定的夥伴使用者。|
|g11n-pipeline.partner-user.create|建立新的夥伴使用者。|
|g11n-pipeline.partner-tr-xliff-bundles.update|使用 XLIFF 資料更新翻譯要求中的資源資料。|
|g11n-pipeline.partner-tr-xliff-bundles-language.read|以 XLIFF 2.0 格式取得翻譯要求中指定語言的資源資料。|



## 事件清單：管理事件
{: #gpevents_admin}

下表列出了與管理者相關且產生事件的動作：

|動作|說明|
|---|---|  
|g11n-pipeline.instances.read|取得服務實例的清單。|
|g11n-pipeline.instance.read|取得服務實例的資訊。|
|g11n-pipeline.instance.update|更新服務實例的配置。|
|g11n-pipeline.instance.create|建立新的服務實例。|
|g11n-pipeline.instance.delete|刪除指定的服務實例。|
|g11n-pipeline.instance.create|建立新的 Cloud Foundry 受管服務實例。|
|g11n-pipeline.partners.read|取得夥伴的清單。|
|g11n-pipeline.partner.create|建立新的夥伴。|
|g11n-pipeline.partner.delete|刪除指定的夥伴。|



## 事件清單：使用者事件
{: #gpevents_user}

下表列出了與使用者相關且產生事件的動作：

|動作|說明|
|---|---|  
|g11n-pipeline.instance-users.read|取得此服務實例中的使用者。|
|g11n-pipeline.instance-user.read|取得指定使用者的資訊。|
|g11n-pipeline.instance-user.update|更新使用者的資訊。|
|g11n-pipeline.instance-user.delete|刪除指定的使用者。|
|g11n-pipeline.instance-users.create|建立新使用者。|


## 事件清單：配置事件
{: #gpevents_config}

下表列出了與翻譯配置相關且產生事件的動作：

|動作|說明|
|---|---|  
|g11n-pipeline.config-mts.read|取得所有 MT 服務連結。|
|g11n-pipeline.config-mt.read|取得 MT 服務連結資料。|
|g11n-pipeline.config-translations.read|取得所有翻譯配置。|
|g11n-pipeline.config-translation.read|取得翻譯配置。|
|g11n-pipeline.config-mt.update|放置指定的 MT 服務連結資料。如果指定的連結資料已存在，那麼會將其取代為指定的 MT 服務連結資料。|
|g11n-pipeline.config-mt.delete|刪除指定的 MT 服務連結資料。|
|g11n-pipeline.config-translation.update|放置指定語言配對的翻譯配置。如果該配置的配置已存在，那麼會將其取代為指定的配置。|
|g11n-pipeline.config-translation.delete|刪除指定語言配對的翻譯配置。|


## 事件清單：實例事件
{: #gpevents_instance}

下表列出了與實例相關且產生事件的動作：

|動作|說明|
|---|---|  
|g11n-pipeline.instance.read|取得此翻譯服務實例的資訊。|


## 尋找事件的位置
{: #gp_at_ui}

{{site.data.keyword.cloudaccesstrailshort}} 事件在 {{site.data.keyword.cloudaccesstrailshort}} **空間網域**中提供，此網域在佈建 {{site.data.keyword.GlobalizationPipeline_short}} 服務的 {{site.data.keyword.Bluemix_notm}} 地區中可用。{{site.data.keyword.cloudaccesstrailshort}} 服務實例和 {{site.data.keyword.GlobalizationPipeline_short}} 實例必須在同一 CF 空間中進行佈建。

對於 {{site.data.keyword.GlobalizationPipeline_short}} 的 RC 實例，Activity Tracker 事件在 {{site.data.keyword.Bluemix_notm}} 地區中產生這些事件的 Activity Tracker **帳戶**網域中提供。
