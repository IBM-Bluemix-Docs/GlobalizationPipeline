---

copyright:
  years: 2015, 2018
lastupdated: "2017-05-26"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# Details zu Bundle ändern
{: #modifybundles}

Wenn Sie ein Bundle öffnen, können Sie alle Details zum Bundle anzeigen. Alle Zielsprachen im Bundle werden zusammen mit dem jeweils aktuellen Übersetzungsstatus aufgelistet.

![Die Detailseite zu einem Bundle enthält Informationen zum betreffenden Bundle und den zugehörigen Übersetzungen.](images/bundleDetails.png)

Der Status für jede Sprache im Bundle kann 'In Bearbeitung', 'Fehlgeschlagen' oder 'Übersetzt' lauten:

| Status | Beschreibung |
|--------|-------------|
| In Bearbeitung | Die automatische Übersetzung ist noch in Bearbeitung. |
| Fehlgeschlagen | Es ist ein Fehler aufgetreten, als die Ressourcendatei in die Zielsprache übersetzt wurde. |
| Übersetzt | Die Übersetzung in die Zielsprache ist abgeschlossen. |

Sie können die Ressourcendatei aktualisieren, die das Bundle verwendet, eine Zielsprache zum Bundle hinzufügen, eine Zielsprache aus dem Bundle löschen und die generierten Übersetzungen für eine Zielsprache herunterladen.

## Ressourcendatei aktualisieren, die vom Bundle verwendet wird

1. Klicken Sie neben der Quellensprache auf das Symbol **Ressourcen hochladen** ![Mit diesem Symbol kann eine neue Ressourcendatei hochgeladen werden](images/uploadIcon.png) in der Aktionsspalte.
2. Klicken Sie auf **Durchsuchen** und wählen Sie eine neue Ressourcendatei zum Hochladen aus.
3. Wählen Sie den Typ der Ressourcendatei aus, den Sie hochladen.
 * Java-Eigenschaftendatei
 * AMD I18N
 * JSON
4. Klicken Sie auf **Aktualisieren**, um die neue Ressourcendatei hochzuladen.

Die Schlüssel/Wertpaare, die sich in der neuen oder aktualisierten Ressourcendatei befinden, werden mit den Werten synchronisiert, die bereits hochgeladen wurden. Nur neuer oder geänderter Inhalt wird übersetzt.

## Eine Zielsprache zu einem Bundle hinzufügen

1. Klicken Sie auf die Schaltfläche **Sprache hinzufügen**.
2. Alle verfügbaren Zielsprachen werden angezeigt. Wählen Sie die Sprachen aus, die zum Bundle hinzugefügt werden sollen.

Die Übersetzung für die ausgewählten Sprachen beginnt sofort.

## Eine Zielsprache aus dem Bundle löschen

Wenn Sie eine Zielsprache aus dem Bundle löschen, entfernen Sie die Zielsprache und alle zugehörigen Übersetzungen aus dem Projekt. Klicken Sie in der Aktionsspalte der zu entfernenden Zielsprache auf das Symbol **Diese Zielsprache entfernen** ![Mit dem Papierkorbsybmol kann diese Zielsprache entfernt werden](images/trashIcon.png).

## Generierte Übersetzungen für eine Zielsprache herunterladen.

{{site.data.keyword.GlobalizationPipeline_short}} bietet mehrere Möglichkeiten, um die Übersetzung in eine Zielsprache in Ihre Anwendung zu integrieren. Sie können die Übersetzung als Ressourcendatei herunterladen und in Ihren Anwendungsbuild einbeziehen. Sie können auf die Übersetzung auch dynamisch von {{site.data.keyword.GlobalizationPipeline_short}} mithilfe eines der Open-Source-[SDKs](https://github.com/IBM-Bluemix/gp-common) verweisen. 

<!-- For information on {{site.data.keyword.GlobalizationPipeline_full}} SDKs, see <link>. -->

Gehen Sie folgt vor, um die Übersetzung als Ressourcendatei herunterzuladen: 

1. Klicken Sie in der Spalte **Aktionen** der Ziel- oder Quellensprache, die heruntergeladen werden soll, auf das Symbol **Übersetzungen herunterladen** ![Mit dem Downloadsymbol können die Quellenschlüssel oder die Übersetzungen für eine Zielsprache heruntergeladen werden](images/downloadIcon.png).
2. Wählen Sie ein Dateiformat aus.
3. Klicken Sie auf **Herunterladen**.
