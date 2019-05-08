---

copyright:
  years: 2015, 2019
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


# 將 {{site.data.keyword.GlobalizationPipeline_short}} 服務實例移轉至資源群組
{: #rg-migration}

現有 {{site.data.keyword.GlobalizationPipeline_short}} CF 實例使用者有 3 個月的時間（自 RC/IAM 版本在正式作業環境中可用之日起算）移轉到 RC/IAM 相容版本的服務。


## 開始之前
{: #prereqs}

開始移轉 {{site.data.keyword.GlobalizationPipeline_short}} 服務實例之前，您應該知道該服務實例的所有資料均已保留。您不會遺失任何內容。移轉後，您可以看到服務實例的狀態與移轉之前相同。   

如需移轉程序的概觀，請參閱[將 Cloud Foundry 服務實例移轉至資源群組](/docs/resources/instance_migration.html)。 

## 移轉步驟
{: #gp_steps_migration}

1. 開啟**其他動作**功能表。
2. 首先選取**移轉**以移轉至資源群組。
3. 選取資源群組。
4. 按一下**移轉**，此時系統會為您移轉實例。

**附註：**一次只能移轉一個實例，因此可以在成功移轉第一個實例後，繼續移轉符合條件的實例。

## 後續步驟
{: #nextsteps}

您可以在資源清單的**服務**區段中看到已移轉的服務實例。別名會保留在資源清單的 Cloud Foundry 區段中。這是就地移轉，因此將保留所有實例資料和認證。您可以繼續使用原始 CF 實例產生的認證。 

如需移轉工作方式的相關資訊，請參閱[移轉的運作方式](/docs/resources/instance_migration.html#how)。


