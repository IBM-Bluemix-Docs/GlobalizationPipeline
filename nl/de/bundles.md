---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}


# Mit Bundles arbeiten
{: #globalizationpipeline_workingwithbundles}

Jedes von Ihnen erstellte Bundle enthält die Schlüssel/Wert-Paare aus Ihrer Ressourcendatei und die vollständige Gruppe von generierten Übersetzungen.
{:shortdesc}

Die Ressourcendateien, die Sie hochladen, können eines der folgenden Formate aufweisen und müssen Inhalt in Form von Schlüssel/Wert-Paaren enthalten, die die Zeichenfolgen der Benutzerschnittstelle Ihrer App darstellen.


* Dateityp: *Java™ Properties files (.properties)*<br>
Beispiel:
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
* Dateityp: *AMD I18N (.js)*<br>
Beispiel:
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
* Dateityp: *JSON (.json)*<br>
Beispiel:
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

Zusätzlich muss eine Ressourcendatei die folgenden Richtlinien einhalten:
* Jeder Schlüssel kann maximal 1023 Zeichen enthalten.
* Jeder Wert kann maximal 8191 Zeichen enthalten.
* Jedes Bundle kann maximal 1000 Schlüssel/Wert-Paare enthalten.

Wenn Sie Bundles erstellen, werden diese zur Registerkarte **Bundles** hinzugefügt, auf der Sie zusätzliche Tasks, wie z. B. Hinzufügen oder Löschen von Sprachen, Anzeigen des übersetzten Inhalts und kleinere Bearbeitungsaktionen für den übersetzten Inhalt, durchführen können. 

{{site.data.keyword.GlobalizationPipeline_short}} übersetzt den Bundleinhalt in die gewünschten Sprachen, indem die Standardengine für die automatische Übersetzung eingesetzt wird. Optional können Sie eine alternative Engine für automatische Übersetzung verwenden. Dies wird im Abschnitt über die [Konfiguration der automatischen Übersetzung](managetranslations.html#machineconfig) beschrieben. Die Standardengine unterstützt die folgenden Zielsprachen:

<table>
<thead>
<tr>
<th>Zielsprachen</th>
</tr>
</thead>
<tbody>
<tr>
<td>Chinesisch (Simplified)</td>
</tr>
<tr>
<td>Chinesisch (Traditional)</td>
</tr>
<tr>
<td>Französisch</td>
</tr>
<tr>
<td>Deutsch</td>
</tr>
<tr>
<td>Italienisch</td>
</tr>
<tr>
<td>Japanisch</td>
</tr>
<tr>
<td>Koreanisch</td>
</tr>
<tr>
<td>Portugiesisch (Brasilianisch)</td>
</tr>
<tr>
<td>Spanisch</td>
</tr>
</tbody>
</table>

**Anmerkung:** Die Standardengine für die automatische Übersetzung von {{site.data.keyword.GlobalizationPipeline_short}} bietet nur Unterstützung für Englisch als Quellensprache. Allerdings sind alternative Engines für die automatische Übersetzung zur Konfiguration innerhalb der {{site.data.keyword.GlobalizationPipeline_short}} verfügbar und unterstützen die Übersetzung weiterer Sprachenpaare außer Englisch.

Nach dem Übersetzen des Bundleinhalts mithilfe der automatischen Übersetzung können Sie kleinere Bearbeitungsaktionen in {{site.data.keyword.GlobalizationPipeline_short}} vornehmen oder Sie können die Bundles zur Überprüfung und Bearbeitung an Humanübersetzer übergeben. Details zur Übergabe einer Anforderung für die Überprüfung und Bearbeitung durch einen Humanübersetzer finden Sie in [Gebührenpflichtige Anforderung für die Humanübersetzung](managetranslations.html#humantranslation). 




## Ein Bundle für die Arbeit auswählen
{: #globalizationpipeline_selectingabundle}

1. Klicken Sie auf die Registerkarte **Bundles**, um alle Bundles anzuzeigen, die Sie erstellt haben.
2. Klicken Sie auf **Bundle-ID** in der Liste, um weitere Details zum jeweiligen Bundle anzuzeigen, oder klicken Sie auf das Symbol **Bundledetails anzeigen** ![Mit dem Symbol zur Anzeige der Bundledetails kann ein Bundle geöffnet und die zugehörige Übersetzung bearbeitet werden](images/viewProjectDetailIcon.png) in der Aktionsspalte.

![Über die Registerkarte für Bundles können alle verfügbaren Bundles angezeigt werden.](images/translationBundles.png)

Nachdem Sie ein Bundle für die Arbeit ausgewählt haben, können Sie den Status der zugehörigen Übersetzungen anzeigen, Sprachen hinzufügen oder entfernen, die Übersetzungen bearbeiten oder Updates für die Ressourcendatei zur Verfügung stellen.

Wenn Sie ein Bundle nicht mehr benötigen, können Sie es von der Registerkarte **Bundles** löschen. Alle Übersetzungen, die dem Bundle zugeordnet sind, werden ebenfalls gelöscht.


