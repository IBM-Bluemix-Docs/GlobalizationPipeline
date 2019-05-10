---

copyright:
  years: 2015, 2018
lastupdated: "2017-06-21"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# Gestión de traducciones
{: #managetranslations}


Una vez que haya creado paquetes y que haya comenzado a generar traducciones para la aplicación, puede elegir entre traducción automática y traducción humana. El contenido generado automáticamente se puede utilizar tal cual o se puede modificar. También puede elegir si desea utilizar una traducción automática que no sea la predeterminada. Esta sección cubre instrucciones para las tareas siguientes:
<ul>
<li>¿Cómo se modifica el motor de traducción automática que realiza las traducciones para sus paquetes?</li>
<li>¿Cómo se realiza la edición humana posterior a la traducción?</li>
<li>¿Cómo se crea la solicitud de traducción humana?</li>
<li>¿Cómo se asignan roles de usuario y restricciones de acceso a las personas que necesitarán acceso a sus traducciones?</li>
</ul>

**Nota**: Para un usuario de plan estándar, si desea crear una solicitud de traducción humana, puede cambiar al plan profesional. Aún puede ver sus datos de solicitud de traducción humana dentro de un plan estándar, pero la solicitud de traducción humana sólo está disponible para los usuarios del plan profesional.

## Configuración de la traducción automática
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

## Visualización y edición de traducciones
{: #edittranslations}

El servicio de {{site.data.keyword.GlobalizationPipeline_short}} proporciona posibilidades de edición humana posterior a la traducción. Puede editar para mejorar la calidad o la coherencia de la traducción o para sustituir el texto preferido. Por ejemplo, es posible que desee sobrescribir la traducción de un nombre de producto.

Para ver y editar las traducciones para un idioma de destino:

1. En la página **Detalles del paquete**, seleccione un idioma de destino o pulse el icono **Ver las traducciones** ![Seleccione el icono Ver traducciones para ver las traducciones de un idioma de destino](images/viewProjectDetailIcon.png) desde la columna Acciones.
2. Las traducciones se presentan en una tabla que muestra la información de clave, origen y traducción.
 * **Clave:** Representa un atributo del archivo de recursos que tiene un valor asociado.
 * **Origen:** Representa una serie traducible que se ha incluido en el archivo de recursos subido.
 * **Traducción:** Representa la versión traducida de un valor de origen.
3. En la columna Acciones, pulse el icono **Modificar la traducción** ![Seleccione el icono Modificar la traducción para editar las traducciones de un par de clave/valor concreto.](images/editIcon.png) para editar un valor traducible automáticamente.
4. Edite la traducción y pulse **Actualizar** para actualizar el valor traducido original con la edición.

![La ventana de diálogo Modificar traducción proporciona una manera sencilla de editar traducciones.](images/editTranslation.png)

***Consejo:***
1. Cuando trabaje con paquetes grandes que incluyan muchas claves traducibles, encontrar un valor determinado puede ser complicado. En la página de traducción de idioma de destino, puede buscar rápidamente en todas las claves, el origen y las traducciones utilizando el recuadro **Buscar...**.
![Utilice el recuadro de búsqueda para buscar las claves, el origen, las traducciones o los tres dentro de un idioma de destino.](images/search.png)

2. El panel de control de {{site.data.keyword.GlobalizationPipeline_short}} proporciona la función de filtro de serie para que seleccione qué tipo de series se mostrará cuando desee ver detalles del paquete. Pulse en el separador **Mostrar todas las series** predeterminado, y podrá elegir entre mostrar todas las series, sólo las series revisadas, o sólo las series no revisadas.
![Utilice la función de filtro de series para elegir entre mostrar todas las series, sólo las series revisadas, o sólo las series no revisadas.](images/stringfilter.png)

## Creación de solicitudes de traducción humana facturables
{: #humantranslation}

Cuando se requiere calidad, puede que desee contratar a traductores profesionales para revisar su traducción automática. Por un cargo adicional en el plan profesional de {{site.data.keyword.GlobalizationPipeline_short}}, puede enviar los paquetes traducidos automáticamente para su revisión y edición humana. Para ello, cambie del plan estándar al plan profesional, cree una solicitud de traducción humana y envíe los paquetes de destino a los servicios de traducción profesional de IBM. Puede utilizar esta capacidad para afinar más la calidad y la coherencia de sus traducciones. Los idiomas disponibles para la revisión y edición humana son los mismos que los idiomas soportados por los motores de traducción automática disponibles mediante {{site.data.keyword.GlobalizationPipeline_short}}.


Para crear una solicitud de traducción, realice los pasos siguientes:

1. Cambie **al plan profesional de {{site.data.keyword.GlobalizationPipeline_short}}**.

2. Pulse el separador **Solicitud de traducción** en el panel de control, y pulse **Nueva solicitud**.

3. Seleccione el paquete de destino y los idiomas de destino para su traducción.

4. Compruebe el ID del paquete, los idiomas de destino y el recuento de palabras de origen para su traducción.

5. Proporcione la información necesaria sobre la solicitud. Los campos marcados con asteriscos deben rellenarse.

6. Confirme y envíe la solicitud.

**Nota**: Se recomienda encarecidamente que se proporcione contexto adicional para el contenido de la traducción en el campo **Instrucción especial** durante el paso 5. Esto puede ayudar a los traductores humanos a comprender mejor el contenido y a entregar un resultado de traducción de calidad.
![Se recomienda encarecidamente proporcionar suficiente contexto adicional en el campo Instrucción especial.](images/specialinstruction.png)

Puede ver todas las solicitudes de traducción y realizar el seguimiento del estado desde el panel de control.
![Interfaz de usuario de solicitud de traducción de muestra para su referencia.](images/translationrequest.png)

**Nota**: Hay 5 estados para cada solicitud de traducción. Puede hacer referencia a la tabla siguiente para que le ayude a realizar el seguimiento del estado de su solicitud de traducción.

| Estado | Notificación por correo electrónico | Explicación de estado |
|--------|--------------------|--------------------|
| Borrador  | No | La solicitud de traducción se ha creado pero todavía no se ha enviado. Puede modificar todavía el contenido de la solicitud de traducción o suprimir la misma. |
| Enviado | Sí | La solicitud de traducción se ha enviado, y no puede modificar el contenido de la misma. |
| Edición iniciada | Sí | Se ha iniciado el trabajo posterior a la edición humana de la solicitud de traducción. |
| Edición finalizada | Sí | Ha finalizado el trabajo posterior a la edición humana de la solicitud de traducción. Tiene que esperar aún a que se vuelvan a fusionar las series traducidas con las series de recursos maestros. |
| Fusionado | Sí | El resultado posterior a la edición humana se ha vuelto a fusionar. Ha finalizado la solicitud de traducción. Puede generar un informe en este momento. Puede guardar la solicitud de traducción para su referencia futura, o suprimirla para ahorrar espacio de almacenamiento. La supresión de la solicitud de traducción no afectará al resultado de traducción fusionado. |

Para ver el detalle de la solicitud de traducción, pulse el icono **Ver el detalle de la solicitud** ![Seleccione el icono Ver el detalle de la solicitud para ver las traducciones del idioma de destino](images/viewProjectDetailIcon.png) desde la columna **Acciones**.

![Ver los detalles de la solicitud de traducción](images/viewtr.png)

Para generar un informe *JSON (.json)* o XLIFF para su solicitud, pulse el botón **Descargar informe** o **Descargar XLIFF**.



## Añadir usuarios de la API
{: #adduser}

A medida que gestione las traducciones, es posible que desee otorgar acceso a usuarios de API adicionales basándose en las tareas que tiene que llevar a cabo. Por ejemplo, puede que desee habilitar a un traductor para editar la traducción, pero no podrá modificar la información del paquete.

| **Tipo de rol** | **Ver traducciones** | **Editar traducciones** | **Modificar información de paquete** | **Crear solicitudes de traducción profesional** | **Ver solicitudes de traducción profesional** |
|-----------|--------------------|--------------------|----------------------------|
| Lector    | Sí | No | No | No | No |
| Traductor | Sí | Sí | No | No | Sí |
| Administrador | Sí | Sí | Sí | Sí | Sí |

Si crea más usuarios de API, puede restringir su acceso para uno o varios paquetes específicos, u otorgarles acceso a todos los paquetes disponibles mediante la autenticación de {{site.data.keyword.GlobalizationPipeline_short}}.

Para otorgar a un usuario de API acceso a paquetes en una instancia de servicio de {{site.data.keyword.GlobalizationPipeline_short}}:

1. En el panel de control de {{site.data.keyword.GlobalizationPipeline_short}}, pulse el separador **Usuarios de API**.
2. Pulse **Nuevo usuario de API**.
3. Escriba un **nombre de visualización** y un **comentario** para describir el nuevo usuario de API.
4. Elija un **tipo** para el nuevo usuario de API.
5. Elija para dar acceso al usuario de API a todos los paquetes o solo a los paquetes seleccionados.
6. Pulse **Guardar**.

![Complete el foro para crear un nuevo usuario de API.](images/newUser.png)

Se generarán y se visualizarán un ID de usuario y una contraseña de API. Copie y guarde las credenciales; después de cerrar la ventana, no podrá acceder a ellas de nuevo. Las credenciales se pueden utilizar para el servicio RESTful a través de [SDK](https://github.com/IBM-Bluemix/gp-common).

Para restablecer la contraseña del usuario de la API:

1. En el panel de control de {{site.data.keyword.GlobalizationPipeline_short}}, pulse el separador **Usuarios de API**.
2. Pulse el icono **Restablecer contraseña** ![Seleccione este icono para restablecer la contraseña de usuarios de API](images/resetPW.png) para restablecer la contraseña para un ID de usuario específico.
3. Pulse **Sí**.
