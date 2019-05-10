---

copyright:
  years: 2018, 2019
lastupdated: "2019-03-22"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:codeblock: .codeblock}
{:tip: .tip}
{:download: .download}


# Alta disponibilidad y recuperación tras desastre
{: #ha-dr}

El servicio {{site.data.keyword.GlobalizationPipeline_full}} es de alta disponibilidad en la ubicación de {{site.data.keyword.Bluemix}} (Dallas, Sídney, Londres y Frankfurt). 
{: shortdesc}

## Alta disponibilidad

El servicio {{site.data.keyword.GlobalizationPipeline_full}} admite la alta disponibilidad. El servicio consigue una alta disponibilidad de forma automática y transparente mediante el equilibrador de carga delante para distribuir solicitudes a los pods en el controlador de réplicas.

## Recuperación tras desastre

La recuperación tras desastre puede convertirse en un problema si una ubicación de {{site.data.keyword.Bluemix}} sufre un fallo significativo que incluye la pérdida potencial de datos. Debido a que la región multizona (MZR) no está disponible en las ubicaciones, debe esperar a que IBM vuelva a poner una ubicación en línea si no está disponible. Si los servicios de datos subyacentes se ven afectados por el fallo, también debe esperar a que IBM restaure estos servicios de datos para recuperar datos de copias de seguridad de base de datos.

Consulte [¿Cómo puedo asegurar un tiempo de inactividad cero?](/docs/overview?topic=overview-zero-downtime#zero-downtime) para obtener más información sobre los estándares de alta disponibilidad y de recuperación tras desastre en {{site.data.keyword.Bluemix_notm}}. También puede encontrar información sobre [Acuerdos de nivel de servicio](/docs/overview?topic=overview-zero-downtime#SLAs).  














