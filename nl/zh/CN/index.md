---

copyright:
  years: 2015, 2018
lastupdated: "2017-12-13"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}


# {{site.data.keyword.GlobalizationPipeline_short}} 入门
{: #globalizationpipeline}

{{site.data.keyword.GlobalizationPipeline_full}} 是一种 {{site.data.keyword.Bluemix}} 服务，通过该服务，应用程序开发者可快速将已翻译的应用程序发布给全球客户。{{site.data.keyword.GlobalizationPipeline_short}} 充当翻译存储库，用于提供机器翻译、人工复查和编辑以及 API 和 SDK，以将翻译无缝集成到 DevOps 和 Continuous Development 基础架构中，从而消除了与传统翻译流程相关联的人工和单线操作。
{:shortdesc}

使用 {{site.data.keyword.GlobalizationPipeline_short}} 服务，可以翻译在 {{site.data.keyword.Bluemix_notm}} 上部署和托管的任何应用程序，或者放开以翻译在其他云平台上托管的应用程序。

{{site.data.keyword.GlobalizationPipeline_short}} 提供仪表板界面以管理应用程序翻译，同时提供 RESTful API 以实现翻译流程完全自动化。有关 {{site.data.keyword.GlobalizationPipeline_short}} API 的信息，请参阅 [API 参考](https://gp-rest.ng.bluemix.net/translate/swagger/index.html){: new_window}。

## 选择翻译套餐
{: #globalizationpipeline_chooseplan}

开始在 {{site.data.keyword.GlobalizationPipeline_short}} 上进行翻译之前，可以选择适合的翻译套餐。

{{site.data.keyword.GlobalizationPipeline_short}} 上提供两种翻译套餐：标准套餐和专业套餐。这两种套餐都提供集成的无限基础机器翻译，以及另行付费与其他机器翻译引擎集成的能力。在专业套餐中，{{site.data.keyword.GlobalizationPipeline_short}} 额外提供专业翻译复查和编辑服务。您可以在 {{site.data.keyword.Bluemix_notm}} 中的 {{site.data.keyword.GlobalizationPipeline_short}} 套餐之间切换，同时保留所有数据。


## 估算 {{site.data.keyword.GlobalizationPipeline_short}} 数据使用情况
{: #globalizationpipeline_documentpricing}

{{site.data.keyword.GlobalizationPipeline_short}} 将您的翻译存储在后端数据库中。要估算活动数据的大小，您可以参考下面的公式：

`<expected resource data storage size in MB> ˜= 0.0005 * <number of key/value pairs in the source resource> * <number of languages including the source language>`

根据公式，典型束的大小为 `(length of key + length of value in UTF-8 = ˜40 bytes)`。

例如，如果您具有 100 个键值对且将它们翻译为 9 种语言，那么估算存储大小为 0.0005 100 (9+1) = 0.5 MB。实际大小可能会因随翻译一起存储的实际键值大小和元数据而有所不同。

使用 {{site.data.keyword.Bluemix_notm}} [定价计算器](https://console.ng.bluemix.net/?direct=classic/#/pricing/cloudOEPaneId=pricing&paneId=pricingSheet&orgGuid=127a45f4-4461-4d5b-a26b-6dc2fdd1a3a2&spaceGuid=208fb1ff-413b-4fd9-9615-e8226062d0f3)可确定每月服务成本。

**注**：使用专业套餐复查功能会使您的数据用量增加至超出先前所述值的范围。
