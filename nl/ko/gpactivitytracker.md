---

copyright:
  years: 2016, 2019

lastupdated: "2019-03-20"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:codeblock: .codeblock}
{:tip: .tip}
{:download: .download}


# {{site.data.keyword.GlobalizationPipeline_short}} {{site.data.keyword.cloudaccesstrailshort}} 이벤트
{: #gpat_events}

{{site.data.keyword.Bluemix}}에서 사용자 및 애플리케이션이 IBM {{site.data.keyword.GlobalizationPipeline_short}}과 어떻게 상호작용하는지 추적하려면 {{site.data.keyword.cloudaccesstrailfull}} 서비스를 사용하십시오.
{:shortdesc}

{{site.data.keyword.cloudaccesstrailfull_notm}} 서비스는 {{site.data.keyword.Bluemix_notm}} 내 서비스의 상태를 변경하는 사용자 시작 활동을 기록합니다. 자세한 정보는 [{{site.data.keyword.cloudaccesstrailfull_notm}}](/docs/services/Activity-Tracker-with-LogDNA?topic=logdnaat-getting-started)의 내용을 참조하십시오. 




## 이벤트의 목록: 번들 이벤트
{: #gpevents_bundle}

다음 표에는 번들과 관련되어 있으며 이벤트를 생성하는 조치가 나열되어 있습니다. 

|조치|설명|
|---|---|  
|g11n-pipeline.bundles.read|번들 ID의 목록을 가져옵니다.|
|g11n-pipeline.bundle.create|새 번들을 작성합니다.|
|g11n-pipeline.bundle.read|번들의 정보를 가져옵니다.|
|g11n-pipeline.bundle.update|번들의 구성을 업데이트합니다.|
|g11n-pipeline.bundle.delete|지정된 번들을 삭제합니다.|
|g11n-pipeline.bundle-language.create|리소스 항목을 업로드합니다.|
|g11n-pipeline.bundle-language.read|해당 언어의 리소스 문자열(키/값 쌍)을 가져옵니다.|
|g11n-pipeline.bundle-language.update|리소스 항목을 업데이트합니다.|
|g11n-pipeline.bundle-language.read|리소스 항목 정보를 가져옵니다.|
|g11n-pipeline.bundle-language.update|리소스 항목을 업데이트합니다.|

## 이벤트의 목록: 번들 번역 요청 이벤트
{: #gpevents_bundle_tr_req}

다음 표에는 번들 번역 요청과 관련되어 있으며 이벤트를 생성하는 조치가 나열되어 있습니다. 

|조치|설명|
|---|---|  
|g11n-pipeline.trs.read|번역 요청의 목록을 가져옵니다.|
|g11n-pipeline.tr.read|지정된 번역 요청의 정보를 가져옵니다.|
|g11n-pipeline.tr.update|지정된 번역 요청의 정보를 업데이트합니다.|
|g11n-pipeline.tr.delete|지정된 번역 요청을 삭제합니다.|
|g11n-pipeline.tr-bundle.read|번들의 정보를 가져옵니다.|
|g11n-pipeline.tr-bundle-language.read|지정된 번들 및 언어의 리소스 항목을 가져옵니다.|
|g11n-pipeline.tr-bundle-language.read|리소스 항목 정보를 가져옵니다.|
|g11n-pipeline.trs.create|새 번역 요청을 작성합니다.|


## 이벤트의 목록: 번들 xliff 이벤트
{: #gpevents_bundle_xliff}

다음 표에는 번들 xliff와 관련되어 있으며 이벤트를 생성하는 조치가 나열되어 있습니다. 

|조치|설명|
|---|---|  
|g11n-pipeline.xliff-bundles.read|XLIFF 2.0 형식의 번들에서 지정된 언어의 리소스 데이터를 가져옵니다.|
|g11n-pipeline.xliff-bundles.update|XLIFF 데이터로 서비스 인스턴스의 번들을 업데이트합니다.|
|g11n-pipeline.xliff-tr-bundles.read|XLIFF 2.0 형식의 번역 요청에서 지정된 언어의 리소스 데이터를 가져옵니다.|


## 이벤트의 목록: 파트너 이벤트
{: #gpevents_partner}

다음 표에는 파트너와 관련되어 있으며 이벤트를 생성하는 조치가 나열되어 있습니다. 

|조치|설명|
|---|---|  
|g11n-pipeline.partner.read|파트너의 정보를 가져옵니다.|
|g11n-pipeline.partner.update|파트너의 정보를 업데이트합니다.|
|g11n-pipeline.partner-trs.read|파트너에게 지정된 번역 요청의 목록을 가져옵니다.|
|g11n-pipeline.partner-tr.read|지정된 번역 요청의 정보를 가져옵니다.|
|g11n-pipeline.partner-tr.update|지정된 번역 요청의 정보를 업데이트합니다.|
|g11n-pipeline.partner-tr.delete|지정된 번역 요청을 삭제합니다.|
|g11n-pipeline.partner-tr-bundle.read|번들의 정보를 가져옵니다.|
|g11n-pipeline.partner-tr-bundle-language.read|지정된 번들 및 언어의 리소스 항목을 가져옵니다.|
|g11n-pipeline.partner-tr-bundle-language.update|지정된 번들 및 언어의 리소스 항목을 업데이트합니다.|
|g11n-pipeline.partner-tr-bundle-language.read|리소스 항목 정보를 가져옵니다.|
|g11n-pipeline.partner-tr-bundle-language.update|리소스 항목을 업데이트합니다.|
|g11n-pipeline.partner-users.read|이 파트너의 사용 가능한 사용자를 가져옵니다.|
|g11n-pipeline.partner-user.read|지정된 파트너 사용자의 정보를 가져옵니다.|
|g11n-pipeline.partner-user.update|파트너 사용자의 정보를 업데이트합니다.|
|g11n-pipeline.partner-user.delete|지정된 파트너 사용자를 삭제합니다.|
|g11n-pipeline.partner-user.create|새 파트너 사용자를 작성합니다.|
|g11n-pipeline.partner-tr-xliff-bundles.update|XLIFF 데이터로 번역 요청의 리소스 데이터를 업데이트합니다.|
|g11n-pipeline.partner-tr-xliff-bundles-language.read|XLIFF 2.0 형식의 번역 요청에서 지정된 언어의 리소스 데이터를 가져옵니다.|



## 이벤트의 목록: 관리자 이벤트
{: #gpevents_admin}

다음 표에는 관리자와 관련되어 있으며 이벤트를 생성하는 조치가 나열되어 있습니다. 

|조치|설명|
|---|---|  
|g11n-pipeline.instances.read|서비스 인스턴스의 목록을 가져옵니다.|
|g11n-pipeline.instance.read|서비스 인스턴스의 정보를 가져옵니다.|
|g11n-pipeline.instance.update|서비스 인스턴스의 구성을 업데이트합니다.|
|g11n-pipeline.instance.create|새 서비스 인스턴스를 작성합니다.|
|g11n-pipeline.instance.delete|지정된 서비스 인스턴스를 삭제합니다.|
|g11n-pipeline.instance.create|새 Cloud Foundry 관리 서비스 인스턴스를 작성합니다.|
|g11n-pipeline.partners.read|파트너의 목록을 가져옵니다.|
|g11n-pipeline.partner.create|새 파트너를 작성합니다.|
|g11n-pipeline.partner.delete|지정된 파트너를 삭제합니다.|



## 이벤트의 목록: 사용자 이벤트
{: #gpevents_user}

다음 표에는 사용자와 관련되어 있으며 이벤트를 생성하는 조치가 나열되어 있습니다. 

|조치|설명|
|---|---|  
|g11n-pipeline.instance-users.read|서비스 인스턴스의 사용자를 가져옵니다.|
|g11n-pipeline.instance-user.read|지정된 사용자의 정보를 가져옵니다.|
|g11n-pipeline.instance-user.update|사용자의 정보를 업데이트합니다.|
|g11n-pipeline.instance-user.delete|지정된 사용자를 삭제합니다.|
|g11n-pipeline.instance-users.create|새 사용자를 작성합니다.|


## 이벤트의 목록: 구성 이벤트
{: #gpevents_config}

다음 표에는 번역 구성과 관련되어 있으며 이벤트를 생성하는 조치가 나열되어 있습니다. 

|조치|설명|
|---|---|  
|g11n-pipeline.config-mts.read|모든 MT 서비스 바인딩을 가져옵니다.|
|g11n-pipeline.config-mt.read|MT 서비스 바인딩 데이터를 가져옵니다.|
|g11n-pipeline.config-translations.read|모든 번역 구성을 가져옵니다.|
|g11n-pipeline.config-translation.read|번역 구성을 가져옵니다.|
|g11n-pipeline.config-mt.update|지정된 MT 서비스 바인딩 데이터를 삽입합니다. 지정된 바인딩 데이터가 이미 있는 경우에는 지정된 MT 서비스 바인딩 데이터로 대체됩니다.|
|g11n-pipeline.config-mt.delete|지정된 MT 서비스 바인딩 데이터를 삭제합니다.|
|g11n-pipeline.config-translation.update|지정된 언어 쌍의 번역 구성을 삽입합니다. 해당 쌍에 대한 구성이 이미 있는 경우에는 지정된 구성으로 대체됩니다.|
|g11n-pipeline.config-translation.delete|지정된 언어 쌍의 번역 구성을 삭제합니다.|


## 이벤트의 목록: 인스턴스 이벤트
{: #gpevents_instance}

다음 표에는 인스턴스와 관련되어 있으며 이벤트를 생성하는 조치가 나열되어 있습니다. 

|조치|설명|
|---|---|  
|g11n-pipeline.instance.read|이 번역 서비스 인스턴스의 정보를 가져옵니다.|


## 이벤트를 찾을 위치
{: #gp_at_ui}

{{site.data.keyword.cloudaccesstrailshort}} 이벤트는 {{site.data.keyword.GlobalizationPipeline_short}} 서비스가 프로비저닝된 {{site.data.keyword.Bluemix_notm}} 지역의 {{site.data.keyword.cloudaccesstrailshort}} **영역 도메인**에 있습니다. {{site.data.keyword.cloudaccesstrailshort}} 서비스와 {{site.data.keyword.GlobalizationPipeline_short}} 인스턴스는 동일한 CF 영역에서 프로비저닝되어야 합니다. 

{{site.data.keyword.GlobalizationPipeline_short}}의 RC 인스턴스의 경우, Activity Tracker 이벤트는 {{site.data.keyword.Bluemix_notm}} 지역에서 이벤트가 생성되는 **계정** 도메인에 있습니다. 
