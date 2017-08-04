---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"

  ---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen:.screen}
{:codeblock:.codeblock}

# Creación de un paquete
{: #createbundles}

Para empezar con la traducción, cree paquetes y cargue archivos de recursos de su app que tenga que traducir {{site.data.keyword.GlobalizationPipeline_short}}. Los archivos de recursos pueden ser archivos Properties de Java, AMD I18N o JSON y deben tener contenido en la forma de pares clave/valor que representen las series de interfaz de usuario de la app. Para obtener más detalles y ejemplos de tipos de archivos soportados, consulte [Cómo trabajar con paquetes](./bundles.html){: new_window}.

Para crear un paquete, siga estos pasos:

<ol>
<li>En el separador <strong>Visión general</strong>, pulse <strong>Nuevo paquete</strong>.</li>

<li>Proporcione información sobre el paquete:<table>
<thead>
<tr>
<th>Campo</th>
<th>Obligatorio</th>
<th>Descripción</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>ID del paquete</strong></td>
<td>Sí</td>
<td>Un nombre exclusivo para identificar el paquete.</td>
</tr>
<tr>
<td><strong>Idioma de origen</strong></td>
<td>Sí</td>
<td>El idioma nativo del archivo de origen.</td>
</tr>
<tr>
<td><strong>Archivo de recursos</strong></td>
<td>No</td>
<td>Un <a href=https://new-console.stage1.ng.bluemix.net/docs/services/GlobalizationPipeline/bundles.html>archivo de recursos</a> que se traducirá. El tamaño de archivo máximo está limitado a 2 MB. Los archivos de recursos especificados se subirán.</td>
</tr>
<tr>
<td><strong>Formato de archivo</strong></td>
<td>No</td>
<td>El tipo de archivo que se está cargando.</td>
</tr>
<tr>
<td><strong>Idioma de destino</strong></td>
<td>No</td>
<td>Los idiomas para los que desea traducciones.</td>
</tr>
</tbody>
</table>

<p><strong>Nota:</strong> Para cambiar el servicio de idiomas que proporciona la traducción automática para los paquetes, pulse el separador <a href=https://new-console.stage1.ng.bluemix.net/docs/services/GlobalizationPipeline/managing_translations.html#globalizationpipeline_service_to_service>Configuración de MT</a> para ver otros motores de traducción automática soportados.</p></li>

<li>Pulse <strong>guardar</strong></li></ol>


Una vez que se haya creado el paquete, el archivo de recursos subido se traducirá a todos los idiomas de destino que haya especificado. El paquete nuevo se añade al separador Paquetes, donde puede:

* Añadir o eliminar idiomas
* Editar las traducciones generadas
* Actualizar el archivo de origen utilizado en el paquete y volver a generar las traducciones
