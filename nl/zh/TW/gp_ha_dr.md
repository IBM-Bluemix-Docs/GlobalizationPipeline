---

copyright:
  years: 2018, 2019
lastupdated: "2019-03-22"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:codeblock: .codeblock}
{:tip: .tip}
{:download: .download}


# 高可用性和災難回復
{: #ha-dr}

{{site.data.keyword.GlobalizationPipeline_full}} 服務在 {{site.data.keyword.Bluemix}} 位置（達拉斯、雪梨、倫敦和法蘭克福）內具備高可用性。
{: shortdesc}

## 高可用性

{{site.data.keyword.GlobalizationPipeline_full}} 服務支援高可用性。該服務藉由前端負載均衡器將要求分散到 Replication Controller 中的各個 Pod，自動、透明地實現高可用性。

## 災難回復

如果 {{site.data.keyword.Bluemix}} 位置遇到包含潛在資料遺失的重大故障，那麼災難回復可能會成為問題。由於多區域地區 (MZR) 不能跨位置使用，因此如果某個位置變為無法使用，您必須等待 IBM 將其恢復連線。如果基礎資料服務受到故障影響，您還必須等待 IBM 還原這些資料服務，以從資料庫備份來回復資料。

請參閱[如何確保運作零中斷](/docs/overview?topic=overview-zero-downtime#zero-downtime)，以瞭解有關 {{site.data.keyword.Bluemix_notm}} 中高可用性和災難回復標準的更多資訊。您也可以找到[服務水準合約](/docs/overview?topic=overview-zero-downtime#SLAs)的相關資訊。  














