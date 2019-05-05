---

copyright:
  years: 2015, 2018
lastupdated: "2017-06-16"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}


# Trabalhando com pacotes configuráveis
{: #globalizationpipeline_workingwithbundles}

Cada pacote configurável que você cria contém os pares de valores de chave de seu arquivo de recursos e o conjunto completo de traduções que foram geradas.
{:shortdesc}

Os arquivos de recursos que você faz upload podem ser de qualquer um dos formatos a seguir e devem ter conteúdo na forma de pares de chave/valor que representem as sequências da IU do seu app.


* Tipo de arquivo: *Arquivos de propriedade Java™ (.properties)*<br>
Exemplo:
```js
logout=Logout
back=Voltar
examples=Menu
home=Página inicial
web=Web
enterprise=Empresa
extra=Recursos
about=Sobre
settings=Configurações
help=Ajuda
support=Suporte
topics=Tópicos
appExitMsg=Tem certeza de que deseja encerrar o aplicativo?
```
* Tipo de arquivo: *AMD I18N (.js)*<br>
Exemplo:
```js
define({
    "root": {
       logout: "Efetuar logout",
       back: "Voltar",
       examples: "Menu",
       home: "Início",
       web: "Web",
       enterprise: "Corporativo",
       extra: "Recursos",
       about: "Sobre",
       settings: "Configurações",
       help: "Ajuda",
       support: "Suporte",
       topics: "Tópicos",
       appExitMsg: "Tem certeza de que deseja sair do aplicativo?"
    }
});
```
* Tipo de arquivo: *JSON (.json)*<br>
Exemplo:
```js
{
  "logout": "Efetuar logout",
  "back": "Voltar",
  "examples": "Menu",
  "home": "Início",
  "web": "Web",
  "enterprise": "Corporativo",
  "extra": "Recursos",
  "about": "Sobre",
  "settings": "Configurações",
  "help": "Ajuda",
  "support": "Suporte",
  "topics": "Tópicos",
  "appExitMsg": "Tem certeza de que deseja sair do aplicativo?"
}
```

Além disso, um arquivo de recursos também deve seguir estas diretrizes:
* Cada chave pode ter no máximo 1023 caracteres.
* Cada valor pode ter no máximo 8191 caracteres.
* Cada pacote configurável pode conter no máximo 1000 pares de chave/valor.

À medida que você cria pacotes configuráveis, eles são incluídos na guia **Pacotes configuráveis** na qual é possível executar tarefas adicionais, como incluir ou excluir idiomas, visualizar o conteúdo traduzido e fazer edições secundárias no conteúdo traduzido. 

O {{site.data.keyword.GlobalizationPipeline_short}} traduz os conteúdos do pacote configurável para os idiomas usando o mecanismo de tradução de máquina padrão. Como
opção, é possível escolher um mecanismo de tradução de máquina alternativo, conforme
descrito na seção
[Configuração
de tradução de máquina](/docs/services/GlobalizationPipeline/managetranslations.html#machineconfig). O mecanismo padrão suporta os idiomas de destino a seguir:

<table>
<thead>
<tr>
<th>Idiomas de destino</th>
</tr>
</thead>
<tbody>
<tr>
<td>Chinês (Simplificado)</td>
</tr>
<tr>
<td>Chinês (Tradicional)</td>
</tr>
<tr>
<td>French</td>
</tr>
<tr>
<td>Alemanha</td>
</tr>
<tr>
<td>Italiano</td>
</tr>
<tr>
<td>japonês</td>
</tr>
<tr>
<td>Korean</td>
</tr>
<tr>
<td>Português do Brasil</td>
</tr>
<tr>
<td>Espanhol</td>
</tr>
</tbody>
</table>

**Nota:** o mecanismo de tradução de máquina padrão do {{site.data.keyword.GlobalizationPipeline_short}} só fornece suporte para inglês como um idioma de origem. Entretanto,
mecanismos de tradução de máquina alternativos disponíveis para configuração no {{site.data.keyword.GlobalizationPipeline_short}} suportam a tradução de outros idiomas de origem/pares de
idiomas não inglês.

Uma vez que você tenha traduzido os conteúdos do pacote configurável usando a tradução de máquina, é possível fazer edições menores no {{site.data.keyword.GlobalizationPipeline_short}} ou enviar pacotes configuráveis para revisão e edição humana por tradutores profissionais. Para obter detalhes sobre como enviar uma solicitação para revisão e edição humana, veja [Criando solicitação de tradução humana debitável](/docs/services/GlobalizationPipeline/managetranslations.html#humantranslation).




## Selecionando um pacote configurável com o qual trabalhar
{: #globalizationpipeline_selectingabundle}

1. Clique na guia **Pacotes configuráveis** para visualizar todos os pacotes configuráveis que você criou.
2. Clique em um **ID de pacote configurável** na lista para ver mais detalhes sobre esse pacote configurável ou clique no ícone **Visualizar os detalhes dos pacotes configuráveis** ![Selecione o ícone Visualizar os detalhes dos pacotes configuráveis para abrir um pacote configurável e trabalhar com suas traduções](images/viewProjectDetailIcon.png) na coluna Ações.

![Visualize todos os pacotes configuráveis disponíveis na guia Pacotes configuráveis.](images/translationBundles.png)

Depois de selecionar um pacote configurável com o qual trabalhar, será possível visualizar o status de suas traduções, incluir ou remover idiomas, editar as traduções ou fornecer atualizações para o arquivo de recursos.

Se você não precisar mais de um pacote configurável, será possível excluí-lo na
guia **Pacotes configuráveis**. Todas as traduções associadas ao
pacote configurável também são excluídas.
