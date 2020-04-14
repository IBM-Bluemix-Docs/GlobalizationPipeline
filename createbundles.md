---

copyright:
  years: 2015, 2020
lastupdated: "2020-04-14"

keywords: bundle, create a bundle, key value pairs, resource file, ui string, translation

subcollection: GlobalizationPipeline

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# Creating a bundle
{: #createbundles}

To get started with translation, you create bundles and upload resource files of your app that need to be translated by {{site.data.keyword.GlobalizationPipeline_short}}. The resource files can be either Java Properties, AMD I18N, or JSON files and must contain content in the form of key/value pairs that represent the UI strings from your app.  For more details and examples of supported file types, see [Working with bundles](/docs/GlobalizationPipeline?topic=GlobalizationPipeline-globalizationpipeline_workingwithbundles).

To create a bundle, complete the following steps:

<ol>
<li>From the <strong>Overview</strong> tab, click <strong>New Bundle</strong>.</li>

<li>Provide information about your bundle:
<table>
<thead>
<tr>
<th>Field</th>
<th>Required</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Bundle ID</strong></td>
<td>Yes</td>
<td>A unique name to identify the bundle.</td>
</tr>
<tr>
<td><strong>Source language</strong></td>
<td>Yes</td>
<td>The native language of the source file.</td>
</tr>
<tr>
<td><strong>Resource File</strong></td>
<td>No</td>
<td>A <a href="https://cloud.ibm.com/docs/GlobalizationPipeline?topic=GlobalizationPipeline-globalizationpipeline_workingwithbundles">resource file</a> to translate. The maximum file size is limited to 2MB. Specified resource files will be uploaded.</td>
</tr>
<tr>
<td><strong>File format</strong></td>
<td>No</td>
<td>The file type that is being uploaded.</td>
</tr>
<tr>
<td><strong>Target language</strong></td>
<td>No</td>
<td>The languages that you want translations for.</td>
</tr>
</tbody>
</table>

<p><strong>Note:</strong> To change the language service that provides machine translation for your bundles, click the <strong>Machine Translation Configuration</strong> tab to view other supported machine translation engines.</p></li>

<li>Click <strong>save</strong></li></ol>


After the bundle is created, the uploaded resource file is translated into all of the target languages that you specified. The new bundle is added to the Bundles tab where you can:

* Add or remove languages
* Edit the generated translations
* Update the source file that is used in the bundle and regenerate the translations
