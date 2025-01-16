---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Formularios de Google
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 45c86879-bc4e-4134-b63c-02410b9de43b
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1493'
ht-degree: 92%

---

# Módulos de [!DNL Google Forms]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Módulos Google Forms](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-forms-modules.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Los módulos [!DNL Adobe Workfront Fusion] de [!DNL Google Forms] permiten supervisar, seleccionar, añadir, actualizar o eliminar respuestas en sus [!DNL Google Forms].

Para usar [!DNL Google Docs] con [!DNL Adobe Workfront Fusion], es necesario tener una cuenta de [!DNL Google]. Si todavía no tiene una cuenta de [!DNL Google], puede crearla en la página de ayuda de la cuenta [!DNL Google].

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

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

Para usar módulos [!DNL Google Forms], debe tener una cuenta de [!DNL Google].

## Información de API de Google Forms

El conector de Google Forms utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>2.0.10</td> 
  </tr>
 </tbody> 
 </table>

## Creación de una hoja de cálculo a partir del formulario

Para trabajar con las respuestas del formulario, se debe crear la hoja de cálculo de las respuestas.

1. Abra el formulario.
1. Vaya a la pestaña **[!UICONTROL Responses]**.
1. Haga clic en el icono **[!UICONTROL Create Spreadsheet]** ![](assets/spreadsheet-icon.png).

1. Seleccione si desea crear una hoja de cálculo nueva o usar una existente
1. Haga clic en **[!UICONTROL Crear]**.

## Módulos de [!DNL Google Forms] y sus campos

Al configurar módulos de [!DNL Google Forms], [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Google Forms] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. El título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Activadores](#triggers)
* [Acciones](#actions)
* [Búsquedas](#searches)

### Activadores

#### [!UICONTROL Watch Responses]

Inspecciona el formulario en busca de nuevas respuestas.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conexión de la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creación de un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Spreadsheet]</td> 
   <td> <p>Seleccione la hoja de cálculo que contiene las respuestas del formulario que desea ver en busca de nuevas respuestas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet]</td> 
   <td> <p> Seleccione la hoja que contiene las respuestas del formulario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Row with headers]</td> 
   <td>Especifique la fila de encabezado de la tabla. La fila predeterminada es <code>A1:Z1</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Value Render Option]</td> 
   <td> <p>Especifique cómo desea que se muestren los valores en la salida.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formatted value]</strong> </p> <p>Los valores se calculan y se les aplica formato en la respuesta según el formato de la celda. El formato se basa en la configuración regional de la hoja de cálculo, no en la configuración regional del usuario solicitante. Por ejemplo, si <code>A1</code> es <code>1. 23</code> y <code>A2 </code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devuelve <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Unformatted value]</strong> </p> <p>Los valores se calculan, pero no se les aplica formato en la respuesta. Por ejemplo, si <code>A1</code> es <code>1. 23</code> y <code>A2 </code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devuelve el número <code>1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Formula]</strong> </p> <p>Los valores no se calculan. La respuesta incluye las fórmulas. Por ejemplo, si <code>A1</code> es <code>1. 23</code> y <code>A2 </code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devuelve <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Date and time render option]</td> 
   <td>Seleccione cómo desea que se muestren las fechas, las horas y la duración en la salida. Este campo se omite si [!UICONTROL Value Render Option] se ha establecido como [!UICONTROL Formatted Value].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p> Establezca el número máximo de respuestas con las que trabaja [!DNL Workfront Fusion] durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Añadir una respuesta]](#add-a-response)
* [[!UICONTROL Actualizar una respuesta]](#update-a-response)
* [[!UICONTROL Eliminar una respuesta]](#delete-a-response)

#### [!UICONTROL Añadir una respuesta]

Este módulo anexa una nueva respuesta a la parte inferior de la hoja de cálculo del formulario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conexión de la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creación de un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Spreadsheet]</td> 
   <td> <p>Seleccione la hoja de cálculo que contiene la hoja a la que desea añadir una respuesta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet]</td> 
   <td> <p> Seleccione la hoja que contiene las respuestas del formulario.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Values]</p> </td> 
   <td> <p>Introduzca los valores deseados en las columnas de la hoja.</p> <p>Para la columna [!UICONTROL Timestamp] con el formato correcto, utilice el siguiente valor:</p><pre>formatDate (ahora;DD/MM/AAAA HH:mm;UTC)</pre> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Value input option]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> Los valores que introduce el usuario no se analizan y se almacenan tal cual. </p> </li> 
     <li> <p><strong>[!UICONTROL User entered]</strong></p> <p>Los valores se analizan como si el usuario los hubiera escrito en la IU. Los números siguen siendo números, pero las cadenas se pueden convertir en números, fechas u otros formatos siguiendo las mismas reglas que se aplican al escribir texto en una celda a través de la interfaz de usuario de [!DNL Google Sheets].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Insert data option]</td> 
   <td> <p>Especifique cómo se cambian los datos existentes al introducir nuevos datos. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Overwrite]</strong> </p> <p>Los nuevos datos sobrescriben los datos existentes en las áreas donde se escriben. Al añadir datos al final de la hoja, se insertan nuevas filas o columnas para poder escribir los datos.</p> </li> 
     <li> <p><strong>[!UICONTROL Insert rows]</strong></p> <p>Las filas se insertan para los nuevos datos.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar una respuesta]

Este módulo actualiza la respuesta seleccionada.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conexión de la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creación de un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Spreadsheet]</td> 
   <td> <p>Seleccione la hoja de cálculo que contiene la hoja en la que desea actualizar una respuesta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet]</td> 
   <td> <p> Seleccione la hoja que contiene las respuestas del formulario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Row number]</p> </td> 
   <td> <p>Introduzca o asigne el número de la fila que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Values]</p> </td> 
   <td> <p>Introduzca los nuevos valores en las columnas deseadas.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Value input option]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> Los valores que introduce el usuario no se analizan y se almacenan tal cual. </p> </li> 
     <li> <p><strong>[!UICONTROL User entered]</strong></p> <p>Los valores se analizan como si el usuario los hubiera escrito en la IU. Los números siguen siendo números, pero las cadenas se pueden convertir en números, fechas u otros formatos siguiendo las mismas reglas que se aplican al escribir texto en una celda a través de la interfaz de usuario de [!DNL Google Sheets].</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar una respuesta]

Este módulo elimina una respuesta seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conexión de la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creación de un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Spreadsheet]</td> 
   <td> <p>Seleccione la hoja de cálculo que contiene la hoja en la que desea eliminar una respuesta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet]</td> 
   <td> <p> Seleccione la hoja que contiene las respuestas del formulario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Row number]</p> </td> 
   <td> <p>Introduzca o asigne el número de la fila que desea eliminar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

* [[!UICONTROL Búsqueda de respuestas]](#search-responses)
* [[!UICONTROL Búsqueda de respuestas (avanzada])](#search-responses-advanced)

#### [!UICONTROL Búsqueda de respuestas]

Este módulo devuelve respuestas que coinciden con los criterios especificados.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
    <td>Conexión</td>
   <td> <p>Para obtener instrucciones sobre la conexión de su cuenta de [!DNL Google] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Spreadsheet]</td>
   <td> <p>Seleccione el formulario en el que desea buscar.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Sheet] </td>
   <td> <p>Seleccione la hoja que contiene las respuestas del formulario.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Column range]</td>
   <td> <p> Seleccione el rango de columnas que desea buscar.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Defina el filtro por el que desea buscar respuestas.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Sort Order] </td>
   <td> <p>Seleccione si desea ordenar las respuestas devueltas en orden ascendente o descendente.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Order By]</td>
   <td> <p> Seleccione la columna por la que desea ordenar las respuestas devueltas.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Value Render Option]</td> 
   <td> <p>Especifique cómo desea que se muestren los valores en la salida.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formatted value]</strong></p> <p>Los valores se calculan y se les aplica formato en la respuesta según el formato de la celda. El formato se basa en la configuración regional de la hoja de cálculo, no en la configuración regional del usuario solicitante. Por ejemplo, si <code>A1</code> es <code>1. 23</code> y <code>A2 </code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devuelve <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Unformatted value]</strong> </p> <p>Los valores se calculan, pero no se les aplica formato en la respuesta. Por ejemplo, si <code>A1</code> es <code>1. 23</code> y <code>A2 </code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devuelve el número <code>1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL Formula]</strong> </p> <p>Los valores no se calculan. La respuesta incluye las fórmulas. Por ejemplo, si <code>A1</code> es <code>1. 23</code> y <code>A2 </code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devuelve <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Date and time render option]</td>
    <td>Seleccione cómo desea que se muestren las fechas, las horas y la duración en la salida. Este campo se omite si la opción [!UICONTROL Value Render] está establecida como valor con formato. </td>
  </tr> 
  <tr>
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Maximum number of returned responses]</td>
   <td> <p> Establezca el número máximo de respuestas que [!DNL Workfront Fusion] devuelve durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Búsqueda de respuestas (avanzada)]

Este módulo realiza una búsqueda utilizando [[!DNL Google Charts Query Language]](https://developers.google.com/chart/interactive/docs/querylanguage). Este módulo no devuelve un número de fila.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conexión de la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Creación de un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Spreadsheet]</td>
   <td> <p>Seleccione la hoja de cálculo que contiene la hoja que desea buscar.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Sheet]</td>
   <td> <p> Seleccione la hoja que contiene las respuestas del formulario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Defina la consulta de búsqueda utilizando <a href="https://developers.google.com/chart/interactive/docs/querylanguage">[!DNL Google Charts Query Language]</a>.</p> <p>Ejemplo: <code>select * where C = "John"</code> recupera todos los valores de la fila donde la columna C es “John”.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Maximum number of returned rows]</td>
   <td> <p> Establezca el número máximo de respuestas que [!DNL Workfront Fusion] devuelve durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>
