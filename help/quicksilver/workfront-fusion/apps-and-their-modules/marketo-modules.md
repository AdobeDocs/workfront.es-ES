---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Marketo
description: En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Marketo], así como conectarlo a múltiples aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 7f6dace5-ab50-45da-a926-1a8919057f7b
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '2068'
ht-degree: 0%

---

# [!DNL Marketo] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Marketo], así como conectarlo a múltiples aplicaciones y servicios de terceros.

Para ver un vídeo introductorio del conector de Marketo, consulte:

* [Marketo](https://video.tv.adobe.com/v/3427026/){target=_blank}

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
   <td>
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito actual del producto: si tiene [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Para usar [!DNL Marketo] módulos, debe tener un [!DNL Marketo] cuenta.

## Connect [!DNL Marketo] a Workfront Fusion {#connect-marketo-to-workfront-fusion}

Puede crear una conexión con su [!DNL Marketo] cuenta directamente desde dentro [!DNL Marketo] módulo.

1. En cualquier [!DNL Marketo] , haga clic en **[!UICONTROL Añadir]** junto al [!UICONTROL Conexión] field.
1. Introduzca su [!DNL Marketo] cuenta o [!DNL Marketo] [!UICONTROL Munchkin] ID. Esta es la parte única de la dirección URL base o punto de conexión asignado a su cuenta de que utiliza para acceder a [!DNL Marketo] mediante su [!UICONTROL REST] API. Para obtener instrucciones sobre cómo localizarlo, consulte [URL básica](https://developers.marketo.com/rest-api/base-url/) en el [!DNL Marketo] documentación.
1. Introduzca su [!UICONTROL ID de cliente] y [!UICONTROL Secreto de cliente]. Para obtener instrucciones sobre cómo localizarlos, consulte [Autenticación](https://developers.marketo.com/rest-api/authentication/) en el [!DNL Marketo] documentación.
1. Clic **[!UICONTROL Continuar]** para crear la conexión y volver al módulo.

## [!DNL Marketo] Módulos y sus campos

Al configurar [!DNL Marketo] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, se añaden [!DNL Marketo] Los campos pueden mostrarse, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheur](#triggers)
* [Acciones](#actions)
* [Búsquedas](#searches)

### Déclencheur

* [[!UICONTROL Ver registros]](#watch-records)
* [[!UICONTROL Ver eventos (instantáneos)]](#watch-events-instant)

#### [!UICONTROL Ver registros]

Este módulo de déclencheur inicia un escenario cuando se crea o actualiza un registro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Marketo] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea crear.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Actividad]</strong> </p> <p>Seleccione el tipo de actividad que desea ver. </p> <p>El módulo solo observa las nuevas actividades.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Posible cliente]</strong> </p> <p>Seleccione si desea inspeccionar registros nuevos, registros actualizados, registros nuevos y actualizados o actualizaciones de campos específicas. Si selecciona inspeccionar actualizaciones de campo específicas, seleccione el campo que desea que el módulo inspeccione.</p> </li> 
     <li> <p><strong>[!UICONTROL Programa]</strong> </p> <p>Seleccione si desea inspeccionar registros nuevos, registros actualizados o registros nuevos y actualizados.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione la información que desee incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ver eventos (instantáneos)]

Este módulo de déclencheur inicia un escenario cuando se crea o actualiza un registro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Webhook]</p> </td> 
   <td> <p>Introduzca el webhook que desea que utilice el módulo.</p> <p>Para obtener más información sobre los webhooks, consulte <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Déclencheur instantáneos (webhooks) en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Llamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Creación de un registro]](#create-a-record)
* [[!UICONTROL Actualización de un registro]](#update-a-record)
* [[!UICONTROL Descargar un archivo]](#download-a-file)
* [[!UICONTROL Cargar un archivo]](#upload-a-file)
* [[!UICONTROL Leer un registro]](#read-a-record)
* [[!UICONTROL Añadir posibles clientes a una lista]](#add-leads-to-a-list)
* [[!UICONTROL Eliminar posibles clientes de una lista]](#remove-leads-from-a-list)
* [[!UICONTROL Programar una campaña]](#schedule-a-campaign)
* [[!UICONTROL Copiar un programa]](#copy-a-program)

#### [!UICONTROL Llamada de API personalizada]

Este módulo de acción le permite realizar una llamada autenticada personalizada a [!DNL Marketo] API. De este modo, se puede crear una automatización del flujo de datos que el otro no puede realizar [!DNL Marketo] módulos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Marketo] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Introduzca una ruta relativa a <code>https://{your-base-url}.mktorest.com/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] agrega los encabezados de autorización automáticamente.</p> </td> 
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
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros con los que desea que trabaje el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Creación de un registro]

Este módulo de acción crea un nuevo registro en [!DNL Marketo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Marketo] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea crear.</p> 
    <ul> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Carpeta]</p> </li> 
     <li> <p>[!UICONTROL Posible cliente]</p> </li> 
     <li> <p>[!UICONTROL Programa]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar campos para asignar]</td> 
   <td>Si está creando una compañía o un posible cliente, seleccione los campos para los que desea establecer valores cuando se cree el nuevo registro y, a continuación, introduzca los valores de estos campos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de programa]</td> 
   <td>Si está creando un programa, seleccione el tipo de programa que desea crear.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Canal de programa] </td> 
   <td>Si está creando un programa, seleccione el canal de programa en el que desea crear el programa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carpeta] / [!UICONTROL Nombre de programa]</td> 
   <td>Si está creando una carpeta o programa, escriba o asigne un nombre para el nuevo registro.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descripción]</td> 
   <td> <p>Si está creando una carpeta o programa, escriba o asigne una descripción para el nuevo registro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de carpeta principal]</td> 
   <td>Si está creando una carpeta o programa, escriba o asigne el identificador de la carpeta principal en la que desea crear el nuevo registro.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costos]</td> 
   <td>Si está creando un programa, agregue los costes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etiquetas]</td> 
   <td>Si está creando un programa, agregue las etiquetas que desee</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualización de un registro]

Este módulo de acción actualiza un registro existente mediante su ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Marketo] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea crear.</p> 
    <ul> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Posible cliente]</p> </li> 
     <li> <p>[!UICONTROL Programa]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Company] / [!UICONTROL Lead] / [!UICONTROL Program ID]</td> 
   <td>Introduzca o asigne el ID del registro que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar campos para asignar]</td> 
   <td>Si va a actualizar una compañía o un posible cliente, seleccione los campos para los que desee actualizar los valores e introduzca los valores de dichos campos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de programa]</td> 
   <td>Si está actualizando un programa, escriba o asigne un nombre nuevo para el programa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descripción]</td> 
   <td> <p>Si está actualizando un programa, escriba o asigne una nueva descripción para el programa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fecha de inicio]</td> 
   <td>Si está actualizando un programa, escriba o asigne una nueva fecha de inicio para el programa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fecha de finalización]</td> 
   <td>Si está actualizando un programa, introduzca o asigne una nueva fecha de finalización para el programa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costos]</td> 
   <td>Si va a actualizar un programa, agregue los costes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etiquetas]</td> 
   <td>Si está actualizando un programa, agregue las etiquetas que desee</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Descargar un archivo]

Este módulo de acción descarga un archivo mediante el ID de archivo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Marketo] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de archivo]</td> 
   <td>Asigne el ID del archivo que desea descargar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cargar un archivo]

Este módulo de acción carga un nuevo archivo en [!UICONTROL Marketo].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Marketo] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de carpeta]</td> 
   <td>Introduzca o asigne el ID de la carpeta en la que desea ubicar el nuevo archivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descripción]</td> 
   <td>Escriba una descripción para el archivo cargado.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leer un registro]

Este módulo de acción lee información sobre un registro mediante su ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Marketo] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea crear.</p> 
    <ul> 
     <li> <p>[!UICONTROL Campaign]</p> </li> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Posible cliente]</p> </li> 
     <li> <p>[!UICONTROL Lista]</p> </li> 
     <li> <p>[!UICONTROL Programa]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td>Seleccione la información que desee incluir en el paquete de salida para este módulo. Los campos están disponibles en función del [!UICONTROL Record Type] seleccionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;object&gt; [ID]</td> 
   <td>Introduzca o asigne el ID del objeto sobre el que desea recuperar información.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Añadir posibles clientes a una lista]

Este módulo de acción agrega uno o más posibles clientes a una lista mediante el uso del ID de posible cliente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Marketo] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Introduzca o asigne el ID de la lista a la que desea agregar posibles clientes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de posibles clientes]</td> 
   <td> <p>Haga clic en cada posible cliente que desee agregar a la lista <b>[!UICONTROL Agregar]</b>A continuación, introduzca o asigne el ID del posible cliente que desea agregar. Puede añadir hasta 300 posibles clientes para que el módulo añada a la lista.</p> <p>Haga clic en el botón de alternancia Asignar para asignar una colección existente de posibles clientes que desee agregar a la lista.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar posibles clientes de una lista]

Este módulo de acción elimina uno o más posibles clientes de una lista mediante el uso del ID de posible cliente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Marketo] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Introduzca o asigne el ID de la lista donde desea eliminar los posibles clientes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de posibles clientes]</td> 
   <td> <p>Para cada posible cliente que desee eliminar de la lista, haga clic en <b>[!UICONTROL Agregar]</b>A continuación, introduzca o asigne el ID del posible cliente que desea eliminar. Puede añadir hasta 300 posibles clientes para que el módulo elimine de la lista. </p> <p>Haga clic en el botón de alternancia Asignar para asignar una colección existente de posibles clientes que desee eliminar de la lista.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Programar una campaña]

Este módulo de acción programa una campaña existente para una fecha determinada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Marketo] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de campaña]</td> 
   <td>Introduzca o asigne el ID de la campaña que desea programar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Programación para la fecha]</p> </td> 
   <td>Seleccione la fecha en la que desea ejecutar la campaña. Si este campo se deja en blanco, la campaña se ejecuta cinco minutos después de que comience el escenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar un programa]

Este módulo de acción realiza una copia de un programa utilizando el ID del programa existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Marketo] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de programa existente]</td> 
   <td>Introduzca o asigne el ID del programa que desea copiar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nuevo nombre de programa]</p> </td> 
   <td> <p>Introduzca o asigne un nombre para el nuevo programa</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de carpeta]</td> 
   <td>Introduzca o asigne el ID de la carpeta en la que desea ubicar el nuevo programa.</td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

* [[!UICONTROL Enumeración de registros]](#list-records)
* [[!UICONTROL Buscar registros]](#update-a-record)

#### [!UICONTROL Enumeración de registros]

Este módulo de acción recupera todos los registros de un tipo específico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Marketo] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea enumerar.</p> 
    <ul> 
     <li> <p>[!UICONTROL Leer todas las campañas]</p> </li> 
     <li> <p>[!UICONTROL Leer todos los programas]</p> </li> 
     <li> <p>[!UICONTROL Leer todos los posibles clientes] </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campo]</td> 
   <td>Si ha seleccionado recuperar posibles clientes, seleccione si desea recuperar posibles clientes de una lista o de un programa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td>Seleccione la información que desee incluir en el paquete de salida para este módulo. Los campos están disponibles en función del [!UICONTROL Record Type] seleccionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Buscar registros]

Este módulo de búsqueda recupera una lista de registros que coinciden con criterios de búsqueda específicos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Marketo] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea buscar.</p> 
    <ul> 
     <li> <p>[!UICONTROL Campañas]</p> </li> 
     <li> <p>[!UICONTROL Posibles clientes]</p> </li> 
     <li> <p>[!UICONTROL Programas]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Campo]</p> </td> 
   <td> <p>Seleccione si desea buscar por nombre, nombre de programa o nombre de espacio de trabajo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valores]</td> 
   <td>Para cada valor que desee buscar, haga clic en <b>[!UICONTROL Agregar elemento]</b> e introduzca el valor.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salida]</td> 
   <td> <p>Seleccione la información que desee incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>
