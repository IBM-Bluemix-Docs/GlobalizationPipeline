---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# Configuration de la traduction automatique
{: #machineconfig}

{{site.data.keyword.GlobalizationPipeline_full}} prend en charge la possibilité d'intégrer d'autres services de traduction automatique afin d'effectuer la traduction automatique pour vos bundles. Il est pratique de pouvoir ajouter un autre service si le moteur utilisé par défaut par {{site.data.keyword.GlobalizationPipeline_short}} ne propose pas une langue dont vous avez besoin ou si vous préférez les traductions automatiques qui sont générées par un autre moteur. L'utilisation et les frais relatifs aux autres services sont traités dans la section sur les conditions d'utilisation de ces services.

Pour ajouter et configurer un autre service de traduction automatique pour {{site.data.keyword.GlobalizationPipeline_short}}, sélectionnez l'onglet **Machine Translation Configuration** du tableau de bord {{site.data.keyword.GlobalizationPipeline_short}}.

* Pour pouvoir ajouter un service de traduction automatique figurant dans le catalogue {{site.data.keyword.Bluemix_notm}} (**Watson Language Translator**), vous devez d'abord l'ajouter à votre espace {{site.data.keyword.Bluemix_notm}}.

* Pour ajouter un service tiers, sélectionnez le bouton correspondant à ce service sur l'onglet **Machine Translation Configuration** et indiquez les données d'identification de l'utilisateur requises pour accéder au service.

Après avoir ajouté un service de traduction automatique à {{site.data.keyword.GlobalizationPipeline_short}}, exécutez les étapes restantes pour finaliser l'intégration de ce service.

1. Cliquez sur **Enable** pour activer l'intégration à ce service.

2. Cliquez sur **Update Languages** pour visualiser la liste mise à jour des langues cible prises en charge.

3. Dans la liste des langues cible, sélectionnez le moteur de traduction automatique qui doit effectuer la traduction.

4. Cliquez sur **Save** pour revenir à l'onglet **Machine Translation Configuration**.

Une fois qu'un autre service a été configuré avec {{site.data.keyword.GlobalizationPipeline_short}}, toutes les langues cible qui ont été affectées à ce moteur commencent à être générées à l'aide de ce moteur. 

Pour cesser d'utiliser un autre moteur de traduction automatique :

1. Sur l'onglet **Machine Translation Configuration**, cliquez sur le bouton **Disable** pour le service que vous souhaitez cesser d'utiliser.

Une fois qu'un autre service de traduction est désactivé, toutes les traductions qu'il a générées sont conservées dans vos bundles. En revanche, il se peut que la traduction dans une langue cible donnée ne soit pas disponible pour des mises à jour ultérieures si cette langue cible n'est plus prise en charge par le moteur de traduction automatique qui est actuellement activé.

<!-- Review comment: When you disable an engine, do you need to go back and reconfigure the languages?? Does it go back to the default engine? What happens? -->
