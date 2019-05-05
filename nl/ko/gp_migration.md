---

copyright:
  years: 2015, 2019
lastupdated: "2019-03-25"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:codeblock: .codeblock}
{:tip: .tip}
{:download: .download}


# 리소스 그룹으로 {{site.data.keyword.GlobalizationPipeline_short}} 서비스 인스턴스 마이그레이션
{: #rg-migration}

기존 {{site.data.keyword.GlobalizationPipeline_short}} CF 인스턴스 사용자에게는 서비스의 RC/IAM 호환 가능 버전으로 마이그레이션하도록 3개월(프로덕션에서 RC/IAM 버전이 사용 가능하게 된 날짜로부터)의 시간이 주어집니다. 


## 시작하기 전에
{: #prereqs}

{{site.data.keyword.GlobalizationPipeline_short}} 서비스 인스턴스의 마이그레이션을 시작하기 전에, 사용자는 서비스 인스턴스의 모든 데이터가 유지된다는 점을 알고 있어야 합니다. 잃어버리는 데이터는 없습니다. 사용자는 마이그레이션 후 서비스 인스턴스의 상태가 마이그레이션 전과 동일한 것을 확인할 수 있습니다.    

마이그레이션 프로세스의 개요는 [Cloud Foundry 서비스 인스턴스를 리소스 그룹으로 마이그레이션](/docs/resources/instance_migration.html)을 참조하십시오.  

## 마이그레이션 단계
{: #gp_steps_migration}

1. **추가 조치** 메뉴를 여십시오. 
2. 리소스 그룹으로 **마이그레이션**을 선택하여 작업을 시작하십시오. 
3. 리소스 그룹을 선택하십시오. 
4. **마이그레이션**을 클릭하면 해당 인스턴스가 마이그레이션됩니다. 

**참고:** 한 번에 하나의 인스턴스만 마이그레이션할 수 있으므로 첫 번째 인스턴스의 마이그레이션을 완료해야 다음 적격 인스턴스의 마이그레이션을 계속할 수 있습니다. 

## 다음 단계
{: #nextsteps}

리소스 목록의 **서비스** 섹션에서 마이그레이션된 서비스 인스턴스를 볼 수 있습니다. 별명은 리소스 목록의 Cloud Foundry 섹션에 유지됩니다. 이는 인플레이스 마이그레이션이므로 모든 인스턴스 데이터 및 인증 정보가 유지됩니다. 사용자는 원본 CF 인스턴스가 생성한 인증 정보를 계속해서 사용할 수 있습니다.  

마이그레이션이 수행되는 방식에 대한 자세한 정보는 [마이그레이션이 수행되는 방식](/docs/resources/instance_migration.html#how)을 참조하십시오. 


