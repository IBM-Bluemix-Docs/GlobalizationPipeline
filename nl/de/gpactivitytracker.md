---

copyright:
  years: 2016, 2019

lastupdated: "2019-06-26"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:codeblock: .codeblock}
{:tip: .tip}
{:download: .download}


# {{site.data.keyword.cloudaccesstrailshort}}-Ereignisse in {{site.data.keyword.GlobalizationPipeline_short}}
{: #gpat_events}

Mit dem {{site.data.keyword.cloudaccesstrailfull}}-Service können Sie die Interaktion von Benutzern und Anwendungen mit IBM {{site.data.keyword.GlobalizationPipeline_short}} in {{site.data.keyword.Bluemix}} verfolgen.
{:shortdesc}

Der {{site.data.keyword.cloudaccesstrailfull_notm}}-Service zeichnet die vom Benutzer initiierten Aktivitäten auf, die den Status eines Service in {{site.data.keyword.Bluemix_notm}} ändern. Weitere Informationen finden Sie in [{{site.data.keyword.cloudaccesstrailfull_notm}}](/docs/services/Activity-Tracker-with-LogDNA?topic=logdnaat-getting-started).




## Ereignisliste: Bundle-Ereignisse
{: #gpevents_bundle}

In der folgenden Tabelle sind die Aktionen aufgeführt, die ein Ereignis im Zusammenhang mit Bundles generieren:

|Aktion|Beschreibung|
|---|---|  
|g11n-pipeline.bundles.read|Ruft eine Liste mit Bundle-IDs ab. |
|g11n-pipeline.bundle.create|Erstellt ein neues Bundle. |
|g11n-pipeline.bundle.read|Ruft Informationen zum Bundle ab. |
|g11n-pipeline.bundle.update|Aktualisiert die Konfiguration des Bundles. |
|g11n-pipeline.bundle.delete|Löscht das angegebene Bundle. |
|g11n-pipeline.bundle-language.create|Lädt Ressourceneinträge hoch. |
|g11n-pipeline.bundle-language.read|Ruft die Ressourcenzeichenfolgen (Schlüssel/Wert-Paare) für die Sprache ab. |
|g11n-pipeline.bundle-language.update|Aktualisiert Ressourceneinträge. |
|g11n-pipeline.bundle-language.read|Ruft Informationen zum Ressourceneintrag ab. |
|g11n-pipeline.bundle-language.update|Aktualisiert den Ressourceneintrag. |

## Ereignisliste: Übersetzungsanforderungsereignisse für Bundles
{: #gpevents_bundle_tr_req}

In der folgenden Tabelle sind die Aktionen aufgeführt, die ein Ereignis im Zusammenhang mit Übersetzungsanforderungen für Bundles generieren:

|Aktion|Beschreibung|
|---|---|  
|g11n-pipeline.trs.read|Ruft eine Liste mit Übersetzungsanforderungen ab. |
|g11n-pipeline.tr.read|Ruft Informationen zur angegebenen Übersetzungsanforderung ab. |
|g11n-pipeline.tr.update|Aktualisiert Informationen zur angegebenen Übersetzungsanforderung. |
|g11n-pipeline.tr.delete|Löscht die angegebene Übersetzungsanforderung. |
|g11n-pipeline.tr-bundle.read|Ruft Informationen zum Bundle ab. |
|g11n-pipeline.tr-bundle-language.read|Ruft Ressourceneinträge für das angegebene Bundle und die angegebene Sprache ab. |
|g11n-pipeline.tr-bundle-language.read|Ruft Informationen zum Ressourceneintrag ab. |
|g11n-pipeline.trs.create|Erstellt eine neue Übersetzungsanforderung. |


## Ereignisliste: XLIFF-Ereignisse für Bundles
{: #gpevents_bundle_xliff}

In der folgenden Tabelle sind die Aktionen aufgeführt, die ein Ereignis im Zusammenhang mit Bundle-XLIFF-Daten generieren:

|Aktion|Beschreibung|
|---|---|  
|g11n-pipeline.xliff-bundles.read|Ruft Ressourcendaten in der angegebenen Sprache im Format XLIFF 2.0 aus den Bundles ab. |
|g11n-pipeline.xliff-bundles.update|Aktualisiert Bundles in der Serviceinstanz mit den XLIFF-Daten. |
|g11n-pipeline.xliff-tr-bundles.read|Ruft Ressourcendaten in der angegebenen Sprache im Format XLIFF 2.0 in der Übersetzungsanforderung ab. |


## Ereignisliste: Partnerereignisse
{: #gpevents_partner}

In der folgenden Tabelle sind die Aktionen aufgeführt, die ein Ereignis im Zusammenhang mit Partnern generieren:

|Aktion|Beschreibung|
|---|---|  
|g11n-pipeline.partner.read|Ruft Informationen zum Partner ab. |
|g11n-pipeline.partner.update|Aktualisiert Informationen zum Partner. |
|g11n-pipeline.partner-trs.read|Ruft eine Liste mit Übersetzungsanforderungen ab, die dem Partner zugewiesen sind. |
|g11n-pipeline.partner-tr.read|Ruft Informationen zur angegebenen Übersetzungsanforderung ab. |
|g11n-pipeline.partner-tr.update|Aktualisiert Informationen zur angegebenen Übersetzungsanforderung. |
|g11n-pipeline.partner-tr.delete|Löscht die angegebene Übersetzungsanforderung. |
|g11n-pipeline.partner-tr-bundle.read|Ruft Informationen zum Bundle ab. |
|g11n-pipeline.partner-tr-bundle-language.read|Ruft Ressourceneinträge für das angegebene Bundle und die angegebene Sprache ab. |
|g11n-pipeline.partner-tr-bundle-language.update|Aktualisiert Ressourceneinträge für das angegebene Bundle und die angegebene Sprache. |
|g11n-pipeline.partner-tr-bundle-language.read|Ruft Informationen zum Ressourceneintrag ab. |
|g11n-pipeline.partner-tr-bundle-language.update|Aktualisiert den Ressourceneintrag. |
|g11n-pipeline.partner-users.read|Ruft verfügbare Benutzer für diesen Partner ab. |
|g11n-pipeline.partner-user.read|Ruft Informationen zum angegebenen Partnerbenutzer ab. |
|g11n-pipeline.partner-user.update|Aktualisiert Informationen zu einem Partnerbenutzer. |
|g11n-pipeline.partner-user.delete|Löscht den angegebenen Partnerbenutzer. |
|g11n-pipeline.partner-user.create|Erstellt einen neuen Partnerbenutzer. |
|g11n-pipeline.partner-tr-xliff-bundles.update|Aktualisiert Ressourcendaten in der Übersetzungsanforderung mit den XLIFF-Daten. |
|g11n-pipeline.partner-tr-xliff-bundles-language.read|Ruft Ressourcendaten in der angegebenen Sprache im Format XLIFF 2.0 in der Übersetzungsanforderung ab. |



## Ereignisliste: Administratorereignisse
{: #gpevents_admin}

In der folgenden Tabelle sind die Aktionen aufgeführt, die ein Ereignis im Zusammenhang mit dem Administrator generieren:

|Aktion|Beschreibung|
|---|---|  
|g11n-pipeline.instances.read|Ruft eine Liste mit Serviceinstanzen ab. |
|g11n-pipeline.instance.read|Ruft Informationen zur Serviceinstanz ab. |
|g11n-pipeline.instance.update|Aktualisiert die Konfiguration der Serviceinstanz. |
|g11n-pipeline.instance.create|Erstellt eine neue Serviceinstanz. |
|g11n-pipeline.instance.delete|Löscht die angegebene Serviceinstanz. |
|g11n-pipeline.instance.create|Erstellt eine neue verwaltete Cloud Foundry-Serviceinstanz. |
|g11n-pipeline.partners.read|Ruft eine Liste mit Partnern ab. |
|g11n-pipeline.partner.create|Erstellt einen neuen Partner. |
|g11n-pipeline.partner.delete|Löscht den angegebenen Partner. |



## Ereignisliste: Benutzerereignisse
{: #gpevents_user}

In der folgenden Tabelle sind die Aktionen aufgeführt, die ein Ereignis im Zusammenhang mit Benutzern generieren:

|Aktion|Beschreibung|
|---|---|  
|g11n-pipeline.instance-users.read|Ruft die Benutzer in dieser Serviceinstanz ab. |
|g11n-pipeline.instance-user.read|Ruft Informationen zum angegebenen Benutzer ab. |
|g11n-pipeline.instance-user.update|Aktualisiert Informationen zu einem Benutzer. |
|g11n-pipeline.instance-user.delete|Löscht den angegebenen Benutzer. |
|g11n-pipeline.instance-users.create|Erstellt einen neuen Benutzer. |


## Ereignisliste: Konfigurationsereignisse
{: #gpevents_config}

In der folgenden Tabelle sind die Aktionen aufgeführt, die ein Ereignis im Zusammenhang mit der Übersetzungskonfiguration generieren:

|Aktion|Beschreibung|
|---|---|  
|g11n-pipeline.config-mts.read|Ruft alle MT-Servicebindungen ab. |
|g11n-pipeline.config-mt.read|Ruft die MT-Servicebindungsdaten ab. |
|g11n-pipeline.config-translations.read|Ruft alle Übersetzungskonfigurationen ab. |
|g11n-pipeline.config-translation.read|Ruft die Übersetzungskonfiguration ab. |
|g11n-pipeline.config-mt.update|Fügt die angegebenen MT-Servicebindungsdaten ein. Falls die angegebenen Bindungsdaten bereits vorhanden sind, werden sie durch die angegebenen MT-Servicebindungsdaten ersetzt. |
|g11n-pipeline.config-mt.delete|Löscht die angegebenen MT-Servicebindungsdaten. |
|g11n-pipeline.config-translation.update|Fügt die Übersetzungskonfiguration für die angegebene Sprachkombination ein. Falls die Konfiguration für die Sprachkombination bereits vorhanden ist, wird sie durch die angegebene Konfiguration ersetzt. |
|g11n-pipeline.config-translation.delete|Löscht die Übersetzungskonfiguration für die angegebene Sprachkombination. |


## Ereignisliste: Instanzereignisse
{: #gpevents_instance}

In der folgenden Tabelle sind die Aktionen aufgeführt, die ein Ereignis im Zusammenhang mit Instanzen generieren:

|Aktion|Beschreibung|
|---|---|  
|g11n-pipeline.instance.read|Ruft Informationen zu dieser Übersetzungsservicesinstanz ab. |


## Position der Ereignisse
{: #gp_at_ui}

{{site.data.keyword.cloudaccesstrailshort}}-Ereignisse sind in der **Bereichsdomäne** von {{site.data.keyword.cloudaccesstrailshort}} verfügbar, die in der {{site.data.keyword.Bluemix_notm}}-Region zur Verfügung steht, in der der {{site.data.keyword.GlobalizationPipeline_short}}-Service bereitgestellt wird. Die {{site.data.keyword.cloudaccesstrailshort}}-Serviceinstanz und die {{site.data.keyword.GlobalizationPipeline_short}}-Instanz müssen im selben CF-Bereich bereitgestellt werden.

Für RC-Instanzen von {{site.data.keyword.GlobalizationPipeline_short}} stehen die Activity Tracker-Ereignisse in der Activity Tracker-**Kontodomäne** zur Verfügung, in der die Ereignisse in der {{site.data.keyword.Bluemix_notm}}-Region generiert werden.
