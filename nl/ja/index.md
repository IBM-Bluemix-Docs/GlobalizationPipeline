---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

 
# {{site.data.keyword.GlobalizationPipeline_short}}概説
{: #globalizationpipeline}

{{site.data.keyword.GlobalizationPipeline_full}} は、アプリの開発者が翻訳済みアプリケーションをグローバル・カスタマーに素早くリリースできるようにする、{{site.data.keyword.Bluemix}} サービスです。{{site.data.keyword.GlobalizationPipeline_short}} には、機械翻訳、人によるレビューと編集、翻訳を DevOps と Continuous Development インフラストラクチャーにシームレスに組み込むための API と SDK が備わっているので、従来の翻訳プロセスに関連していた手動の孤立した操作が除去されます。
{:shortdesc}

{{site.data.keyword.GlobalizationPipeline_short}} サービスを使用して {{site.data.keyword.Bluemix}} 上でデプロイされてホストされるアプリを翻訳することや、アンバインドして他のクラウド・プラットフォーム上でホストされるアプリを翻訳することができます。

{{site.data.keyword.GlobalizationPipeline_short}} は、翻訳を管理するダッシュボード・インターフェースと翻訳プロセスを完全自動化する RESTful API の両方を提供します。{{site.data.keyword.GlobalizationPipeline_short}} API については、[API リファレンス](https://gp-rest.ng.bluemix.net/translate/swagger/index.html){: new_window}を参照してください。 

## 翻訳プランの選択
{: #globalizationpipeline_chooseplan}

{{site.data.keyword.GlobalizationPipeline_short}} の翻訳作業を開始する前に、適切な翻訳プランを選択できます。

{{site.data.keyword.GlobalizationPipeline_short}} では、Standard プランと Professional プランの 2 つの翻訳プランが使用可能です。これらプランはどちらも、統合された無制限の基本的な機械翻訳と、追加料金で他の機械翻訳エンジンと統合する機能を提供します。Professional プランで、{{site.data.keyword.GlobalizationPipeline_short}} はさらに、専門家によるレビューと編集のサービスを提供します。Bluemix 内では、すべてのデータを予約して {{site.data.keyword.GlobalizationPipeline_short}} のプランを切り替えることができます。 


## {{site.data.keyword.GlobalizationPipeline_short}}のデータ使用量の見積もり
{: #globalizationpipeline_documentpricing}

{{site.data.keyword.GlobalizationPipeline_short}}は、ユーザーの翻訳をバックエンド・データベースに格納します。アクティブ・データのサイズを見積もるには、以下の公式を使用します。

`<expected resource data storage size in MB> ˜= 0.0005 * <number of key/value pairs in the source resource> * <number of languages including the source language>`

この公式では、典型的なバンドルのサイズは `(UTF-8 でのキーの長さ + 値の長さ = 40 バイト)` です。

例えば、100 個のキー/値ペアがあり、それらを 9 個の言語に翻訳する場合、ストレージ・サイズの見積もりは 0.0005 100 (9+1) = 0.5 MB になります。実際のサイズは、実際のキー/値のサイズや翻訳と共に保管されるメタデータに応じて異なります。

Bluemix の[料金カリキュレーター](https://console.ng.bluemix.net/?direct=classic/#/pricing/cloudOEPaneId=pricing&paneId=pricingSheet&orgGuid=127a45f4-4461-4d5b-a26b-6dc2fdd1a3a2&spaceGuid=208fb1ff-413b-4fd9-9615-e8226062d0f3)を使用して、サービスの月額料金を計算してください。

**注**: Professional プランのレビュー・フィーチャーを使用すると、データの使用方法が上記の説明よりも増大します。



