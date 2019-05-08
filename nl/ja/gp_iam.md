---

copyright:
  years:  2015, 2019
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


# IBM Cloud IAM for {{site.data.keyword.GlobalizationPipeline_short}}
{: #gp_iam}

## アクセス
{: #gp_iam_access}
お客様のアカウント内のユーザーによる {{site.data.keyword.GlobalizationPipeline_short}} RC 対応サービス・インスタンスへのアクセスは、{{site.data.keyword.Bluemix_notm}} の Identity and Access Management (IAM) と {{site.data.keyword.GlobalizationPipeline_short}} 認証によって制御されます。CF インスタンスの場合は {{site.data.keyword.GlobalizationPipeline_short}} 認証だけを使用できます。

## {{site.data.keyword.GlobalizationPipeline_short}} 認証
{: #gp_iam_ca}
この認証メカニズムを使用するには、[API ユーザーの追加](/docs/services/GlobalizationPipeline/managetranslations.html#adduser)を参照してください。


## Identity Access Management (IAM)
{: #gp_iam_ovw}
ご使用のアカウント内の {{site.data.keyword.GlobalizationPipeline_short}} サービスにアクセスするすべてのユーザーには、IAM ユーザー役割が定義されたアクセス・ポリシーを割り当てる必要があります。そのポリシーによって、選択したサービスまたはインスタンスのコンテキスト内でユーザーが実行できるアクションが決まります。 許可されるアクションは、サービス上で実行できる操作として、{{site.data.keyword.Bluemix_notm}} サービスによってカスタマイズされて定義されます。 その後、アクションは IAM ユーザー役割にマップされます。

ポリシーにより、アクセス権限をさまざまなレベルで付与することができます。 以下のようなオプションがあります。

* 自分のアカウント内のサービスのすべてのインスタンスにわたるアクセス
* アカウント内の個別のサービス・インスタンスに対するアクセス権限
* インスタンス内の特定のリソースへのアクセス
* 自分のアカウント内のすべての IAM 対応のサービスへのアクセス

アクセス・ポリシーの有効範囲を定義した後に、役割を割り当てることができます。 次の表は、サービス・アクセス役割にマップされたアクションについて詳しく示しています。 サービス・アクセス役割が割り当てられたユーザーは、{{site.data.keyword.GlobalizationPipeline_short}} にアクセスし、{{site.data.keyword.GlobalizationPipeline_short}} の API を呼び出すことができます。

| **役割タイプ** | **翻訳の表示** | **翻訳の編集** | **バンドル情報の変更** | **プロフェッショナル翻訳要求の作成** | **プロフェッショナル翻訳要求の表示** |
|---------------|-----------------------|-----------------------|-------------------------------|----------------------------------------------|--------------------------------------------|
| リーダー        | はい | いいえ | いいえ | いいえ | いいえ |
| ライター        | はい | はい | いいえ | いいえ | はい |
| 管理者       | はい | はい | はい | はい | はい |
{: caption="表 1. IAM ユーザーの役割とアクション" caption-side="top"}

現在、IAM ユーザーにはサービス・インスタンス・レベルでのアクセス権限が付与されており、IAM ユーザーに対しバンドル・レベルでのアクセスの許可または拒否は実行できません。細かく制御する場合は、{{site.data.keyword.GlobalizationPipeline_short}} 認証を使用してください。

UI でのユーザー役割の割り当てについては、[IAM アクセス権限の管理](/docs/iam/iammanidaccser.html#iammanidaccser)を参照してください。

### API 呼び出しの生成
{: #gp_iam_apicalls}

サービス資格情報を生成または取得するには、以下の手順に従います。
1. [{{site.data.keyword.Bluemix}} ダッシュボード](https://cloud.ibm.com/)で {{site.data.keyword.Bluemix}} アカウントにログオンします。
2. [{{site.data.keyword.Bluemix}} ダッシュボード](https://cloud.ibm.com/) でサービス・インスタンスをクリックします。
3. **「サービス資格情報」**をクリックしてサービス・インスタンスを開きます。 
4. **「新規資格情報」**をクリックし、プロンプトに従って新規資格情報を作成します。
5. 資格情報の作成が完了したら**「資格情報の表示」**をクリックします。
![サンプル API キーに関する情報を示すスクリーン・ショット](images/gp_iam_apicalls.gif)

IAM 認証を使用して {{site.data.keyword.GlobalizationPipeline_short}} の API を呼び出す例を以下に示します。

* IAM ベアラー・トークンの使用
```
curl -X GET \
  https://gp-rest.us-south.g11n-pipeline.test.cloud.ibm.com/translate/rest/50341556337c581c208188ff8908ebc7/v2/bundles \
  -H 'Authorization: Bearer eyJjsksd…w'
```

* API キーの使用
```
curl -X GET \
  https://gp-rest.us-south.g11n-pipeline.test.cloud.ibm.com/translate/rest/50341556337c581c208188ff8908ebc7/v2/bundles \
  -H 'Authorization: API-KEY MklfrP…ACem'
```
上記の例では、以下の情報を取得できます。
* 「50341556337c581c208188ff8908ebc7」は instanceId です (資格情報セクションから取得)
* 「https://gp-rest.us-south.g11n-pipeline.test.cloud.ibm.com/translate/rest」は URL です (資格情報セクションから取得)
* 「MklfrP…ACem」は apikey です (資格情報セクションから取得)
* 「eyJjsksd…w」は IAM ベアラー・トークンです

IAM ベアラー・トークンを apikey から取得する手順については、[API キーを使用した {{site.data.keyword.Bluemix_notm}} IAM トークンの取得](/docs/iam?topic=iam-iamtoken_from_apikey#iamtoken_from_apikey)を参照してください。
