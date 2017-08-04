---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# 机器翻译配置
{: #machineconfig}

{{site.data.keyword.GlobalizationPipeline_full}} 支持集成替代机器翻译服务，以对束执行机器翻译的能力。如果 {{site.data.keyword.GlobalizationPipeline_short}} 使用的缺省引擎不提供您所需的特定语言，或者如果您更愿意使用不同引擎所生成的机器翻译，那么添加替代服务会很有益处。替代服务的使用和收费涵盖在那些服务的条款下。

要添加并配置 {{site.data.keyword.GlobalizationPipeline_short}} 的替代机器翻译服务，请从 {{site.data.keyword.GlobalizationPipeline_short}} 仪表板选择**机器翻译配置**选项卡。

* 要添加 {{site.data.keyword.Bluemix_notm}} 目录中的机器翻译服务（**Watson 语言转换程序**），必须首先将该服务添加到您的 {{site.data.keyword.Bluemix_notm}} 空间。

* 要添加第三方服务，请在**机器翻译配置**选项卡上选择该服务的按钮，然后提供访问该服务所需的用户凭证。

在向 {{site.data.keyword.GlobalizationPipeline_short}} 添加了机器翻译服务之后，请完成其余的步骤，以完成该服务的集成。

1. 单击**启用**，以开启与该服务的集成。

2. 单击**更新语言**，以查看受支持目标语言的更新列表。

3. 从目标语言列表中，选择应该执行翻译的机器翻译引擎。

4. 单击**保存**，以返回到**机器翻译配置**选项卡。

在使用 {{site.data.keyword.GlobalizationPipeline_short}} 配置替代服务之后，将会使用该引擎开始生成分配给该引擎的所有目标语言。 

要停止使用替代机器翻译引擎：

1. 从**机器翻译配置**选项卡中，单击您要停止使用的服务的**禁用**按钮。

在禁用替代机器翻译服务之后，该服务所生成的所有翻译仍会在您的束中。但是，如果目前启用的机器翻译引擎不再支持特定目标语言，那么可能无法进一步更新该目标语言的翻译。

<!-- Review comment: When you disable an engine, do you need to go back and reconfigure the languages?? Does it go back to the default engine? What happens? -->
