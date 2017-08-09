---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

 
# Initiation à {{site.data.keyword.GlobalizationPipeline_short}}
{: #globalizationpipeline}

{{site.data.keyword.GlobalizationPipeline_full}} est un service {{site.data.keyword.Bluemix}} qui permet aux développeurs d'applications de livrer rapidement des applications traduites à des clients avec un marché global. {{site.data.keyword.GlobalizationPipeline_short}} propose une traduction automatique, une revue et une édition humaine, et des API et des SDK pour intégrer de manière transparente les traductions dans votre infrastructure DevOps et Continuous Development, en éliminant les opérations manuelles et cloisonnées associées au processus de traduction traditionnel.
{:shortdesc}

Vous pouvez utiliser le service {{site.data.keyword.GlobalizationPipeline_short}} pour traduire n'importe quelle application déployée et hébergée sur {{site.data.keyword.Bluemix}}, ou les dissocier pour traduire des applications hébergées sur d'autres plateformes cloud.

{{site.data.keyword.GlobalizationPipeline_short}} offre une interface de tableau de bord pour gérer votre traduction d'application  , ainsi qu'une API RESTful automatisant entièrement le processus de traduction. Pour plus d'informations sur l'API {{site.data.keyword.GlobalizationPipeline_short}}, voir [Référence d'API](https://gp-rest.ng.bluemix.net/translate/swagger/index.html){: new_window}. 

## Sélection d'un plan de traduction
{: #globalizationpipeline_chooseplan}

Avant de commencer à travailler sur vos traductions dans {{site.data.keyword.GlobalizationPipeline_short}}, vous pouvez choisir un plan de traduction adapté.

Deux plans de traduction sont disponibles dans {{site.data.keyword.GlobalizationPipeline_short}} : le plan Standard et le plan Professional. Les deux permettent une traduction automatique de base illimitée, tout comme une possibilité d'intégration avec d'autres moteurs de traduction automatique au prix d'une redevance supplémentaire. Dans le plan Professional, {{site.data.keyword.GlobalizationPipeline_short}} propose également un service professionnel de révision et d'édition des traductions. Vous pouvez basculer entre les plans {{site.data.keyword.GlobalizationPipeline_short}} dans Bluemix en conservant toutes vos données. 


## Estimation de l'utilisation des données {{site.data.keyword.GlobalizationPipeline_short}}
{: #globalizationpipeline_documentpricing}

{{site.data.keyword.GlobalizationPipeline_short}} stocke vos traductions dans une base de données de back end. Pour estimer la taille des données actives, vous pouvez vous référer à la formule ci-dessous :

`<expected resource data storage size in MB> ˜= 0.0005 * <number of key/value pairs in the source resource> * <number of languages including the source language>`

En fonction de la formule, la taille d'un bundle typique est `longueur de clé + longueur de valeur en UTF-8 = ˜40  octets)à`.

Par exemple, si vous disposez des 100 paires clé/valeur et que vous les traduisez dans 9 langues, la taille de stockage estimée est : 0,0005 100 (9+1) = 0,5 Mo. La taille réelle peut être différente selon la taille clé/valeur réelle et les métadonnées stockées avec la traduction.

Utilisez la [calculatrice de prix](https://console.ng.bluemix.net/?direct=classic/#/pricing/cloudOEPaneId=pricing&paneId=pricingSheet&orgGuid=127a45f4-4461-4d5b-a26b-6dc2fdd1a3a2&spaceGuid=208fb1ff-413b-4fd9-9615-e8226062d0f3) de Bluemix pour déterminer quels seront vos coûts de service mensuels.

**Remarque **: l'utilisation de la fonction de revue du plan Professional augmentera votre utilisation de données au-delà des évaluations mentionnées ci-dessus.



