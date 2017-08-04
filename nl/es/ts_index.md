---

copyright:
  years: 2015, 2017
lastupdated: "2017-07-19"

  ---

{:tsSymptoms: .tsSymptoms} 
{:tsCauses: .tsCauses} 
{:tsResolve: .tsResolve} 
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Resolución de problemas de {{site.data.keyword.GlobalizationPipeline_short}}
{: #globalizationpipelinets}

A continuación se muestran algunas respuestas a preguntas comunes sobre cómo utilizar {{site.data.keyword.GlobalizationPipeline_full}}.
{:shortdesc}


## El nombre de mi app no se ha traducido correctamente
{: #problem1}

Las traducciones generadas de determinadas series no era lo que se esperaba.
{:shortdesc}

Cuando se traduce un archivo de recursos, es posible que no se traduzcan correctamente las series que contienen nombres de producto u otros nombres propios.
{: tsSymptoms}

A menudo, los nombres de productos o los nombres propios no se traducen correctamente en otros idiomas, especialmente si el nombre contiene palabras reales. Cuando se traducen estos tipos de palabras y frases, en función del significado de dichas palabras en un idioma específico, el texto traducido puede tener un significado distinto del nombre en inglés.
{: tsCauses}

Pruebe la traducción de nombres de producto antes de utilizarlos y, si encuentra problemas, modifique el texto o la traducción en consonancia. Para obtener consejos de estilo de escritura al utilizar la traducción automática, consulte [Consejos de traducción automática](./tips.html#globalizationpipeline_tips).
{: tsResolve}



## No puedo subir un archivo de recursos
{: #problem2}

El archivo de recursos que estoy intentando subir no está aceptado.
{:shortdesc}

Al añadir un archivo de recursos a un nuevo paquete de traducción o al actualizar un archivo de recursos existente para que se traduzca, recibo un error.
{: tsSymptoms}

{{site.data.keyword.GlobalizationPipeline_short}} solo acepta archivos de recursos de los siguientes tipos: .properties de Java™, JSON y AMD I18N.
{: tsCauses}

Asegúrese de que el archivo de recursos que se está subiendo sea de uno de estos tipos.
{: tsResolve}
* .properties de Java
* JSON
* AMD I18N



## No puedo subir mi archivo de recursos porque es demasiado grande
{: #problem3}

El archivo de recursos que estoy intentando subir no está aceptado.
{:shortdesc}

Al añadir o actualizar un archivo de recursos a un proyecto de traducción, se produce un error porque una parte del archivo es demasiado grande.
{: tsSymptoms}

{{site.data.keyword.GlobalizationPipeline_short}} solo puede aceptar archivos de recursos que cumplen determinados requisitos de tamaño.
{: tsCauses}

Asegúrese de que el archivo de recursos se ajusta a las directrices siguientes:
{: tsResolve}
* Cada clave puede tener un máximo de 256 caracteres.
* Cada valor puede tener un máximo de 2048 caracteres.
* Cada proyecto de traducción puede contener un máximo de 500 pares clave/valor.
* Un archivo de recursos no puede ser mayor de 2 MB.



## El espaciado alrededor de las variables contenido en las series no es coherente
{: #problem5}

El espaciado que se utiliza alrededor de las variables después de la traducción no es siempre el mismo.
{:shortdesc}

El espaciado que se utiliza alrededor de las variables que se encuentran dentro de las series no es siempre coherente de un idioma a otro tras la traducción.
{: tsSymptoms}

Los motores de traducción automática están diseñados para funcionar con idioma natural y es posible que no siempre reconozcan o sepan cómo manejar sintaxis específica utilizada por los lenguajes de programación. Como resultado, puede variar el manejo de sintaxis que está mezclada con texto sin formato.
{: tsCauses}

{{site.data.keyword.GlobalizationPipeline_short}} actualmente reconoce el patrón "{}" que normalmente se utiliza para representar variables y conservará el formato original del contenido.
{: tsResolve}
