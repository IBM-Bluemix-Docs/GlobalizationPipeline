---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# Gerenciando traduções
{: #managetranslations}


Uma vez criados os pacotes configuráveis e iniciada a geração de traduções para seu aplicativo, é possível escolher entre tradução de máquina e tradução humana. O conteúdo gerado pela máquina pode ser usado no estado em que se encontra ou modificado posteriormente. Você também tem a opção de usar uma tradução de máquina diferente do padrão. Esta seção abrange as instruções para as tarefas a seguir:
<ul>
<li>Como mudar o mecanismo de tradução de máquina que executa as traduções para seus pacotes configuráveis?</li>
<li>Como executar a edição pós-tradução humana?</li>
<li>Como criar a solicitação de tradução humana?</li>
<li>Como designar funções de usuário e restrições de acesso para as pessoas que precisarão acessar suas traduções?</li>
</ul>

**Nota**: para um usuário do plano Padrão, se você desejar criar solicitação de tradução humana, será possível alternar para o plano Profissional. Ainda assim será possível visualizar seus dados de solicitação de tradução humana em um plano Padrão, mas a solicitação de tradução humana estará disponível somente para usuários do plano Profissional. 

## Configuração da tradução de máquina
{: #machineconfig}

O {{site.data.keyword.GlobalizationPipeline_full}} suporta a capacidade de integrar serviços de tradução de máquina alternativos para executar a tradução de máquina de seus pacotes configuráveis. A inclusão de um serviço alternativo poderá ser benéfica se o mecanismo padrão utilizado pelo {{site.data.keyword.GlobalizationPipeline_short}} não oferecer um idioma específico que você precisa ou se você preferir as traduções de máquina que são geradas por um mecanismo diferente. O uso ou os encargos de serviços alternativos são cobertos sob os termos desses serviços.

Para incluir e configurar um serviço de tradução de máquina alternativo para o {{site.data.keyword.GlobalizationPipeline_short}}, selecione a guia **Configuração de tradução de máquina** no painel do {{site.data.keyword.GlobalizationPipeline_short}}.

* Para incluir um serviço de tradução de máquina que esteja no catálogo do {{site.data.keyword.Bluemix_notm}}, (**Watson Language Translator**), o serviço deve
primeiro ser incluído em seu espaço do {{site.data.keyword.Bluemix_notm}}.

* Para incluir um serviço de terceiros, selecione o botão desse serviço na guia **Configuração de tradução de máquina** e forneça as credenciais de usuário requeridas para acessar o serviço.

Após um serviço de tradução de máquina ter sido incluído no {{site.data.keyword.GlobalizationPipeline_short}}, conclua as etapas restantes para concluir a integração desse serviço.

1. Clique em **Ativar** para ativar a integração com esse serviço.

2. Clique em **Atualizar idiomas** para visualizar uma lista atualizada de idiomas de destino suportados.

3. Na lista de idiomas de destino, selecione o mecanismo de tradução de máquina que deverá executar a tradução.

4. Clique em **Salvar** para retornar à guia **Configuração de tradução de máquina**.

Depois que um serviço alternativo tiver sido configurado com o {{site.data.keyword.GlobalizationPipeline_short}}, todos os idiomas de destino que tiverem sido designados a esse mecanismo começarão a ser gerados usando esse mecanismo. 

Para parar de usar um mecanismo de tradução de máquina alternativo:

1. Na guia **Configuração de tradução de máquina**, clique no
botão **Desativar** para o serviço que você deseja parar de usar.

Depois que um serviço de tradução de máquina alternativo for desativado, todas as traduções que foram geradas pelo serviço permanecerão nos pacotes configuráveis. Entretanto, a tradução em um determinado idioma de destino poderá não estar disponível para atualizações futuras se o idioma de destino não for mais suportado pelo mecanismo de tradução de máquina atualmente ativado.

<!-- Review comment: When you disable an engine, do you need to go back and reconfigure the languages?? Does it go back to the default engine? What happens? -->

## Visualizando e editando traduções
{: #edittranslations}

O serviço {{site.data.keyword.GlobalizationPipeline_short}} fornece recursos
de edição humana pós-tradução. É possível editar
para melhorar a qualidade ou a consistência da tradução ou substituir palavras
preferenciais. Por exemplo, talvez você queira sobrescrever a tradução do nome de um
produto.

Para visualizar e editar as traduções de um idioma de destino:

1. Na página **Detalhes do pacote configurável**, selecione um idioma de destino ou clique no ícone **Visualizar as traduções** ![Selecione o ícone Visualizar traduções para visualizar as traduções de um idioma de destino](images/viewProjectDetailIcon.png) na coluna Ações.
2. As traduções são apresentadas em uma tabela que mostra informações de chave, origem e tradução.
 * **Chave:** representa um atributo no arquivo de recursos que tem um valor associado.
 * **Origem:** representa uma sequência traduzível que foi incluída no arquivo de recursos transferido por upload.
 * **Tradução:** representa a versão traduzida de um valor de origem.
3. Na coluna Ações, clique no ícone **Modificar a tradução** ![Selecione o ícone Modificar a tradução para editar as traduções de um determinado par de chave/valor.](images/editIcon.png) para editar um valor traduzido por máquina.
4. Edite a tradução e clique em **Atualizar** para atualizar o valor traduzido original com sua edição.

![A janela de diálogo Modificar tradução fornece uma maneira simples de editar traduções.](images/editTranslation.png) 

***Dica:*** 
1. Quando você trabalha com pacotes configuráveis grandes que incluem muitas chaves traduzíveis, a descoberta de um valor específico pode ser difícil. Na página de tradução do idioma de destino, é possível procurar rapidamente entre todas as chaves, origens e traduções usando a caixa **Procurar...**.
![Use a caixa de procura fornecida na página de tradução do idioma de destino para procurar as chaves, origens, traduções ou todas as três em um idioma de destino.](images/search.png) 

2. O painel do {{site.data.keyword.GlobalizationPipeline_short}} fornece a função de filtragem de sequência para você selecionar quais tipos de sequência mostrar quando desejar visualizar detalhes do pacote configurável. Clique na guia padrão **Mostrar todas as sequências**, é possível escolher entre mostrar todas as sequências, somente as sequências revisadas ou somente as sequências não revisadas.
![Use a função de filtragem de sequência para escolher entre mostrar todas as sequências, somente as sequências revisadas ou somente as sequências não revisadas.](images/stringfilter.png)

## Criando solicitações de tradução humana debitável
{: #humantranslation}

Onde a qualidade é crucial, você talvez deseje encaixar os tradutores profissionais para revisar sua tradução de máquina. Para um encargo adicional no plano Profissional do {{site.data.keyword.GlobalizationPipeline_short}}, é possível enviar seus pacotes configuráveis traduzidos por máquina para revisão e edição humana. Para fazer isso, alterne do plano Padrão para o plano Profissional, crie uma solicitação de tradução humana e envie seus pacotes configuráveis de destino para os serviços de tradução profissional da IBM. É possível usar esse recurso para refinar melhor a qualidade e consistência de suas traduções. Os idiomas que estão disponíveis para revisão e edição humana são os mesmos que os idiomas suportados pelos mecanismos de tradução de máquina disponíveis por meio do {{site.data.keyword.GlobalizationPipeline_short}}. 


Para criar uma solicitação de tradução, conclua as etapas a seguir: 

1. Alterne para **o plano Profissional do {{site.data.keyword.GlobalizationPipeline_short}}**.

2. Clique na guia **Solicitação de tradução** no painel e clique em **Nova solicitação**.

3. Selecione seu pacote configurável de destino e os idiomas de destino para tradução. 

4. Verifique o ID de pacote configurável, os idiomas de destino e a contagem de palavras de origem para tradução. 

5. Forneça as informações necessárias sobre sua solicitação. Os campos marcados com asteriscos devem ser preenchidos.

6. Confirme e envie sua solicitação.

**Nota**: é altamente recomendado fornecer contexto adicional para seu conteúdo de tradução no campo **Instrução especial** durante a etapa 5. Isso pode ajudar os tradutores humanos a entender seu conteúdo e entregar um resultado de tradução de qualidade.
![É altamente recomendado fornecer contexto adicional suficiente no campo Instrução especial.](images/specialinstruction.png)

É possível visualizar todas as suas solicitações de tradução e rastrear o status no painel.
![Interface com o usuário da solicitação de tradução de amostra para sua referência.](images/translationrequest.png)

**Nota**: há 5 estados para cada solicitação de tradução. É possível se referir à tabela a seguir para ajudar a rastrear o status de sua solicitação de tradução.

| Barra de Status | Notificação por email | Explicação do status |
|--------|--------------------|--------------------|
| Rascunho  | NÃO | A solicitação de tradução foi criada, mas não enviada ainda. Ainda é possível modificar o conteúdo da solicitação de tradução ou excluir a solicitação de tradução. |
| Submetidos | Sim | A solicitação de tradução foi enviada e não é possível modificar o conteúdo da solicitação de tradução. |
| Edição iniciada | Sim | O trabalho de pós-edição humana para a solicitação de tradução foi iniciado. |
| Edição concluída | Sim | O trabalho de pós-edição humana para a solicitação de tradução foi concluído. Ainda é necessário aguardar que as sequências traduzidas sejam mescladas de volta com as sequências de caracteres de recursos principais. |
| Intercalada | Sim | O resultado de pós-edição manual foi mesclado de volta. A solicitação de tradução foi concluída. É possível gerar um relatório neste ponto. É possível manter a solicitação de tradução para referência futura ou excluí-la para economizar armazenamento. A exclusão da solicitação de tradução não afetará o resultado da tradução mesclada. |

Para visualizar o detalhe da solicitação de tradução, clique no ícone **Visualizar o detalhe da solicitação** ![Selecione o ícone Visualizar o detalhe para visualizar as traduções do idioma de destino](images/viewProjectDetailIcon.png) na coluna **Ações**.

![Visualizar detalhes da solicitação de tradução](images/viewtr.png)

Para gerar um relatório *JSON (.json)* ou XLIFF para sua solicitação, clique no botão **Fazer download do relatório** ou **Fazer download do XLIFF**.



## Incluir usuários da API
{: #adduser}

À medida que gerencia suas traduções, você poderá desejar conceder acesso a usuários da API adicionais com base nas tarefas que eles precisam executar. Por exemplo, talvez você queira permitir que um tradutor edite a tradução, mas não possa modificar as informações do pacote configurável.

| Tipo de função | Visualizar traduções? | Editar traduções? | Modificar informações do pacote configurável? |
|-----------|--------------------|--------------------|----------------------------|
| Reader | Sim | NÃO | NÃO |
| Translator | Sim | Sim | NÃO |
| Administrador | Sim | Sim | Sim |

Se você criar mais usuários da API, será possível restringir o acesso deles a um ou mais pacotes configuráveis específicos, ou conceder a eles acesso a todos os pacotes configuráveis disponíveis.

Para conceder a um usuário da API acesso a pacotes configuráveis em uma instância
de serviço do {{site.data.keyword.GlobalizationPipeline_short}}:

1. No painel do {{site.data.keyword.GlobalizationPipeline_short}}, clique na guia **Usuários da API**.
2. Clique em **Novo usuário da API**.
3. Digite um **nome de exibição** e **comentário** para descrever o novo usuário da API.
4. Escolha um **tipo** para o novo usuário da API.
5. Escolha conceder ao usuário da API acesso a todos os pacotes configuráveis ou somente pacotes configuráveis selecionados.
6. Clique em **Salvar**.

![Conclua o fórum para criar um novo usuário da API.](images/newUser.png)

Um ID e uma senha do usuário da API são gerados e exibidos. Copie e salve essas credenciais; depois de fechar a janela, não será possível acessá-las novamente. As credenciais podem ser usadas para serviço RESTful via [SDKs](https://github.com/IBM-Bluemix/gp-common). 

Para reconfigurar a senha de usuário da API:

1. No painel do {{site.data.keyword.GlobalizationPipeline_short}}, clique na guia **Usuários da API**.
2. Clique no ícone **Reconfiguração de senha** ![Selecione este ícone para reconfigurar a senha de usuários da API](images/resetPW.png) para reconfigurar a senha para um ID do usuário específico. 
3. Clique
em **Sim**. 
