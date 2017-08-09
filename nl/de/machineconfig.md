---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# Konfiguration zur automatischen Übersetzung
{: #machineconfig}

{{site.data.keyword.GlobalizationPipeline_full}} unterstützt die Fähigkeit zur Integration alternativer Services für automatische Übersetzung, um automatische Übersetzungen für Ihre Bundles auszuführen. Das Hinzufügen eines alternativen Service kann vorteilhaft sein, wenn die von {{site.data.keyword.GlobalizationPipeline_short}} verwendete Standard-Engine eine bestimmte Sprache, die Sie benötigen, nicht anbietet oder wenn Sie automatische Übersetzungen bevorzugen, die von einer anderen Engine generiert wurden. Die Verwendung von und die Gebühren für alternative Services werden unter den Bedingungen des jeweiligen Service aufgeführt.

Um einen alternativen Service für automatische Übersetzung für {{site.data.keyword.GlobalizationPipeline_short}} hinzuzufügen und zu konfigurieren, wählen Sie die Registerkarte **Automatische Übersetzung - Konfiguration** im {{site.data.keyword.GlobalizationPipeline_short}}-Dashboard aus.

* Um einen Service für automatische Übersetzung hinzuzufügen, der sich im {{site.data.keyword.Bluemix_notm}}-Katalog befindet, (**Watson Language Translator**), muss der Service zuerst zu Ihrem {{site.data.keyword.Bluemix_notm}}-Bereich hinzugefügt werden.

* Um einen Service anderer Anbieter hinzuzufügen, wählen Sie die Schaltfläche für diesen Service auf der Registerkarte **Automatische Übersetzung - Konfiguration** aus und stellen die erforderliche Benutzerberechtigung für den Zugriff auf den Service bereit.

Nachdem der Service für automatische Übersetzung zu {{site.data.keyword.GlobalizationPipeline_short}} hinzugefügt wurde, führen Sie die verbleibenden Schritte aus, um die Integration dieses Service abzuschließen.

1. Klicken Sie auf **Aktivieren**, um die Integration dieses Service zu aktivieren.

2. Klicken Sie auf **Sprachen aktualisieren**, um die aktualisierte Liste der unterstützten Zielsprachen anzuzeigen.

3. Wählen Sie in der Liste der Zielsprachen die Engine für automatische Übersetzung aus, die die Übersetzung ausführen soll.

4. Klicken Sie auf **Speichern**, um zur Registerkarte **Automatische Übersetzung - Konfiguration** zurückzukehren.

Sobald ein alternativer Service für {{site.data.keyword.GlobalizationPipeline_short}} konfiguriert wurde, werden alle Zielsprachen, die dieser Engine zugeordnet wurden, mithilfe der Engine generiert. 

Gehen Sie wie folgt vor, um die Verwendung der alternativen Engine für automatische Übersetzung zu stoppen:

1. Klicken Sie auf der Registerkarte **Automatische Übersetzung - Konfiguration** für den Service, dessen Verwendung Sie stoppen möchten, auf die Schaltfläche **Inaktivieren**.

Wenn ein alternativer Service für automatische Übersetzung inaktiviert wurde, verbleiben alle Übersetzungen, die von diesem Service generiert wurden, innerhalb Ihrer Bundles. Die Übersetzung in eine bestimmte Zielsprache ist jedoch für künftige Updates möglicherweise nicht mehr verfügbar, wenn die Zielsprache nicht mehr von der Engine für automatische Übersetzung unterstützt wird, die dann aktiviert ist.

<!-- Review comment: When you disable an engine, do you need to go back and reconfigure the languages?? Does it go back to the default engine? What happens? -->
