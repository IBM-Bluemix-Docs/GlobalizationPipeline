---

copyright:
  years: 2015, 2018
lastupdated: "2017-06-16"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}


# Cómo trabajar con paquetes
{: #globalizationpipeline_workingwithbundles}

Cada paquete que cree contiene los pares clave valor del archivo de recursos y el conjunto completo de traducciones que se han generado.
{:shortdesc}

Los archivos de recursos que suba pueden ser de cualquiera de los formatos siguientes y deben tener contenido en el formato de pares clave/valor que representan las series de interfaz de usuario de la app.


* Tipo de archivo: *archivos Properties de Java™ (.properties)*<br>
Ejemplo:
```js
logout=Logout
back=Back
examples=Menu
home=Home
web=Web
enterprise=Enterprise
extra=Resources
about=About
settings=Settings
help=Help
support=Support
topics=Topics
appExitMsg=Are you sure you want to quit the application?
```
* Tipo de archivo: *AMD I18N (.js)*<br>
Ejemplo:
```js
define({
    "root": {
       logout: "Logout",
       back: "Back",
       examples: "Menu",
       home: "Home",
       web: "Web",
       enterprise: "Enterprise",
       extra: "Resources",
       about: "About",
       settings: "Settings",
       help: "Help",
       support: "Support",
       topics: "Topics",
       appExitMsg: "Are you sure you want to quit the application?"
    }
});
```
* Tipo de archivo: *JSON (.json)*<br>
Ejemplo:
```js
{
  "logout": "Logout",
  "back": "Back",
  "examples": "Menu",
  "home": "Home",
  "web": "Web",
  "enterprise": "Enterprise",
  "extra": "Resources",
  "about": "About",
  "settings": "Settings",
  "help": "Help",
  "support": "Support",
  "topics": "Topics",
  "appExitMsg": "Are you sure you want to quit the application?"
}
```

Además, un archivo de recursos también se debe ajustar a estas directrices:
* Cada clave puede tener un máximo de 1023 caracteres.
* Cada valor puede tener un máximo de 8191 caracteres.
* Cada paquete puede tener un máximo de 1000 pares clave/valor.

A medida que cree paquetes, estos se irán añadiendo al separador **Paquetes**, donde puede realizar tareas adicionales como la adición o la supresión de idiomas, la visualización del contenido traducido y la realización de pequeñas ediciones en el contenido traducido. 

{{site.data.keyword.GlobalizationPipeline_short}} traduce el contenido del paquete en los idiomas con el motor de traducción de automática predeterminado. Opcionalmente, puede elegir un motor de traducción automática alternativo tal como se describe en la sección [Configuración de la traducción automática](/docs/services/GlobalizationPipeline/managetranslations.html#machineconfig). El motor predeterminado da soporte a los siguientes idiomas de destino:

<table>
<thead>
<tr>
<th>Idiomas de destino</th>
</tr>
</thead>
<tbody>
<tr>
<td>Chino (simplificado)</td>
</tr>
<tr>
<td>Chino (tradicional)</td>
</tr>
<tr>
<td>Francés</td>
</tr>
<tr>
<td>Alemán</td>
</tr>
<tr>
<td>Italiano</td>
</tr>
<tr>
<td>Japonés</td>
</tr>
<tr>
<td>Coreano</td>
</tr>
<tr>
<td>Portugués (de Brasil)</td>
</tr>
<tr>
<td>Español</td>
</tr>
</tbody>
</table>

**Nota:** El motor de traducción automática predeterminado de {{site.data.keyword.GlobalizationPipeline_short}} solo proporciona soporte para inglés como idioma de origen. Sin embargo, los motores de traducción automática alternativos disponibles para configurar dentro de {{site.data.keyword.GlobalizationPipeline_short}} dan soporte a la traducción de otras combinaciones de idiomas distintas del inglés.

Una vez que haya traducido el contenido del paquete con la traducción automática, puede realizar pequeñas ediciones dentro de {{site.data.keyword.GlobalizationPipeline_short}} o puede enviar paquetes para que los revisen y editen traductores profesionales. Para obtener detalles sobre el envío de una solicitud para su revisión y edición por parte de personas, consulte [Creación de solicitud de traducción humana cargable](/docs/services/GlobalizationPipeline/managetranslations.html#humantranslation).




## Selección de un paquete con el que trabajar
{: #globalizationpipeline_selectingabundle}

1. Pulse el separador **Paquetes** para ver todos los paquetes que ha creado.
2. Pulse un **ID de paquete** de la lista para ver más detalles acerca de dicho paquete, o pulse el icono **Ver el detalle de paquetes** ![Seleccione el icono Ver el detalle de paquetes para abrir un paquete y trabajar con sus traducciones](images/viewProjectDetailIcon.png) en la columna Acciones.

![Ver todos los paquetes disponibles desde el separador Paquetes.](images/translationBundles.png)

Después de seleccionar un paquete con el que trabajar, puede ver el estado de sus traducciones, añadir o eliminar idiomas, editar las traducciones o proporcionar actualizaciones para el archivo de recursos.

Si ya no necesita un paquete, puede suprimirlo desde el separador **Paquetes**. Todas las traducciones asociadas con el paquete también se suprimirán.
