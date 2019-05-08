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


# 高可用性和灾难恢复
{: #ha-dr}

{{site.data.keyword.GlobalizationPipeline_full}} 服务在 {{site.data.keyword.Bluemix}} 位置（达拉斯、悉尼、伦敦和法兰克福）内具备高可用性。
{: shortdesc}

## 高可用性

{{site.data.keyword.GlobalizationPipeline_full}} 服务支持高可用性。该服务通过前端负载均衡器将请求分发到 Replication Controller 中的各个 pod，从而自动、透明地实现高可用性。

## 灾难恢复

如果 {{site.data.keyword.Bluemix}} 位置遇到包含潜在数据丢失的重大故障，那么灾难恢复可能会成为问题。由于多专区区域 (MZR) 不能跨位置使用，因此如果某个位置变为不可用，您必须等待 IBM 将其恢复联机。如果底层数据服务受到故障影响，您还必须等待 IBM 复原这些数据服务，以通过数据库备份来恢复数据。

请参阅[如何确保零停机时间](/docs/overview?topic=overview-zero-downtime#zero-downtime)，以了解有关 {{site.data.keyword.Bluemix_notm}} 中高可用性和灾难恢复标准的更多信息。您还可以找到有关[服务级别协议](/docs/overview?topic=overview-zero-downtime#SLAs)的信息。  














