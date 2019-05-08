---

copyright:
  years: 2015, 2018
lastupdated: "2017-06-16"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}


# Gestione dei bundle
{: #globalizationpipeline_workingwithbundles}

Ogni bundle che hai creato contiene la coppia di valore chiave dal tuo file di risorsa e la serie completa di traduzioni che sono state generate.
{:shortdesc}

I file di risorsa caricati possono essere in uno dei seguenti formati e devono avere il contenuto nel formato di coppie chiave/valore che rappresentano le stringhe IU dalla tua applicazione.


* Tipo di file: *File delle proprietà Java™ (.properties)*<br>
Esempio:
```js
logout=Logout 
back=Back 
examples=Menu 
home=Home 
web=Web 
enterprise=Enterprise 
extra=Resources 
about=About 
settings=Settings 
help=Help 
support=Support 
topics=Topics 
appExitMsg=Are you sure you want to quit the application?
```
* Tipo di file: *AMD I18N (.js)*<br>
Esempio:
```js
define({
    "root": {
       logout: "Logout",
       back: "Back",
       examples: "Menu",
       home: "Home",
       web: "Web",
       enterprise: "Enterprise",
       extra: "Resources",
       about: "About",
       settings: "Settings",
       help: "Help",
       support: "Support",
       topics: "Topics",
       appExitMsg: "Are you sure you want to quit the application?"
    }
});
```
* Tipo di file: *JSON (.json)*<br>
Esempio:
```js
{
  "logout": "Logout",
  "back": "Back",
  "examples": "Menu",
  "home": "Home",
  "web": "Web",
  "enterprise": "Enterprise",
  "extra": "Resources",
  "about": "About",
  "settings": "Settings",
  "help": "Help",
  "support": "Support",
  "topics": "Topics",
  "appExitMsg": "Are you sure you want to quit the application?"
}
```

In aggiunta, un file di risorsa deve anche rispettare queste linee guida:
* Ogni chiave può essere di 1023 caratteri massimo.
* Ogni valore può essere di 8191 caratteri massimo.
* Ogni bundle può contenere al massimo 1000 coppie chiave / valore.

Man mano che crei i bundle, questi vengono aggiunti alla scheda **Bundles** in cui puoi eseguire attività aggiuntive come l'aggiunta o l'eliminazione di lingue, la visualizzazione del contenuto tradotto e l'esecuzione di modifiche minori al contenuto tradotto. 

{{site.data.keyword.GlobalizationPipeline_short}} traduce il tuo contenuto del bundle nelle lingue utilizzando il motore della machine translation predefinito. Facoltativamente puoi scegliere un motore della machine translation alternativo come descritto nella sezione [Configurazione di Machine translation](/docs/services/GlobalizationPipeline/managetranslations.html#machineconfig). Il motore predefinito supporta le seguenti lingue di destinazione:

<table>
<thead>
<tr>
<th>Lingue di destinazione</th>
</tr>
</thead>
<tbody>
<tr>
<td>Cinese (semplificato)</td>
</tr>
<tr>
<td>Cinese (tradizionale)</td>
</tr>
<tr>
<td>Francese</td>
</tr>
<tr>
<td>Tedesco</td>
</tr>
<tr>
<td>Italiano</td>
</tr>
<tr>
<td>Giapponese</td>
</tr>
<tr>
<td>Coreano</td>
</tr>
<tr>
<td>Portoghese (brasiliano)</td>
</tr>
<tr>
<td>Spagnolo</td>
</tr>
</tbody>
</table>

**Nota:** il motore della machine translation predefinito di {{site.data.keyword.GlobalizationPipeline_short}} fornisce supporto solo per l'inglese come lingua di origine. Tuttavia, i motori della machine translation alternativi disponibili per la configurazione in {{site.data.keyword.GlobalizationPipeline_short}} supportano la traduzione di altre coppie di lingue di origine non in inglese/lingua.

Una volta che hai tradotto il contenuto del bundle utilizzando la machine translation, puoi effettuare piccole modifiche in {{site.data.keyword.GlobalizationPipeline_short}} o puoi inviare i bundle per un controllo umano e la modifica da parte di traduttori professionisti. Per i dettagli sull'invio di una richiesta di revisione umana e modifica, consulta [Creazione di una richiesta di traduzione umana a pagamento](/docs/services/GlobalizationPipeline/managetranslations.html#humantranslation).




## Selezionare un bundle da utilizzare
{: #globalizationpipeline_selectingabundle}

1. Fai clic sulla scheda **Bundles** per visualizzare tutti i bundle che hai creato.
2. Fai clic su un **Bundle ID** dall'elenco per visualizzare ulteriori dettagli su tale bundle o fai clic sull'icona **View the bundles detail** ![Seleziona l'icona View the bundles detail per aprire un bundle e lavorare con le sue traduzioni](images/viewProjectDetailIcon.png)	nella colonna delle azioni.

![Visualizza tutti i bundle disponibili nella scheda Bundles.](images/translationBundles.png)

Dopo che hai selezionato un bundle da utilizzare, puoi visualizzare lo stato delle relative traduzioni, aggiungere o rimuovere le lingue, modificare le traduzioni o fornire gli aggiornamenti al file di risorsa.

Se non hai più bisogno di un bundle, puoi eliminarlo dalla scheda **Bundles**. Saranno inoltre eliminate tutte le traduzioni associate con il bundle.
