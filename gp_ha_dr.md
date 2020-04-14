---

copyright:
  years: 2018, 2019
lastupdated: "2019-03-22"

keywords: high availability, disaster recovery, failure, loss of data, backup

subcollection: GlobalizationPipeline

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:codeblock: .codeblock}
{:tip: .tip}
{:download: .download}
{:external: target="_blank" .external}


# High availability and disaster recovery
{: #ha-dr}

The {{site.data.keyword.GlobalizationPipeline_full}} service is highly available within {{site.data.keyword.Bluemix}} location (Dallas, Sydney, London and Frankfurt).
{: shortdesc}

## High availability

The {{site.data.keyword.GlobalizationPipeline_full}} service supports high availability. The service achieves high availability automatically and transparently by means of load balancer in front to distribute requests to the Pods in the Replication Controller.

## Disaster recovery

Disaster recovery can become an issue if an {{site.data.keyword.Bluemix}} location experiences a significant failure that includes the potential loss of data. Because Multi-Zone Region (MZR) is not available across locations, you must wait for IBM to bring a location back online if it becomes unavailable. If underlying data services are compromised by the failure, you must also wait for IBM to restore those data services to recover data from database backups.

See [How do I ensure zero downtime](/docs/overview?topic=overview-zero-downtime#zero-downtime){: external} to learn more about the high availability and disaster recovery standards in {{site.data.keyword.Bluemix_notm}}. You can also find information about [Service Level Agreements](/docs/overview?topic=overview-zero-downtime#SLAs){: external}.
