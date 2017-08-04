---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# Configuração da tradução de máquina
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
