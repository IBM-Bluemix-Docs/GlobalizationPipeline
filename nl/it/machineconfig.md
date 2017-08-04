---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# Configurazione della machine translation
{: #machineconfig}

{{site.data.keyword.GlobalizationPipeline_full}} supporta la capacità di integrare servizi machine translation alternativi per eseguire la machine translation dei tuoi bundle. L'aggiunta di un servizio alternativo può essere utile se il motore predefinito utilizzato dalla {{site.data.keyword.GlobalizationPipeline_short}} non offre una lingua specifica di cui hai bisogno o se preferisci le machine translation generate da un motore differente. L'utilizzo e gli addebiti dei servizi alternativi sono inclusi nei termini di tali servizi.

Per aggiungere e configurare un servizio machine translation alternativo per {{site.data.keyword.GlobalizationPipeline_short}}, seleziona la scheda **Machine Translation Configuration** dal dashboard {{site.data.keyword.GlobalizationPipeline_short}}.

* Per aggiungere un servizio machine translation nel catalogo {{site.data.keyword.Bluemix_notm}}, (**Watson Language Translator**), il servizio deve prima essere aggiunto nello spazio {{site.data.keyword.Bluemix_notm}}.

* Per aggiungere un servizio di terze parti, seleziona il pulsante per tale servizio nella scheda **Machine Translation Configuration** e fornisci le credenziali utente necessarie per accedere al servizio.

Dopo aver aggiunto un servizio machine translation a {{site.data.keyword.GlobalizationPipeline_short}}, segui i rimanenti passi per completare l'integrazione di tale servizio.

1. Fai clic su **Enable** per abilitare l'integrazione con tale servizio.

2. Fai clic su **Update Languages** per visualizzare un elenco aggiornato di lingue di destinazione supportate.

3. Dall'elenco delle lingue di destinazione, seleziona il motore della machine translation per la quale eseguire la traduzione.

4. Fai clic su **Save** per ritornare alla scheda **Machine Translation Configuration**.

Dopo aver configurato un servizio alternativo con {{site.data.keyword.GlobalizationPipeline_short}}, tutte le lingue che sono state assegnate a tale motore inizieranno ad essere generate utilizzando quel motore. 

Per arrestare l'utilizzo di un motore della machine translation alternativo:

1. Dalla scheda **Machine Translation Configuration**, fai clic sul pulsante **Disable** per il servizio per cui vuoi arrestare l'utilizzo.

Quando un servizio machine translation alternativo è disabilitato, tutte le traduzioni generate dal servizio rimarranno nel tuo bundle. Tuttavia, la traduzione in una lingua di destinazione particolare, può non essere disponibile per gli aggiornamenti futuri se la lingua di destinazione non è più supportata dal motore della machine translation che è al momento abilitato.

<!-- Review comment: When you disable an engine, do you need to go back and reconfigure the languages?? Does it go back to the default engine? What happens? -->
