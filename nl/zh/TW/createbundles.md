---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# 建立軟體組
{: #createbundles}

若要開始使用翻譯，請建立軟體組，並針對需要由 {{site.data.keyword.GlobalizationPipeline_short}} 翻譯的應用程式，上傳其資源檔。資源檔可以是 Java Properties、AMD I18N 或 JSON 檔案，而且必須包含代表應用程式中使用者介面字串之鍵值組形式的內容。如需所支援檔案類型的詳細資料和範例，請參閱[使用軟體組](./bundles.html){: new_window}。

若要建立軟體組，請完成下列步驟：

<ol>
<li>從<strong>概觀</strong>標籤中，按一下<strong>新建軟體組</strong>。</li>

<li>提供您軟體組的相關資訊：<table>
<thead>
<tr>
<th>欄位</th>
<th>必要</th>
<th>說明</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>軟體組 ID</strong></td>
<td>是</td>
<td>用來識別軟體組的唯一名稱。</td>
</tr>
<tr>
<td><strong>來源語言</strong></td>
<td>是</td>
<td>來源檔的國家語言。</td>
</tr>
<tr>
<td><strong>資源檔</strong></td>
<td>否</td>
<td>要翻譯的<a href=https://new-console.stage1.ng.bluemix.net/docs/services/GlobalizationPipeline/bundles.html>資源檔</a>。檔案大小上限限制為 2MB。將會上傳指定的資源檔。</td>
</tr>
<tr>
<td><strong>檔案格式</strong></td>
<td>否</td>
<td>正在上傳的檔案類型。</td>
</tr>
<tr>
<td><strong>目標語言</strong></td>
<td>否</td>
<td>您想要翻譯的語言。</td>
</tr>
</tbody>
</table>

<p><strong>附註：</strong>若要變更提供軟體組之機器翻譯的語言服務，請按一下 <a href=https://new-console.stage1.ng.bluemix.net/docs/services/GlobalizationPipeline/managing_translations.html#globalizationpipeline_service_to_service>MT 配置</a>標籤，以檢視其他支援的機器翻譯引擎。</p></li>

<li>按一下<strong>儲存</strong></li></ol>


建立軟體組之後，上傳的資源檔會翻譯為所有您指定的目標語言。新的軟體組會新增至「軟體組」標籤，您可以在其中執行下列動作：

* 新增或移除語言
* 編輯產生的翻譯
* 更新軟體組中所使用的來源檔，然後重新產生翻譯
