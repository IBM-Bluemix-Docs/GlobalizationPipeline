---

copyright:
  years: 2015, 2018
lastupdated: "2017-12-13"


---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}


# Iniciación a {{site.data.keyword.GlobalizationPipeline_short}}
{: #globalizationpipeline}

{{site.data.keyword.GlobalizationPipeline_full}} es un servicio de {{site.data.keyword.Bluemix}} que permite a los desarrolladores de la app lanzar rápidamente aplicaciones traducidas en los clientes globales. {{site.data.keyword.GlobalizationPipeline_short}} sirve como repositorio de traducción para proporcionar traducción automática, revisión y edición humana, y que las API y SDK integren la traducción sin problemas en la infraestructura de DevOps y de Desarrollo continuo, eliminando las operaciones manuales y compartimentadas asociadas con el proceso de traducción tradicional.
{:shortdesc}

Puede utilizar el servicio {{site.data.keyword.GlobalizationPipeline_short}} para traducir cualquier app desplegada y alojada en {{site.data.keyword.Bluemix_notm}}, o desenlazar para traducir apps alojadas en otras plataformas en la nube.

{{site.data.keyword.GlobalizationPipeline_short}} ofrece una interfaz de panel de control para gestionar la traducción de su app y una API RESTful que automatiza completamente el proceso de traducción. Para obtener información sobre la API de {{site.data.keyword.GlobalizationPipeline_short}}, consulte [Referencia de la API](https://gp-rest.ng.bluemix.net/translate/swagger/index.html){: new_window}.

## Elección de un plan de traducción
{: #globalizationpipeline_chooseplan}

Antes de empezar a trabajar con la traducción en {{site.data.keyword.GlobalizationPipeline_short}}, puede elegir un plan de traducción adecuado.

Hay dos planes de traducción disponibles en {{site.data.keyword.GlobalizationPipeline_short}}: el plan estándar y el plan profesional. Estos planes proporcionan traducción automática básica ilimitada integrada, así como la capacidad de integrarse con otros motores de traducción automática por un precio adicional. En el plan profesional, {{site.data.keyword.GlobalizationPipeline_short}} ofrece de forma adicional un servicio de edición y de revisión de traducción profesional. Puede conmutar entre los planes de {{site.data.keyword.GlobalizationPipeline_short}} dentro de {{site.data.keyword.Bluemix_notm}} con todos los datos reservados.


## Estimación de uso de datos de {{site.data.keyword.GlobalizationPipeline_short}}
{: #globalizationpipeline_documentpricing}

{{site.data.keyword.GlobalizationPipeline_short}} almacena sus traducciones en una base de datos de fondo. Para calcular el tamaño de datos activo, puede hacer referencia a la fórmula siguiente:

`<expected resource data storage size in MB> ˜= 0.0005 * <number of key/value pairs in the source resource> * <number of languages including the source language>`

Según la fórmula, el tamaño de un paquete típico es `(longitud de clave + longitud del valor en UTF-8 = ˜40 bytes)`.

Por ejemplo, si tiene 100 pares clave/valor y los traduce a 9 idiomas, el tamaño de almacenamiento estimado es 0,0005 100 (9+1) = 0,5 MB. El tamaño real puede diferir en función del tamaño real de la clave/valor y de los metadatos almacenados junto con la traducción.

Utilice la [calculadora de tarifas](https://console.ng.bluemix.net/?direct=classic/#/pricing/cloudOEPaneId=pricing&paneId=pricingSheet&orgGuid=127a45f4-4461-4d5b-a26b-6dc2fdd1a3a2&spaceGuid=208fb1ff-413b-4fd9-9615-e8226062d0f3) de {{site.data.keyword.Bluemix_notm}} para determinar los costes de servicio mensuales.

**Nota**: El uso de la característica de revisión del plan profesional aumentará el uso de datos más allá de lo indicado anteriormente.
