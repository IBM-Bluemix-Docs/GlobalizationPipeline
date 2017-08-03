---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# 機械翻訳の構成
{: #machineconfig}

{{site.data.keyword.GlobalizationPipeline_full}}は、バンドルの機械翻訳を実行するために別の機械翻訳サービスと統合する機能をサポートしています。別のサービスを追加する機能は、{{site.data.keyword.GlobalizationPipeline_short}}で使用されるデフォルトのエンジンでは必要な特定の言語がサポートされていない場合や、別のエンジンで生成される機械翻訳を使用したい場合に便利です。別のサービスの使用や料金については、そのサービスの利用規約の対象になります。

{{site.data.keyword.GlobalizationPipeline_short}}に別の機械翻訳サービスを追加して構成するには、{{site.data.keyword.GlobalizationPipeline_short}}・ダッシュボードの**「機械翻訳の構成 (Machine Translation Configuration)」**タブを選択します。

* {{site.data.keyword.Bluemix_notm}} カタログに含まれている機械翻訳サービス (**Watson 言語翻訳プログラム**) を追加するために、先にそのサービスを {{site.data.keyword.Bluemix_notm}} スペースに追加しておく必要があります。

* サード・パーティーのサービスを追加するには、**「機械翻訳の構成 (Machine Translation Configuration)」**タブでそのサービスのボタンを選択し、そのサービスへのアクセスに必要なユーザー資格情報を入力します。

機械翻訳サービスが{{site.data.keyword.GlobalizationPipeline_short}}に追加されたら、残りの手順を実行してサービスの統合を完了させます。

1. **「有効にする (Enable)」**をクリックして、そのサービスとの統合をオンにします。

2. 「**言語を更新する (Update Languages)**」をクリックして、サポートされるターゲット言語の更新されたリストを表示します。

3. ターゲット言語のリストから、翻訳を実行する機械翻訳エンジンを選択します。

4. **「保存」**をクリックして、**「機械翻訳の構成 (Machine Translation Configuration)」**タブに戻ります。

{{site.data.keyword.GlobalizationPipeline_short}}に別のサービスが構成されると、そのエンジンに割り当てられているすべてのターゲット言語の生成が、そのエンジンを使用して開始されます。 

別の機械翻訳エンジンの使用を停止するには、次のようにします。

1. **「機械翻訳の構成 (Machine Translation Configuration)」**タブで、使用を停止するサービスの**「無効にする (Disable)」**ボタンをクリックします。

別の機械翻訳サービスを無効にしても、そのサービスによって生成された翻訳はすべてバンドル内に残されます。しかし、現在有効にしている機械翻訳エンジンで特定のターゲット言語がサポートされなくなった場合は、そのターゲット言語への翻訳を今後更新できなくなる可能性があります。

<!-- Review comment: When you disable an engine, do you need to go back and reconfigure the languages?? Does it go back to the default engine? What happens? -->
