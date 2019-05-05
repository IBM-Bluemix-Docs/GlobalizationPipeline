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


# Eventos de {{site.data.keyword.cloudaccesstrailshort}} do {{site.data.keyword.GlobalizationPipeline_short}}
{: #gpat_events}

Use o serviço {{site.data.keyword.cloudaccesstrailfull}} para controlar como os usuários e aplicativos interagem com o IBM {{site.data.keyword.GlobalizationPipeline_short}} no {{site.data.keyword.Bluemix}}.
{:shortdesc}

O serviço {{site.data.keyword.cloudaccesstrailfull_notm}} registra as atividades iniciadas pelo usuário que mudam
o estado de um serviço no {{site.data.keyword.Bluemix_notm}}. Para obter informações adicionais, consulte [{{site.data.keyword.cloudaccesstrailfull_notm}}](/docs/services/cloud-activity-tracker/index.html).




## Lista de eventos: eventos de pacotes configuráveis
{: #gpevents_bundle}

A tabela a seguir lista as ações que estão relacionadas a pacotes configuráveis e geram um evento:

|Ações|Descri‡Æo|
|---|---|  
|g11n-pipeline.bundles.read|Obtém uma lista de IDs de pacote configurável.|
|g11n-pipeline.bundle.create|Cria um novo pacote configurável.|
|g11n-pipeline.bundle.read|Obtém as informações do pacote configurável.|
|g11n-pipeline.bundle.update|Atualiza a configuração do pacote configurável.|
|g11n-pipeline.bundle.delete|Exclui o pacote configurável especificado.|
|g11n-pipeline.bundle-language.create|Faz upload de entradas de recursos.|
|g11n-pipeline.bundle-language.read|Obtém as sequências de recursos (pares de chave/valor) para o idioma.|
|g11n-pipeline.bundle-language.update|Atualiza entradas de recursos.|
|g11n-pipeline.bundle-language.read|Obtém as informações de entrada de recurso.|
|g11n-pipeline.bundle-language.update|Atualiza a entrada de recurso.|

## Lista de eventos: eventos de solicitação de tradução de pacote
{: #gpevents_bundle_tr_req}

A tabela a seguir lista as ações que estão relacionadas às solicitações de tradução de pacote configurável e geram um evento:

|Ações|Descri‡Æo|
|---|---|  
|g11n-pipeline.trs.read|Obtém uma lista de solicitações de tradução.|
|g11n-pipeline.tr.read|Obtém as informações da solicitação de tradução especificada.|
|g11n-pipeline.tr.update|Atualiza as informações da solicitação de tradução especificada.|
|g11n-pipeline.tr.delete|Exclui a solicitação de tradução especificada.|
|g11n-pipeline.tr-bundle.read|Obtém as informações do pacote configurável.|
|g11n-pipeline.tr-bundle-language.read|Obtém entradas de recursos para o pacote configurável e o idioma especificados.|
|g11n-pipeline.tr-bundle-language.read|Obtém as informações de entrada de recurso.|
|g11n-pipeline.trs.create|Cria uma nova solicitação de tradução.|


## Lista de eventos: eventos xliff do pacote configurável
{: #gpevents_bundle_xliff}

A tabela a seguir lista as ações que estão relacionadas ao pacote configurável xliff e geram um evento:

|Ações|Descri‡Æo|
|---|---|  
|g11n-pipeline.xliff-bundles.read|Obtém dados de recurso no idioma especificado por meio dos pacotes configuráveis no formato XLIFF 2.0.|
|g11n-pipeline.xliff-bundles.update|Atualiza os pacotes configuráveis na instância de serviço com os dados XLIFF.|
|g11n-pipeline.xliff-tr-bundles.read|Obtém os dados de recurso no idioma especificado na solicitação de tradução no formato XLIFF 2.0.|


## Lista de eventos: eventos de parceiros
{: #gpevents_partner}

A tabela a seguir lista as ações que estão relacionadas a parceiros e geram um evento:

|Ações|Descri‡Æo|
|---|---|  
|g11n-pipeline.partner.read|Obtém as informações do parceiro.|
|g11n-pipeline.partner.update|Atualiza as informações do parceiro.|
|g11n-pipeline.partner-trs.read|Obtém uma lista de solicitações de tradução designadas ao parceiro.|
|g11n-pipeline.partner-tr.read|Obtém as informações da solicitação de tradução especificada.|
|g11n-pipeline.partner-tr.update|Atualiza as informações da solicitação de tradução especificada.|
|g11n-pipeline.partner-tr.delete|Exclui a solicitação de tradução especificada.|
|g11n-pipeline.partner-tr-bundle.read|Obtém as informações do pacote configurável.|
|g11n-pipeline.partner-tr-bundle-language.read|Obtém entradas de recursos para o pacote configurável e o idioma especificados.|
|g11n-pipeline.partner-tr-bundle-language.update|Atualiza entradas de recursos para o pacote configurável e o idioma especificados.|
|g11n-pipeline.partner-tr-bundle-language.read|Obtém as informações de entrada de recurso.|
|g11n-pipeline.partner-tr-bundle-language.update|Atualiza a entrada de recurso.|
|g11n-pipeline.partner-users.read|Obtém os usuários disponíveis para esse parceiro.|
|g11n-pipeline.partner-user.read|Obtém as informações do usuário de parceiro especificado.|
|g11n-pipeline.partner-user.update|Atualize as informações de um usuário do parceiro.|
|g11n-pipeline.partner-user.delete|Exclui o usuário do parceiro especificado.|
|g11n-pipeline.partner-user.create|Cria um novo usuário de parceiro.|
|g11n-pipeline.partner-tr-xliff-bundles.update|Atualiza os dados de recurso na solicitação de tradução com os dados XLIFF.|
|g11n-pipeline.partner-tr-xliff-bundles-language.read|Obtém os dados de recurso no idioma especificado na solicitação de tradução no formato XLIFF 2.0.|



## Lista de eventos: eventos do administrador
{: #gpevents_admin}

A tabela a seguir lista as ações que estão relacionadas ao administrador e geram um evento:

|Ações|Descri‡Æo|
|---|---|  
|g11n-pipeline.instances.read|Obtém uma lista de instâncias de serviço.|
|g11n-pipeline.instance.read|Obtém as informações da instância de serviço.|
|g11n-pipeline.instance.update|Atualiza a configuração da instância de serviço.|
|g11n-pipeline.instance.create|Cria uma nova instância de serviço.|
|g11n-pipeline.instance.delete|Exclui a instância de serviço especificada.|
|g11n-pipeline.instance.create|Cria uma nova instância de serviço gerenciado do Cloud Foundry.|
|g11n-pipeline.partners.read|Obtém uma lista de parceiros.|
|g11n-pipeline.partner.create|Cria um novo parceiro.|
|g11n-pipeline.partner.delete|Exclui o parceiro especificado.|



## Lista de eventos: eventos do usuário
{: #gpevents_user}

A tabela a seguir lista as ações que estão relacionadas aos usuários e geram um evento:

|Ações|Descri‡Æo|
|---|---|  
|g11n-pipeline.instance-users.read|Obtém os usuários nessa instância de serviço.|
|g11n-pipeline.instance-user.read|Obtém as informações do usuário especificado.|
|g11n-pipeline.instance-user.update|Atualiza as informações de um usuário.|
|g11n-pipeline.instance-user.delete|Exclui o usuário especificado.|
|g11n-pipeline.instance-users.create|Cria um novo usuário.|


## Lista de eventos: eventos de configuração
{: #gpevents_config}

A tabela a seguir lista as ações que estão relacionadas à configuração de tradução e geram um evento:

|Ações|Descri‡Æo|
|---|---|  
|g11n-pipeline.config-mts.read|Obtém todas as ligações de serviço de MT.|
|g11n-pipeline.config-mt.read|Obtém os dados de ligação de serviço de MT.|
|g11n-pipeline.config-translations.read|Obtém todas as configurações de tradução.|
|g11n-pipeline.config-translation.read|Obtém a configuração de tradução.|
|g11n-pipeline.config-mt.update|Coloca os dados de ligação de serviço de MT especificados. Se os dados de ligação especificados já existirem, eles serão substituídos pelos dados de ligação de serviço de MT especificados.|
|g11n-pipeline.config-mt.delete|Exclui os dados de ligação de serviço de MT especificados.|
|g11n-pipeline.config-translation.update|Coloca a configuração de tradução para o par de idiomas especificado. Se a configuração para o par já existir, ela será substituída pela configuração especificada.|
|g11n-pipeline.config-translation.delete|Exclui a configuração de tradução para o par de idiomas especificado.|


## Lista de eventos: eventos de instância
{: #gpevents_instance}

A tabela a seguir lista as ações que estão relacionadas a instâncias e geram um evento:

|Ações|Descri‡Æo|
|---|---|  
|g11n-pipeline.instance.read|Obtém as informações dessa instância de serviço de tradução.|


## Onde procurar os eventos
{: #gp_at_ui}

Os eventos de {{site.data.keyword.cloudaccesstrailshort}} estão disponíveis no **domínio de espaço** do {{site.data.keyword.cloudaccesstrailshort}} que está disponível na região do {{site.data.keyword.Bluemix_notm}} na qual o serviço {{site.data.keyword.GlobalizationPipeline_short}} é provisionado. A instância de serviço do {{site.data.keyword.cloudaccesstrailshort}} e a instância do {{site.data.keyword.GlobalizationPipeline_short}} devem ser aprovisionadas no mesmo espaço do CF.

Para instâncias do RC do {{site.data.keyword.GlobalizationPipeline_short}}, os eventos do Activity Tracker estão disponíveis no domínio de **conta** do Activity Tracker no qual os eventos são gerados na região do {{site.data.keyword.Bluemix_notm}}.
