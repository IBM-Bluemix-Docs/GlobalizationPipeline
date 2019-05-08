---

copyright:
  years: 2015, 2017
lastupdated: "2017-05-26"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# バンドルの作成
{: #createbundles}

翻訳を開始するには、バンドルを作成し、{{site.data.keyword.GlobalizationPipeline_short}} による翻訳が必要なアプリのリソース・ファイルをアップロードします。 リソース・ファイルとしては、Java プロパティー、AMD I18N、JSON ファイルのいずれかを使用できます。このファイルには、アプリの UI 文字列を表すキー/値ペアの形式の内容が含まれていなければなりません。  サポートされるファイル・タイプの詳細と例については、[バンドルの操作](/docs/services/GlobalizationPipeline/bundles.html){: new_window}を参照してください。

バンドルを作成するには、以下の手順を実行します。

<ol>
<li><strong>「概要」</strong>タブから、<strong>「新しいバンドル (New Bundle)」</strong>をクリックします。</li>

<li>バンドルに関する情報を指定します。
<table>
<thead>
<tr>
<th>フィールド</th>
<th>必須</th>
<th>説明</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>バンドル ID (Bundle ID)</strong></td>
<td>はい</td>
<td>バンドルを識別する固有の名前。</td>
</tr>
<tr>
<td><strong>ソース言語 (Source language)</strong></td>
<td>はい</td>
<td>ソース・ファイルのネイティブ言語。</td>
</tr>
<tr>
<td><strong>リソース・ファイル (Resource File)</strong></td>
<td>いいえ</td>
<td>翻訳する<a href=https://new-console.stage1.ng.bluemix.net/docs/services/GlobalizationPipeline/bundles.html>リソース・ファイル</a>。 最大ファイル・サイズは 2 MB に制限されます。 指定されたリソース・ファイルがアップロードされます。</td>
</tr>
<tr>
<td><strong>ファイル形式 (File format)</strong></td>
<td>いいえ</td>
<td>アップロードするファイル・タイプ。</td>
</tr>
<tr>
<td><strong>ターゲット言語 (Target language)</strong></td>
<td>いいえ</td>
<td>翻訳後の言語。</td>
</tr>
</tbody>
</table>

<p><strong>注:</strong> バンドルの機械翻訳を提供する言語サービスを変更するには、<strong>「機械翻訳の構成 (Machine Translation Configuration)」</strong>タブをクリックして、サポートされている他の機械翻訳エンジンを表示します。</p></li>

<li><strong>「保存」</strong>をクリックします。</li></ol>


バンドルを作成すると、アップロードしたリソース・ファイルが、指定したすべてのターゲット言語に翻訳されます。 新しいバンドルが「バンドル」タブに追加されます。ここで、次の操作を実行できます。

* 言語を追加または除去する
* 生成された翻訳を編集する
* バンドルで使用されているソース・ファイルを更新し、翻訳を再生成する
