---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos de Marketo
description: En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Marketo], así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 7f6dace5-ab50-45da-a926-1a8919057f7b
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2014'
ht-degree: 0%

---

# [!DNL Marketo] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Marketo], así como conectarlo a varias aplicaciones y servicios de terceros.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Para usar [!DNL Marketo] módulos, debe tener un [!DNL Marketo] cuenta.

## Connect [!DNL Marketo] a Workfront Fusion {#connect-marketo-to-workfront-fusion}

Puede crear una conexión con su [!DNL Marketo] cuenta directamente desde dentro [!DNL Marketo] módulo.

1. En cualquier [!DNL Marketo] módulo, haga clic en **[!UICONTROL Agregar]** junto a la variable [!UICONTROL Conexión] campo .
1. Escriba la [!DNL Marketo] o [!DNL Marketo] [!UICONTROL Munchkin] ID. Esta es la parte única de la dirección URL base o del extremo asignado a su cuenta, que utiliza para acceder a [!DNL Marketo] a través de su [!UICONTROL REST] API. Para obtener instrucciones sobre cómo localizar esto, consulte [Dirección URL base](https://developers.marketo.com/rest-api/base-url/) en el [!DNL Marketo] documentación.
1. Escriba la [!UICONTROL ID de cliente] y [!UICONTROL Secreto de cliente]. Para obtener instrucciones sobre cómo ubicarlas, consulte [Autenticación](https://developers.marketo.com/rest-api/authentication/) en el [!DNL Marketo] documentación.
1. Haga clic en **[!UICONTROL Continuar]** para crear la conexión y volver al módulo .

## [!DNL Marketo] Módulos y sus campos

Al configurar [!DNL Marketo] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL Marketo] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheur](#triggers)
* [Acciones](#actions)
* [Búsquedas](#searches)

### Déclencheur

* [[!UICONTROL Registros de Watch]](#watch-records)
* [[!UICONTROL Eventos Watch (Instant)]](#watch-events-instant)

#### [!UICONTROL Registros de Watch]

Este módulo de déclencheur inicia un escenario cuando se crea o actualiza un registro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Marketo] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea crear.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Actividad]</strong> </p> <p>Seleccione el tipo de actividad que desea ver. </p> <p>El módulo solo ve las actividades nuevas.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Lead]</strong> </p> <p>Seleccione si desea ver registros nuevos, registros actualizados, registros nuevos y actualizados, o actualizaciones de campos específicas. Si selecciona ver actualizaciones de campos específicas, seleccione el campo que desea que vea el módulo.</p> </li> 
     <li> <p><strong>[!UICONTROL Program]</strong> </p> <p>Seleccione si desea buscar registros nuevos, registros actualizados o registros nuevos y actualizados.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione la información que desee incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eventos Watch (Instant)]

Este módulo de déclencheur inicia un escenario cuando se crea o actualiza un registro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Weblock]</p> </td> 
   <td> <p>Introduzca el enlace web que desea que utilice el módulo.</p> <p>Para obtener más información sobre los enlaces web, consulte <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Déclencheur instantáneos (enlaces web) en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Llamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Crear un registro]](#create-a-record)
* [[!UICONTROL Actualizar un registro]](#update-a-record)
* [[!UICONTROL Descargar un archivo]](#download-a-file)
* [[!UICONTROL Cargar un archivo]](#upload-a-file)
* [[!UICONTROL Leer un registro]](#read-a-record)
* [[!UICONTROL Agregar posibles clientes a una lista]](#add-leads-to-a-list)
* [[!UICONTROL Eliminar posibles clientes de una lista]](#remove-leads-from-a-list)
* [[!UICONTROL Programar una campaña]](#schedule-a-campaign)
* [[!UICONTROL Copiar un programa]](#copy-a-program)

#### [!UICONTROL Llamada de API personalizada]

Este módulo de acción le permite realizar una llamada autenticada personalizada al [!DNL Marketo] API. De este modo, puede crear una automatización del flujo de datos que no se pueda lograr con la otra [!DNL Marketo] módulos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Marketo] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Especifique una ruta relativa a <code>https://{your-base-url}.mktorest.com/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada a la API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] añade los encabezados de autorización por usted.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Al utilizar afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros con los que desea que funcione el módulo durante cada ciclo de ejecución del escenario.</p> </td> 
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
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Marketo] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea crear.</p> 
    <ul> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Folder]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL Program]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar campos para asignar]</td> 
   <td>Si va a crear una empresa o un posible cliente, seleccione los campos en los que desea definir los valores cuando se cree el nuevo registro y, a continuación, introduzca los valores para estos campos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de programa]</td> 
   <td>Si está creando un programa, seleccione el tipo de programa que desea crear.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Channel] </td> 
   <td>Si está creando un programa, seleccione el canal del programa en el que desea crear el programa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] / [!UICONTROL Program Name]</td> 
   <td>Si está creando una carpeta o programa, introduzca o asigne un nombre para el nuevo registro.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descripción]</td> 
   <td> <p>Si está creando una carpeta o programa, introduzca o asigne una descripción para el nuevo registro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de carpeta principal]</td> 
   <td>Si está creando una carpeta o programa, introduzca o asigne el ID de la carpeta principal en la que desea crear el nuevo registro.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costes]</td> 
   <td>Si está creando un programa, agregue cualquier coste.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etiquetas]</td> 
   <td>Si está creando un programa, agregue cualquier etiqueta</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar un registro]

Este módulo de acción actualiza un registro existente con su ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Marketo] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea crear.</p> 
    <ul> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL Program]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Company] / [!UICONTROL Lead] / [!UICONTROL Program ID]</td> 
   <td>Introduzca o asigne el ID del registro que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar campos para asignar]</td> 
   <td>Si va a actualizar una empresa o un posible cliente, seleccione los campos para los que desea actualizar los valores y, a continuación, introduzca valores para estos campos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre del programa]</td> 
   <td>Si está actualizando un Programa, introduzca o asigne un nuevo nombre para el programa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descripción]</td> 
   <td> <p>Si está actualizando un Programa, introduzca o asigne una nueva descripción para el programa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fecha de inicio]</td> 
   <td>Si está actualizando un Programa, introduzca o asigne una nueva fecha de inicio del programa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fecha de finalización]</td> 
   <td>Si está actualizando un Programa, introduzca o asigne una nueva fecha de finalización para el programa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costes]</td> 
   <td>Si va a actualizar un programa, agregue cualquier coste.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etiquetas]</td> 
   <td>Si va a actualizar un programa, agregue cualquier etiqueta</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Descargar un archivo]

Este módulo de acción descarga un archivo utilizando el ID de archivo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Marketo] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
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
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Marketo] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID]</td> 
   <td>Introduzca o asigne el ID de la carpeta en la que desea localizar el nuevo archivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descripción]</td> 
   <td>Introduzca una descripción para el archivo cargado.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leer un registro]

Este módulo de acción lee información sobre un registro utilizando su ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Marketo] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
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
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td>Seleccione la información que desee incluir en el paquete de salida para este módulo. Los campos están disponibles según el [!UICONTROL Record Type] seleccionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;object&gt; ID]</td> 
   <td>Introduzca o asigne el ID del objeto del que desea recuperar información.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Agregar posibles clientes a una lista]

Este módulo de acción agrega uno o más posibles clientes a una lista mediante el uso del ID de posible cliente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Marketo] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Introduzca o asigne el ID de la lista donde desea añadir posibles clientes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de posibles clientes]</td> 
   <td> <p>Para cada posible cliente que desee agregar a la lista, haga clic en <b>[!UICONTROL Agregar]</b>y, a continuación, introduzca o asigne el ID del posible cliente que desee añadir. Puede añadir hasta 300 posibles clientes para que el módulo se añada a la lista.</p> <p>Haga clic en el botón de asignación para asignar una colección existente de posibles clientes que desee agregar a la lista.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar posibles clientes de una lista]

Este módulo de acción elimina uno o más posibles clientes de una lista, utilizando el ID de posible cliente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Marketo] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>Introduzca o asigne el ID de la lista donde desea eliminar posibles clientes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de posibles clientes]</td> 
   <td> <p>Para cada posible cliente que desee eliminar de la lista, haga clic en <b>[!UICONTROL Agregar]</b>y, a continuación, introduzca o asigne el ID del posible cliente que desea eliminar. Puede agregar hasta 300 posibles clientes para que el módulo se elimine de la lista. </p> <p>Haga clic en el botón de alternancia de asignación para asignar una colección existente de posibles clientes que desee eliminar de la lista.</p> </td> 
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
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Marketo] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de campaña]</td> 
   <td>Introduzca o asigne el ID de la campaña que desea programar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Programar para fecha]</p> </td> 
   <td>Seleccione la fecha en la que desea que se ejecute la campaña. Si este campo se deja en blanco, la campaña se ejecuta cinco minutos después de que comience el escenario.</td> 
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
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Marketo] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de programa existente]</td> 
   <td>Introduzca o asigne el ID del programa que desea copiar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nuevo nombre del programa]</p> </td> 
   <td> <p>Escriba o asigne un nombre para el nuevo programa</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID]</td> 
   <td>Introduzca o asigne el ID de la carpeta en la que desea que se encuentre el nuevo programa.</td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

* [[!UICONTROL Registros de lista]](#list-records)
* [[!UICONTROL Registros de búsqueda]](#update-a-record)

#### [!UICONTROL Registros de lista]

Este módulo de acción recupera todos los registros de un tipo específico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Marketo] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Field]</td> 
   <td>Si ha seleccionado recuperar posibles clientes, seleccione si desea recuperar los posibles clientes de una lista o de un programa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td>Seleccione la información que desee incluir en el paquete de salida para este módulo. Los campos están disponibles según el [!UICONTROL Record Type] seleccionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Registros de búsqueda]

Este módulo de búsqueda recupera una lista de registros que coinciden con criterios de búsqueda específicos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Marketo] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Connect [!DNL Marketo] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
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
   <td>Para cada valor que desee buscar, haga clic en <b>[!UICONTROL Agregar elemento]</b> e introduzca el valor.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salida]</td> 
   <td> <p>Seleccione la información que desee incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>
