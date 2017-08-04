---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}


# 使用束
{: #globalizationpipeline_workingwithbundles}

您所创建的每个束都包含资源文件的键值对，以及生成的完整翻译集。
{:shortdesc}

您所上传的资源文件可以是以下格式中的任何一种，且必须以代表应用程序中 UI 字符串的键值对形式包含内容。


* 文件类型：*Java™ 属性文件 (.properties)*<br>
示例：
```js
logout=Logout 
back=Back 
examples=Menu 
home=Home 
web=Web 
enterprise=Enterprise 
extra=Resources 
about=About 
settings=Settings 
help=Help 
support=Support 
topics=Topics 
appExitMsg=Are you sure you want to quit the application?
```
* 文件类型：*AMD I18N (.js)*<br>
示例：
```js
define({
    "root": {
       logout: "Logout",
       back: "Back",
       examples: "Menu",
       home: "Home",
       web: "Web",
       enterprise: "Enterprise",
       extra: "Resources",
       about: "About",
       settings: "Settings",
       help: "Help",
       support: "Support",
       topics: "Topics",
       appExitMsg: "Are you sure you want to quit the application?"
    }
});
``` 
* 文件类型：*JSON (.json)*<br>
示例：
```js
{
  "logout": "Logout",
  "back": "Back",
  "examples": "Menu",
  "home": "Home",
  "web": "Web",
  "enterprise": "Enterprise",
  "extra": "Resources",
  "about": "About",
  "settings": "Settings",
  "help": "Help",
  "support": "Support",
  "topics": "Topics",
  "appExitMsg": "Are you sure you want to quit the application?"
}
``` 

此外，资源文件还必须遵循以下准则：
* 每个键最多可为 1023 个字符。
* 每个值最多可为 8191 个字符。
* 每个束最多可包含 1000 个键值对。

当您创建束时，它们会添加到**束**选项卡中，您可在该选项卡中执行其他任务，如添加或删除语言、查看已翻译的内容，以及对已翻译的内容进行一些小修改。 

{{site.data.keyword.GlobalizationPipeline_short}} 可使用缺省机器翻译引擎，将束内容翻译为语言。或者，您可以选择替代的机器翻译引擎，如[机器翻译配置](managetranslations.html#machineconfig)一节中所述。缺省引擎支持以下目标语言：

<table>
<thead>
<tr>
<th>目标语言</th>
</tr>
</thead>
<tbody>
<tr>
<td>中文（简体）</td>
</tr>
<tr>
<td>中文（繁体）</td>
</tr>
<tr>
<td>法语</td>
</tr>
<tr>
<td>德语</td>
</tr>
<tr>
<td>意大利语</td>
</tr>
<tr>
<td>日语</td>
</tr>
<tr>
<td>韩语</td>
</tr>
<tr>
<td>葡萄牙语（巴西）</td>
</tr>
<tr>
<td>西班牙语</td>
</tr>
</tbody>
</table>

**注：**{{site.data.keyword.GlobalizationPipeline_short}} 的缺省机器翻译引擎仅提供对将英语作为源语言的支持。但可在 {{site.data.keyword.GlobalizationPipeline_short}} 中配置替代的机器翻译引擎来支持其他非英语源语言/语言对。

使用机器翻译对束内容进行翻译后，可以在 {{site.data.keyword.GlobalizationPipeline_short}} 中进行一些小修改，或者提交束供专业翻译人员复查和编辑。有关提交人工复查和编辑的请求，请参阅[创建收费人工翻译请求](managetranslations.html#humantranslation)。 




## 选择要使用的束
{: #globalizationpipeline_selectingabundle}

1. 单击**束**选项卡，以查看已创建的所有束。
2. 单击列表中的**束标识**，以查看该束的更多详细信息，或者在“操作”列中单击**查看束详细信息**图标 ![选择“查看束详细信息”图标，以打开束并使用其翻译](images/viewProjectDetailIcon.png)。

![从“束”选项卡查看所有可用束。](images/translationBundles.png)

在您选择要使用的束之后，您可以查看其翻译的状态、添加或移除语言、编辑翻译或提供资源文件的更新。

如果您不再需要某个束，那么您可以将其从**束**选项卡中删除。同时也会删除与该束相关联的所有翻译。


