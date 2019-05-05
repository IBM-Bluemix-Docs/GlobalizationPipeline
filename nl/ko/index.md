---

copyright:
  years: 2015, 2018
lastupdated: "2017-12-13"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}


# {{site.data.keyword.GlobalizationPipeline_short}} 시작
{: #globalizationpipeline}

{{site.data.keyword.GlobalizationPipeline_full}}은 앱 개발자가 번역된 애플리케이션을 글로벌 고객에게 신속하게 릴리스하는 데 사용할 수 있는 {{site.data.keyword.Bluemix}} 서비스입니다. {{site.data.keyword.GlobalizationPipeline_short}}은 번역을 DevOps 및 Continuous Development 인프라에 원활하게 통합할 수 있도록 기계 번역, 사람에 의한 검토 및 편집, API 및 SDK를 제공하는 번역 저장소 역할을 수행하여 기존 번역 프로세스와 연관된, 격리된 수작업을 제거합니다.
{:shortdesc}

{{site.data.keyword.GlobalizationPipeline_short}} 서비스를 사용하여 {{site.data.keyword.Bluemix_notm}}에서 개발되어 호스트되는 앱을 번역하거나 다른 클라우드 플랫폼에서 호스트되는 앱을 번역하도록 바인드를 해제할 수 있습니다.

{{site.data.keyword.GlobalizationPipeline_short}}에서는 앱 번역을 관리하는 대시보드 인터페이스와 번역 프로세스를 완전히 자동화하는 RESTful API를 둘 다 제공합니다. {{site.data.keyword.GlobalizationPipeline_short}} API에 대한 정보는 [API 참조](https://gp-rest.ng.bluemix.net/translate/swagger/index.html){: new_window}를 확인하십시오.

## 번역 플랜 선택
{: #globalizationpipeline_chooseplan}

{{site.data.keyword.GlobalizationPipeline_short}}에 대한 번역 작업을 시작하기 전에 적절한 번역 플랜을 선택할 수 있습니다.

{{site.data.keyword.GlobalizationPipeline_short}}에서 사용할 수 있는 번역 플랜은 Standard 플랜과 Professional 플랜의 두 가지가 있습니다. 두 플랜 모두 통합된 무제한 기본 기계 번역을 제공할 뿐만 아니라 추가 비용을 지불하면 다른 기계 번역 엔진과 통합하는 기능도 제공합니다. Professional 플랜에서 {{site.data.keyword.GlobalizationPipeline_short}}은 전문가 번역 검토 및 편집 서비스를 추가로 제공합니다. 모든 데이터를 유지하면서 {{site.data.keyword.Bluemix_notm}} 내에서 {{site.data.keyword.GlobalizationPipeline_short}} 플랜을 전환할 수 있습니다. 


## {{site.data.keyword.GlobalizationPipeline_short}} 데이터 사용 추정
{: #globalizationpipeline_documentpricing}

{{site.data.keyword.GlobalizationPipeline_short}}에서는 백엔드 데이터베이스에 번역을 저장합니다. 활성 데이터 크기를 추정하려면 다음 공식을 참조할 수 있습니다. 

`<expected resource data storage size in MB> ˜= 0.0005 * <number of key/value pairs in the source resource> * <number of languages including the source language>`

공식에 따라 일반 번들의 크기는 `(length of key + length of value in UTF-8 = ˜40 bytes)`입니다.

예를 들어, 100개의 키/값 쌍이 있고 이를 9개의 언어로 번역하는 경우 예상되는 스토리지 크기는 0.0005 100(9+1) = 0.5MB입니다. 실제 크기는 번역과 함께 저장된 메타데이터 및 실제 키/값 크기에 따라 다를 수 있습니다.

월별 서비스 비용을 판별하려면 {{site.data.keyword.Bluemix_notm}} [가격 계산기](https://console.ng.bluemix.net/?direct=classic/#/pricing/cloudOEPaneId=pricing&paneId=pricingSheet&orgGuid=127a45f4-4461-4d5b-a26b-6dc2fdd1a3a2&spaceGuid=208fb1ff-413b-4fd9-9615-e8226062d0f3)를 사용하십시오. 

**참고**: Professional 플랜 검토 기능을 사용하면 이전에 언급된 크기 이상으로 데이터 사용량이 증가합니다. 
