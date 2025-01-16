---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Marketo
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 7f6dace5-ab50-45da-a926-1a8919057f7b
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '2136'
ht-degree: 94%

---

# Módulos de [!DNL Marketo]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Módulos Marketo](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/adobe-marketo-modules.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

En un escenario de [!DNL Adobe Workfront Fusion], es posible automatizar los flujos de trabajo que utilizan [!DNL Marketo], así como conectarlo a varias aplicaciones y servicios de terceros.

Para ver un vídeo introductorio del conector de Marketo, consulte:

* [Marketo](https://video.tv.adobe.com/v/3427026/){target=_blank}

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información acerca de los módulos, consulte [Módulos de  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere ninguna licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Para usar módulos [!DNL Marketo], debe tener una cuenta de [!DNL Marketo].

## Información de API de Marketo

El conector de Marketo utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Versión de API</td> 
   <td> Versión 1 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 1.14.19</td> 
  </tr>
 </tbody> 
 </table>

## Conexión de [!DNL Marketo] a Workfront Fusion {#connect-marketo-to-workfront-fusion}

Puede crear una conexión con su cuenta de [!DNL Marketo] directamente desde el módulo [!DNL Marketo].

1. En cualquier módulo de [!DNL Marketo], haga clic en **[!UICONTROL Añadir]** junto al campo [!UICONTROL Conexión].
1. Escriba su cuenta de [!DNL Marketo] o [!DNL Marketo] [!UICONTROL Munchkin] ID. Esta es la única parte de la dirección URL base o punto final asignado a la cuenta que usa para acceder a [!DNL Marketo] a través de su API [!UICONTROL REST]. Para obtener instrucciones sobre cómo encontrarla, consulte [URL base](https://developers.marketo.com/rest-api/base-url/) en la documentación de [!DNL Marketo].
1. Escriba su [!UICONTROL Client ID] y [!UICONTROL Client secret]. Para obtener instrucciones sobre cómo localizarlos, consulte [Autenticación](https://developers.marketo.com/rest-api/authentication/) en la documentación de [!DNL Marketo].
1. Haga clic en **[!UICONTROL Continuar]** para crear la conexión y volver al módulo.

## Módulos de [!DNL Marketo] y sus campos

Al configurar módulos de [!DNL Marketo], [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Marketo] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. El título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Activadores](#triggers)
* [Acciones](#actions)
* [Búsquedas](#searches)

### Activadores

* [[!UICONTROL Ver eventos (instantáneo)]](#watch-events-instant)
* [[!UICONTROL Ver registros]](#watch-records)

#### [!UICONTROL Ver eventos (instantáneo)]

Este módulo de activador inicia un escenario cuando se crea o se actualiza un registro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Webhook]</p> </td> 
   <td> <p>Introduzca el webhook que desea que utilice el módulo.</p> <p>Para obtener más información sobre los webhooks, consulte <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Activadores instantáneos (webhooks) en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ver registros]

Este módulo de activador inicia un escenario cuando se crea o se actualiza un registro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Marketo] a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Seleccione el tipo de registro que desea crear.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Activity]</strong> </p> <p>Seleccione el tipo de actividad que desea ver. </p> <p>El módulo solo ve las nuevas actividades.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Lead]</strong> </p> <p>Seleccione si desea ver nuevos registros, registros actualizados, registros nuevos y actualizados o actualizaciones de campos específicos. Si selecciona ver actualizaciones de campos específicos, seleccione el campo que desea que el módulo vea.</p> </li> 
     <li> <p><strong>[!UICONTROL Programa]</strong> </p> <p>Seleccione si desea ver registros nuevos, registros actualizados o registros nuevos y actualizados.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Seleccione la información que desea incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Añadir posibles clientes a una lista]](#add-leads-to-a-list)
* [[!UICONTROL Clonar un programa]](#clone-a-program)
* [[!UICONTROL Create a record]](#create-a-record)
* [[!UICONTROL Llamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Descargar un archivo]](#download-a-file)
* [[!UICONTROL Leer un registro]](#read-a-record)
* [[!UICONTROL Quitar posibles clientes de una lista]](#remove-leads-from-a-list)
* [[!UICONTROL Programar una campaña]](#schedule-a-campaign)
* [[!UICONTROL Actualizar un registro]](#update-a-record)
* [[!UICONTROL Subir un archivo]](#upload-a-file)

#### [!UICONTROL Añadir posibles clientes a una lista]

Este módulo de acción añade uno o más posibles clientes a una lista mediante el uso del ID de posible cliente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de la cuenta de [!DNL Marketo] a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Introduzca o asigne el ID de la lista a la que desea añadir posibles clientes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lead IDs]</td> 
   <td> <p>Para cada posible cliente que desee añadir a la lista, haga clic en <b>[!UICONTROL Añadir]</b> y, a continuación, escriba o asigne el identificador del posible cliente que desee añadir. Puede añadir hasta 300 posibles clientes para que el módulo los añada a la lista.</p> <p>Haga clic en el botón de alternancia Asignar para asignar una colección existente de posibles clientes que desee añadir a la lista.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Clonar un programa]

Este módulo de acción realiza una copia de un programa utilizando el ID del programa existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Marketo] a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Folder ID]</td> 
   <td>Introduzca o asigne el ID de la carpeta en la que desea ubicar el nuevo programa.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un registro]

Este módulo de acción crea un nuevo registro en [!DNL Marketo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Marketo] a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Seleccione el tipo de registro que desea crear.</p> 
    <ul> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Folder]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL Program]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select fields to map]</td> 
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
   <td role="rowheader">[!UICONTROL Carpeta] / [!UICONTROL Nombre del programa]</td> 
   <td>Si está creando una carpeta o programa, escriba o asigne un nombre para el nuevo registro.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td> <p>Si está creando una carpeta o un programa, introduzca o asigne una descripción para el nuevo registro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parent Folder ID]</td> 
   <td>Si está creando una carpeta o programa, introduzca o asigne el identificador de la carpeta principal en la que desea crear el nuevo registro.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costs]</td> 
   <td>Si está creando un programa, añada los costes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td>Si está creando un programa, añada las etiquetas</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Llamada de API personalizada]

Este módulo de acción le permite realizar una llamada autenticada personalizada a la API de [!DNL Marketo]. De este modo, puede crear una automatización del flujo de datos que no puedan realizar los otros módulos de [!DNL Marketo].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Marketo] a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Escriba una ruta relativa a <code>https://{your-base-url}.mktorest.com/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Seleccione el método de petición HTTP que necesita para configurar la llamada de la API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de petición HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] añade los encabezados de autorización automáticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando utilice instrucciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la instrucción condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros con los que desea que trabaje el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
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
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Marketo] a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td>Asigne el ID del archivo que desea descargar.</td> 
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
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Marketo] a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Seleccione el tipo de registro que desea crear.</p> 
    <ul> 
     <li> <p>[!UICONTROL Campaign]</p> </li> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL List]</p> </li> 
     <li> <p>[!UICONTROL Program]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Seleccione la información que desea incluir en el paquete de salida para este módulo. Los campos están disponibles en función del [!UICONTROL Record Type] seleccionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;Object&gt; ID]</td> 
   <td>Introduzca o asigne el ID del objeto sobre el que desea recuperar información.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Quitar posibles clientes de una lista]

Este módulo de acción elimina uno o más posibles clientes de una lista mediante el uso del ID de posible cliente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de la cuenta de [!DNL Marketo] a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Introduzca o asigne el ID de la lista donde desea quitar los posibles clientes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lead IDs]</td> 
   <td> <p>Para cada posible cliente que desee eliminar de la lista, haga clic en <b>[!UICONTROL Añadir]</b> y, a continuación, escriba o asigne el identificador del posible cliente que desee eliminar. Puede añadir hasta 300 posibles clientes para que el módulo los quite de la lista. </p> <p>Haga clic en el botón de alternancia Asignar para asignar una colección existente de posibles clientes que desee eliminar de la lista.</p> </td> 
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
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Marketo] a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campaign ID]</td> 
   <td>Introduzca o asigne el ID de la campaña que desea programar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Programación para la fecha]</p> </td> 
   <td>Seleccione la fecha en la que desea ejecutar la campaña. Si este campo se deja en blanco, la campaña se ejecuta cinco minutos después de que comience el escenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar un registro]

Este módulo de acción actualiza un registro existente mediante su identificador.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Marketo] a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Seleccione el tipo de registro que desea crear.</p> 
    <ul> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL Program]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compañía] / [!UICONTROL Posible cliente] / [!UICONTROL Programa ID]</td> 
   <td>Introduzca o asigne el ID del registro que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select fields to map]</td> 
   <td>Si está actualizando una compañía o un posible cliente, seleccione los campos para los que desee actualizar los valores e introduzca los valores de dichos campos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de programa]</td> 
   <td>Si va a actualizar un programa, escriba o asigne un nombre nuevo para el programa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td> <p>Si va a actualizar un programa, escriba o asigne una nueva descripción para el programa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start Date]</td> 
   <td>Si va a actualizar un programa, introduzca o asigne una nueva fecha de inicio para el programa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL End Date]</td> 
   <td>Si va a actualizar un programa, introduzca o asigne una nueva fecha de finalización para el programa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costs]</td> 
   <td>Si va a actualizar un programa, añada los costes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td>Si va a actualizar un programa, añada las etiquetas </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Subir un archivo]

Este módulo de acción sube un nuevo archivo a [!UICONTROL Marketo].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Marketo] a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID]</td> 
   <td>Introduzca o asigne el ID de la carpeta en la que desea ubicar el nuevo archivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Escriba una descripción para el archivo que ha subido.</td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

* [[!UICONTROL Enumerar registros]](#list-records)
* [[!UICONTROL Buscar registros]](#update-a-record)

#### [!UICONTROL Enumerar registros]

Este módulo de acción recupera todos los registros de un tipo específico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Marketo] a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Seleccione el tipo de registro que desea enumerar.</p> 
    <ul> 
     <li> <p>[!UICONTROL Leer todas las campañas]</p> </li> 
     <li> <p>[!UICONTROL Leer todos los programas]</p> </li> 
     <li> <p>[!UICONTROL Leer todos los posibles clientes] </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Field]</td> 
   <td>Si ha seleccionado recuperar posibles clientes, seleccione si desea recuperar posibles clientes de una lista o de un programa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Seleccione la información que desea incluir en el paquete de salida para este módulo. Los campos están disponibles en función del [!UICONTROL Record Type] seleccionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución de escenario.</p> </td> 
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
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Marketo] a [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Seleccione el tipo de registro que desea buscar.</p> 
    <ul> 
     <li> <p>[!UICONTROL Campañas]</p> </li> 
     <li> <p>[!UICONTROL Posibles clientes]</p> </li> 
     <li> <p>[!UICONTROL Programs]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Field]</p> </td> 
   <td> <p>Seleccione si desea buscar por nombre, nombre de programa o nombre de espacio de trabajo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values]</td> 
   <td>Para cada valor que desee buscar, haga clic en <b>[!UICONTROL Añadir elemento]</b> e introduzca el valor.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salida]</td> 
   <td> <p>Seleccione la información que desea incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>
