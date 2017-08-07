---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# 기계 번역 구성
{: #machineconfig}

{{site.data.keyword.GlobalizationPipeline_full}}에서는 대체 기계 번역 서비스를 통합하는 기능을 지원하여 번들에 대해 기계 번역을 수행합니다. {{site.data.keyword.GlobalizationPipeline_short}}에서 활용되는 기본 엔진이 필요한 특정 언어를 제공하지 않는 경우나 다른 엔진에서 생성되는 기계 번역을 선호하는 경우 대체 서비스를 추가하면 유용할 수 있습니다. 대체 서비스의 사용 및 담당은 해당 서비스의 이용 약관에 따릅니다.

{{site.data.keyword.GlobalizationPipeline_short}}에 대해 대체 기계 번역 서비스를 추가하고 구성하려면 {{site.data.keyword.GlobalizationPipeline_short}} 대시보드에서 **기계 번역 구성** 탭을 선택하십시오.

* {{site.data.keyword.Bluemix_notm}} 카탈로그에 있는 기계 번역 서비스(**Watson 언어 번역기**)를 추가하려면 먼저 서비스를 {{site.data.keyword.Bluemix_notm}} 영역에 추가해야 합니다.

* 써드파티 서비스를 추가하려면 **기계 번역 구성** 탭의 해당 서비스 단추를 선택하고 서비스에 액세스하는 데 필요한 사용자 신임 정보를 제공하십시오.

기계 번역 서비스가 {{site.data.keyword.GlobalizationPipeline_short}}에 추가된 후 나머지 단계를 수행하여 해당 서비스의 통합을 완료하십시오.

1. **사용**을 클릭하여 해당 서비스와의 통합을 켜십시오.

2. **언어 업데이트**를 클릭하여 지원되는 대상 언어의 업데이트된 목록을 보십시오.

3. 대상 언어의 목록에서 번역을 수행해야 하는 기계 번역 엔진을 선택하십시오.

4. **저장**을 클릭하여 **기계 번역 구성** 탭으로 돌아가십시오.

대체 서비스가 {{site.data.keyword.GlobalizationPipeline_short}}과 함께 구성되었으면 해당 엔진에 지정된 모든 대상 언어가 해당 엔진을 통해 생성되기 시작합니다. 

대체 기계 번역 엔진 사용을 중지하려면 다음을 수행하십시오.

1. **기계 번역 구성** 탭에서 사용을 중지할 서비스에 대한 **사용 안함** 단추를 클릭하십시오.

대체 기계 번역 서비스를 사용 안함으로 설정하면 서비스에서 생성된 모든 번역이 번들 내에 남습니다. 그러나 특정 대상 언어로의 번역은 현재 사용으로 설정한 기계 번역 엔진에서 대상 언어를 지원하지 않는 경우 향후 업데이트에 사용하지 못할 수 있습니다. 

<!-- Review comment: When you disable an engine, do you need to go back and reconfigure the languages?? Does it go back to the default engine? What happens? -->
