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


# Migrando as instâncias de serviço do {{site.data.keyword.GlobalizationPipeline_short}} para um grupo de recursos
{: #rg-migration}

Os usuários existentes da instância do CF do {{site.data.keyword.GlobalizationPipeline_short}} têm 3 meses (da data em que a versão do RC/IAM está disponível em produção) para migrar para a versão de serviço compatível com RC/IAM.


## Antes de Começar
{: #prereqs}

Antes de iniciar a migração de suas instâncias de serviço do {{site.data.keyword.GlobalizationPipeline_short}}, é necessário saber que todos os dados para a instância de serviço são preservados. Você não perde nada. Após a migração, será possível ver suas instâncias de serviço no mesmo estado que elas eram antes da migração.   

Para obter uma visão geral do processo de migração, consulte [Migrando as instâncias de serviço do Cloud Foundry para um grupo de recursos](/docs/resources/instance_migration.html). 

## Etapas para migração
{: #gp_steps_migration}

1. Abra o menu **Mais ações**.
2. Selecione **Migrar** para um grupo de recursos ser iniciado.
3. Selecione um grupo de recursos.
4. Clique em **Migrar** e a instância é migrada para você.

**Nota:** é possível migrar somente uma instância por vez, para que seja possível continuar a migração de instâncias elegíveis depois de migrar com sucesso a primeira.

## Próximas Etapas
{: #nextsteps}

Você vê as instâncias de serviço migradas na seção **Serviços** da sua lista de recursos. O alias permanece na seção Cloud Foundry da lista de recursos. Essa é uma migração no local, portanto, todos os dados de instância e credenciais são preservados. É possível continuar usando as credenciais geradas pela instância do CF original. 

Para obter mais informações sobre como a migração funciona, consulte [Como a migração funciona](/docs/resources/instance_migration.html#how).


