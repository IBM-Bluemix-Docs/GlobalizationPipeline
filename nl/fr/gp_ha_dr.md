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


# Haute disponibilité et récupération après sinistre
{: #ha-dr}

Le service {{site.data.keyword.GlobalizationPipeline_full}} est à haute disponibilité dans l'emplacement {{site.data.keyword.Bluemix}} (Dallas, Sydney, Londres et Francfort).
{: shortdesc}

## Haute disponibilité

Le service {{site.data.keyword.GlobalizationPipeline_full}} prend en charge la haute disponibilité. Le service obtient la haute disponibilité automatiquement et en toute transparence au moyen d'un équilibreur de charge en position frontale qui distribue les demandes aux pods dans le contrôleur de réplication.

## Récupération après sinistre

La récupération après sinistre peut devenir un problème lorsqu'un emplacement {{site.data.keyword.Bluemix}} est confronté à une défaillance majeure susceptible d'entraîner une perte de données. Etant donné que les régions multi-zone ne sont pas disponibles dans les emplacements, vous devez attendre qu'IBM remette l'emplacement en ligne lorsqu'il est devenu indisponible. Si des services de données sous-jacents ont été compromis par l'incident, vous devez également attendre qu'IBM restaure ces services de données pour récupérer les données à partir des sauvegardes de base de données.

Voir [Comment garantir une disponibilité permanente ?](/docs/overview?topic=overview-zero-downtime#zero-downtime) pour en savoir plus sur la haute disponibilité et les normes de récupération après sinistre dans {{site.data.keyword.Bluemix_notm}}. Vous pouvez également consultez les informations sur les [Accords sur les niveaux de service (SLA)](/docs/overview?topic=overview-zero-downtime#SLAs).  














