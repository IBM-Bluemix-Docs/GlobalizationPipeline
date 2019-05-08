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


# Alta disponibilità e ripristino di emergenza
{: #ha-dr}

Il servizio {{site.data.keyword.GlobalizationPipeline_full}} è altamente disponibile all'interno delle ubicazioni {{site.data.keyword.Bluemix}} (Dallas, Sydney, Londra e Francoforte).
{: shortdesc}

## Alta disponibilità

Il servizio {{site.data.keyword.GlobalizationPipeline_full}} supporta l'alta disponibilità. Il servizio ottiene l'alta disponibilità in modo automatico e trasparente tramite il programma di bilanciamento del carico in primo piano per distribuire le richieste ai pod nel controller di replica.

## Ripristino di emergenza

Il ripristino di emergenza può diventare un problema se in un'ubicazione {{site.data.keyword.Bluemix}} si verifica un guasto significativo che include la potenziale perdita di dati. Poiché la funzione MZR (Multi-Zone Region) non è disponibile in tutte le ubicazioni, devi attendere che IBM riporti online un'ubicazione se diventa non disponibile. Se i servizi di dati sottostanti sono compromessi dal guasto, devi anche attendere che IBM ripristini tali servizi per recuperare i dati dai backup del database.

Vedi [Come posso garantire nessun tempo di inattività?](/docs/overview?topic=overview-zero-downtime#zero-downtime) per ulteriori informazioni sugli standard di alta disponibilità e ripristino di emergenza in {{site.data.keyword.Bluemix_notm}}. Puoi anche trovare informazioni relative agli [SLA (Service Level Agreement)](/docs/overview?topic=overview-zero-downtime#SLAs).  














