---

copyright:
  years: 2015, 2018
lastupdated: "2017-12-13"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}


# Einführung in {{site.data.keyword.GlobalizationPipeline_short}}
{: #globalizationpipeline}

{{site.data.keyword.GlobalizationPipeline_full}} ist ein {{site.data.keyword.Bluemix}}-Service, der es App-Entwicklern ermöglicht, übersetzte Anwendungen ohne zeitliche Verzögerung für ihre globalen Kunden bereitzustellen. {{site.data.keyword.GlobalizationPipeline_short}} dient als Übersetzungsrepository und bietet automatische Übersetzung, Überprüfung und Bearbeitung durch Humanübersetzer sowie APIs und SDKs für eine reibungslose Integration der Übersetzung in die DevOps- und Continuous Development-Infrastruktur, indem die manuellen und isolierten Operationen, die mit dem traditionellen Übersetzungsprozess verbunden sind, eliminiert werden.
{:shortdesc}

Sie können den {{site.data.keyword.GlobalizationPipeline_short}}-Service nutzen, um jede beliebige App, die in {{site.data.keyword.Bluemix_notm}} bereitgestellt oder gehostet wird, zu übersetzen; die nicht gebundene Version des Service kann zu Übersetzung von Apps verwendete werden, die auf anderen Cloudplattformen gehostet werden.

{{site.data.keyword.GlobalizationPipeline_short}} bietet sowohl eine Dashboardschnittstelle zur Verwaltung der App-Übersetzungen als auch eine REST-konforme API zur vollständigen Automatisierung des Übersetzungsprozesses. Informationen zur {{site.data.keyword.GlobalizationPipeline_short}}-API finden Sie in der [API-Referenz](https://gp-rest.ng.bluemix.net/translate/swagger/index.html){: new_window}.

## Übersetzungsplan auswählen
{: #globalizationpipeline_chooseplan}

Bevor Sie mit der Arbeit mit Übersetzungen in {{site.data.keyword.GlobalizationPipeline_short}} beginnen, können Sie einen geeigneten Übersetzungsplan auswählen.

In {{site.data.keyword.GlobalizationPipeline_short}} stehen  zwei Übersetzungspläne zur Verfügung: der Standardplan und der Professional-Plan. Beide Pläne umfassen die integrierte, uneingeschränkte automatische Basisübersetzung sowie die Möglichkeit der gebührenpflichtigen Integration mit anderen Engines zur automatischen Übersetzung. Im Rahmen des Professional-Plans bietet {{site.data.keyword.GlobalizationPipeline_short}} darüber hinaus einen Service, bei dem die Übersetzungen durch einen Humanübersetzer überprüft und bearbeitet werden. Sie können zwischen den {{site.data.keyword.GlobalizationPipeline_short}}-Plänen in {{site.data.keyword.Bluemix_notm}} wechseln, wobei alle Daten beibehalten werden.


## Datennutzung von {{site.data.keyword.GlobalizationPipeline_short}} schätzen
{: #globalizationpipeline_documentpricing}

{{site.data.keyword.GlobalizationPipeline_short}} speichert Ihre Übersetzungen in einer Back-End-Datenbank. Um die Größe des Datenarchivs zu schätzen, können Sie die folgende Formel verwenden:

`<expected resource data storage size in MB> ˜= 0.,005 * <number of key/value pairs in the source resource> * <number of languages including the source language>`

Nach der Formel ist die Größe eines typischen Bundles `(Länge des Schlüssels + Länge des Wertes in UTF-8 = ˜40 Byte `.

Wenn Sie zum Beispiel über 100 Schlüssel/Wert-Paare verfügen und diese in 9 Sprachen übersetzen, beträgt die geschätzte Speichergröße 0,0005 100 (9+1) = 0,5 MB. Die tatsächliche Größe kann sich abhängig von der tatsächlichen Größe der Schlüssel/Wert-Paare und der Metadaten, die mit der Übersetzung gespeichert werden, davon unterscheiden.

Verwenden Sie den {{site.data.keyword.Bluemix_notm}}-[Preisrechner](https://console.ng.bluemix.net/?direct=classic/#/pricing/cloudOEPaneId=pricing&paneId=pricingSheet&orgGuid=127a45f4-4461-4d5b-a26b-6dc2fdd1a3a2&spaceGuid=208fb1ff-413b-4fd9-9615-e8226062d0f3), um Ihre monatlichen Kosten zu ermitteln.

**Hinweis**: Durch die Verwendung des Überprüfungsfeatures im Rahmen des Professional-Plans erhöht sich die Datennutzung über die oben angeführten Werte hinaus.
