---

copyright:
  years:  2015, 2019
lastupdated: "2019-03-25"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:codeblock: .codeblock}
{:tip: .tip}
{:download: .download}


# IBM Cloud IAM for {{site.data.keyword.GlobalizationPipeline_short}}
{: #gp_iam}

## 访问权
{: #gp_iam_access}
如果您帐户中的用户要访问启用 {{site.data.keyword.GlobalizationPipeline_short}} RC 的服务实例，这些用户的访问权通过 {{site.data.keyword.Bluemix_notm}} Identity and Access Management (IAM) 和/或 {{site.data.keyword.GlobalizationPipeline_short}} 认证进行控制。而对于 CF 实例，只能使用 {{site.data.keyword.GlobalizationPipeline_short}} 认证。

## {{site.data.keyword.GlobalizationPipeline_short}} 认证
{: #gp_iam_ca}
要使用认证机制，请参阅[添加 API 用户](/docs/services/GlobalizationPipeline/managetranslations.html#adduser)。


## Identity and Access Management (IAM)
{: #gp_iam_ovw}
对于访问您帐户中 {{site.data.keyword.GlobalizationPipeline_short}} 服务的每个用户，必须向其分配定义了 IAM 用户角色的访问策略。该策略确定用户可在您所选服务或实例的上下文中执行的操作。允许的操作由 {{site.data.keyword.Bluemix_notm}} 服务进行定制，并定义为允许在服务上执行的操作。然后，这些操作将映射到 IAM 用户角色。

策略支持在不同级别授予访问权。部分选项包括：

* 对帐户中所有服务实例的访问权
* 对帐户中单个服务实例的访问权
* 对实例中特定资源的访问权
* 对帐户中所有启用 IAM 的服务的访问权

在定义访问策略的作用域后，可以分配角色。下表详细描述了映射到服务访问角色的操作。通过服务访问角色，用户可以访问 {{site.data.keyword.GlobalizationPipeline_short}}，并能够调用 {{site.data.keyword.GlobalizationPipeline_short}} 的 API。

|**角色类型**|**查看翻译**|**编辑翻译**|**修改束信息**|**创建专业翻译请求**|**查看专业翻译请求**|
|---------------|-----------------------|-----------------------|-------------------------------|----------------------------------------------|--------------------------------------------|
|读取者|是|否|否|否|否|
|写入者|是|是|否|否|是|
|管理者|是|是|是|是|是|
{: caption="表 1. IAM 用户角色和操作" caption-side="top"}

目前是在服务实例级别向 IAM 用户授予访问权，无法在束级别允许或拒绝 IAM 用户的访问权。要进行细颗粒度控制，请使用 {{site.data.keyword.GlobalizationPipeline_short}} 认证。

有关在 UI 中分配用户角色的信息，请参阅[管理 IAM 访问权](/docs/iam/iammanidaccser.html#iammanidaccser)。

### 生成 API 调用
{: #gp_iam_apicalls}

要生成或获取服务凭证，请执行以下步骤。
1. 在 [{{site.data.keyword.Bluemix}} 仪表板](https://cloud.ibm.com/)中登录到您的 {{site.data.keyword.Bluemix}} 帐户。
2. 在 [{{site.data.keyword.Bluemix}} 仪表板](https://cloud.ibm.com/)中单击服务实例。
3. 单击**服务凭证**以打开服务实例。 
4. 单击**新建凭证**并遵循提示来创建新凭证。
5. 创建凭证后，单击**查看凭证**。![屏幕快照显示了有关样本 API 密钥的信息。](images/gp_iam_apicalls.gif)

下面是使用 IAM 认证调用 {{site.data.keyword.GlobalizationPipeline_short}} 的 API 的示例。

* 使用 IAM 不记名令牌
```
curl -X GET \
  https://gp-rest.us-south.g11n-pipeline.test.cloud.ibm.com/translate/rest/50341556337c581c208188ff8908ebc7/v2/bundles \
  -H 'Authorization: Bearer eyJjsksd…w'
```

* 使用 API 密钥
```
curl -X GET \
  https://gp-rest.us-south.g11n-pipeline.test.cloud.ibm.com/translate/rest/50341556337c581c208188ff8908ebc7/v2/bundles \
  -H 'Authorization: API-KEY MklfrP…ACem'
```
在上面的示例中，可以获得以下信息：
* “50341556337c581c208188ff8908ebc7”是 instanceId（在“凭证”部分中）
* “https://gp-rest.us-south.g11n-pipeline.test.cloud.ibm.com/translate/rest”是 url（在“凭证”部分中）
* “MklfrP…ACem”是 apikey（在“凭证”部分中）
* “eyJjsksd…w”是 IAM 不记名令牌

有关从 API 密钥中获取 IAM 不记名令牌的指示信息，请参阅[使用 API 密钥获取 {{site.data.keyword.Bluemix_notm}} IAM 令牌](/docs/iam?topic=iam-iamtoken_from_apikey#iamtoken_from_apikey)。
