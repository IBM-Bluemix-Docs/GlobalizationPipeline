---

copyright:
  years: 2015, 2018
lastupdated: "2017-12-13"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}


# Introdução do {{site.data.keyword.GlobalizationPipeline_short}}
{: #globalizationpipeline}

O {{site.data.keyword.GlobalizationPipeline_full}} é um serviço {{site.data.keyword.Bluemix}} que permite que os desenvolvedores de aplicativo liberem rapidamente os aplicativos traduzidos para clientes globais. O {{site.data.keyword.GlobalizationPipeline_short}} serve como um repositório de tradução que fornece tradução de máquina, revisão e edição humana e APIs e SDKs para integrar perfeitamente a tradução em sua infraestrutura do DevOps and Continuous Development, eliminando operações manuais e isoladas associadas ao processo de tradução tradicional.
{:shortdesc}

É possível usar o serviço {{site.data.keyword.GlobalizationPipeline_short}} para traduzir qualquer app implementado e hospedado no {{site.data.keyword.Bluemix_notm}} ou desvincular para traduzir apps hospedados em outras plataformas de nuvem.

O {{site.data.keyword.GlobalizationPipeline_short}} oferece uma interface de painel para gerenciar sua tradução de app e uma API RESTful que automatiza totalmente o processo de tradução. Para obter informações sobre a API do {{site.data.keyword.GlobalizationPipeline_short}}, veja [Referência de API](https://gp-rest.ng.bluemix.net/translate/swagger/index.html){: new_window}.

## Escolhendo um plano de tradução
{: #globalizationpipeline_chooseplan}

Antes de começar a trabalhar com tradução no {{site.data.keyword.GlobalizationPipeline_short}}, é possível escolher um plano de tradução adequado.

Há dois planos de tradução disponíveis no {{site.data.keyword.GlobalizationPipeline_short}}, o plano Padrão e o plano Profissional. Ambos os planos fornecem tradução básica de máquina ilimitada e integrada, bem como o recurso para integração com outros mecanismos de tradução de máquina por um encargo adicional. No plano Profissional, o {{site.data.keyword.GlobalizationPipeline_short}} oferece também um serviço de revisão e edição de tradução profissional. É possível alternar entre os planos do {{site.data.keyword.GlobalizationPipeline_short}} dentro do {{site.data.keyword.Bluemix_notm}} com todos os dados reservados.


## Estimando o uso de dados do {{site.data.keyword.GlobalizationPipeline_short}}
{: #globalizationpipeline_documentpricing}

O {{site.data.keyword.GlobalizationPipeline_short}} armazena suas traduções em um banco de dados de backend. Para estimar o tamanho de dados ativos, é possível consultar a fórmula a seguir:

`<expected resource data storage size in MB> ˜= 0.0005 * <number of key/value pairs in the source resource> * <number of languages including the source language>`

De acordo com a fórmula, o tamanho de um pacote configurável típico é `(comprimento da chave + comprimento do valor em UTF-8 = ˜40 bytes)`.

Por exemplo, se você tiver 100 pares de chave/valor e traduzi-los para 9 idiomas, o tamanho estimado do armazenamento será 0.0005 100 (9+1) = 0.5 MB. O tamanho real poderá ser diferente dependendo do tamanho real da chave/valor e dos metadados armazenados com a tradução.

Use a {{site.data.keyword.Bluemix_notm}}[calculadora de precificação](https://console.ng.bluemix.net/?direct=classic/#/pricing/cloudOEPaneId=pricing&paneId=pricingSheet&orgGuid=127a45f4-4461-4d5b-a26b-6dc2fdd1a3a2&spaceGuid=208fb1ff-413b-4fd9-9615-e8226062d0f3) para determinar seus custos de serviço mensais.

**Nota**: a utilização do recurso de revisão do plano Professional aumentará o uso de dados além do que é indicado anteriormente.
