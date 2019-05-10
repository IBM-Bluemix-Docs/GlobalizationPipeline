---

copyright:
  years: 2016, 2019

lastupdated: "2019-03-20"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:codeblock: .codeblock}
{:tip: .tip}
{:download: .download}


# Sucesos de {{site.data.keyword.cloudaccesstrailshort}} de {{site.data.keyword.GlobalizationPipeline_short}}
{: #gpat_events}

Utilice el servicio {{site.data.keyword.cloudaccesstrailfull}} para realizar un seguimiento de la forma en la que los usuarios y las aplicaciones interactúan con IBM {{site.data.keyword.GlobalizationPipeline_short}} en {{site.data.keyword.Bluemix}}.
{:shortdesc}

El servicio {{site.data.keyword.cloudaccesstrailfull_notm}} registra las actividades iniciadas por el usuario que cambian el estado de un servicio en {{site.data.keyword.Bluemix_notm}}. Para obtener más información, consulte [{{site.data.keyword.cloudaccesstrailfull_notm}}](/docs/services/cloud-activity-tracker/index.html).




## Lista de sucesos: sucesos de paquete
{: #gpevents_bundle}

En la tabla siguiente, se enumeran las acciones que están relacionadas con paquetes y generan un suceso:

|Acción|Descripción|
|---|---|  
|g11n-pipeline.bundles.read|Obtiene una lista de ID de paquete.|
|g11n-pipeline.bundle.create|Crea un nuevo paquete.|
|g11n-pipeline.bundle.read|Obtiene la información del paquete.|
|g11n-pipeline.bundle.update|Actualiza la configuración del paquete.|
|g11n-pipeline.bundle.delete|Suprime el paquete especificado.|
|g11n-pipeline.bundle-language.create|Carga entradas de recurso.|
|g11n-pipeline.bundle-language.read|Obtiene las series de recurso (pares clave/valor) para el idioma.|
|g11n-pipeline.bundle-language.update|Actualiza entradas de recurso.|
|g11n-pipeline.bundle-language.read|Obtiene la información de entradas de recurso.|
|g11n-pipeline.bundle-language.update|Actualiza la entrada de recurso.|

## Lista de sucesos: sucesos de solicitud de traducción de paquete
{: #gpevents_bundle_tr_req}

En la tabla siguiente, se enumeran las acciones que están relacionadas con solicitudes de traducción de paquete y generan un suceso:

|Acción|Descripción|
|---|---|  
|g11n-pipeline.trs.read|Obtiene una lista de solicitudes de traducción.|
|g11n-pipeline.tr.read|Obtiene la información de la solicitud de traducción especificada.|
|g11n-pipeline.tr.update|Actualiza la información de la solicitud de traducción especificada.|
|g11n-pipeline.tr.delete|Suprime la solicitud de traducción especificada.|
|g11n-pipeline.tr-bundle.read|Obtiene la información del paquete.|
|g11n-pipeline.tr-bundle-language.read|Obtiene las entradas de recurso para el idioma y el paquete especificados.|
|g11n-pipeline.tr-bundle-language.read|Obtiene la información de entradas de recurso.|
|g11n-pipeline.trs.create|Crea una nueva solicitud de traducción.|


## Lista de sucesos: sucesos de xliff de paquete
{: #gpevents_bundle_xliff}

En la tabla siguiente, se enumeran las acciones que están relacionadas con xliff de paquete y generan un suceso:

|Acción|Descripción|
|---|---|  
|g11n-pipeline.xliff-bundles.read|Obtiene datos de recurso en el idioma especificado de los paquetes en formato XLIFF 2.0.|
|g11n-pipeline.xliff-bundles.update|Actualiza paquetes en la instancia de servicio con los datos XLIFF.|
|g11n-pipeline.xliff-tr-bundles.read|Obtiene datos de recurso en el idioma especificado de la solicitud de traducción en formato XLIFF 2.0.|


## Lista de sucesos: sucesos de socio
{: #gpevents_partner}

En la tabla siguiente, se enumeran las acciones que están relacionadas con socios y generan un suceso:

|Acción|Descripción|
|---|---|  
|g11n-pipeline.partner.read|Obtiene la información del socio.|
|g11n-pipeline.partner.update|Actualiza la información del socio.|
|g11n-pipeline.partner-trs.read|Obtiene una lista de solicitudes de traducción asignadas al socio.|
|g11n-pipeline.partner-tr.read|Obtiene la información de la solicitud de traducción especificada.|
|g11n-pipeline.partner-tr.update|Actualiza la información de la solicitud de traducción especificada.|
|g11n-pipeline.partner-tr.delete|Suprime la solicitud de traducción especificada.|
|g11n-pipeline.partner-tr-bundle.read|Obtiene la información del paquete.|
|g11n-pipeline.partner-tr-bundle-language.read|Obtiene las entradas de recurso para el idioma y el paquete especificados.|
|g11n-pipeline.partner-tr-bundle-language.update|Actualiza las entradas de recurso para el idioma y el paquete especificados.|
|g11n-pipeline.partner-tr-bundle-language.read|Obtiene la información de entradas de recurso.|
|g11n-pipeline.partner-tr-bundle-language.update|Actualiza la entrada de recurso.|
|g11n-pipeline.partner-users.read|Obtiene los usuarios disponibles para este socio.|
|g11n-pipeline.partner-user.read|Obtiene la información del usuario asociado especificado.|
|g11n-pipeline.partner-user.update|Actualiza la información de un usuario asociado.|
|g11n-pipeline.partner-user.delete|Suprime el usuario asociado especificado.|
|g11n-pipeline.partner-user.create|Crea un usuario asociado nuevo.|
|g11n-pipeline.partner-tr-xliff-bundles.update|Actualiza los datos de recurso de la solicitud de traducción con los datos XLIFF.|
|g11n-pipeline.partner-tr-xliff-bundles-language.read|Obtiene datos de recurso en el idioma especificado de la solicitud de traducción en formato XLIFF 2.0.|



## Lista de sucesos: sucesos de administrador
{: #gpevents_admin}

En la tabla siguiente, se enumeran las acciones que están relacionadas con el administrador y generan un suceso:

|Acción|Descripción|
|---|---|  
|g11n-pipeline.instances.read|Obtiene una lista de instancias de servicio.|
|g11n-pipeline.instance.read|Obtiene la información de la instancia de servicio.|
|g11n-pipeline.instance.update|Actualiza la configuración de la instancia de servicio.|
|g11n-pipeline.instance.create|Crea una nueva instancia de servicio.|
|g11n-pipeline.instance.delete|Suprime la instancia de servicio especificada.|
|g11n-pipeline.instance.create|Crea una nueva instancia de servicio gestionada de Cloud Foundry.|
|g11n-pipeline.partners.read|Obtiene una lista de socios.|
|g11n-pipeline.partner.create|Crea un socio nuevo.|
|g11n-pipeline.partner.delete|Suprime el socio especificado.|



## Lista de sucesos: sucesos de usuario
{: #gpevents_user}

En la tabla siguiente, se enumeran las acciones que están relacionadas con usuarios y generan un suceso:

|Acción|Descripción|
|---|---|  
|g11n-pipeline.instance-users.read|Obtiene usuarios de esta instancia de servicio.|
|g11n-pipeline.instance-user.read|Obtiene la información del usuario especificado.|
|g11n-pipeline.instance-user.update|Actualiza la información de un usuario.|
|g11n-pipeline.instance-user.delete|Suprime el usuario especificado.|
|g11n-pipeline.instance-users.create|Crea un nuevo usuario.|


## Lista de sucesos: sucesos de configuración
{: #gpevents_config}

En la tabla siguiente, se enumeran las acciones que están relacionadas con la configuración de traducción y generan un suceso:

|Acción|Descripción|
|---|---|  
|g11n-pipeline.config-mts.read|Obtiene todos los enlaces de servicio de MT.|
|g11n-pipeline.config-mt.read|Obtiene los datos de enlace de servicio de MT.|
|g11n-pipeline.config-translations.read|Obtiene todas las configuraciones de traducción.|
|g11n-pipeline.config-translation.read|Obtiene la configuración de traducción.|
|g11n-pipeline.config-mt.update|Pone los datos de enlace de servicio de MT especificados. Si los datos de enlace de servicio especificados ya existen, son sustituidos por los datos de enlace de servicio de MT especificados.|
|g11n-pipeline.config-mt.delete|Suprime los datos de enlace de servicio de MT especificados.|
|g11n-pipeline.config-translation.update|Pone la configuración de traducción para el par de idiomas especificado. Si la configuración del par ya existe, es sustituida por la configuración especificada.|
|g11n-pipeline.config-translation.delete|Suprime la configuración de traducción para el par de idiomas especificado.|


## Lista de sucesos: sucesos de instancia
{: #gpevents_instance}

En la tabla siguiente, se enumeran las acciones que están relacionadas con instancias y generan un suceso:

|Acción|Descripción|
|---|---|  
|g11n-pipeline.instance.read|Obtiene la información de esta instancia de servicio de traducción.|


## Dónde buscar los sucesos
{: #gp_at_ui}

Los sucesos de {{site.data.keyword.cloudaccesstrailshort}} están disponibles en el **dominio de espacio** de {{site.data.keyword.cloudaccesstrailshort}} que está disponible en la región de {{site.data.keyword.Bluemix_notm}} en la que se suministra el servicio de {{site.data.keyword.GlobalizationPipeline_short}}. La instancia de servicio de {{site.data.keyword.cloudaccesstrailshort}} y la instancia de {{site.data.keyword.GlobalizationPipeline_short}} se deben suministrar en el mismo espacio de CF.

Para instancias de RC de {{site.data.keyword.GlobalizationPipeline_short}}, los sucesos de Activity Tracker están disponibles en el dominio de **cuenta** de Activity Tracker en el que se generan los sucesos en la región de {{site.data.keyword.Bluemix_notm}}.
