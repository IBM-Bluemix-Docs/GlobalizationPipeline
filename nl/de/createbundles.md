---

copyright:
  years: 2015, 2017
lastupdated: "2017-05-26"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# Bundle erstellen
{: #createbundles}

Beginnen Sie mit der Übersetzung, indem Sie Bundles und Uploadressourcendateien Ihrer App erstellen, die von {{site.data.keyword.GlobalizationPipeline_short}} übersetzt werden sollen. Die Ressourcendateien können entweder Java-Eigenschaften, AMD I18N oder JSON-Dateien sein und müssen den Inhalt in Form von Schlüssel/Wertpaaren enthalten, die die Zeichenfolgen der Benutzerschnittstelle Ihrer App darstellen.  Weitere Details und Beispiele unterstützter Dateitypen finden Sie unter [Mit Bundles arbeiten](/docs/services/GlobalizationPipeline/bundles.html){: new_window}.

Führen Sie die folgenden Schritte aus, um ein Bundle zu erstellen:

<ol>
<li>Klicken Sie auf der Registerkarte <strong>Übersicht</strong> auf <strong>Neues Bundle</strong>.</li>

<li>Geben Sie Informationen zu Ihrem Bundle an:
<table>
<thead>
<tr>
<th>Feld</th>
<th>Erforderlich</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Bundle-ID</strong></td>
<td>Ja</td>
<td>Ein eindeutiger Name, der das Bundle angibt.</td>
</tr>
<tr>
<td><strong>Quellensprache</strong></td>
<td>Ja</td>
<td>Die Landessprache der Quellendatei.</td>
</tr>
<tr>
<td><strong>Ressourcendatei</strong></td>
<td>Nein</td>
<td>Eine zu übersetzende <a href=https://new-console.stage1.ng.bluemix.net/docs/services/GlobalizationPipeline/bundles.html>Ressourcendatei</a>. Die maximale Dateigröße ist auf 2MB begrenzt. Angegebene Ressourcendateien werden hochgeladen.</td>
</tr>
<tr>
<td><strong>Dateiformat</strong></td>
<td>Nein</td>
<td>Der Dateityp, der hochgeladen wird.</td>
</tr>
<tr>
<td><strong>Zielsprache</strong></td>
<td>Nein</td>
<td>Die Sprachen, für die Sie Übersetzungen wünschen.</td>
</tr>
</tbody>
</table>

<p><strong>Hinweis:</strong> Um den Sprachservice zu ändern, der die automatische Übersetzung für Ihre Bundle anbietet, klicken Sie auf die Registerkarte <strong>Konfiguration der Maschinenübersetzung</strong>, um andere unterstützte Engines für automatische Übersetzungen anzuzeigen.</p></li>

<li>Klicken Sie auf <strong>Speichern</strong>.</li></ol>


Nach der Erstellung des Bundles wird die hochgeladene Ressourcendatei in alle angegebenen Zielsprachen übersetzt. Das neue Bundle wird zur Registerkarte 'Bundles' hinzugefügt. Auf dieser Registerkarte können Sie folgende Aktionen ausführen:

* Sprachen hinzufügen und entfernen
* Generierte Übersetzungen bearbeiten
* Die Quellendatei aktualisieren, die im Bundle verwendet wird, und die Übersetzungen neu erstellen
