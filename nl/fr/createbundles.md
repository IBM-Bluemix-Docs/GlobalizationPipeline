---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# Création d'un bundle
{: #createbundles}

Pour entamer votre traduction, créez des bundles et téléchargez des fichiers de ressources de votre application devant être traduits par {{site.data.keyword.GlobalizationPipeline_short}}. Les fichiers de ressources peuvent être des fichiers de propriétés Java, des fichiers AMD I18N ou des fichiers JSON et leur contenu doit se présenter sous la forme de paires clé/valeur qui représentent les chaînes d'interface utilisateur de votre application.  Pour obtenir plus d'informations et des exemples des types de fichiers pris en charge, voir [Utilisation de bundles](./bundles.html){: new_window}.

Pour créer un bundle, procédez comme suit :

<ol>
<li>Sur l'onglet <strong>Overview</strong>, cliquez sur <strong>New Bundle</strong>.</li>

<li>Entrez des informations sur votre bundle :
<table>
<thead>
<tr>
<th>Champ</th>
<th>Obligatoire</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Bundle ID</strong></td>
<td>Oui</td>
<td>Nom unique permettant d'identifier le bundle.</td>
</tr>
<tr>
<td><strong>Source language</strong></td>
<td>Oui</td>
<td>Langue d'origine du fichier source.</td>
</tr>
<tr>
<td><strong>Resource File</strong></td>
<td>Non</td>
<td><a href=https://new-console.stage1.ng.bluemix.net/docs/services/GlobalizationPipeline/bundles.html>Fichier de ressources</a> à traduire. La taille de fichier maximale est limitée à 2 Mo. Les fichiers de ressources spécifiés seront téléchargés.</td>
</tr>
<tr>
<td><strong>File format</strong></td>
<td>Non</td>
<td>Type de fichier téléchargé.</td>
</tr>
<tr>
<td><strong>Target language</strong></td>
<td>Non</td>
<td>Langue dans laquelle vous souhaitez effectuer la traduction.</td>
</tr>
</tbody>
</table>

<p><strong>Remarque :</strong> Pour modifier le service de langue qui fournit la traduction automatique pour vos bundles, cliquez sur l'onglet <a href=https://new-console.stage1.ng.bluemix.net/docs/services/GlobalizationPipeline/managing_translations.html#globalizationpipeline_service_to_service>MT Configuration</a> pour afficher les autres moteurs de traduction automatique pris en charge.</p></li>

<li>Cliquez sur <strong>Sauvegarder</strong></li></ol>


Une fois le bundle créé, le fichier de ressources téléchargé est traduit dans toutes les langues cible que vous avez spécifiées. Le nouveau bundle est ajouté à l'onglet Bundles à partir duquel vous pouvez effectuer les actions suivantes :

* Ajouter ou retirer des langues
* Editer les traductions générées
* Mettre à jour le fichier source qui est utilisé dans le bundle et régénérer les traductions
