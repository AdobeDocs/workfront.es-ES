---
content-type: api
navigation-topic: general-api
title: Campos de texto enriquecido en la API de Adobe Workfront
description: Campos de texto enriquecido en la API de Adobe Workfront
author: John
feature: Workfront API
exl-id: 67fc34dc-0722-4419-8254-0371ad5abfc3
source-git-commit: 40698643b0fa530b38da465f3bc1e4d841fcc190
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---


# Campos de texto enriquecido en la API de Adobe Workfront

Algunos objetos de Adobe Workfront permiten el almacenamiento de texto con formato de texto enriquecido. En la API de Workfront, el texto enriquecido se almacena como JSON utilizando el marco de código abierto Draft.js.

## Ejemplo de información general

Un campo personalizado con formato de texto enriquecido se llama **Campo con texto enriquecido** y puede tener asociados los siguientes valores:

![](assets/rich-text-example-350x158.png)

**Ejemplo:** Una solicitud de GET básica para recuperar el valor del campo de formulario personalizado **Campo con texto enriquecido**:

<!-- [Copy](javascript:void(0);) -->
<pre><OBJ Code><OBJ ID><OBJ Code><OBJ ID></pre>

**Ejemplo:** Esta solicitud devolverá el valor de **Campo con texto enriquecido** en JSON almacenada en la variable **parameterValue** **DE:Campo con texto enriquecido**

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

**Ejemplo:** Esta es una versión formateada de la respuesta mostrada en la figura directamente anterior

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

## Bloques

Los objetos JSON que almacenan el contenido de texto enriquecido están compuestos por dos partes principales: **bloques** y **entityMaps**.

Un bloque es un objeto JSON que representa una sola línea de texto con formato. Dado que un solo campo personalizado puede tener más de una línea de texto, cada línea de texto tiene su propio bloque y cada bloque se representa como un elemento en una matriz principal denominada **bloques**.

**Ejemplo:** Aquí, cada línea de texto de un campo personalizado se asigna a un elemento de bloque en los bloques de matriz

![](assets/copy-of-rich-text-mapping-350x159.png)

Dado que cada elemento de bloque también es un objeto JSON, cada bloque está compuesto por los elementos siguientes: **key**, **text**, **type**, **depth**, **inlineStyleRanges**, **entityRanges** y **data**. Cada uno de estos elementos funciona de la siguiente manera:

* **Clave** es el identificador único de ese bloque. La clave se utiliza para asignar una línea de texto mediante entityMaps. Puede encontrar detalles sobre entityMaps en la sección entityMaps de este documento.
* **Texto** es la línea de contenido de texto que se está almacenando desde el campo personalizado.
* **Tipo** describe el tipo de texto que se está representando. Por ejemplo, una línea de texto almacenada en un bloque podría formar parte de una lista. Si esa línea de texto formaba parte de una lista sin ordenar, su tipo se definiría como: unordered-list-item.
* Actualmente no se admiten listas, pero deberían estar disponibles próximamente.
* **Profundidad** Este parámetro define la profundidad de la línea cuando esta es una parte anidada de una lista ordenada o desordenada.
* **inlineStyleRanges** Es una matriz que describe los tipos de formato aplicados a la línea de texto representada por el bloque actual.

**Ejemplo:** Esta es una matriz inlineStyleRanges que describe cada estilo en el nivel de carácter. En este caso: 9 caracteres (longitud: 9) partiendo del índice 0 (offset: 0) tenía el estilo **Negrita** aplicado:

![](assets/copy-of-rich-text-mapping-2-350x136.png)

En el caso de que se hayan aplicado varios tipos de formato a una sola línea, los estilos se asignarán a elementos adicionales de la matriz** inlineStyleRanges**.

**Ejemplo:** Este es el aspecto que tendría un bloque al almacenar una línea de texto que contiene el formato mixto: **Texto en negrita y cursiva**

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

>[!NOTE]
>
>Todas las versiones posteriores a la versión 20.3 admitirán opciones de formato en negrita, cursiva y subrayado.

## entityMaps y entityRanges

Un bloque de datos puede contener potencialmente entidades como hipervínculos u otros tipos de formato estilizado que estén conectados a orígenes de datos ubicados fuera del campo de texto personalizado.

## Ejemplos

### Recuperación de texto sin formato desde JSON

Cuando se envía un campo personalizado con formato de texto enriquecido, todo el texto se almacena en la matriz **bloques**. Sin embargo, cada línea del texto completo se almacena en la variable **parámetro de texto** dentro de cada uno de los elementos de bloque independientes que conforman la matriz principal **bloques**. Por lo tanto, para recuperar el texto completo, cada línea de texto independiente debe extraerse y separarse. Esto se puede lograr montando en bucle todos los elementos de bloques y concatenando cada parámetro de texto junto con un delimitador de línea (\n).

**Ejemplo:** A continuación se indica el aspecto que podría tener el JS:

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

### Guardado de un valor de campo de texto enriquecido mediante la API de Workfront

Para guardar los siguientes valores de un campo de texto enriquecido con la API de Workfront:
<pre>
		Hello <strong>World</strong>¡¡¡¡¡¡¡¡¡¡¡¡¡¡¡¡¡¡¡¡¡¡¡¡!!!!!!
		Esta es mi primera <strong>Texto enriquecido</strong></pre>

1. Construya JSON que represente el valor del campo de texto enriquecido que está intentando capturar organizando cada línea de texto en un elemento de bloque, en la matriz **bloques**

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Capture el formato de texto enriquecido con la variable **inlineStyleRanges** parameter

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Para capturar la segunda línea, el texto &quot;Texto enriquecido&quot; debe tener el formato negrita y cursiva.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

   >[!NOTE]
   >
   >Aunque la funcionalidad entityMap no se admite durante la versión inicial, sigue siendo un campo obligatorio para pasar este JSON en una solicitud

1. Utilice la variable **estringify** método en el JSON descrito anteriormente para hacer un **PUT** solicitar y enviar actualizaciones

   <!-- [Copy](javascript:void(0);) -->
   <pre><OBJ Code><OBJ ID></pre>
