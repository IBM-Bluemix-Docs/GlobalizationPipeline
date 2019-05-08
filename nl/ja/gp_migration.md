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


# リソース・グループへの {{site.data.keyword.GlobalizationPipeline_short}} サービス・インスタンスのマイグレーション
{: #rg-migration}

既存の {{site.data.keyword.GlobalizationPipeline_short}} CF インスタンス・ユーザーには、RC/IAM 互換バージョンのサービスへのマイグレーション期間として 3 カ月 (RC/IAM バージョンが実動環境で使用可能になった日付から開始) の猶予があります。


## 始める前に
{: #prereqs}

{{site.data.keyword.GlobalizationPipeline_short}} サービス・インスタンスのマイグレーションを開始する前に、サービス・インスタンスのすべてのデータは保持されることを知っておいてください。データは失われません。マイグレーション完了後のサービス・インスタンスの状態は、マイグレーション前と同じです。   

マイグレーション・プロセスの概要については、[リソース・グループへの Cloud Foundry サービス・インスタンスのマイグレーション](/docs/resources/instance_migration.html)を参照してください。 

## マイグレーションの手順
{: #gp_steps_migration}

1. **「その他のアクション」**メニューを開きます。
2. 始めにリソース・グループへの**「マイグレーション」**を選択します。
3. リソース・グループを選択します。
4. **「マイグレーション」**をクリックします。そうすると、インスタンスがマイグレーションされます。

**注:** 一度にマイグレーションできるインスタンスは 1 つのみであるため、最初のマイグレーションが正常に完了したら、マイグレーション可能な他のインスタンスのマイグレーションを続けることができます。

## 次のステップ
{: #nextsteps}

リソース・リストの**「サービス」**セクションに、マイグレーションしたサービス・インスタンスが表示されます。別名は、リソース・リストの「Cloud Foundry」セクションに残ります。 これはインプレース・マイグレーションであるため、すべてのインスタンス・データと資格情報が保持されます。元の CF インスタンスにより生成された資格情報を引き続き使用できます。 

マイグレーションの仕組みについて詳しくは、[マイグレーションの仕組み](/docs/resources/instance_migration.html#how)を参照してください。


