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


# Migration d'instances de service {{site.data.keyword.GlobalizationPipeline_short}} vers un groupe de ressources
{: #rg-migration}

Les utilisateurs des instances Cloud Foundry {{site.data.keyword.GlobalizationPipeline_short}} existantes disposent de 3 mois (à partir de la date à laquelle la version de RC/IAM est disponible en production) pour migrer vers une version du service compatible avec RC/IAM.


## Avant de commencer
{: #prereqs}

Avant de commencer à migrer vos instances de service {{site.data.keyword.GlobalizationPipeline_short}}, vous devez savoir que toutes les données de l'instance de service sont préservées. Vous ne perdez rien. Après la migration, vos instances de service présentent le même état qu'avant la migration.   

Pour une présentation du processus de migration, voir [Migration d'instances de service Cloud Foundry vers un groupe de ressources](/docs/resources/instance_migration.html). 

## Procédure de migration
{: #gp_steps_migration}

1. Ouvrez le menu **Plus d'actions**.
2. Sélectionnez **Migrer** vers un groupe de ressources pour démarrer.
3. Sélectionnez un groupe de ressources.
4. Cliquez sur **Migrer** ; la migration de l'instance est effectuée automatiquement.

**Remarque :** vous ne pouvez migrer qu'une seule instance à la fois. Vous pouvez continuer à migrer les instances éligibles après avoir migré avec succès la première.

## Etapes suivantes
{: #nextsteps}

Les instances de service migrées s'affichent dans la section **Services** de votre liste de ressources. L'alias reste dans la section Cloud Foundry de la liste de ressources. Il s'agit d'une migration "in-place" (sans suppression de la version précédente) de sorte que toutes les données d'identification et données d'instance sont préservées. Vous pouvez continuer à utiliser les données d'identification générées par l'instance Cloud Foundry d'origine. 

Pour plus d'informations sur le fonctionnement de la migration, voir [Fonctionnement de la migration](/docs/resources/instance_migration.html#how).


