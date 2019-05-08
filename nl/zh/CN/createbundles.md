---

copyright:
  years: 2015, 2017
lastupdated: "2017-05-26"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# 创建束
{: #createbundles}

要开始翻译，您创建束并上传需要 {{site.data.keyword.GlobalizationPipeline_short}} 翻译的应用程序的资源文件。资源文件可以是 Java 属性文件、AMD I18N 文件或 JSON 文件，且必须以代表应用程序中 UI 字符串的键值对形式包含内容。有关受支持文件类型的详细信息和示例，请参阅[使用束](/docs/services/GlobalizationPipeline/bundles.html){: new_window}。

要创建束，请完成以下步骤：

<ol>
<li>从<strong>概述</strong>选项卡中，单击<strong>新建束</strong>。</li>

<li>提供束的相关信息：<table>
<thead>
<tr>
<th>字段</th>
<th>必填</th>
<th>描述</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>束标识</strong></td>
<td>是</td>
<td>用于识别束的唯一名称。</td>
</tr>
<tr>
<td><strong>源语言</strong></td>
<td>是</td>
<td>源文件的母语。</td>
</tr>
<tr>
<td><strong>资源文件</strong></td>
<td>否</td>
<td>要翻译的<a href=https://new-console.stage1.ng.bluemix.net/docs/services/GlobalizationPipeline/bundles.html>资源文件</a>。文件大小上限为 2MB。将上传指定的资源文件。</td>
</tr>
<tr>
<td><strong>文件格式</strong></td>
<td>否</td>
<td>要上传的文件类型。</td>
</tr>
<tr>
<td><strong>目标语言</strong></td>
<td>否</td>
<td>要翻译为的目标语言。</td>
</tr>
</tbody>
</table>

<p><strong>注：</strong>要更改针对束提供机器翻译的语言服务，请单击<strong>机器翻译配置</strong>选项卡，以查看其他受支持的机器翻译引擎。</p></li>

<li>单击<strong>保存</strong></li></ol>


创建束之后，已上传的资源文件即会翻译为您指定的所有目标语言。新束会添加到“束”选项卡，您可以在这里：

* 添加或移除语言
* 编辑生成的翻译
* 更新束中使用的源文件并重新生成翻译
