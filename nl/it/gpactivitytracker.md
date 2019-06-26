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


# Eventi {{site.data.keyword.cloudaccesstrailshort}} {{site.data.keyword.GlobalizationPipeline_short}}
{: #gpat_events}

Utilizza il servizio {{site.data.keyword.cloudaccesstrailfull}} per tracciare il modo in cui gli utenti e le applicazioni interagiscono con IBM {{site.data.keyword.GlobalizationPipeline_short}} in {{site.data.keyword.Bluemix}}.
{:shortdesc}

Il servizio {{site.data.keyword.cloudaccesstrailfull_notm}} registra le attività avviate dall'utente che modificano lo stato di un servizio in {{site.data.keyword.Bluemix_notm}}. Per ulteriori informazioni, vedi [{{site.data.keyword.cloudaccesstrailfull_notm}}](/docs/services/Activity-Tracker-with-LogDNA?topic=logdnaat-getting-started).




## Elenco di eventi: eventi di bundle
{: #gpevents_bundle}

La seguente tabella elenca le azioni correlate ai bundle e che generano un evento:

|Azione|Descrizione|
|---|---|  
|g11n-pipeline.bundles.read|Ottiene un elenco di ID bundle|
|g11n-pipeline.bundle.create|Crea un nuovo bundle.|
|g11n-pipeline.bundle.read|Ottiene le informazioni sul bundle.|
|g11n-pipeline.bundle.update|Aggiorna la configurazione del bundle.|
|g11n-pipeline.bundle.delete|Elimina il bundle specificato.|
|g11n-pipeline.bundle-language.create|Carica le voci di risorsa.|
|g11n-pipeline.bundle-language.read|Ottiene le stringhe di risorsa (coppie chiave/valore) per la lingua.|
|g11n-pipeline.bundle-language.update|Aggiorna le voci di risorsa.|
|g11n-pipeline.bundle-language.read|Ottiene le informazioni sulla voce di risorsa.|
|g11n-pipeline.bundle-language.update|Aggiorna la voce di risorsa.|

## Elenco di eventi: eventi di richiesta di traduzione del bundle
{: #gpevents_bundle_tr_req}

La seguente tabella elenca le azioni correlate alle richieste di traduzione del bundle e che generano un evento:

|Azione|Descrizione|
|---|---|  
|g11n-pipeline.trs.read|Ottiene un elenco di richieste di traduzione.|
|g11n-pipeline.tr.read|Ottiene le informazioni sulla richiesta di traduzione specificata.|
|g11n-pipeline.tr.update|Aggiorna le informazioni sulla richiesta di traduzione specificata.|
|g11n-pipeline.tr.delete|Elimina la richiesta di traduzione specificata.|
|g11n-pipeline.tr-bundle.read|Ottiene le informazioni sul bundle.|
|g11n-pipeline.tr-bundle-language.read|Richiede le voci di risorsa per il bundle e la lingua specificati.|
|g11n-pipeline.tr-bundle-language.read|Ottiene le informazioni sulla voce di risorsa.|
|g11n-pipeline.trs.create|Crea una nuova richiesta di traduzione.|


## Elenco di eventi: eventi di xliff del bundle
{: #gpevents_bundle_xliff}

La seguente tabella elenca le azioni correlate allo xliff del bundle e che generano un evento:

|Azione|Descrizione|
|---|---|  
|g11n-pipeline.xliff-bundles.read|Ottiene i dati di risorsa nella lingua specificata dai bundle in formato XLIFF 2.0.|
|g11n-pipeline.xliff-bundles.update|Aggiorna i bundle nell'istanza del servizio con i dati XLIFF.|
|g11n-pipeline.xliff-tr-bundles.read|Ottiene i dati di risorsa nella lingua specificata nella richiesta di traduzione in formato XLIFF 2.0.|


## Elenco di eventi: eventi di partner
{: #gpevents_partner}

La seguente tabella elenca le azioni correlate ai partner e che generano un evento:

|Azione|Descrizione|
|---|---|  
|g11n-pipeline.partner.read|Ottiene le informazioni sul partner.|
|g11n-pipeline.partner.update|Aggiorna le informazioni sul partner.|
|g11n-pipeline.partner-trs.read|Ottiene un elenco di richieste di traduzione assegnate al partner.|
|g11n-pipeline.partner-tr.read|Ottiene le informazioni sulla richiesta di traduzione specificata.|
|g11n-pipeline.partner-tr.update|Aggiorna le informazioni sulla richiesta di traduzione specificata.|
|g11n-pipeline.partner-tr.delete|Elimina la richiesta di traduzione specificata.|
|g11n-pipeline.partner-tr-bundle.read|Ottiene le informazioni sul bundle.|
|g11n-pipeline.partner-tr-bundle-language.read|Richiede le voci di risorsa per il bundle e la lingua specificati.|
|g11n-pipeline.partner-tr-bundle-language.update|Aggiorna le voci di risorsa per il bundle e la lingua specificati.|
|g11n-pipeline.partner-tr-bundle-language.read|Ottiene le informazioni sulla voce di risorsa.|
|g11n-pipeline.partner-tr-bundle-language.update|Aggiorna la voce di risorsa.|
|g11n-pipeline.partner-users.read|Ottiene gli utenti disponibili per questo partner.|
|g11n-pipeline.partner-user.read|Ottiene le informazioni sull'utente partner specificato.|
|g11n-pipeline.partner-user.update|Aggiorna le informazioni su un utente partner.|
|g11n-pipeline.partner-user.delete|Elimina l'utente partner specificato.|
|g11n-pipeline.partner-user.create|Crea un nuovo utente partner.|
|g11n-pipeline.partner-tr-xliff-bundles.update|Aggiorna i dati di risorsa nella richiesta di traduzione con i dati XLIFF.|
|g11n-pipeline.partner-tr-xliff-bundles-language.read|Ottiene i dati di risorsa nella lingua specificata nella richiesta di traduzione in formato XLIFF 2.0.|



## Elenco di eventi: eventi di amministratore
{: #gpevents_admin}

La seguente tabella elenca le azioni correlate all'amministratore e che generano un evento:

|Azione|Descrizione|
|---|---|  
|g11n-pipeline.instances.read|Ottiene un elenco di istanze del servizio.|
|g11n-pipeline.instance.read|Ottiene le informazioni sull'istanza del servizio.|
|g11n-pipeline.instance.update|Aggiorna la configurazione dell'istanza del servizio.|
|g11n-pipeline.instance.create|Crea una nuova istanza del servizio.|
|g11n-pipeline.instance.delete|Elimina l'istanza del servizio specificata.|
|g11n-pipeline.instance.create|Crea una nuova istanza del servizio gestita da Cloud Foundry.|
|g11n-pipeline.partners.read|Ottiene un elenco di partner.|
|g11n-pipeline.partner.create|Crea un nuovo partner.|
|g11n-pipeline.partner.delete|Elimina il partner specificato.|



## Elenco di eventi: eventi di utente
{: #gpevents_user}

La seguente tabella elenca le azioni correlate agli utenti e che generano un evento:

|Azione|Descrizione|
|---|---|  
|g11n-pipeline.instance-users.read|Ottiene gli utenti in questa istanza del servizio.|
|g11n-pipeline.instance-user.read|Ottiene le informazioni sull'utente specificato.|
|g11n-pipeline.instance-user.update|Aggiorna le informazioni su un utente.|
|g11n-pipeline.instance-user.delete|Elimina l'utente specificato.|
|g11n-pipeline.instance-users.create|Crea un nuovo utente.|


## Elenco di eventi: eventi di configurazione
{: #gpevents_config}

La seguente tabella elenca le azioni correlate alla configurazione di traduzione e che generano un evento:

|Azione|Descrizione|
|---|---|  
|g11n-pipeline.config-mts.read|Ottiene tutti i bind del servizio MT.|
|g11n-pipeline.config-mt.read|Ottiene i dati di bind del servizio MT.|
|g11n-pipeline.config-translations.read|Ottiene tutte le configurazioni di traduzione.|
|g11n-pipeline.config-translation.read|Ottiene la configurazione di traduzione.|
|g11n-pipeline.config-mt.update|Inserisce i dati di bind del servizio MT specificato. Se i dati di bind specificati esistono già, vengono sostituiti dai dati di bind del servizio MT specificato.|
|g11n-pipeline.config-mt.delete|Elimina i dati di bind del servizio MT specificato.|
|g11n-pipeline.config-translation.update|Inserisce la configurazione di traduzione per la coppia di lingue specificata. Se la configurazione per la coppia esiste già, viene sostituita dalla configurazione specificata.|
|g11n-pipeline.config-translation.delete|Elimina la configurazione di traduzione per la coppia di lingue specificata.|


## Elenco di eventi: eventi di istanza
{: #gpevents_instance}

La seguente tabella elenca le azioni correlate alle istanze e che generano un evento:

|Azione|Descrizione|
|---|---|  
|g11n-pipeline.instance.read|Ottiene le informazioni su questa istanza del servizio di traduzione.|


## Dove ricercare gli eventi
{: #gp_at_ui}

Gli eventi di {{site.data.keyword.cloudaccesstrailshort}} sono disponibili nel **dominio dello spazio** di {{site.data.keyword.cloudaccesstrailshort}} che è disponibile nella regione {{site.data.keyword.Bluemix_notm}} in cui viene eseguito il provisioning del servizio {{site.data.keyword.GlobalizationPipeline_short}}. Il provisioning dell'istanza del servizio {{site.data.keyword.cloudaccesstrailshort}} e dell'istanza {{site.data.keyword.GlobalizationPipeline_short}} deve essere eseguito nello stesso spazio CF.

Per le istanze RC di {{site.data.keyword.GlobalizationPipeline_short}}, gli eventi di Activity Tracker sono disponibili nel dominio dell'**account** Activity Tracker in cui vengono generati gli eventi nella regione {{site.data.keyword.Bluemix_notm}}.
