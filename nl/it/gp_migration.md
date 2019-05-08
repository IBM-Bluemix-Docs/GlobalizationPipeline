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


# Migrazione delle istanze del servizio {{site.data.keyword.GlobalizationPipeline_short}} a un gruppo di risorse
{: #rg-migration}

Gli utenti delle istanze {{site.data.keyword.GlobalizationPipeline_short}} CF esistenti hanno 3 mesi (dalla data in cui la versione di RC/IAM è disponibile in produzione) per migrare alla versione del servizio compatibile con RC/IAM.


## Prima di cominciare
{: #prereqs}

Prima di iniziare a migrare le tue istanze del servizio {{site.data.keyword.GlobalizationPipeline_short}}, devi sapere che tutti i dati relativi all'istanza del servizio vengono conservati e non perderai nulla. Dopo la migrazione, puoi vedere le tue istanze del servizio nello stesso stato in cui erano prima della migrazione.   

Per una panoramica del processo di migrazione, vedi [Migrazione delle istanze del servizio Cloud Foundry a un gruppo di risorse](/docs/resources/instance_migration.html). 

## Passi per la migrazione
{: #gp_steps_migration}

1. Apri il menu **Ulteriori azioni**.
2. Per iniziare, seleziona **Migra** a un gruppo di risorse.
3. Seleziona un gruppo di risorse.
4. Fai clic su **Migra**; l'istanza viene migrata per tuo conto.

**Nota:** puoi migrare solo un'istanza alla volta, quindi puoi continuare la migrazione delle istanze idonee dopo aver migrato correttamente la prima.

## Passi successivi
{: #nextsteps}

Puoi visualizzare le tue istanze del servizio migrate nella sezione **Servizi** del tuo elenco risorse. L'alias rimane nella sezione Cloud Foundry dell'elenco risorse. Questa è una migrazione sul posto, quindi tutti i dati e le credenziali dell'istanza vengono conservati. Puoi continuare a utilizzare le credenziali generate dall'istanza CF originale. 

Per ulteriori informazioni sul funzionamento della migrazione, vedi [Come funziona la migrazione](/docs/resources/instance_migration.html#how).


