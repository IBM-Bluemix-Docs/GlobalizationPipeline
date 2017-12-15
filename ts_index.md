---

copyright:
  years: 2015, 2017
lastupdated: "2017-12-15"

---

{:tsSymptoms: .tsSymptoms} 
{:tsCauses: .tsCauses} 
{:tsResolve: .tsResolve} 
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# FAQ
{: #globalizationpipelinets}

Here are some answers to common questions about using {{site.data.keyword.GlobalizationPipeline_full}}. 
{:shortdesc}


## The name of my app was not translated correctly
{: #problem1}

The generated translations of certain strings was not what was expected.
{:shortdesc}

When a resource file is translated, strings that contain product names or other proper nouns might not translate properly.
{: tsSymptoms}

Often times, product names or proper names do not translate properly into other languages, especially if the name contains real words. When these types of words and phrases are translated, depending on the meaning of those words in a specific language, the translated text may have a different meaning from the English name.
{: tsCauses}

Test the translation of product names before you use them, and if you find problems, modify the text or translation accordingly. For writing style tips when using machine translation, see [Machine translation tips](./tips.html#globalizationpipeline_tips).
{: tsResolve}



## I am unable to upload a resource file
{: #problem2}

The resource file I am trying to upload is not accepted.
{:shortdesc}

When adding a resource file to a new translation bundle or updating an existing resource file to be translated, I receive an error.
{: tsSymptoms}

{{site.data.keyword.GlobalizationPipeline_short}} only accepts resource files of the following types: Java™ .properties, JSON, and AMD I18N.
{: tsCauses}

Ensure that the resource file being uploaded is of one of these types.
{: tsResolve}
* Java .properties
* JSON
* AMD I18N



## I can't upload my resource file because it is too large
{: #problem3}

The resource file I am trying to upload is not accepted.
{:shortdesc}

When adding or updating a resource file to a translation project, an error is occurring because a portion of the file is too large.
{: tsSymptoms}

{{site.data.keyword.GlobalizationPipeline_short}} can only accept resource files that meet certain size requirements.
{: tsCauses}

Ensure that the resource file conforms to the following guidelines:
{: tsResolve}
* Each key can be a maximum of 1024 characters.
* Each value can be a maximum of 8192 characters.
* Each translation project can contain a maximum of 1000 key / value pairs.
* A resource file can be no larger than 2 MB.



## The spacing around variables contained in strings is not consistent
{: #problem5}

The spacing that is used around variables after translation is not always the same.
{:shortdesc}

The spacing that is used around variables that are contained within strings is not always consistent from language to language after translation.
{: tsSymptoms}

Machine translation engines are designed to work with natural language and might not always recognize or know how to handle specific syntax used by programming languages. As a result, the handling of syntax that is mixed with plain text might vary.
{: tsCauses}

{{site.data.keyword.GlobalizationPipeline_short}} currently recognizes the pattern "{}" commonly used to represent variables and will preserve the original format of the content contained within.
{: tsResolve}


## I want to send a bundle for professional review, however, I don't see the Translation Requests tab.
{: #problem6}

If you want to utilize {{site.data.keyword.GlobalizationPipeline_short}}'s professional review feature, you need to be using the Professional plan. See [Managing Translation](https://console-regional.ng.bluemix.net/docs/services/GlobalizationPipeline/managetranslations.html) for more information.
{: tsResolve}

## I want to use the Globalization Pipeline API instead of the dashboard. How do I get started?
{: #problem7}

The {{site.data.keyword.GlobalizationPipeline_short}} API provides you with all the features of the dashboard, plus support for additional resource file formats and more. To get started using the API, consult the [API Swagger docs](https://gp-rest.ng.bluemix.net/translate/swagger/index.html).
{: tsResolve}
