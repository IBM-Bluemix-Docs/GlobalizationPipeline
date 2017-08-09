---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}


# Gestion des bundles
{: #globalizationpipeline_workingwithbundles}

Chaque bundle que vous créez contient les paires clé/valeur de votre fichier de ressources et le jeu complet de traductions qui a été généré.
{:shortdesc}

Les fichiers de ressources que vous téléchargez peuvent correspondre à n'importe lequel des formats suivants et leur contenu doit se présenter sous la forme de paires clé/valeur qui représentent les chaînes d'interface utilisateur de votre application.


* Type de fichier : *Fichiers de propriétés Java (.properties)*<br>
Exemple :
```js
logout=Logout
back=Back
examples=Menu
home=Home
web=Web
enterprise=Enterprise
extra=Resources
about=About
settings=Settings
help=Help
support=Support
topics=Topics
appExitMsg=Are you sure you want to quit the application?
```
* Type de fichier : *AMD I18N (.js)*<br>
Exemple :
```js
define({
    "root": {
       logout: "Logout",
       back: "Back",
       examples: "Menu",
       home: "Home",
       web: "Web",
       enterprise: "Enterprise",
       extra: "Resources",
       about: "About",
       settings: "Settings",
       help: "Help",
       support: "Support",
       topics: "Topics",
       appExitMsg: "Are you sure you want to quit the application?"
    }
});
``` 
* Type de fichier : *JSON (.json)*<br>
Exemple :
```js
{
  "logout": "Logout",
  "back": "Back",
  "examples": "Menu",
  "home": "Home",
  "web": "Web",
  "enterprise": "Enterprise",
  "extra": "Resources",
  "about": "About",
  "settings": "Settings",
  "help": "Help",
  "support": "Support",
  "topics": "Topics",
  "appExitMsg": "Are you sure you want to quit the application?"
}
``` 

De plus, un fichier de ressources doit également être conforme aux instructions suivantes :
* Chaque clé peut comporter au maximum 1023 caractères.
* Chaque valeur peut comporter 8191 caractères maximum.
* Chaque bundle peut contenir au maximum 1000 paires clé / valeur.

Lorsque vous créez des bundles, ils sont ajoutés à l'onglet **Bundles** depuis lequel vous pouvez effectuer des tâches supplémentaires comme l'ajout ou la suppression de langues, l'affichage du contenu traduit et apporter des modifications mineures à ce contenu. 

{{site.data.keyword.GlobalizationPipeline_short}} traduit le contenu de votre bundle vers les langues désignées à l'aide du moteur de traduction automatique par défaut. Vous pouvez éventuellement choisir un autre moteur de traduction automatique, comme indiqué dans la section [Configuration de la traduction automatique](managetranslations.html#machineconfig). Le moteur par défaut est compatible avec les langues cible suivantes :

<table>
<thead>
<tr>
<th>Langues cible</th>
</tr>
</thead>
<tbody>
<tr>
<td>Chinois (simplifié)</td>
</tr>
<tr>
<td>Chinois (traditionnel)</td>
</tr>
<tr>
<td>Français</td>
</tr>
<tr>
<td>Allemand</td>
</tr>
<tr>
<td>Italien</td>
</tr>
<tr>
<td>Japonais</td>
</tr>
<tr>
<td>Coréen</td>
</tr>
<tr>
<td>Portugais (Brésil)</td>
</tr>
<tr>
<td>Espagnol</td>
</tr>
</tbody>
</table>

**Remarque : ** le moteur de traduction automatique par défaut de {{site.data.keyword.GlobalizationPipeline_short}} ne fournit une prise en charge que pour l'anglais comme langue source. Toutefois, d'autres moteurs de traduction automatique disponibles pour configuration au sein de {{site.data.keyword.GlobalizationPipeline_short}} prennent en charge la traduction d'autres paires de langues, avec une langue source différente de l'anglais.

Une fois que vous avez traduit le contenu de votre bundle via la traduction automatique, vous pouvez apporter des modifications mineures à ce contenu dans {{site.data.keyword.GlobalizationPipeline_short}} ou soumettre les bundles pour revue et édition humaine par des traducteurs professionnels. Pour plus d'informations sur la soumission d'une demande de revue et d'édition humaine, voir [Création d'une demande de traduction humaine facturable](managetranslations.html#humantranslation). 




## Sélection d'un bundle à gérer
{: #globalizationpipeline_selectingabundle}

1. Cliquez sur l'onglet **Bundles** pour afficher tous les bundles que vous avez créés.
2. Cliquez sur un **ID de bundle** dans la liste pour afficher plus de détails sur ce bundle ou cliquez sur l'icône **View the bundles detail** ![Sélectionnez dans la colonne Actions l'icône d'affichage des détails des bundles pour ouvrir un bundle et gérer ses traductions](images/viewProjectDetailIcon.png).

![Affichage de tous les bundles disponibles dans l'onglet Bundles.](images/translationBundles.png)

Après avoir sélectionné un bundle à gérer, vous pouvez afficher le statut de ses traductions, ajouter ou retirer des langues, éditer les traductions ou appliquer des mises à jour au fichier de ressources.

Si vous n'avez plus besoin d'un bundle, vous pouvez le supprimer à partir de l'onglet **Bundles**. Toutes les traductions qui sont associées au bundle sont également supprimées.


