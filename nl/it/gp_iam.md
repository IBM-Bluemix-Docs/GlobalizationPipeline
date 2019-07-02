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


# IBM Cloud IAM per {{site.data.keyword.GlobalizationPipeline_short}}
{: #gp_iam}

## Accesso
{: #gp_iam_access}
L'accesso alle istanze del servizio abilitate per {{site.data.keyword.GlobalizationPipeline_short}} RC per gli utenti nel tuo account è controllato da {{site.data.keyword.Bluemix_notm}} IAM (Identity and Access Management) e/o dall'autenticazione {{site.data.keyword.GlobalizationPipeline_short}}. Mentre per le istanze CF è possibile utilizzare solo l'autenticazione {{site.data.keyword.GlobalizationPipeline_short}}.

## Autenticazione {{site.data.keyword.GlobalizationPipeline_short}}
{: #gp_iam_ca}
Per utilizzare il meccanismo di autenticazione, vedi [Aggiungi utenti API](/docs/services/GlobalizationPipeline/managetranslations.html#adduser).


## IAM (Identity Access Management)
{: #gp_iam_ovw}
A ogni utente che accede al servizio {{site.data.keyword.GlobalizationPipeline_short}} nel tuo account deve essere assegnata una politica di accesso con un ruolo utente IAM definito. Tale politica determina quali azioni possono essere effettuate dall'utente all'interno del contesto del servizio o dell'istanza che selezioni. Le azioni consentite sono personalizzate e definite dal servizio {{site.data.keyword.Bluemix_notm}} come operazioni che è consentito eseguire sul servizio. Le azioni vengono quindi associate ai ruoli utente IAM.

Le politiche consentono di concedere l'accesso a diversi livelli. Alcune delle opzioni includono quanto segue:

* Accesso a tutte le istanze del servizio nel tuo account
* Accesso a una singola istanza del servizio nel tuo account
* Accesso a una specifica risorsa all'interno di un'istanza
* Accesso a tutti i servizi abilitati a IAM nel tuo account

Dopo aver definito l'ambito della politica di accesso, assegna un ruolo. La seguente tabella illustra le azioni associate ai ruoli di accesso al servizio. I ruoli di accesso al servizio consentono agli utenti di accedere a {{site.data.keyword.GlobalizationPipeline_short}} e offrono la possibilità di chiamare l'API di {{site.data.keyword.GlobalizationPipeline_short}}.

| **Tipo di ruolo** | **Visualizza le traduzioni** | **Modifica le traduzioni** | **Modifica le informazioni del bundle** | **Crea richieste di traduzione professionale** | **Visualizza richieste di traduzione professionale** |
|---------------|-----------------------|-----------------------|-------------------------------|----------------------------------------------|--------------------------------------------|
| Lettore        | Sì | No | No | No | No |
| Scrittore        | Sì | Sì | No | No | Sì |
| Gestore       | Sì | Sì | Sì | Sì | Sì |
{: caption="Tabella 1. Ruoli utente IAM e azioni" caption-side="top"}

Attualmente agli utenti IAM viene concesso l'accesso a livello di istanza del servizio e non può essere consentito o negato l'accesso a livello di bundle. Per il controllo dettagliato, utilizza l'autenticazione {{site.data.keyword.GlobalizationPipeline_short}}.

Per informazioni sull'assegnazione dei ruoli utente nell'IU, vedi [Gestione dell'accesso IAM](/docs/iam?topic=iam-iammanidaccser).

### Generazione di chiamate API
{: #gp_iam_apicalls}

Per generare o per ottenere le credenziali del servizio, attieniti alla seguente procedura.
1. Accedi al tuo account {{site.data.keyword.Bluemix}} nel [dashboard {{site.data.keyword.Bluemix}}](https://cloud.ibm.com/).
2. Fai clic sull'istanza del servizio nel [dashboard {{site.data.keyword.Bluemix}}](https://cloud.ibm.com/).
3. Fai clic su **Credenziale del servizio** per aprire la tua istanza del servizio.
4. Fai clic su **Nuova credenziale** per seguire la richiesta per la creazione di nuove credenziali.
5. Fai clic su **Visualizza credenziali** dopo aver creato la credenziale.
![La schermata mostra informazioni su una chiave API di esempio](images/gp_iam_apicalls.gif)

Di seguito sono riportati alcuni esempi di chiamata dell'API di {{site.data.keyword.GlobalizationPipeline_short}} mediante l'autenticazione IAM.

* Utilizzo del token bearer IAM
```
curl -X GET \
  https://gp-rest.us-south.g11n-pipeline.test.cloud.ibm.com/translate/rest/50341556337c581c208188ff8908ebc7/v2/bundles \
  -H 'Authorization: Bearer eyJjsksd…w'
```

* Utilizzo della chiave API
```
curl -X GET \
  https://gp-rest.us-south.g11n-pipeline.test.cloud.ibm.com/translate/rest/50341556337c581c208188ff8908ebc7/v2/bundles \
  -H 'Authorization: API-KEY MklfrP…ACem'
```
Nell'esempio precedente, puoi ottenere le seguenti informazioni:
* “50341556337c581c208188ff8908ebc7” è l'ID istanza (dalla sezione delle credenziali)
* “https://gp-rest.us-south.g11n-pipeline.test.cloud.ibm.com/translate/rest” è l'URL (dalla sezione delle credenziali)
* “MklfrP…ACem” è la chiave API (dalla sezione delle credenziali)
* “eyJjsksd…w” è il token bearer IAM

Per istruzioni su come ottenere il token bearer IAM dalla chiave API, vedi [Ottenimento di un token IAM {{site.data.keyword.Bluemix_notm}} utilizzando una chiave API](/docs/iam?topic=iam-iamtoken_from_apikey#iamtoken_from_apikey).
