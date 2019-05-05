---

copyright:
  years: 2018, 2019
lastupdated: "2019-03-22"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:codeblock: .codeblock}
{:tip: .tip}
{:download: .download}


# 고가용성 및 재해 복구
{: #ha-dr}

{{site.data.keyword.GlobalizationPipeline_full}} 서비스는 {{site.data.keyword.Bluemix}} 위치(댈러스, 시드니, 런던 및 프랑크푸르트) 내에서 고가용성을 제공합니다.
{: shortdesc}

## 고가용성

{{site.data.keyword.GlobalizationPipeline_full}} 서비스는 고가용성을 지원합니다. 이 서비스는 복제 제어기 내 팟(Pod) 간에 요청을 먼저 분배하는 로드 밸런서를 통해 자동으로, 그리고 투명하게 고가용성을 달성합니다. 

## 재해 복구

{{site.data.keyword.Bluemix}} 위치에서 잠재적 데이터 손실을 포함한 심각한 장애가 발생하는 경우에는 재해 복구가 문제가 될 수 있습니다. 다중 구역 지역(MZR)은 위치 간에 사용할 수 없으므로, 특정 위치가 사용 불가능 상태가 되는 경우 사용자는 IBM이 이를 온라인 상태로 복구할 때까지 기다려야 합니다. 이 장애로 인해 기반 데이터 서비스에 장애가 발생하는 경우에도 데이터베이스 백업에서 데이터를 복원하기 위해서는 IBM이 이러한 데이터 서비스를 복원하기를 기다려야 합니다. 

{{site.data.keyword.Bluemix_notm}}의 고가용성 및 재해 복구 표준에 대해 더 자세히 알아보려면 [작동 중단이 발생하지 않도록 하는 방법](/docs/overview?topic=overview-zero-downtime#zero-downtime)을 참조하십시오. [서비스 레벨 계약](/docs/overview?topic=overview-zero-downtime#SLAs)에 대한 정보도 찾아볼 수 있습니다.   














