---

copyright:
  years: 2015, 2019
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


# Migración de instancias de servicio de {{site.data.keyword.GlobalizationPipeline_short}} a un grupo de recursos
{: #rg-migration}

Los usuarios actuales de instancias de CF de {{site.data.keyword.GlobalizationPipeline_short}} disponen de 3 meses (a partir de la fecha de disponibilidad en producción de la versión RC/IAM) para migrar a una versión del servicio que sea compatible con RC/IAM.


## Antes de empezar
{: #prereqs}

Antes de empezar a migrar las instancias de servicio de {{site.data.keyword.GlobalizationPipeline_short}}, debe saber que se conservan todos los datos de la instancia de servicio. No se pierde nada. Tras la migración, se ven las instancias de servicio en el mismo estado que antes de la migración.   

Para ver una descripción general del proceso de migración, consulte [Migración de instancias de servicio de Cloud Foundry a un grupo de recursos](/docs/resources/instance_migration.html). 

## Pasos para realizar la migración
{: #gp_steps_migration}

1. Abra el menú **Más acciones**.
2. Seleccione **Migrar** a un grupo de recursos para empezar.
3. Seleccione un grupo de recursos.
4. Pulse **Migrar** y la instancia se migrará.

**Nota:** Solo se puede migrar las instancias de una en una, de modo que puede seguir migrando instancias una vez que haya migrado correctamente la primera.

## Pasos siguientes
{: #nextsteps}

Puede ver las instancias de servicio migradas en la sección **Servicios** de la lista de recursos. El alias permanece en la sección de Cloud Foundry de la lista de recursos. Se trata de una migración in situ, de modo que se conservan todos los datos de instancia y las credenciales. Puede seguir utilizando las credenciales generadas por la instancia de CF original. 

Para obtener más información sobre el funcionamiento de la migración, consulte [Cómo funciona la migración](/docs/resources/instance_migration.html#how).


