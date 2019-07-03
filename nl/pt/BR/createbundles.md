---

copyright:
  years: 2015, 2017
lastupdated: "2017-05-26"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# Criando um pacote configurável
{: #createbundles}

Para iniciar a tradução, você cria pacotes configuráveis e faz upload de arquivos de recursos de seu app que precisam ser traduzidos pelo {{site.data.keyword.GlobalizationPipeline_short}}. Os arquivos de recursos podem ser de propriedades Java, AMD I18N ou JSON e
devem ter conteúdo na forma de pares de chave/valor que representem as sequências da IU
do seu app.  Para obter mais detalhes e exemplos de tipos de arquivos suportados, consulte
[Trabalhando com pacotes configuráveis](/docs/services/GlobalizationPipeline/bundles.html){: new_window}.

Para criar um pacote configurável, conclua as etapas a seguir:

<ol>
<li>Na guia <strong>Visão geral</strong>, clique em <strong>Novo pacote configurável</strong>.</li>

<li>Forneça as informações sobre o pacote configurável:
<table>
<thead>
<tr>
<th>Campo</th>
<th>Obrigatória</th>
<th>Descrição</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>ID do pacote
</strong></td>
<td>Sim</td>
<td>Um nome exclusivo para identificar o pacote configurável.</td>
</tr>
<tr>
<td><strong>Idioma de origem
</strong></td>
<td>Sim</td>
<td>O idioma nativo do arquivo de origem.</td>
</tr>
<tr>
<td><strong>Arquivo de Recursos</strong></td>
<td>Não</td>
<td>Um <a href=https://new-console.stage1.ng.bluemix.net/docs/services/GlobalizationPipeline/bundles.html>arquivo de recursos</a> a ser traduzido. O tamanho máximo do arquivo é limitado a 2MB. Os arquivos de recursos especificados serão transferidos por upload.</td>
</tr>
<tr>
<td><strong>Formato de arquivo </strong></td>
<td>Não</td>
<td>O tipo de arquivo que está sendo transferido por upload.</td>
</tr>
<tr>
<td><strong>Idioma de destino</strong></td>
<td>Não</td>
<td>Os idiomas para os quais você deseja traduções.</td>
</tr>
</tbody>
</table>

<p><strong>Nota:</strong> para mudar o serviço de idioma que fornece tradução de máquina para seus pacotes configuráveis, clique na guia <strong>Configuração de tradução de máquina</strong> para visualizar outros mecanismos de tradução de máquina suportados.</p></li>

<li>Clique em <strong>salvar</strong></li></ol>


Após o pacote configurável ser criado, o arquivo de recursos transferido por
upload é traduzido em todos os idiomas de destino especificados. O novo pacote
configurável é incluído na guia Pacotes configuráveis, na qual é possível:

* Incluir ou remover idiomas
* Editar as traduções geradas
* Atualizar o arquivo de origem usado no pacote configurável e gerar novamente as traduções
