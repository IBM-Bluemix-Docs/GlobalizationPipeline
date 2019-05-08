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


# {{site.data.keyword.GlobalizationPipeline_short}}-Serviceinstanzen in eine Ressourcengruppe migrieren
{: #rg-migration}

Vorhandene Benutzer von {{site.data.keyword.GlobalizationPipeline_short}}-CF-Instanzen können innerhalb von 3 Monaten (von dem Datum an gerechnet, zu dem die RC/IAM-Version in der Produktion verfügbar ist) auf die mit RC/IAM kompatible Version des Service migrieren. 


## Vorbereitungen
{: #prereqs}

Beachten Sie vor der Migration der {{site.data.keyword.GlobalizationPipeline_short}}-Serviceinstanzen, dass alle Daten für die Serviceinstanz beibehalten werden. Es gehen keine Daten verloren. Nach der Migration befinden sich Ihre Serviceinstanzen im selben Status wie vor der Migration.    

Eine Übersicht zum Migrationsprozess finden Sie in [Cloud Foundry-Serviceinstanzen in eine Ressourcengruppe migrieren](/docs/resources/instance_migration.html).  

## Migrationsschritte
{: #gp_steps_migration}

1. Öffnen Sie das Menü **Weitere Aktionen**. 
2. Wählen Sie **Migrieren** für die Migration in eine Ressourcengruppe aus, um den Prozess zu starten. 
3. Wählen Sie eine Ressourcengruppe aus. 
4. Klicken auf **Migrieren**. Die Instanz wird migriert. 

**Hinweis:** Sie können nur jeweils eine Instanz migrieren, d. h., Sie können die Migration infrage kommender Instanzen fortsetzen, nachdem die erste Instanz erfolgreich migriert wurde. 

## Weitere Schritte
{: #nextsteps}

Migrierte Serviceinstanzen werden im Abschnitt **Services** der Ressourcenliste angezeigt. Der Aliasname bleibt im Cloud Foundry-Abschnitt der Ressourcenliste erhalten. Hierbei handelt es sich um eine Inplace-Migration, d. h., alle Instanzdaten und Berechtigungsnachweise bleiben erhalten. Sie können die Berechtigungsnachweise, die von der ursprünglichen CF-Instanz generiert wurden, weiterverwenden.  

Weitere Informationen zur Migration finden Sie in [Vorgehensweise bei der Migration](/docs/resources/instance_migration.html#how). 


