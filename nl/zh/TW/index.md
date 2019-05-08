---

copyright:
  years: 2015, 2018
lastupdated: "2017-12-13"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}


# 開始使用 {{site.data.keyword.GlobalizationPipeline_short}}
{: #globalizationpipeline}

{{site.data.keyword.GlobalizationPipeline_full}} 是一項 {{site.data.keyword.Bluemix}} 服務，讓應用程式開發人員能快速地釋出翻譯過的應用程式給全球客戶。{{site.data.keyword.GlobalizationPipeline_short}} 充當翻譯儲存庫，用於提供機器翻譯、人工檢閱和編輯，也提供 API 及 SDK，以將翻譯無縫整合到 DevOps 和 Continuous Development 基礎架構中，消除了與傳統翻譯流程相關聯的人工和單線作業。
{:shortdesc}

您可以使用 {{site.data.keyword.GlobalizationPipeline_short}} 服務，來翻譯 {{site.data.keyword.Bluemix_notm}} 上部署和管理的任何應用程式，或是取消連結以翻譯在其他雲端平台上管理的應用程式。

{{site.data.keyword.GlobalizationPipeline_short}} 提供儀表板介面來管理應用程式翻譯，也提供 RESTful API 來使翻譯程序完全自動化。如需 {{site.data.keyword.GlobalizationPipeline_short}} API 的相關資訊，請參閱 [API 參考資料](https://gp-rest.ng.bluemix.net/translate/swagger/index.html){: new_window}。

## 選擇翻譯方案
{: #globalizationpipeline_chooseplan}

在開始使用 {{site.data.keyword.GlobalizationPipeline_short}} 上的翻譯之前，您可以選擇適合的翻譯方案。

在 {{site.data.keyword.GlobalizationPipeline_short}} 上有兩個可用的翻譯方案：標準方案與專業方案。這些方案都提供整合式且無限制的基本機器翻譯，以及與其他機器翻譯引擎整合的功能（要額外付費）。在專業方案中，{{site.data.keyword.GlobalizationPipeline_short}} 額外提供專業翻譯檢閱及編輯服務。您可以在 {{site.data.keyword.Bluemix_notm}} 中的 {{site.data.keyword.GlobalizationPipeline_short}} 方案之間切換，同時保留所有資料。


## 預估 {{site.data.keyword.GlobalizationPipeline_short}} 資料使用量
{: #globalizationpipeline_documentpricing}

{{site.data.keyword.GlobalizationPipeline_short}} 會將您的翻譯儲存在後端資料庫中。要預估作用中資料的大小，您可以參考下面的公式：

`<expected resource data storage size in （以 MB 為單位）> ˜= 0.0005 * <number of key/value pairs in the source resource> * <number of languages including the source language>`

根據公式，一般組合大小為 `(length of key + length of value in UTF-8 = ˜40 bytes)`。

例如，如果您有 100 個鍵值組，並將它們翻譯成 9 種語言，則預估的儲存空間大小為 0.0005 100 (9+1) = 0.5 MB。根據與翻譯一起儲存的實際鍵值大小和 meta 資料，實際大小可能會不同。

使用 {{site.data.keyword.Bluemix_notm}} [定價計算機](https://console.ng.bluemix.net/?direct=classic/#/pricing/cloudOEPaneId=pricing&paneId=pricingSheet&orgGuid=127a45f4-4461-4d5b-a26b-6dc2fdd1a3a2&spaceGuid=208fb1ff-413b-4fd9-9615-e8226062d0f3)可確定按月服務成本。

**附註**：使用專業方案檢閱特性，將會使您的資料用量超過上述數量。
