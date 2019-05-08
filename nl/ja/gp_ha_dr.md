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


# 高可用性および災害復旧
{: #ha-dr}

{{site.data.keyword.GlobalizationPipeline_full}} サービスは、{{site.data.keyword.Bluemix}} ロケーション (ダラス、シドニー、ロンドン、およびフランクフルト) の内部では可用性が高くなっています。
{: shortdesc}

## 高可用性

{{site.data.keyword.GlobalizationPipeline_full}} サービスは高可用性をサポートします。このサービスは、レプリケーション・コントローラーの各ポッドに要求を分散させるロード・バランサーを前方に配置することで、高可用性を自動的かつ透過的に実現します。

## 災害復旧

{{site.data.keyword.Bluemix}} ロケーションでデータを損失する可能性のある重大な障害が発生した場合に、災害復旧の問題が持ち上がってくる場合があります。ロケーションをまたいだ複数ゾーン地域 (MZR) を使用できないため、あるロケーションが使用できない状態になった場合は、IBM がそこをオンラインに復旧するまで待機する必要があります。基盤となるデータ・サービスが障害の影響を受けた場合にも、IBM がこれらのデータ・サービスを復元し、データベース・バックアップからデータをリカバリーするまで待つ必要があります。

{{site.data.keyword.Bluemix_notm}} での高可用性と災害復旧の規格について詳しくは、[ダウン時間をゼロにする方法](/docs/overview?topic=overview-zero-downtime#zero-downtime)を参照してください。[サービス・レベル・アグリーメント](/docs/overview?topic=overview-zero-downtime#SLAs)についての情報もご確認いただけます。  














