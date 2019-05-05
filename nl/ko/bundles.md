---

copyright:
  years: 2015, 2018
lastupdated: "2017-06-16"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}


# 번들 작업
{: #globalizationpipeline_workingwithbundles}

작성하는 각 번들에는 생성된 번역의 전체 세트 및 리소스 파일의 키 값 쌍이 포함되어 있습니다.
{:shortdesc}

업로드하는 리소스 파일은 다음과 같은 형식으로 되어 있을 수 있으며 앱에서 UI 문자열을 나타내는 키/값 쌍의 양식으로 컨텐츠를 포함해야 합니다.


* 파일 유형: *Java™ 특성 파일(.properties)*<br>
예:
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
* 파일 유형: *AMD I18N(.js)*<br>
예:
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
* 파일 유형: *JSON(.json)*<br>
예:
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

또한, 리소스 파일이 다음 가이드라인을 지켜야 합니다.
* 각 키는 최대 1023자일 수 있습니다.
* 각 값은 최대 8191자일 수 있습니다.
* 각 번들에는 최대 1000개의 키/값 쌍이 포함될 수 있습니다.

번들을 작성하면 언어를 추가하거나 삭제하고, 번역된 컨텐츠를 보고, 번역된 컨텐츠를 일부 편집하는 등의 추가 태스크를 수행할 수 있는 **번들** 탭에 해당 번들이 추가됩니다.  

{{site.data.keyword.GlobalizationPipeline_short}}에서는 기본 기계 번역 엔진을 사용하여 번들 컨텐츠를 언어로 번역합니다. 선택적으로 [기계 번역 구성](/docs/services/GlobalizationPipeline/managetranslations.html#machineconfig) 섹션에 설명된 대로 대체 기계 번역 엔진을 선택할 수 있습니다. 기본 엔진에서는 다음과 같은 대상 언어를 지원합니다.

<table>
<thead>
<tr>
<th>대상 언어</th>
</tr>
</thead>
<tbody>
<tr>
<td>중국어</td>
</tr>
<tr>
<td>대만어</td>
</tr>
<tr>
<td>프랑스어</td>
</tr>
<tr>
<td>독일어</td>
</tr>
<tr>
<td>이탈리아어</td>
</tr>
<tr>
<td>일본어</td>
</tr>
<tr>
<td>한국어</td>
</tr>
<tr>
<td>포르투갈어(브라질)</td>
</tr>
<tr>
<td>스페인어</td>
</tr>
</tbody>
</table>

**참고:** {{site.data.keyword.GlobalizationPipeline_short}}의 기본 기계 번역 엔진은 소스 언어로 영어만 지원합니다. 그러나 {{site.data.keyword.GlobalizationPipeline_short}} 내의 구성에 사용 가능한 대체 기계 번역 엔진은 영어가 아닌 다른 소스 언어/언어 쌍의 번역을 지원합니다.

기계 번역을 사용하여 번들 컨텐츠를 번역하고 나면 {{site.data.keyword.GlobalizationPipeline_short}} 내에서 일부 편집하거나 번들을 제출하여 검토하고 전문 번역가가 편집할 수 있습니다. 인간이 검토하고 편집하도록 요청을 제출하는 데 대한 자세한 정보는 [비용이 청구되는 인간 번역 요청 작성](/docs/services/GlobalizationPipeline/managetranslations.html#humantranslation)을 참조하십시오.




## 작업할 번들 선택
{: #globalizationpipeline_selectingabundle}

1. **번들** 탭을 클릭하여 작성한 모든 번들을 보십시오.
2. 목록에서 **번들 ID**를 클릭하여 번들에 대한 추가 세부사항을 보거나 **번들 세부사항 보기** 아이콘 ![번들 세부사항 아이콘 보기를 선택하여 번들을 열고 해당 번역으로 작업](images/viewProjectDetailIcon.png)을 조치 열에서 클릭하십시오.

![번들 탭에서 사용 가능한 모든 번들을 보십시오.](images/translationBundles.png)

작업할 번들을 선택한 후 해당 번역의 상태를 보고 언어를 추가하거나 제거하고 번역을 편집하거나 리소스 파일에 대한 업데이트를 제공할 수 있습니다.

번들이 이제 필요하지 않으면 **번들** 탭에서 이를 삭제할 수 있습니다. 번들과 연관된 모든 번역도 삭제됩니다.
