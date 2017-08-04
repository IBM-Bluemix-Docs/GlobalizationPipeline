---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# Creazione di un bundle
{: #createbundles}

Per iniziare a tradurre, devi creare i bundle e caricare i file di risorsa della tua applicazione che devono essere tradotti da {{site.data.keyword.GlobalizationPipeline_short}}. I file di risorsa possono essere file Java Properties, AMD I18N o JSON e devono avere il contenuto nel formato di coppie chiave/valore che rappresentano le stringhe IU dalla tua applicazione.  Per ulteriori dettagli e esempi di tipi di file supportati, consulta [Gestione dei bundle](./bundles.html){: new_window}.

Per creare un bundle, completa la seguente procedura:

<ol>
<li>Dalla scheda <strong>Overview</strong>, fai clic su <strong>New Bundle</strong>.</li>

<li>Fornisci informazioni sul tuo bundle:
<table>
<thead>
<tr>
<th>Campo</th>
<th>Obbligatorio</th>
<th>Descrizione</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>ID Bundle</strong></td>
<td>Sì</td>
<td>Un nome univoco per identificare il bundle.</td>
</tr>
<tr>
<td><strong>Lingua di origine</strong></td>
<td>Sì</td>
<td>La lingua nativa del file di origine.</td>
</tr>
<tr>
<td><strong>File di risorsa</strong></td>
<td>No</td>
<td>Un <a href=https://new-console.stage1.ng.bluemix.net/docs/services/GlobalizationPipeline/bundles.html>file di risorsa</a> da tradurre. La dimensione massima del file è limitata a 2MB. I file di risorsa specificati saranno caricati.</td>
</tr>
<tr>
<td><strong>Formato file</strong></td>
<td>No</td>
<td>Il tipo di file che sta venendo caricato.</td>
</tr>
<tr>
<td><strong>Lingua di destinazione</strong></td>
<td>No</td>
<td>Le lingue di cui si desidera la traduzione.</td>
</tr>
</tbody>
</table>

<p><strong>Nota:</strong> per modificare il servizio della lingua che fornisce la machine translation per i tuoi bundle, fai clic sulla scheda <a href=https://new-console.stage1.ng.bluemix.net/docs/services/GlobalizationPipeline/managing_translations.html#globalizationpipeline_service_to_service>MT Configuration</a> per visualizzare gli altri motori machine translation supportati.</p></li>

<li>Fai clic su <strong>salva</strong></li></ol>


Dopo che è stato creato il bundle, il file di risorsa caricato viene tradotto nelle lingue di destinazione che hai specificato. Il nuovo bundle viene aggiunto alla scheda Bundles dove puoi:

* Aggiungere o rimuovere le lingue
* Modificare le traduzioni generate
* Aggiornare il file di origine utilizzato nel bundle e rigenerare le traduzioni.
