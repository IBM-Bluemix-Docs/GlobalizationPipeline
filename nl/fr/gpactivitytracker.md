---

copyright:
  years: 2016, 2019

lastupdated: "2019-03-20"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:codeblock: .codeblock}
{:tip: .tip}
{:download: .download}


# Evénements {{site.data.keyword.GlobalizationPipeline_short}} {{site.data.keyword.cloudaccesstrailshort}}
{: #gpat_events}

Utilisez le service {{site.data.keyword.cloudaccesstrailfull}} pour suivre la façon dont les utilisateurs et les applications interagissent avec IBM {{site.data.keyword.GlobalizationPipeline_short}} dans {{site.data.keyword.Bluemix}}.
{:shortdesc}

Le service {{site.data.keyword.cloudaccesstrailfull_notm}} enregistre des activités initiées par l'utilisateur qui change l'état d'un service dans {{site.data.keyword.Bluemix_notm}}. Pour plus d'informations, [{{site.data.keyword.cloudaccesstrailfull_notm}}](/docs/services/cloud-activity-tracker/index.html).




## Liste des événements : événements de bundle
{: #gpevents_bundle}

Le tableau suivant répertorie les actions liées à des bundles et qui génèrent un événement :

|Action|Description|
|---|---|  
|g11n-pipeline.bundles.read|Obtention de la liste des ID de bundle.|
|g11n-pipeline.bundle.create|Création d'un nouveau bundle.|
|g11n-pipeline.bundle.read|Obtention des informations relatives au bundle.|
|g11n-pipeline.bundle.update|Mise à jour de la configuration du bundle.|
|g11n-pipeline.bundle.delete|Suppression du bundle spécifié.|
|g11n-pipeline.bundle-language.create|Téléchargement d'entrées de ressource.|
|g11n-pipeline.bundle-language.read|Obtention des chaînes ressource (paires clé-valeur) de la langue.|
|g11n-pipeline.bundle-language.update|Mise à jour des entrées de ressource.|
|g11n-pipeline.bundle-language.read|Obtention des informations relatives à l'entrée de ressource.|
|g11n-pipeline.bundle-language.update|Mise à jour de l'entrée de ressource.|

## Liste des événements : événements de demande de traduction de bundle
{: #gpevents_bundle_tr_req}

Le tableau suivant répertorie les actions liées à des demandes de traduction de bundle et qui génèrent un événement :

|Action|Description|
|---|---|  
|g11n-pipeline.trs.read|Obtention de la liste des demandes de traduction.|
|g11n-pipeline.tr.read|Obtention des informations relatives à la demande de traduction spécifiée.|
|g11n-pipeline.tr.update|Mise à jour des informations relatives à la demande de traduction spécifiée.|
|g11n-pipeline.tr.delete|Suppression de la demande de traduction spécifiée.|
|g11n-pipeline.tr-bundle.read|Obtention des informations relatives au bundle.|
|g11n-pipeline.tr-bundle-language.read|Obtention des entrées de ressource pour la langue et le bundle spécifiés.|
|g11n-pipeline.tr-bundle-language.read|Obtention des informations relatives à l'entrée de ressource.|
|g11n-pipeline.trs.create|Création d'une nouvelle demande de traduction.|


## Liste des événements : événements xliff de bundle
{: #gpevents_bundle_xliff}

Le tableau suivant répertorie les actions liées aux données xliff de bundle et qui génèrent un événement :

|Action|Description|
|---|---|  
|g11n-pipeline.xliff-bundles.read|Obtention des données de ressource dans la langue spécifiée depuis les bundles au format XLIFF 2.0.|
|g11n-pipeline.xliff-bundles.update|Mise à jour des bundles dans l'instance de service avec les données XLIFF.|
|g11n-pipeline.xliff-tr-bundles.read|Obtention des données de ressource dans la langue spécifiée dans la demande de traduction au format XLIFF 2.0.|


## Liste des événements : événements de partenaire
{: #gpevents_partner}

Le tableau suivant répertorie les actions liées à des partenaires et qui génèrent un événement :

|Action|Description|
|---|---|  
|g11n-pipeline.partner.read|Obtention des informations relatives au partenaire.|
|g11n-pipeline.partner.update|Mise à jour des informations relatives au information.|
|g11n-pipeline.partner-trs.read|Obtention de la liste des demandes de traduction affectées au partenaire.|
|g11n-pipeline.partner-tr.read|Obtention des informations relatives à la demande de traduction spécifiée.|
|g11n-pipeline.partner-tr.update|Mise à jour des informations relatives à la demande de traduction spécifiée.|
|g11n-pipeline.partner-tr.delete|Suppression de la demande de traduction spécifiée.|
|g11n-pipeline.partner-tr-bundle.read|Obtention des informations relatives au bundle.|
|g11n-pipeline.partner-tr-bundle-language.read|Obtention des entrées de ressource pour la langue et le bundle spécifiés.|
|g11n-pipeline.partner-tr-bundle-language.update|Mise à jour des entrées de ressource pour la langue et le bundle spécifiés.|
|g11n-pipeline.partner-tr-bundle-language.read|Obtention des informations relatives à l'entrée de ressource.|
|g11n-pipeline.partner-tr-bundle-language.update|Mise à jour de l'entrée de ressource.|
|g11n-pipeline.partner-users.read|Obtention des utilisateurs disponibles pour ce partenaire.|
|g11n-pipeline.partner-user.read|Obtention des informations relatives aux utilisateurs partenaires.|
|g11n-pipeline.partner-user.update|Mise à jour des informations relatives à un utilisateur partenaire.|
|g11n-pipeline.partner-user.delete|Suppression de l'utilisateur partenaire spécifié.|
|g11n-pipeline.partner-user.create|Création d'un nouvel utilisateur partenaire.|
|g11n-pipeline.partner-tr-xliff-bundles.update|Mise à jour des données de ressource dans la demande de traduction avec les données XLIFF.|
|g11n-pipeline.partner-tr-xliff-bundles-language.read|Obtention des données de ressource dans la langue spécifiée dans la demande de traduction au format XLIFF 2.0.|



## Liste des événements : événements d'administrateur
{: #gpevents_admin}

Le tableau suivant répertorie les actions liées à l'administrateur et qui génèrent un événement :

|Action|Description|
|---|---|  
|g11n-pipeline.instances.read|Obtention de la liste des instances de service.|
|g11n-pipeline.instance.read|Obtention des informations relatives à l'instance de service.|
|g11n-pipeline.instance.update|Mise à jour de la configuration de l'instance de service.|
|g11n-pipeline.instance.create|Création d'une nouvelle instance de service.|
|g11n-pipeline.instance.delete|Suppression de l'instance de service spécifiée.|
|g11n-pipeline.instance.create|Création d'une nouvelle instance de service gérée par Cloud Foundry.|
|g11n-pipeline.partners.read|Obtention de la liste des partenaires.|
|g11n-pipeline.partner.create|Création d'un nouveau partenaire.|
|g11n-pipeline.partner.delete|Suppression du partenaire spécifié.|



## Liste des événements : événements d'utilisateurs
{: #gpevents_user}

Le tableau suivant répertorie les actions liées aux utilisateurs et qui génèrent un événement :

|Action|Description|
|---|---|  
|g11n-pipeline.instance-users.read|Obtention des utilisateur dans cette instance de service.|
|g11n-pipeline.instance-user.read|Obtention des informations relatives à l'utilisateur spécifié.|
|g11n-pipeline.instance-user.update|Mise à jour des informations relatives à un utilisateur.|
|g11n-pipeline.instance-user.delete|Suppression de l'utilisateur spécifié.|
|g11n-pipeline.instance-users.create|Création d'un nouvel utilisateur.|


## Liste des événements : événements de configuration
{: #gpevents_config}

Le tableau suivant répertorie les actions liées à la configuration de la traduction et qui génèrent un événement :

|Action|Description|
|---|---|  
|g11n-pipeline.config-mts.read|Obtention de toutes les liaisons de service MT.|
|g11n-pipeline.config-mt.read|Obtention des données de liaison de service MT.|
|g11n-pipeline.config-translations.read|Obtention de toutes les configurations de traduction.|
|g11n-pipeline.config-translation.read|Obtention de la configuration de traduction.|
|g11n-pipeline.config-mt.update|Insertion des données de la liaison de service MT spécifiée. Si les données de la liaison spécifiée existent déjà, elles sont remplacées par les données de la liaison de service MT spécifiée.|
|g11n-pipeline.config-mt.delete|Suppression des données de la liaison de service MT spécifiée. |
|g11n-pipeline.config-translation.update|Insertion de la configuration de traduction pour la paire de langues spécifiée. Si la configuration pour la paire de langues existe déjà, elle est remplacée par la configuration spécifiée.|
|g11n-pipeline.config-translation.delete|Suppression de la configuration de traduction pour la paire de langues spécifiée.|


## Liste des événements : événements d'instances
{: #gpevents_instance}

Le tableau suivant répertorie les actions liées aux instances et qui génèrent un événement :

|Action|Description|
|---|---|  
|g11n-pipeline.instance.read|Obtention des informations relatives à l'instance de service de traduction.|


## Où rechercher les événements ?
{: #gp_at_ui}

Les événements {{site.data.keyword.cloudaccesstrailshort}} sont disponibles dans le **domaine d'espace** {{site.data.keyword.cloudaccesstrailshort}}, accessible dans la région {{site.data.keyword.Bluemix_notm}} où le service {{site.data.keyword.GlobalizationPipeline_short}} est mis à disposition. L'instance de service {{site.data.keyword.cloudaccesstrailshort}} et l'instance {{site.data.keyword.GlobalizationPipeline_short}} doivent être mises à disposition dans le même espace Cloud Foundry.

Pour les instances RC de {{site.data.keyword.GlobalizationPipeline_short}}, les événements Activity Tracker sont disponibles dans le domaine du **compte** Activity Tracker où les événements sont générés dans la région {{site.data.keyword.Bluemix_notm}}.
