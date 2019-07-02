---

copyright:
  years:  2015, 2019
lastupdated: "2019-07-02"

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

## 存取權
{: #gp_iam_access}
如果您帳戶中的使用者要存取已啟用 {{site.data.keyword.GlobalizationPipeline_short}} RC 的服務實例，這些使用者的存取權會由 {{site.data.keyword.Bluemix_notm}} Identity and Access Management (IAM) 和/或 {{site.data.keyword.GlobalizationPipeline_short}} 鑑別進行控制。而對於 CF 實例，只能使用 {{site.data.keyword.GlobalizationPipeline_short}} 鑑別。

## {{site.data.keyword.GlobalizationPipeline_short}} 鑑別
{: #gp_iam_ca}
要使用鑑別機制，請參閱[新增 API 使用者](/docs/services/GlobalizationPipeline/managetranslations.html#adduser)。


## Identity and Access Management (IAM)
{: #gp_iam_ovw}
對於存取您帳戶中 {{site.data.keyword.GlobalizationPipeline_short}} 服務的每個使用者，必須向其指派定義了 IAM 使用者角色的存取原則。該原則確定使用者可在您所選服務或實例的環境定義中執行的動作。容許的作業由 {{site.data.keyword.Bluemix_notm}} 服務進行自訂，並定義為容許在服務上執行的動作。然後，這些動作將對映到 IAM 使用者角色。

原則可讓您在不同層次授與存取權。部分選項包括：

* 對帳戶中所有服務實例的存取權
* 對您帳戶中個別服務實例的存取權
* 對實例中特定資源的存取權
* 對您帳戶中所有已啟用 IAM 功能之服務的存取權

在定義存取原則的範圍後，可以指派角色。下表詳細描述了對映到服務存取角色的動作。藉由服務存取角色，使用者可以存取 {{site.data.keyword.GlobalizationPipeline_short}}，並能夠呼叫 {{site.data.keyword.GlobalizationPipeline_short}} 的 API。

|**角色類型**|**檢視翻譯**|**編輯翻譯**|**修改組合資訊**|**建立專業翻譯要求**|**檢視專業翻譯要求**|
|---------------|-----------------------|-----------------------|-------------------------------|----------------------------------------------|--------------------------------------------|
|讀者|是|否|否|否|否|
|撰寫者|是|是|否|否|是|
|管理員|是|是|是|是|是|
{: caption="表 1. IAM 使用者角色和動作" caption-side="top"}

目前是在服務實例層次向 IAM 使用者授權存取權，無法在組合層次容許或拒絕 IAM 使用者的存取權。要進行精細控制，請使用 {{site.data.keyword.GlobalizationPipeline_short}} 鑑別。

如需在使用者介面中指派使用者角色的相關資訊，請參閱[管理 IAM 存取](/docs/iam?topic=iam-iammanidaccser)。

### 產生 API 呼叫
{: #gp_iam_apicalls}

要產生或取得服務認證，請執行下列步驟。
1. 在 [{{site.data.keyword.Bluemix}} 儀表板](https://cloud.ibm.com/)中登入到您的 {{site.data.keyword.Bluemix}} 帳戶。
2. 在 [{{site.data.keyword.Bluemix}} 儀表板](https://cloud.ibm.com/)中按一下服務實例。
3. 按一下**服務認證**以開啟服務實例。
4. 按一下**新建認證**並遵循提示來建立新認證。
5. 建立認證後，按一下**檢視認證**。![擷取畫面顯示了有關範例 API 金鑰的資訊。](images/gp_iam_apicalls.gif)

下面是使用 IAM 鑑別呼叫 {{site.data.keyword.GlobalizationPipeline_short}} 的 API 的範例。

* 使用 IAM Bearer 記號
```
curl -X GET \
  https://gp-rest.us-south.g11n-pipeline.test.cloud.ibm.com/translate/rest/50341556337c581c208188ff8908ebc7/v2/bundles \
  -H 'Authorization: Bearer eyJjsksd…w'
```

* 使用 API 金鑰
```
curl -X GET \
  https://gp-rest.us-south.g11n-pipeline.test.cloud.ibm.com/translate/rest/50341556337c581c208188ff8908ebc7/v2/bundles \
  -H 'Authorization: API-KEY MklfrP…ACem'
```
在上面的範例中，可以獲得下列資訊：
* "50341556337c581c208188ff8908ebc7" 是 instanceId（在「認證」區段中）
* "https://gp-rest.us-south.g11n-pipeline.test.cloud.ibm.com/translate/rest" 是 url（在「認證」區段中）
* "MklfrP…ACem" 是 apikey（在「認證」區段中）
* "eyJjsksd…w" 是 IAM Bearer 記號

如需從 API 金鑰中取得 IAM Bearer 記號的指示，請參閱[使用 API 金鑰取得 {{site.data.keyword.Bluemix_notm}} IAM 記號](/docs/iam?topic=iam-iamtoken_from_apikey#iamtoken_from_apikey)。
