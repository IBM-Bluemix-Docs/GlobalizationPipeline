---

copyright:
  years: 2015, 2018
lastupdated: "2017-05-26"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# Modificando detalhes do pacote configurável
{: #modifybundles}

Ao abrir um pacote configurável, é possível visualizar todos os detalhes sobre ele. Todos os idiomas de destino que estiverem no pacote configurável serão listados, com o status de tradução atual de cada um.

![A página de detalhes do pacote configurável mostra informações sobre um pacote configurável e suas traduções.](images/bundleDetails.png)

O status de cada idioma no pacote configurável pode ser Em andamento, Com falha ou Traduzido:

| Barra de Status | Descri‡Æo |
|--------|-------------|
| Em Progresso | A tradução de máquina ainda está em andamento. |
| Reprovado | Ocorreu um erro enquanto o arquivo de recursos estava sendo traduzido para o idioma de destino. |
| Translated | A tradução para o idioma de destino está concluída. |

É possível atualizar o arquivo de recursos que o pacote configurável usa, incluir
um idioma de destino em um pacote configurável, excluir um idioma de destino de um pacote
configurável e fazer download das traduções geradas para um idioma de destino.

## Atualizando o arquivo de recursos usado pelo pacote configurável

1. Ao lado do idioma de origem, clique no ícone **Fazer upload de recursos** ![Selecione este ícone para fazer upload de um novo arquivo de recursos](images/uploadIcon.png) na coluna Ações.
2. Clique em **Procurar** e selecione o novo arquivo de recursos a ser transferido por upload.
3. Selecione o tipo de arquivo de recursos que você está fazendo upload
 * Arquivo de propriedades Java
 * AMD I18N
 * JSON
4. Clique em **Atualizar** para fazer upload do novo arquivo de recursos.

Os pares de chave/valor que estão no arquivo de recursos novo ou atualizado são
sincronizados com os valores que já foram transferidos por upload. Somente o conteúdo
novo ou mudado será traduzido.

## Incluindo um idioma de destino em um pacote configurável

1. Clique no botão **Incluir idioma**.
2. Todos os idiomas de destino disponíveis são mostrados. Selecione os idiomas a serem incluídos no pacote configurável.

A tradução para os idiomas selecionados será iniciada imediatamente.

## Excluindo um idioma de destino de um pacote configurável

Ao excluir um idioma de destino de um pacote configurável, você remove o idioma de
destino e todas as traduções associadas do projeto. Na coluna Ações do idioma de destino a ser removido, clique no ícone **Remover este idioma de destino** ![Selecione o ícone de lixeira Remover este idioma de destino](images/trashIcon.png).

## Fazendo download das traduções geradas para um idioma de destino

O {{site.data.keyword.GlobalizationPipeline_short}} fornece diversas
maneiras de incorporar a tradução para um idioma de destino em seu aplicativo. É possível
fazer download da tradução como arquivo de recursos e incluí-la na construção do seu
aplicativo. É possível também referenciar a tradução dinamicamente a partir do
{{site.data.keyword.GlobalizationPipeline_short}} usando um dos
[SDKs](https://github.com/IBM-Bluemix/gp-common) de software livre. 

<!-- For information on {{site.data.keyword.GlobalizationPipeline_full}} SDKs, see <link>. -->

Para fazer download da tradução como arquivo de recursos: 

1. Na coluna **Ações** do idioma de destino ou de origem a ser transferido por download, clique no ícone **Fazer download das traduções** ![Selecione o ícone de download para fazer download das chaves ou traduções de origem para um idioma de destino](images/downloadIcon.png).
2. Selecione um formato de arquivo.
3. Clique em **Fazer o Download**.
