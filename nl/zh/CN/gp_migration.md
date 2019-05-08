---

copyright:
  years: 2015, 2019
lastupdated: "2019-03-25"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:codeblock: .codeblock}
{:tip: .tip}
{:download: .download}


# 将 {{site.data.keyword.GlobalizationPipeline_short}} 服务实例迁移到资源组
{: #rg-migration}

现有 {{site.data.keyword.GlobalizationPipeline_short}} CF 实例用户有 3 个月的时间（自 RC/IAM 版本在生产环境中可用之日起算）迁移到 RC/IAM 兼容版本的服务。


## 开始之前
{: #prereqs}

开始迁移 {{site.data.keyword.GlobalizationPipeline_short}} 服务实例之前，您应该知道该服务实例的所有数据均已保留。您不会丢失任何内容。迁移后，您可以看到服务实例的状态与迁移之前相同。   

有关迁移过程的概述，请参阅[将 Cloud Foundry 服务实例迁移到资源组](/docs/resources/instance_migration.html)。 

## 迁移步骤
{: #gp_steps_migration}

1. 打开**更多操作**菜单。
2. 首先选择**迁移**以迁移到资源组。
3. 选择资源组。
4. 单击**迁移**，此时系统会为您迁移实例。

**注：**一次只能迁移一个实例，因此可以在成功迁移第一个实例后，继续迁移符合条件的实例。

## 后续步骤
{: #nextsteps}

您可以在资源列表的**服务**部分中看到已迁移的服务实例。别名会保留在资源列表的 Cloud Foundry 部分中。这是就地迁移，因此将保留所有实例数据和凭证。您可以继续使用原始 CF 实例生成的凭证。 

有关迁移工作方式的更多信息，请参阅[迁移工作方式](/docs/resources/instance_migration.html#how)。


