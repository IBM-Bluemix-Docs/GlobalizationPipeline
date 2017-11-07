---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

 
# Getting started with {{site.data.keyword.GlobalizationPipeline_short}}
{: #globalizationpipeline}

{{site.data.keyword.GlobalizationPipeline_full}} is an {{site.data.keyword.Bluemix}} service that enables app developers to rapidly release translated applications to global customers. {{site.data.keyword.GlobalizationPipeline_short}} provides machine translation, human review and editing, and APIs and SDKs to seamlessly integrate translation into your DevOps and Continuous Development infrastructure, eliminating manual and siloed operations associated with traditional translation process.
{:shortdesc}

You can use the {{site.data.keyword.GlobalizationPipeline_short}} service to translate any app deployed and hosted on {{site.data.keyword.Bluemix}}, or unbound to translate apps hosted on other cloud platforms.

{{site.data.keyword.GlobalizationPipeline_short}} offers both a dashboard interface to manage your app translation and a RESTful API that fully automates the translation process. For information about the {{site.data.keyword.GlobalizationPipeline_short}} API, see [API Reference](https://gp-rest.ng.bluemix.net/translate/swagger/index.html){: new_window}. 

## Choosing a translation plan
{: #globalizationpipeline_chooseplan}

Before you start to work with translation on {{site.data.keyword.GlobalizationPipeline_short}}, you can choose a suitable translation plan.

There are two translation plans available on {{site.data.keyword.GlobalizationPipeline_short}}, the Standard plan and Professional plan. Both these plans provide integrated unlimited basic machine translation as well as the capability to integrate with other machine translation engines for an additional charge. In the Professional plan, {{site.data.keyword.GlobalizationPipeline_short}} additionally offers a professional translation review and editing service. You can switch between {{site.data.keyword.GlobalizationPipeline_short}} plans within {{site.data.keyword.Bluemix_notm}} with all data reserved. 


## Estimating {{site.data.keyword.GlobalizationPipeline_short}} Data Usage
{: #globalizationpipeline_documentpricing}

{{site.data.keyword.GlobalizationPipeline_short}} stores your translations in a backend database. To estimate active data size, you can refer to the formula below:

`<expected resource data storage size in MB> ˜= 0.0005 * <number of key/value pairs in the source resource> * <number of languages including the source language>`

According to the formula, the size of a typical bundle is `(length of key + length of value in UTF-8 = ˜40 bytes)`.

For example, if you have 100 key/value pairs and translate them to 9 languages, the estimated storage size is 0.0005 100 (9+1) = 0.5 MB. The actual size may be different depending on actual key/value size and metadata stored along with the translation.

Use the {{site.data.keyword.Bluemix_notm}} [pricing calculator](https://console.ng.bluemix.net/?direct=classic/#/pricing/cloudOEPaneId=pricing&paneId=pricingSheet&orgGuid=127a45f4-4461-4d5b-a26b-6dc2fdd1a3a2&spaceGuid=208fb1ff-413b-4fd9-9615-e8226062d0f3) to determine your monthly service costs.

**Note**: Using the Professional plan review feature will increase your data usage beyond what is stated above.



