---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos OpenAI (ChatGPT)
description: En un escenario de Adobe Workfront Fusion, puede automatizar los flujos de trabajo que utilizan OpenAIT (ChatGPT), así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
source-git-commit: a8bc882f393dcf17bca80da86c25c053272e27c9
workflow-type: tm+mt
source-wordcount: '1395'
ht-degree: 0%

---

# [!DNL OpenAI (ChatGPT & DALL-E)] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL OpenAI (ChatGPT & DALL-E)], así como conectarlo a múltiples aplicaciones y servicios de terceros.

Si necesita instrucciones sobre cómo crear un escenario, consulte [Creación de un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] o superior</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Para usar [!DNL OpenAI (ChatGPT & DALL-E)] módulos, debe tener un [!DNL OpenAI] Cuenta de, incluida una clave de API y un ID de organización.

## Conectando [!DNL OpenAI (ChatGPT & DALL-E)] hasta [!DNL Workfront Fusion]

Puede crear una conexión con su [!DNL OpenAI (ChatGPT & DALL-E)] cuenta directamente desde dentro de un [!DNL OpenAI (ChatGPT & DALL-E)] módulo.

1. En cualquier [!DNL OpenAI (ChatGPT & DALL-E)] , haga clic en **[!UICONTROL Añadir]** junto al [!UICONTROL Conexión] field.
1. Introduzca la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nombre de conexión]</p> </td> 
      <td> <p>Introduzca un nombre para la nueva conexión.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Clave de API [!UICONTROL]</td> 
      <td>Puede localizar la clave de API en la configuración de usuario de OpenAI.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID de organización] </td> 
      <td>Puede localizar el identificador de su organización en la página Configuración de la organización en OpenAI.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **[!UICONTROL Continuar]** para crear la conexión y volver al módulo.


## [!DNL OpenAI (ChatGPT & DALL-E)] módulos y sus campos

Al configurar [!DNL OpenAI (ChatGPT & DALL-E)] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, se añaden [!DNL OpenAI (ChatGPT & DALL-E)] Los campos pueden mostrarse, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Crear una finalización

Este módulo de acción crea una finalización para la solicitud o el chat proporcionados.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL OpenAI (ChatGPT & DALL-E)] cuenta de Workfront Fusion, consulte <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Conectando [!DNL OpenAI (ChatGPT & DALL-E)] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Modelo]</td> 
   <td> Introduzca o asigne el ID del modelo que desea utilizar. Puede utilizar el módulo Obtener modelos para ver todos los modelos disponibles. </td> 
  </tr> 
  <!--<tr> 
   <td role="rowheader">[!UICONTROL Temperature]</td> 
   <td> This value must be between 0 and 2, and determines the randomness of the output. Higher values produce output that is more random, while lower values produce more focused output. </td> 
  </tr> -->
  <tr> 
   <td role="rowheader">[!UICONTROL Configuración avanzada]</td> 
   <td> <p>Para obtener información sobre la configuración avanzada opcional de este módulo, consulte la información sobre la creación de finalizaciones en la <a href="https://platform.openai.com/docs/api-reference/completions/create" class="MCXref xref">Documentación de API de OpenAI</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Crear una moderación

Este módulo de acción determina si el texto infringe la política de contenido de OpenAI.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL OpenAI (ChatGPT & DALL-E)] cuenta de Workfront Fusion, consulte <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Conectando [!DNL OpenAI (ChatGPT & DALL-E)] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrada]</td> 
   <td> Para cada muestra de texto que desee incluir, haga clic en <b>Añadir elemento</b> y escriba o asigne el texto. Incluya todo el ejemplo de texto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Modelo]</td> 
   <td> Introduzca o asigne el ID del modelo que desea utilizar. Puede utilizar el módulo Obtener modelos para ver todos los modelos disponibles. </td> 
  </tr> 
 </tbody> 
</table>

### Crear una edición

Este módulo de acción devuelve una versión editada de un mensaje que ha proporcionado, siguiendo sus instrucciones.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL OpenAI (ChatGPT & DALL-E)] cuenta de Workfront Fusion, consulte <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Conectando [!DNL OpenAI (ChatGPT & DALL-E)] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Modelo]</td> 
   <td> Introduzca o asigne el ID del modelo que desea utilizar. Puede utilizar el módulo Obtener modelos para ver todos los modelos disponibles. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrada]</td> 
   <td> Escriba o asigne el texto que desea editar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Instrucción]</td> 
   <td> Introduzca o asigne las instrucciones de edición. Ejemplo: "Corregir los errores ortográficos". </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Configuración avanzada]</td> 
   <td> <p>Para obtener información sobre la configuración avanzada opcional de este módulo, consulte la información sobre la creación de ediciones en la <a href="https://platform.openai.com/docs/api-reference/edits/create" class="MCXref xref">Documentación de API de OpenAI</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Crear una incrustación

Este módulo de acción crea un vector de incrustación que representa el texto de entrada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL OpenAI (ChatGPT & DALL-E)] cuenta de Workfront Fusion, consulte <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Conectando [!DNL OpenAI (ChatGPT & DALL-E)] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Modelo]</td> 
   <td> Introduzca o asigne el ID del modelo que desea utilizar. Puede utilizar el módulo Obtener modelos para ver todos los modelos disponibles. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Texto de entrada para incrustar]</td> 
   <td> Escriba o asigne el texto que desea incrustar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de usuario]</td> 
   <td> Introduzca o asigne un identificador único que represente a su usuario final, lo que puede ayudar a OpenAI a monitorizar y detectar el abuso </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> Introduzca o asigne el número máximo de ediciones con las que desea que funcione el módulo durante cada ciclo de ejecución de escenario.</td> 
  </tr> 
 </tbody> 
</table>

### Creación de finalización de chat

Dada una lista de mensajes que describen una conversación, este módulo de acción devuelve una respuesta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL OpenAI (ChatGPT & DALL-E)] cuenta de Workfront Fusion, consulte <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Conectando [!DNL OpenAI (ChatGPT & DALL-E)] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Modelo]</td> 
   <td> Introduzca o asigne el ID del modelo que desea utilizar. Puede utilizar el módulo Obtener modelos para ver todos los modelos disponibles. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mensajes]</td> 
   <td>Los mensajes describen la conversación hasta el momento. Para cada mensaje que desee añadir, haga clic en <b>Añadir elemento</b> y rellene lo siguiente:
   <ul>
   <li> <b>Rol</b>: seleccione la función del autor de este mensaje.</li>
   <li> <b>Contenido</b>: introduzca o asigne el contenido de este mensaje.</li>
   <li> <b>Nombre</b>: introduzca o asigne el nombre del autor de este mensaje. El nombre puede contener letras en mayúsculas y minúsculas, números y guiones bajos. La longitud máxima del nombre es de 64 caracteres.</li>
   </ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Configuración avanzada]</td> 
   <td> <p>Para obtener información sobre la configuración avanzada opcional de este módulo, consulte la información sobre la creación de finalizaciones de chat en el <a href="https://platform.openai.com/docs/api-reference/chat/create" class="MCXref xref">Documentación de API de OpenAI</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--

### Edit image

This action module makes edits or creates variations of existing images.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL OpenAI (ChatGPT & DALL-E)] account to Workfront Fusion, see <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connecting [!DNL OpenAI (ChatGPT & DALL-E)] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select the operation]</td> 
   <td> Select whether you want to create edits or variations of the image.
   <p>NOTE: Images must be a valid PNG file, less than 4MB, and square. If mask is not provided, the image must have transparency, which will be used as the mask.</p> 
 </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Text description of desired image]</td> 
   <td> <p>If editing an image, enter or map a description of the edits you want to create. Maximum length is 1000 characters.</p> </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>For information about the optional advanced settings in this module, see the information about creating image edits or variations in the <a href="https://platform.openai.com/docs/api-reference/images/createEdit" class="MCXref xref">OpenAI API documentation</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

### Generación de imágenes

Este módulo de acción genera o manipula imágenes con modelos Dall-E.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL OpenAI (ChatGPT & DALL-E)] cuenta de Workfront Fusion, consulte <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Conectando [!DNL OpenAI (ChatGPT & DALL-E)] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descripción de texto de la imagen deseada]</td> 
   <td> Introduzca o asigne una descripción de la imagen deseada. La longitud máxima de la descripción es de 1000 caracteres. 
 </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Configuración avanzada]</td> 
   <td> <p>Para obtener información sobre la configuración avanzada opcional de este módulo, consulte la información sobre la creación de imágenes en <a href="https://platform.openai.com/docs/api-reference/images/create" class="MCXref xref">Documentación de API de OpenAI</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Obtener modelos

Este módulo enumera y describe los distintos modelos disponibles en la API de OpenAI.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL OpenAI (ChatGPT & DALL-E)] cuenta de Workfront Fusion, consulte <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Conectando [!DNL OpenAI (ChatGPT & DALL-E)] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Acción]</td> 
   <td> Seleccione si desea obtener una lista de todos los modelos o recuperar un modelo específico.
    <ul>
    <li><p><b>Enumerar modelos </b></p><p>Esta acción enumera los modelos disponibles actualmente y proporciona información básica sobre cada uno, como el propietario y la disponibilidad.</p></li>
    <li><p><b>Recuperar modelo </b></p><p>Introduzca o asigne el ID del modelo que desea recuperar. </p></li>
   </ul>
 </td> 
 </tbody> 
</table>

### Realizar una llamada de API personalizada

Este módulo de acción envía una solicitud HTTP personalizada a la API de OpenAI.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL OpenAI (ChatGPT & DALL-E)] cuenta de Workfront Fusion, consulte <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Conectando [!DNL OpenAI (ChatGPT & DALL-E)] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Introduzca una ruta relativa a <code>https://api.openai.com/v1/</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion añade los encabezados de autorización automáticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuerpo]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando se utilizan afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera del enunciado condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

<!--

### Manage Audio

This action modules converts audio to text.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL OpenAI (ChatGPT & DALL-E)] account to Workfront Fusion, see <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connecting [!DNL OpenAI (ChatGPT & DALL-E)] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select the operation]</td> 
   <td> Select whether you want to transcribe the audio into the input language, or into English.
   <p>If transcribing into the input language, you can select the language in this module's advanced settings. </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> Enter or map the maximum number of edits you want the module to work with during each scenario execution cycle.</td> 
   <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>For information about the optional advanced settings in this module, see the information about creating transcriptions in the <a href="https://platform.openai.com/docs/api-reference/audio/createTranscription" class="MCXref xref">OpenAI API documentation</a>.</p> </td> 
  </tr> 
  </tr> 
 </tbody> 
</table>

-->

### Administrar archivos

Este módulo de acción enumera, elimina o recupera archivos o contenido de archivo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL OpenAI (ChatGPT & DALL-E)] cuenta de Workfront Fusion, consulte <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Conectando [!DNL OpenAI (ChatGPT & DALL-E)] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Acción]</td> 
   <td> Seleccione la acción que desea realizar. 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL ID de archivo]</td> 
   <td> Si está eliminando un archivo o recuperando un archivo o contenido de archivo, introduzca o asigne el ID del archivo. 
  </tr> 
</tbody>
</table>

### Administrar ajustes

Administre trabajos de ajuste para adaptar un modelo a los datos de formación específicos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL OpenAI (ChatGPT & DALL-E)] cuenta de Workfront Fusion, consulte <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Conectando [!DNL OpenAI (ChatGPT & DALL-E)] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccione la operación]</td> 
   <td> Seleccione la acción que desea realizar.
   <ul>
   <li><p>Ajuste de un modelo de un conjunto de datos</p><p>Introduzca o asigne una descripción para la imagen deseada.</p>
     <li><p>Obtener información sobre un trabajo de ajuste preciso</p><p>Introduzca o asigne el ID del trabajo.</p>
   <li><p>Cancelar un trabajo de ajuste</p><p>Introduzca o asigne el ID del trabajo.</p>
   <li><p>Cancelar un trabajo de ajuste</p><p>Introduzca o asigne el ID del trabajo.</p>
   <li><p>Obtener actualizaciones de estado para un trabajo de ajuste</p><p>Introduzca o asigne el ID del trabajo y seleccione si desea transmitir estas actualizaciones.</p>
   <li><p>Eliminación de un modelo ajustado</p><p>Introduzca o asigne el ID del modelo que desea eliminar.</p>
 </ul> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL ID de archivo]</td> 
   <td> Si está eliminando un archivo o recuperando un archivo o contenido de archivo, introduzca o asigne el ID del archivo. 
  </tr> 
</tbody>

