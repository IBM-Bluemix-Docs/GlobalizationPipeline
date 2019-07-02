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


# IBM Cloud IAM für {{site.data.keyword.GlobalizationPipeline_short}}
{: #gp_iam}

## Zugriff
{: #gp_iam_access}
Der Zugriff auf {{site.data.keyword.GlobalizationPipeline_short}}-Serviceinstanzen, die für RC aktiviert sind, wird für Benutzer in Ihrem Konto durch {{site.data.keyword.Bluemix_notm}} Identity and Access Management (IAM) und/oder die {{site.data.keyword.GlobalizationPipeline_short}}-Authentifizierung gesteuert. Dagegen kann für CF-Instanzen nur die {{site.data.keyword.GlobalizationPipeline_short}}-Authentifizierung verwendet werden.

## {{site.data.keyword.GlobalizationPipeline_short}}-Authentifizierung
{: #gp_iam_ca}
Informationen zur Verwendung des Authentifizierungsmechanismus finden Sie in [API-Benutzer hinzufügen](/docs/services/GlobalizationPipeline/managetranslations.html#adduser).


## Identity Access Management (IAM)
{: #gp_iam_ovw}
Jedem Benutzer, der auf den {{site.data.keyword.GlobalizationPipeline_short}}-Service in Ihrem Konto zugreift, muss eine Zugriffsrichtlinie mit einer definierten IAM-Benutzerrolle zugeordnet worden sein. Diese Richtlinie bestimmt, welche Aktionen der Benutzer innerhalb des Kontexts des Service oder der von Ihnen ausgewählten Instanz ausführen kann. Die zulässigen Aktionen werden von dem {{site.data.keyword.Bluemix_notm}}-Service angepasst und definiert als Operationen, die für den Service ausgeführt werden dürfen. Die Aktionen werden dann IAM-Benutzerrollen zugeordnet.

Richtlinien ermöglichen es, Zugriff auf verschiedenen Ebenen zu gewähren. Zu den Optionen gehören unter anderem:

* Zugriff über alle Instanzen eines Service in Ihrem Konto
* Zugriff auf eine einzelne Serviceinstanz in Ihrem Konto
* Zugriff auf eine bestimmte Ressource innerhalb einer Instanz
* Zugriff auf alle für IAM aktivierten Services in Ihrem Konto

Nachdem Sie den Umfang der Zugriffsrichtlinie definiert haben, weisen Sie eine Rolle zu. Die folgende Tabelle führt die Aktionen detailliert auf, die zu Servicezugriffsrollen zugeordnet sind. Servicezugriffsrollen ermöglichen es Benutzern, auf {{site.data.keyword.GlobalizationPipeline_short}} zuzugreifen und die API von {{site.data.keyword.GlobalizationPipeline_short}} aufzurufen.

| **Rollentyp** | **Übersetzungen anzeigen** | **Übersetzungen bearbeiten** | **Bundle-Informationen ändern** | **Anforderungen für professionelle Übersetzung erstellen** | **Anforderungen für professionelle Übersetzung anzeigen** |
|---------------|-----------------------|-----------------------|-------------------------------|----------------------------------------------|--------------------------------------------|
| Leseberechtigter | Ja | Nein | Nein | Nein | Nein |
| Schreibberechtigter | Ja | Ja | Nein | Nein | Ja |
| Manager       | Ja | Ja | Ja | Ja | Ja |
{: caption="Tabelle 1. IAM-Benutzerrollen und Aktionen" caption-side="top"}

Zum gegenwärtigen Zeitpunkt erhalten IAM-Benutzer Zugriff auf Serviceinstanzebene; es ist nicht möglich, IAM-Benutzern Zugriff auf Bundle-Ebene zu erteilen oder zu verweigern. Für eine differenziertere Zugriffssteuerung verwenden Sie die {{site.data.keyword.GlobalizationPipeline_short}}-Authentifizierung.

Informationen zur Zuordnung von Benutzerrollen in der Benutzerschnittstelle finden Sie in [IAM-Zugriff verwalten](/docs/iam?topic=iam-iammanidaccser).

### API-Aufrufe generieren
{: #gp_iam_apicalls}

Führen Sie die folgenden Schritte aus, um die Serviceberechtigungsnachweise zu generieren oder abzurufen.
1. Melden Sie sich im [{{site.data.keyword.Bluemix}}-Dashboard](https://cloud.ibm.com/) bei Ihrem {{site.data.keyword.Bluemix}}-Konto an.
2. Klicken Sie im [{{site.data.keyword.Bluemix}}-Dashboard](https://cloud.ibm.com/) auf die Serviceinstanz.
3. Klicken Sie auf **Serviceberechtigungsnachweise**, um die Serviceinstanz zu öffnen.  
4. Klicken Sie auf **Neuer Berechtigungsnachweis**, um anhand der Eingabeaufforderung neue Berechtigungsnachweise zu erstellen.
5. Klicken Sie nach dem Erstellen des Berechtigungsnachweises auf **Berechtigungsnachweise anzeigen**.
![Screenshot mit Informationen zu einem API-Beispielschlüssel](images/gp_iam_apicalls.gif)

Die folgenden Beispiele veranschaulichen Aufrufe der API von {{site.data.keyword.GlobalizationPipeline_short}} mithilfe der IAM-Authentifizierung.

* IAM-Trägertoken verwenden
```
curl -X GET \
  https://gp-rest.us-south.g11n-pipeline.test.cloud.ibm.com/translate/rest/50341556337c581c208188ff8908ebc7/v2/bundles \
  -H 'Authorization: Bearer eyJjsksd…w'
```

* API-Schlüssel verwenden
```
curl -X GET \
  https://gp-rest.us-south.g11n-pipeline.test.cloud.ibm.com/translate/rest/50341556337c581c208188ff8908ebc7/v2/bundles \
  -H 'Authorization: API-KEY MklfrP…ACem'
```
Im vorherigen Beispiel können Sie die folgenden Informationen abrufen:
* “50341556337c581c208188ff8908ebc7” ist die Instanz-ID (aus dem Abschnitt mit den Berechtigungsnachweisen)
* “https://gp-rest.us-south.g11n-pipeline.test.cloud.ibm.com/translate/rest” ist die URL (aus dem Abschnitt mit den Berechtigungsnachweisen)
* “MklfrP…ACem” ist der API-Schlüssel (aus dem Abschnitt mit den Berechtigungsnachweisen)
* “eyJjsksd…w” ist das IAM-Trägertoken

Anweisungen zum Abrufen des IAM-Trägertokens aus dem API-Schlüssel finden Sie in [{{site.data.keyword.Bluemix_notm}}-IAM-Token mithilfe eines API-Schlüssels abrufen](/docs/iam?topic=iam-iamtoken_from_apikey#iamtoken_from_apikey).
