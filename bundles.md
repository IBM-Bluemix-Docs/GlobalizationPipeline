---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}


# Working with bundles
{: #globalizationpipeline_workingwithbundles}

Each bundle you create contains the key value pairs from your resource file and the complete set of translations that have been generated.
{:shortdesc}

The resource files you upload can be of any of the following formats and must contain content in the form of key/value pairs that represent the UI strings from your app.


* File type: *Java™ Properties files (.properties)*<br>
Example:
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
* File type: *AMD I18N (.js)*<br>
Example:
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
* File type: *JSON (.json)*<br>
Example:
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

In addition, a resource file must also adhere to these guidelines:
* Each key can be a maximum of 1023 characters.
* Each value can be a maximum of 8191 characters.
* Each bundle can contain a maximum of 1000 key / value pairs.

As you create bundles, they are added to the **Bundles** tab where you can perform additional tasks such as adding or deleting languages, viewing the translated content, and making monior edits to the translated content. 

{{site.data.keyword.GlobalizationPipeline_short}} translates your bundle contents into the languages by using the default machine translation engine. Optionally you can choose an alternative machine translation engine as described in the [Machine translation configuration](managetranslations.html#machineconfig) section. The default engine supports the following target languages:

<table>
<thead>
<tr>
<th>Target languages</th>
</tr>
</thead>
<tbody>
<tr>
<td>Chinese (Simplified)</td>
</tr>
<tr>
<td>Chinese (Traditional)</td>
</tr>
<tr>
<td>French</td>
</tr>
<tr>
<td>German</td>
</tr>
<tr>
<td>Italian</td>
</tr>
<tr>
<td>Japanese</td>
</tr>
<tr>
<td>Korean</td>
</tr>
<tr>
<td>Portuguese (Brazilian)</td>
</tr>
<tr>
<td>Spanish</td>
</tr>
</tbody>
</table>

**Note:** {{site.data.keyword.GlobalizationPipeline_short}}'s default machine translation engine only provides support for English as a source language. However, alternative machine translation engines available for configuration within {{site.data.keyword.GlobalizationPipeline_short}} support the translation of other non-English source languages/language pairs.

Once you have translated your bundle contents using machine translation, you can make minor edits within {{site.data.keyword.GlobalizationPipeline_short}} or you can submit bundles for human review and editing by professional translators. For details about submitting a request for human review and editing, see [Creating chargeable human translation request](managetranslations.html#humantranslation). 




## Selecting a bundle to work with
{: #globalizationpipeline_selectingabundle}

1. Click the **Bundles** tab to view all of the bundles that you have created.
2. Click a **Bundle ID** from the list to see more details about that bundle, or click the **View the bundles detail** icon ![Select the View the bundles detail icon to open a bundle and work with its translations](images/viewProjectDetailIcon.png)	in the Actions column.

![View all of the available bundles from the Bundles tab.](images/translationBundles.png)

After you select a bundle to work with, you can view the status of its translations, add or remove languages, edit the translations, or provide updates to the resource file.

If you no longer need a bundle, you can delete it from the **Bundles** tab. All translations that are associated with the bundle are also deleted.


