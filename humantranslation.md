---

copyright:
  years: 2015, 2017
lastupdated: "2017-05-31"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# Creating chargeable human translation requests
{: #humantranslation}

Where quality over speed is paramount, you may wish to engage professional translators to review your machine translation. For an additional charge in the professional plan of {{site.data.keyword.GlobalizationPipeline_short}}, you are able to submit your machine translated bundles for human review and editing. To do this, you switch from the standard plan to the professional plan, create a human translation request and send your target bundles to IBM's professional translation services. You can use this capability to further refine the quality and consistency of your translations. Languages that are available for human review and editing are the same as the languages supported by the machine translation engines available through {{site.data.keyword.GlobalizationPipeline_short}}. 

To create a human translation request, complete the following steps: 

1. Switch to **Professional plan** of {{site.data.keyword.GlobalizationPipeline_short}}.

2. Click the **Translation request** tab on the dashboard, and click **New Request**.

3. Select your target bundle and target languages for translation. 

4. Verify the bundle ID, target languages and source wordcount for translation. 

5. Provide necessary information about your request. Fields that are marked with asterisks must be filled in.

6. Confirm and submit the request.


**Note**: There are 5 states of each translation request. You can refer to the following table to help track the status of your translation request.

| Status | Email notification | Status explanation |
|--------|--------------------|--------------------|
| Draft  | No | The translation request is created but not submitted yet. You can still modify the content of the translation request. |
| Submitted | Yes | The translation request is submitted, and you cannot modify the content of the translation request. |
| Editing started | Yes | The human post editing work of the translation request is started. |
| Editing Finished | Yes | The human post editing work of the translation request is finished. Still need to wait for the translated strings to be merged back to the master resource strings. |
| Merged | Yes | The human post editing result is merged back to the master resource strings. The translation request is finished. You can generate a report at this point.|


To generate a *JSON (.json)* report or XLIFF for your request, click the **View the request detail** icon ![Select the view request detail icon to view the translations of target language](images/viewProjectDetailIcon.png) from the **Actions** column.  

**Note**: You can still view your human translation request data within a standard plan, but you can only create human translation request when you are a professional plan user of {{site.data.keyword.GlobalizationPipeline_short}}.
