---

copyright:
  years: 2016, 2019

lastupdated: "2019-03-20"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:codeblock: .codeblock}
{:tip: .tip}
{:download: .download}


# {{site.data.keyword.GlobalizationPipeline_short}} {{site.data.keyword.cloudaccesstrailshort}} イベント
{: #gpat_events}

ユーザーとアプリケーションが {{site.data.keyword.Bluemix}} 内の IBM {{site.data.keyword.GlobalizationPipeline_short}} とどのように対話するのかを  {{site.data.keyword.cloudaccesstrailfull}} サービスを使用して追跡します。
{:shortdesc}

{{site.data.keyword.cloudaccesstrailfull_notm}} サービスは、{{site.data.keyword.Bluemix_notm}} のサービスの状態を変更するアクティビティーをユーザーが開始すると、そのアクティビティーを記録します。詳細については、[{{site.data.keyword.cloudaccesstrailfull_notm}}](/docs/services/cloud-activity-tracker/index.html)を参照してください。




## イベントのリスト: バンドル・イベント
{: #gpevents_bundle}

バンドルに関連した、イベントを生成するアクションを以下の表にリストします。

|アクション|説明|
|---|---|  
|g11n-pipeline.bundles.read|バンドル ID のリストを取得します。|
|g11n-pipeline.bundle.create|新規バンドルを作成します。|
|g11n-pipeline.bundle.read|バンドルの情報を取得します。|
|g11n-pipeline.bundle.update|バンドルの構成を更新します。|
|g11n-pipeline.bundle.delete|指定されたバンドルを削除します。|
|g11n-pipeline.bundle-language.create|リソース項目をアップロードします。|
|g11n-pipeline.bundle-language.read|言語のリソース・ストリング (キー/値のペア) を取得します。|
|g11n-pipeline.bundle-language.update|リソース項目を更新します。|
|g11n-pipeline.bundle-language.read|リソース項目情報を取得します。|
|g11n-pipeline.bundle-language.update|リソース項目を更新します。|

## イベントのリスト: バンドル翻訳要求イベント
{: #gpevents_bundle_tr_req}

バンドル翻訳要求に関連した、イベントを生成するアクションを以下の表にリストします。

|アクション|説明|
|---|---|  
|g11n-pipeline.trs.read|翻訳要求のリストを取得します。|
|g11n-pipeline.tr.read|指定された翻訳要求の情報を取得します。|
|g11n-pipeline.tr.update|指定された翻訳要求の情報を更新します。|
|g11n-pipeline.tr.delete|指定された翻訳要求を削除します。|
|g11n-pipeline.tr-bundle.read|バンドルの情報を取得します。|
|g11n-pipeline.tr-bundle-language.read|指定されたバンドルと言語のリソース項目を取得します。|
|g11n-pipeline.tr-bundle-language.read|リソース項目情報を取得します。|
|g11n-pipeline.trs.create|新規翻訳要求を作成します。|


## イベントのリスト: バンドル XLIFF イベント
{: #gpevents_bundle_xliff}

バンドル XLIFF に関連した、イベントを生成するアクションを以下の表にリストします。

|アクション|説明|
|---|---|  
|g11n-pipeline.xliff-bundles.read|XLIFF 2.0 形式のバンドルから指定された言語のリソース・データを取得します。|
|g11n-pipeline.xliff-bundles.update|サービス・インスタンスのバンドルを XLIFF データで更新します。|
|g11n-pipeline.xliff-tr-bundles.read|XLIFF 2.0 形式の翻訳要求で指定された言語のリソース・データを取得します。|


## イベントのリスト: パートナー・イベント
{: #gpevents_partner}

パートナーに関連した、イベントを生成するアクションのリストを以下の表に示します。

|アクション|説明|
|---|---|  
|g11n-pipeline.partner.read|パートナーの情報を取得します。|
|g11n-pipeline.partner.update|パートナーの情報を更新します。|
|g11n-pipeline.partner-trs.read|パートナーに割り当てられている翻訳要求のリストを取得します。|
|g11n-pipeline.partner-tr.read|指定された翻訳要求の情報を取得します。|
|g11n-pipeline.partner-tr.update|指定された翻訳要求の情報を更新します。|
|g11n-pipeline.partner-tr.delete|指定された翻訳要求を削除します。|
|g11n-pipeline.partner-tr-bundle.read|バンドルの情報を取得します。|
|g11n-pipeline.partner-tr-bundle-language.read|指定されたバンドルと言語のリソース項目を取得します。|
|g11n-pipeline.partner-tr-bundle-language.update|指定されたバンドルと言語のリソース項目を更新します。|
|g11n-pipeline.partner-tr-bundle-language.read|リソース項目情報を取得します。|
|g11n-pipeline.partner-tr-bundle-language.update|リソース項目を更新します。|
|g11n-pipeline.partner-users.read|このパートナーの使用可能なユーザーを取得します。|
|g11n-pipeline.partner-user.read|指定されたパートナー・ユーザーの情報を取得します。|
|g11n-pipeline.partner-user.update|パートナー・ユーザーの情報を更新します。|
|g11n-pipeline.partner-user.delete|指定されたパートナー・ユーザーを削除します。|
|g11n-pipeline.partner-user.create|新規パートナー・ユーザーを作成します。|
|g11n-pipeline.partner-tr-xliff-bundles.update|変換要求のリソース・データを XLIFF データで更新します。|
|g11n-pipeline.partner-tr-xliff-bundles-language.read|XLIFF 2.0 形式の翻訳要求で指定された言語のリソース・データを取得します。|



## イベントのリスト: 管理イベント
{: #gpevents_admin}

管理者に関連した、イベントを生成するアクションのリストを以下の表に示します。

|アクション|説明|
|---|---|  
|g11n-pipeline.instances.read|サービス・インスタンスのリストを取得します。|
|g11n-pipeline.instance.read|サービス・インスタンスの情報を取得します。|
|g11n-pipeline.instance.update|サービス・インスタンスの構成を更新します。|
|g11n-pipeline.instance.create|新規サービス・インスタンスを作成します。|
|g11n-pipeline.instance.delete|指定されたサービス・インスタンスを削除します。|
|g11n-pipeline.instance.create|新規 Cloud Foundry マネージド・サービス・インスタンスを作成します。|
|g11n-pipeline.partners.read|パートナーのリストを取得します。|
|g11n-pipeline.partner.create|新規パートナーを作成します。|
|g11n-pipeline.partner.delete|指定されたパートナーを削除します。|



## イベントのリスト: ユーザー・イベント
{: #gpevents_user}

ユーザーに関連した、イベントを生成するアクションのリストを以下の表に示します。

|アクション|説明|
|---|---|  
|g11n-pipeline.instance-users.read|このサービス・インスタンスのユーザーを取得します。|
|g11n-pipeline.instance-user.read|指定されたユーザーの情報を取得します。|
|g11n-pipeline.instance-user.update|ユーザーの情報を更新します。|
|g11n-pipeline.instance-user.delete|指定されたユーザーを削除します。|
|g11n-pipeline.instance-users.create|新規ユーザーを作成します。|


## イベントのリスト: 構成イベント
{: #gpevents_config}

翻訳構成に関連した、イベントを生成するアクションのリストを以下の表に示します。

|アクション|説明|
|---|---|  
|g11n-pipeline.config-mts.read|すべての MT サービス・バインディングを取得します。|
|g11n-pipeline.config-mt.read|MT サービス・バインディング・データを取得します。|
|g11n-pipeline.config-translations.read|すべての翻訳構成を取得します。|
|g11n-pipeline.config-translation.read|翻訳構成を取得します。|
|g11n-pipeline.config-mt.update|指定された MT サービス・バインディング・データを取得します。指定されたバインディング・データが既に存在する場合は、指定された MT サービス・バインディング・データに置き換えられます。|
|g11n-pipeline.config-mt.delete|指定された MT サービス・バインディング・データを削除します。|
|g11n-pipeline.config-translation.update|指定された言語ペアの翻訳構成を配置します。このペアの構成が既に存在している場合は、指定された構成に置き換えられます。|
|g11n-pipeline.config-translation.delete|指定された言語ペアの翻訳構成を削除します。|


## イベントのリスト: インスタンス・イベント
{: #gpevents_instance}

インスタンスに関連した、イベントを生成するアクションのリストを以下の表に示します。

|アクション|説明|
|---|---|  
|g11n-pipeline.instance.read|この翻訳サービス・インスタンスの情報を取得します。|


## イベントを探す場所
{: #gp_at_ui}

{{site.data.keyword.cloudaccesstrailshort}} イベントは、{{site.data.keyword.GlobalizationPipeline_short}} サービスがプロビジョンされる {{site.data.keyword.Bluemix_notm}} 地域で使用可能な {{site.data.keyword.cloudaccesstrailshort}} **スペース・ドメイン** で使用可能です。{{site.data.keyword.cloudaccesstrailshort}} サービス・インスタンスと {{site.data.keyword.GlobalizationPipeline_short}} インスタンスは同じ CF スペースでプロビジョンされる必要があります。

{{site.data.keyword.GlobalizationPipeline_short}} の RC インスタンスの場合、Activity Tracker イベントは、{{site.data.keyword.Bluemix_notm}} 地域でイベントが生成される Activity Tracker **アカウント**・ドメインで使用できます。
