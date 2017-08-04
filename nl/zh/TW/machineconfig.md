---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# 機器翻譯配置
{: #machineconfig}

{{site.data.keyword.GlobalizationPipeline_full}} 支援整合替代機器翻譯服務來執行軟體組之機器翻譯的能力。如果 {{site.data.keyword.GlobalizationPipeline_short}} 所使用的預設引擎未提供您所需的特定語言，或者您偏好不同引擎所產生的機器翻譯，則新增替代服務可能十分有幫助。替代服務條款涵蓋這些服務的使用和費用。

若要新增和配置 {{site.data.keyword.GlobalizationPipeline_short}} 的替代機器翻譯服務，請從 {{site.data.keyword.GlobalizationPipeline_short}} 儀表板中選取**機器翻譯配置**標籤。

* 若要新增 {{site.data.keyword.Bluemix_notm}} 型錄中的機器翻譯服務（**Watson 語言翻譯程式**），則必須先將該服務新增至 {{site.data.keyword.Bluemix_notm}} 空間。

* 若要新增協力廠商服務，請在**機器翻譯配置**標籤上選取該服務的按鈕，並提供存取服務所需的使用者認證。

已將機器翻譯服務新增至 {{site.data.keyword.GlobalizationPipeline_short}} 之後，請完成其餘步驟來完成該服務的整合。

1. 按一下**啟用**，以開啟與該服務的整合。

2. 按一下**更新語言**，以檢視已更新的所支援目標語言清單。

3. 從目標語言清單中，選取應該執行翻譯的機器翻譯引擎。

4. 按一下**儲存**，以回到**機器翻譯配置**標籤。

使用 {{site.data.keyword.GlobalizationPipeline_short}} 配置替代服務之後，將使用該引擎開始產生已指派給該引擎的所有目標語言。 

若要停止使用替代機器翻譯引擎，請執行下列動作：

1. 從**機器翻譯配置**標籤中，按一下您要停止使用之服務的**停用**按鈕。

停用替代機器翻譯服務之後，服務已產生的所有翻譯將會保留在軟體組內。不過，如果目前已啟用的機器翻譯引擎不再支援目標語言，則未來更新可能無法再翻譯為特定目標語言。

<!-- Review comment: When you disable an engine, do you need to go back and reconfigure the languages?? Does it go back to the default engine? What happens? -->
