---

copyright:
  years:  2015, 2019
lastupdated: "2019-07-02"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:codeblock: .codeblock}
{:tip: .tip}
{:download: .download}


# IBM Cloud IAM for {{site.data.keyword.GlobalizationPipeline_short}}
{: #gp_iam}

## Acesso
{: #gp_iam_access}
O acesso às instâncias de serviço ativadas pelo RC do {{site.data.keyword.GlobalizationPipeline_short}} para usuários em sua conta é controlado pela autenticação do {{site.data.keyword.Bluemix_notm}} Identity and Access Management (IAM) e/ou do {{site.data.keyword.GlobalizationPipeline_short}}. Enquanto que para instâncias do CF, somente a autenticação do {{site.data.keyword.GlobalizationPipeline_short}} pode ser usada.

## Autenticação do {{site.data.keyword.GlobalizationPipeline_short}}
{: #gp_iam_ca}
Para usar o mecanismo de autenticação, consulte [Incluir usuários da API](/docs/services/GlobalizationPipeline/managetranslations.html#adduser).


## Identity Access Management (IAM)
{: #gp_iam_ovw}
A todo usuário que acessa o serviço {{site.data.keyword.GlobalizationPipeline_short}} em sua conta deve ser designada uma política de acesso com uma função de usuário do IAM definida. Essa política determina quais ações o usuário pode executar dentro do contexto do serviço ou instância que você seleciona. As ações permitidas são customizadas e definidas pelo serviço {{site.data.keyword.Bluemix_notm}} como operações que têm permissão para serem executadas no serviço. As ações são, então, mapeadas para funções de usuário do IAM.

As políticas permitem que o acesso seja concedido em diferentes níveis. Algumas das opções incluem o seguinte:

* Acesso em todas as instâncias do serviço em sua conta
* Acesso a uma instância de serviço individual em sua conta
* Acesso a um recurso específico dentro de uma instância
* Acesso a todos os serviços ativados para o IAM em sua conta

Depois de definir o escopo da política de acesso, você designa uma função. A tabela a seguir detalha as ações que são mapeadas para as funções de acesso de serviço. As funções de acesso ao serviço permitem que os usuários acessem o {{site.data.keyword.GlobalizationPipeline_short}}, bem como a capacidade de chamar a API do {{site.data.keyword.GlobalizationPipeline_short}}.

| **Tipo de função** | **Visualizar traduções** | **Editar traduções** | **Modificar informações do pacote configurável** | **Criar solicitações de tradução profissional** | **Visualizar solicitações de tradução profissional** |
|---------------|-----------------------|-----------------------|-------------------------------|----------------------------------------------|--------------------------------------------|
| Leitor        | Sim | Não | Não | Não | Não |
| Gravador        | Sim | Sim | Não | Não | Sim |
| Gerente       | Sim | Sim | Sim | Sim | Sim |
{: caption="Tabela 1. Funções e ações do usuário do IAM" caption-side="top"}

Atualmente, os usuários do IAM recebem acesso no nível da instância de serviço, e os usuários do IAM não podem ter acesso permitido ou negado no nível do pacote configurável. Para controle de baixa granularidade, use a autenticação do {{site.data.keyword.GlobalizationPipeline_short}}.

Para obter informações sobre como designar funções de usuário na IU, consulte [Gerenciando o acesso ao IAM](/docs/iam?topic=iam-iammanidaccser).

### Gerando chamadas API
{: #gp_iam_apicalls}

Para gerar ou obter as credenciais de serviço, siga as etapas a seguir.
1. Efetue logon em sua conta do {{site.data.keyword.Bluemix}} no [ painel do {{site.data.keyword.Bluemix}}](https://cloud.ibm.com/).
2. Clique na instância de serviço no [ painel do {{site.data.keyword.Bluemix}}](https://cloud.ibm.com/).
3. Clique em **Credenciais de serviço** para abrir sua instância de serviço.
4. Clique em **Nova credencial** para seguir o prompt para criar novas credenciais.
5. Clique em **Visualizar credenciais** depois de criar a credencial.
![A captura de tela mostra informações sobre uma chave de API de amostra](images/gp_iam_apicalls.gif)

A seguir estão exemplos de como chamar a API do {{site.data.keyword.GlobalizationPipeline_short}} usando a autenticação do IAM.

* Usando o token de acesso do IAM
```
curl -X GET \
  https://gp-rest.us-south.g11n-pipeline.test.cloud.ibm.com/translate/rest/50341556337c581c208188ff8908ebc7/v2/bundles \
  -H 'Authorization: Bearer eyJjsksd…w'
```

* Usando a chave de API
```
curl -X GET \
  https://gp-rest.us-south.g11n-pipeline.test.cloud.ibm.com/translate/rest/50341556337c581c208188ff8908ebc7/v2/bundles \
  -H 'Authorization: API-KEY MklfrP…ACem'
```
No exemplo anterior, é possível obter as informações a seguir:
* “50341556337c581c208188ff8908ebc7” é o instanceId (da seção de credenciais)
* “https://gp-rest.us-south.g11n-pipeline.test.cloud.ibm.com/translate/rest” é a URL (da seção de credenciais)
* “MklfrP…ACem” é a apikey (da seção de credenciais)
* “eyJjsksd…w” é o token de acesso do IAM

Para obter instruções para obter o token de acesso do IAM por meio da apikey, consulte [Obtendo um token do IAM do {{site.data.keyword.Bluemix_notm}} usando uma chave de API](/docs/iam?topic=iam-iamtoken_from_apikey#iamtoken_from_apikey).
