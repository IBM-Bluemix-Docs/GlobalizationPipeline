---

copyright:
  years: 2015, 2018
lastupdated: "2017-12-13"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}


# Introduzione alla {{site.data.keyword.GlobalizationPipeline_short}}
{: #globalizationpipeline}

{{site.data.keyword.GlobalizationPipeline_full}} è un servizio {{site.data.keyword.Bluemix}} che consente agli sviluppatori dell'applicazione di distribuire rapidamente le applicazioni tradotte ai clienti globali. {{site.data.keyword.GlobalizationPipeline_short}} funge da repository di traduzioni che fornisce machine translation, revisione e modifica umana e API ed SDK per integrare la traduzione senza interruzioni nella tua infrastruttura DevOps e Continuous Development, eliminando le operazioni manuali e isolate associate al processo di traduzione tradizionale.
{:shortdesc}

Puoi utilizzare il servizio {{site.data.keyword.GlobalizationPipeline_short}} per tradurre qualsiasi applicazione distribuita e ospitata in {{site.data.keyword.Bluemix_notm}} o per annullare l'associazione per tradurre le applicazioni ospitate in altre piattaforme cloud.

{{site.data.keyword.GlobalizationPipeline_short}} offre un'interfaccia dashboard per gestire la tua traduzione dell'applicazione e un'API RESTful che automatizza completamente il processo di traduzione. Per informazioni sull'API {{site.data.keyword.GlobalizationPipeline_short}}, consulta [Guida di riferimento API](https://gp-rest.ng.bluemix.net/translate/swagger/index.html){: new_window}.

## Scegliere un piano di traduzione
{: #globalizationpipeline_chooseplan}

Prima di iniziare ad utilizzare la traduzione in {{site.data.keyword.GlobalizationPipeline_short}}, puoi scegliere un piano di traduzione adatto.

Sono disponibili due piani di traduzione in {{site.data.keyword.GlobalizationPipeline_short}}, il piano Standard e Professional. Entrambi questi piani forniscono machine translation di base illimitata integrata così come la capacità di integrazione con altri motori machine translation a un costo aggiuntivo. Nel piano Professional, {{site.data.keyword.GlobalizationPipeline_short}} viene inoltre offerto un servizio di modifica e revisione della traduzione professionale. Puoi passare tra i piani di {{site.data.keyword.GlobalizationPipeline_short}} all'interno di {{site.data.keyword.Bluemix_notm}} con tutti i dati riservati.


## Stima dell'utilizzo dati della {{site.data.keyword.GlobalizationPipeline_short}}
{: #globalizationpipeline_documentpricing}

{{site.data.keyword.GlobalizationPipeline_short}} memorizza le tue traduzioni in un database di backend. Per stimare la dimensione dei dati attivi, puoi fare riferimento alla seguente formula:

`<expected resource data storage size in MB> ˜= 0,0005 * <number of key/value pairs in the source resource> * <number of languages including the source language>`

In basa alla formula, la dimensione di un bundle tipico è `(length of key + length of value in UTF-8 = ˜40 bytes)`.

Ad esempio, se hai 100 coppie chiave/valore e le hai tradotte in 9 lingue, la dimensione di memorizzazione stimata è 0.0005 100 (9+1) = 0.5 MB. La dimensione attuale può essere differente a seconda della dimensione chiave/valore attuale e ai metadati archiviati con la traduzione.

Utilizza il [calcolatore dei prezzi](https://console.ng.bluemix.net/?direct=classic/#/pricing/cloudOEPaneId=pricing&paneId=pricingSheet&orgGuid=127a45f4-4461-4d5b-a26b-6dc2fdd1a3a2&spaceGuid=208fb1ff-413b-4fd9-9615-e8226062d0f3) {{site.data.keyword.Bluemix_notm}} per determinare i tuoi costi di servizio mensili.

**Nota**: l'utilizzo della funzione di revisione del piano Professional aumenterà l'utilizzo dei dati oltre a quanto precedentemente indicato.
