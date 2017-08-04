---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"

  ---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# Configuración de la traducción automática
{: #machineconfig}

{{site.data.keyword.GlobalizationPipeline_full}} da soporte a la posibilidad de integrar servicios de traducción automática alternativos para realizar la traducción automática de los paquetes. La adición de un servicio alternativo puede resultar beneficioso si el motor predeterminado utilizado por {{site.data.keyword.GlobalizationPipeline_short}} no ofrece un idioma específico que necesite o si prefiere las traducciones automáticas generadas por otro motor. El uso y los cargos para servicios alternativos están cubiertos bajo los términos de dichos servicios.

Para añadir y configurar un servicio de traducción automática alternativo para {{site.data.keyword.GlobalizationPipeline_short}}, seleccione el separador **Configuración de traducción automática** desde el panel de control {{site.data.keyword.GlobalizationPipeline_short}}.

* Para añadir un servicio de traducción automática que se encuentre en el catálogo de {{site.data.keyword.Bluemix_notm}}, (**Watson Language Translator**), el servicio debe añadirse en primer lugar al espacio de {{site.data.keyword.Bluemix_notm}}.

* Para añadir un servicio de terceros, seleccione el botón para dicho servicio en el separador **Configuración de traducción automática** y proporcione las credenciales de usuario necesarias para acceder al servicio.

Una vez que se haya añadido un servicio de traducción automática a {{site.data.keyword.GlobalizationPipeline_short}}, complete el resto de los pasos para completar la integración de dicho servicio.

1. Pulse **Habilitar** para activar la integración con dicho servicio.

2. Pulse **Actualizar idiomas** para ver la lista actualizada de idiomas de destino soportados.

3. En la lista de idiomas de destino, seleccione el motor de traducción automática que debe realizar la traducción.

4. Pulse **Guardar** para volver al separador **Configuración de traducción automática**.

Una vez que se haya configurado un servicio alternativo con {{site.data.keyword.GlobalizationPipeline_short}}, todos los idiomas de destino que se hayan asignado a dicho motor comenzarán a generarse utilizando dicho motor. 

Para dejar de utilizar un motor de traducción automática alternativo:

1. En el separador **Configuración de traducción automática**, pulse el botón **Inhabilitar** para el servicio que desea dejar de utilizar.

Una vez que esté inhabilitado un servicio de traducción automática alternativo, todas las traducciones generadas por el servicio permanecerán dentro de los paquetes. Sin embargo, la traducción a un determinado idioma de destino puede no estar disponible para futuras actualizaciones si el idioma de destino ya no está soportado por el motor de traducción automática que está habilitado actualmente.

<!-- Review comment: When you disable an engine, do you need to go back and reconfigure the languages?? Does it go back to the default engine? What happens? -->
