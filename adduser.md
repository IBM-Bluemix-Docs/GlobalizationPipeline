---

copyright:
  years: 2015, 2017
lastupdated: "2017-05-26"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# Add API users
{: #adduser}

As you manage your translations, you may wish to grant access to additional API users based on the tasks they need to perform. For example, you may want to enable a translator to edit the translation, but not be able to modify the bundle information.

| Role type | View translations? | Edit translations? | Modify bundle information? |
|-----------|--------------------|--------------------|----------------------------|
| Reader | Yes | No | No |
| Translator | Yes | Yes | No |
| Administrator | Yes | Yes | Yes |

If you create more API users, you can restrict their access to one or more specific bundles, or grant them access to all of the available bundles.

To grant an API user access to bundles in a {{site.data.keyword.GlobalizationPipeline_short}} service instance:

1. On the {{site.data.keyword.GlobalizationPipeline_short}} dashboard, click the ** API Users** tab.
2. Click **New API User**.
3. Type a **display name** and **comment** to describe the new API user.
4. Choose a **type** for the new API user.
5. Choose to give the API user access to all bundles or only selected bundles.
6. Click **Save**.

![Complete the forum in order to create a new API user.](images/newUser.png)

An API user ID and password are generated and displayed. Copy and save those credentials; after you close the window, you cannot access them again. The credentials can be used for RESTful service via [SDKs](https://github.com/IBM-Bluemix/gp-common). 

To reset the API user password:

1. On the {{site.data.keyword.GlobalizationPipeline_short}} dashboard, click the **API Users** tab.
2. Click the **Reset Password** icon ![Select this icon to reset the API users password](images/resetPW.png) to reset password for a specific user ID. 
3. Click **Yes**. 
