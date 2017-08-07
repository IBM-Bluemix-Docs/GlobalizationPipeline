---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# 번들 작성
{: #createbundles}

번역을 시작하기 위해, 번들을 작성하고 {{site.data.keyword.GlobalizationPipeline_short}}에서 번역해야 하는 앱의 리소스 파일을 업로드합니다. 리소스 파일은 Java 특성, AMD I18N 또는 JSON 파일 중 하나이며 앱에서 UI 문자열을 나타내는 키/값 쌍의 양식으로 된 컨텐츠를 포함해야 합니다. 지원되는 파일 유형의 세부사항 및 예제는 [번들 작업](./bundles.html){: new_window}을 참조하십시오.

번들을 작성하려면 다음 단계를 완료하십시오.

<ol>
<li><strong>개요</strong> 탭에서 <strong>새 번들</strong>을 클릭하십시오.</li>

<li>번들에 대한 정보를 제공하십시오.<table>
<thead>
<tr>
<th>필드</th>
<th>필수</th>
<th>설명</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>번들 ID</strong></td>
<td>예</td>
<td>번들을 식별하는 고유 이름입니다.</td>
</tr>
<tr>
<td><strong>소스 언어</strong></td>
<td>예</td>
<td>소스 파일의 모국어입니다.</td>
</tr>
<tr>
<td><strong>리소스 파일</strong></td>
<td>아니오</td>
<td>번역할 <a href=https://new-console.stage1.ng.bluemix.net/docs/services/GlobalizationPipeline/bundles.html>리소스 파일</a>입니다. 최대 파일 크기는 2MB로 제한됩니다. 지정된 리소스 파일이 업로드됩니다.</td>
</tr>
<tr>
<td><strong>파일 형식</strong></td>
<td>아니오</td>
<td>업로드되는 파일 유형입니다.</td>
</tr>
<tr>
<td><strong>대상 언어</strong></td>
<td>아니오</td>
<td>번역하려는 해당 언어입니다.</td>
</tr>
</tbody>
</table>

<p><strong>참고:</strong> 번들에 대해 기계 번역을 제공하는 언어 서비스를 변경하려면 <a href=https://new-console.stage1.ng.bluemix.net/docs/services/GlobalizationPipeline/managing_translations.html#globalizationpipeline_service_to_service>MT 구성</a> 탭을 클릭하여 기타 지원되는 기계 번역 엔진을 보십시오.</p></li>

<li><strong>저장</strong> 클릭</li></ol>


번들이 작성된 후 업로드된 리소스 파일이 사용자가 지정한 모든 대상 언어로 번역됩니다. 새 번들이 번들 탭에 추가되며, 여기서 다음을 수행할 수 있습니다.

* 언어 추가 또는 제거
* 생성된 번역 편집
* 번들에서 사용되는 소스 파일 업데이트 및 번역 재생성
