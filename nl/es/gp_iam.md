---

copyright:
  years:  2015, 2019
lastupdated: "2019-03-25"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:codeblock: .codeblock}
{:tip: .tip}
{:download: .download}


# IBM Cloud IAM para {{site.data.keyword.GlobalizationPipeline_short}}
{: #gp_iam}

## Acceso
{: #gp_iam_access}
El acceso a las instancias de servicio habilitadas para {{site.data.keyword.GlobalizationPipeline_short}} RC para los usuarios de la cuenta se controla por medio de {{site.data.keyword.Bluemix_notm}} Identity and Access Management (IAM) y/o la autenticación de {{site.data.keyword.GlobalizationPipeline_short}}. Sin embargo, para las instancias de CF solo se puede utilizar la autenticación de {{site.data.keyword.GlobalizationPipeline_short}}.

## Autenticación de {{site.data.keyword.GlobalizationPipeline_short}}
{: #gp_iam_ca}
Para utilizar el mecanismo de autenticación, consulte [Añadir usuarios de la API](/docs/services/GlobalizationPipeline/managetranslations.html#adduser).


## Identity Access Management (IAM)
{: #gp_iam_ovw}
Todos los usuarios que acceden al servicio de {{site.data.keyword.GlobalizationPipeline_short}} en su cuenta deben tener asignada una política de acceso con un rol de usuario IAM definido. Esta política determina qué acciones puede realizar el usuario dentro del contexto del servicio o instancia que seleccione. Las acciones permitidas se personalizan y definen mediante el servicio {{site.data.keyword.Bluemix_notm}} como operaciones que se permiten que se realicen en el servicio. A continuación, las acciones se correlacionan con los roles de usuario de IAM.

Las políticas permiten otorgar el acceso en distintos niveles. Algunas de las opciones son las siguientes:

* Acceso a todas las instancias del servicio de su cuenta
* Acceso a una instancia de servicio individual de su cuenta
* Acceso a un recurso específico dentro de una instancia
* Acceso a todos los servicios habilitados para IAM de su cuenta

Después de definir el ámbito de la política de acceso, debe asignar un rol. En la tabla siguiente se detallan las acciones que se correlacionan con los roles de acceso al servicio. Los roles de acceso al servicio habilitan el acceso de usuario a {{site.data.keyword.GlobalizationPipeline_short}}, así como la capacidad de llamar a la API de {{site.data.keyword.GlobalizationPipeline_short}}.

| **Tipo de rol** | **Ver traducciones** | **Editar traducciones** | **Modificar información de paquete** | **Crear solicitudes de traducción profesional** | **Ver solicitudes de traducción profesional** |
|---------------|-----------------------|-----------------------|-------------------------------|----------------------------------------------|--------------------------------------------|
| Lector        | Sí | No | No | No | No |
| Escritor        | Sí | Sí | No | No | Sí |
| Gestor       | Sí | Sí | Sí | Sí | Sí |
{: caption="Tabla 1. Roles de usuario y acciones de IAM" caption-side="top"}

Actualmente, a los usuarios de IAM se les otorga a nivel de instancia de servicio, y no se les puede permitir ni denegar el acceso a nivel de paquete. Para aplicar un control preciso, utilice la autenticación de {{site.data.keyword.GlobalizationPipeline_short}}.

Para obtener información sobre la asignación de roles de usuario en la interfaz de usuario, consulte [Gestión del acceso de IAM](/docs/iam/iammanidaccser.html#iammanidaccser).

### Generación de llamadas de API
{: #gp_iam_apicalls}

Para generar u obtener las credenciales de servicio, siga estos pasos.
1. Inicie sesión en la cuenta de {{site.data.keyword.Bluemix}} en el [panel de control de {{site.data.keyword.Bluemix}}](https://cloud.ibm.com/).
2. Pulse la instancia de servicio en el [panel de control de {{site.data.keyword.Bluemix}}](https://cloud.ibm.com/).
3. Pulse **Credenciales de servicio** para abrir la instancia de servicio. 
4. Pulse **Nueva credencial** para seguir la solicitud para crear nuevas credenciales.
5. Pulse **Ver credenciales** después de crear la credencial.
![La captura de pantalla muestra información sobre una clave de API de ejemplo](images/gp_iam_apicalls.gif)

A continuación, se muestran ejemplos de llamada de API de {{site.data.keyword.GlobalizationPipeline_short}} mediante la autenticación de IAM.

* Mediante señal portadora de IAM
```
curl -X GET \
  https://gp-rest.us-south.g11n-pipeline.test.cloud.ibm.com/translate/rest/50341556337c581c208188ff8908ebc7/v2/bundles \
  -H 'Authorization: Bearer eyJjsksd…w'
```

* Mediante clave de API
```
curl -X GET \
  https://gp-rest.us-south.g11n-pipeline.test.cloud.ibm.com/translate/rest/50341556337c581c208188ff8908ebc7/v2/bundles \
  -H 'Authorization: API-KEY MklfrP…ACem'
```
En el ejemplo anterior, puede obtener la información siguiente:
* “50341556337c581c208188ff8908ebc7” es el ID de instancia (de la sección de credenciales)
* “https://gp-rest.us-south.g11n-pipeline.test.cloud.ibm.com/translate/rest” es el url (de la sección de credenciales)
* “MklfrP…ACem” es la clave de API (de la sección de credenciales)
* “eyJjsksd…w” es la señal portadora de IAM

Para obtener instrucciones para obtener la señal portadora de IAM de la clave de API, consulte [Obtención de una señal de {{site.data.keyword.Bluemix_notm}} IAM mediante una clave de API](/docs/iam?topic=iam-iamtoken_from_apikey#iamtoken_from_apikey).
