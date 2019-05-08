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


# Hochverfügbarkeit und Disaster-Recovery
{: #ha-dr}

Für den {{site.data.keyword.GlobalizationPipeline_full}}-Service steht an den {{site.data.keyword.Bluemix}}-Standorten (Dallas, Sydney, London und Frankfurt) Hochverfügbarkeit bereit.
{: shortdesc}

## Hochverfügbarkeit

Der {{site.data.keyword.GlobalizationPipeline_full}}-Service unterstützt die Hochverfügbarkeit. Der Service bietet automatische und transparente Hochverfügbarkeit mithilfe einer vorgeschalteten Lastausgleichsfunktion, die Anforderungen an die Replication Controller-Pods verteilt. 

## Disaster-Recovery

Disaster-Recovery kann dann akut werden, wenn an einem {{site.data.keyword.Bluemix}}-Standort ein signifikanter Ausfall mit potenziellem Datenverlust auftritt. Da MZR (Multi-Zone Region) nicht standortübergreifend verfügbar ist, müssen Sie warten, bis IBM einen Standort nach einem Ausfall wieder in den Onlinestatus versetzt. Wenn zugrunde liegende Datenservices durch den Ausfall beeinträchtigt sind, müssen Sie darüber hinaus warten, bis IBM diese Datenservices wiederherstellt, um Daten aus den Datenbanksicherungen wiederherzustellen. 

[Wie kann sichergestellt werden, dass keine Ausfallzeiten auftreten?](/docs/overview?topic=overview-zero-downtime#zero-downtime) enthält weitere Informationen zu den Hochverfügbarkeits- und Disaster-Recovery-Standards in {{site.data.keyword.Bluemix_notm}}. Informationen zu [Service-Level-Agreements](/docs/overview?topic=overview-zero-downtime#SLAs) sind ebenfalls verfügbar.   














