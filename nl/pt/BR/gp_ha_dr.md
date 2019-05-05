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


# Alta disponibilidade e recuperação de desastre
{: #ha-dr}

O serviço {{site.data.keyword.GlobalizationPipeline_full}} está altamente disponível no local do {{site.data.keyword.Bluemix}} (Dallas, Sydney, Londres e Frankfurt).
{: shortdesc}

## Alta disponibilidade

O serviço {{site.data.keyword.GlobalizationPipeline_full}} suporta alta disponibilidade. O serviço atinge alta disponibilidade de forma automática e transparente por meio do balanceador de carga na frente para distribuir solicitações para os Pods no Controlador de replicação.

## Recuperação de desastre

A recuperação de desastre poderá tornar-se um problema se um local do {{site.data.keyword.Bluemix}} tiver uma falha significativa que inclua a perda potencial de dados. Como a Multi-Zone Region (MZR) não está disponível em todos os locais, deve-se aguardar a IBM colocar um local novamente on-line se ele ficar indisponível. Se os serviços de dados subjacentes estiverem comprometidos com a falha, você deverá também esperar que a IBM restaure esses serviços de dados para recuperar dados de backups de banco de dados.

Consulte [Como assegurar o tempo de inatividade zero](/docs/overview?topic=overview-zero-downtime#zero-downtime) para saber mais sobre os padrões de alta disponibilidade e de recuperação de desastre no {{site.data.keyword.Bluemix_notm}}. Também é possível localizar informações sobre [Acordos de Nível de Serviço](/docs/overview?topic=overview-zero-downtime#SLAs).  














