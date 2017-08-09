---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# Modification des détails de bundle
{: #modifybundles}

Lorsque vous ouvrez un bundle, vous pouvez afficher tous les détails le concernant. Toutes les langues cible contenues dans le bundle sont répertoriées, ainsi que le statut de traduction en cours pour chacune d'elles.

![La page des détails du bundle affiche des informations sur un bundle et ses traductions.](images/bundleDetails.png)

Le statut possible pour chaque langue contenue dans le bundle est In Progress, Failed ou Translated :

| Statut | Description |
|--------|-------------|
| In Progress | La traduction automatique est toujours en cours. |
| Failed | Une erreur s'est produite lors de la traduction du fichier de ressources dans la langue cible. |
| Translated | La traduction dans la langue cible est terminée. |

Vous pouvez mettre à jour le fichier de ressources que le bundle utilise, ajouter une langue cible à un bundle, supprimer une langue cible d'un bundle et télécharger les traductions générées pour une langue cible.

## Mise à jour du fichier de ressources utilisé par le bundle

1. En regard de la langue source, cliquez sur l'icône **Upload resources** ![Sélectionnez cette icône dans la colonne Actions pour télécharger un nouveau fichier de ressource](images/uploadIcon.png).
2. Cliquez sur **Browse** et sélectionnez le nouveau fichier de ressources à télécharger.
3. Sélectionnez le type de fichier de ressources que vous téléchargez :
 * Fichier de propriété Java
 * AMD I18N
 * JSON
4. Cliquez sur **Update** pour télécharger le nouveau fichier de ressources.

Les paires clé/valeur contenues dans le fichier de ressources nouveau ou mis à jour sont synchronisées avec les valeurs qui étaient déjà téléchargées. Seul le contenu nouveau ou modifié sera traduit.

## Ajout d'une langue cible à un bundle

1. Cliquez sur le bouton **Add Language**.
2. Toutes les langues cible disponibles sont affichées. Sélectionnez les langues à ajouter au bundle.

La traduction pour les langues sélectionnées va immédiatement commencer.

## Suppression d'une langue cible d'un bundle

Lorsque vous supprimez une langue cible d'un bundle, vous retirez du projet la langue cible et toutes les traductions qui lui sont associées. Dans la colonne Actions de la langue cible à retirer, cliquez sur l'icône **Remove this target language** ![Sélectionnez l'icône de dépôt dans la corbeille de cette langue source](images/trashIcon.png).

## Téléchargement des traductions générées pour une langue cible

{{site.data.keyword.GlobalizationPipeline_short}} vous offre la possibilité de procéder de différentes manières pour intégrer la traduction pour une langue cible dans votre application. Vous pouvez télécharger la traduction sous la forme d'un fichier de ressources et l'inclure dans votre génération d'application. Vous pouvez également faire référence à la traduction de manière dynamique à partir de {{site.data.keyword.GlobalizationPipeline_short}} en utilisant l'un des [SDK](https://github.com/IBM-Bluemix/gp-common) open source. 

<!-- For information on {{site.data.keyword.GlobalizationPipeline_full}} SDKs, see <link>. -->

Pour télécharger la traduction d'un fichier de ressources : 

1. Dans la colonne **Actions** de la langue cible ou source à télécharger, cliquez sur l'icône **Download the translations** ![Sélectionnez l'icône de téléchargement pour télécharger les clés source ou les traductions pour une langue cible](images/downloadIcon.png).
2. Sélectionnez un format de fichier.
3. Cliquez sur **Download**.
