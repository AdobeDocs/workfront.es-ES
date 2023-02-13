---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos de hojas de Google
description: Para usar [!DNL Google Sheets] con [!DNL Adobe Workfront Fusion],you need the [!UICONTROL Workfront Fusion Google Sheets] extensión (opcional, pero necesaria para déclencheur instantáneos).
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 11d62222-df34-472d-93d7-f0d53eb95c9b
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3894'
ht-degree: 0%

---

# [!DNL Google Sheets] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Google Sheets], así como conectarlo a varias aplicaciones y servicios de terceros.

Para obtener instrucciones sobre cómo conectar su [!DNL Google Sheets] cuenta para [!DNL Workfront Fusion], consulte [Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

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

Para usar [!UICONTROL Hojas de Google] módulos, debe tener un [!UICONTROL Google] cuenta.

## Déclencheur

### [!UICONTROL Filas de observación]

Recupera valores de todas las filas agregadas recientemente en la hoja de cálculo.

El módulo solo recupera las filas nuevas que no se hayan rellenado anteriormente. El déclencheur no procesa una fila sobrescrita.

>[!IMPORTANT]
>
>Si la hoja de cálculo contiene una fila en blanco, no se procesará ninguna fila después de la fila en blanco.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Sheets] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Hoja de cálculo] </td> 
   <td> <p>Seleccione la hoja de cálculo que contiene la hoja que desea ver.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet] </td> 
   <td> <p>Seleccione la hoja que desee ver para una fila nueva.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL La tabla contiene encabezados]</td> 
   <td> <p> Seleccione si la hoja de cálculo contiene la fila de encabezado.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Sí]</strong> </p> <p>El módulo no recupera la fila de encabezado como datos de salida. </p> <p>Los encabezados llaman a los nombres de variables en la salida.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>El módulo también recupera la primera fila de la tabla</p> <p>Los nombres de las variables en la salida se denominan A, B, C, D, etc.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fila con encabezados] </td> 
   <td> <p>Introduzca el rango de la fila de encabezado. Por ejemplo, <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Primera fila de tabla]</td> 
   <td> <p>Introduzca el rango de la primera fila de la tabla. Por ejemplo, <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Valor render option]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Valor con formato]</p> <p>Los valores se calculan y se les da formato en la respuesta según el formato de la celda. El formato se basa en la configuración regional de la hoja de cálculo, no en la configuración regional del usuario solicitante. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y formateado como moneda, <code>A2</code> devuelve <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Valor sin formato]</p> <p>Los valores se calcularán, pero no se les aplicará formato en la respuesta. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y formateado como moneda, <code>A2</code> devolverá el número <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Formula]</p> <p>Los valores no se calculan. La respuesta incluirá las fórmulas. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y formateado como moneda, <code>A2</code> devuelve <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Opción de representación de fecha y hora]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Número de serie]</p> <p>Indica a los campos de fecha, hora, fecha y hora que se deben generar como dobles en formato de "número de serie", tal y como se rellena en Lotus 1-2-3. La parte numérica completa del valor (a la izquierda del decimal) cuenta los días desde el 30 de diciembre de 1899. La parte fraccionada (derecha del decimal) cuenta el tiempo como una fracción del día. Por ejemplo, el 1 de enero de 1900 al mediodía sería de 2,5, 2 porque son 2 días después del 30 de diciembre de 1899 y 0,5 porque el mediodía es de medio día. El 1 de febrero de 1900 a las 3 pm sería 33.625. Esto trata correctamente al año 1900 como un año bisiesto.</p> <p style="font-weight: bold;">[!UICONTROL Cadena con formato]</p> <p>Indica a los campos de fecha, hora, fecha y hora que se exporten como cadenas en su formato de número dado (que depende de la configuración regional de la hoja de cálculo).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td> <p>Establezca el número máximo de resultados que [!DNL Workfront Fusion] funcionará con durante un ciclo de ejecución.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Acciones

* [[!UICONTROL Agregar una fila]](#add-a-row)
* [[!UICONTROL Actualizar una fila]](#update-a-row)
* [[!UICONTROL Borrar una fila]](#clear-a-row)
* [[!UICONTROL Eliminar una fila]](#delete-a-row)
* [[!UICONTROL Obtener una celda]](#get-a-cell)
* [[!UICONTROL Actualizar una celda]](#update-a-cell)
* [[!UICONTROL Borrar una celda]](#clear-a-cell)
* [[!UICONTROL Agregar una hoja]](#add-a-sheet)
* [[!UICONTROL Creación de una hoja de cálculo]](#create-a-spreadsheet)
* [[!UICONTROL Eliminar una hoja]](#delete-a-sheet)
* [[!UICONTROL Realizar una llamada de API]](#make-an-api-call)

### [!UICONTROL Agregar una fila]

Este módulo añade una fila a una hoja.

Al configurar [!DNL Google Sheets] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL Google Sheets] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Sheets] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mode]</td> 
   <td> <p>Seleccione si desea seleccionar la hoja de cálculo manualmente o mediante asignación.</p> <p>Nota: La asignación manual resulta útil, por ejemplo, cuando se crea una nueva hoja de cálculo en una [!DNL Workfront Fusion] y desea agregar datos en la hoja de cálculo recién creada directamente en el escenario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja de cálculo] </td> 
   <td> <p>Seleccione el [!DNL Google] hoja de cálculo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Seleccione la hoja a la que desee añadir una fila.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Intervalo de columnas]</td> 
   <td>Seleccione el rango de columnas con el que desea trabajar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL La tabla contiene encabezados]</td> 
   <td> <p> Seleccione si la hoja de cálculo contiene la fila de encabezado.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Sí]</strong> </p> <p>El módulo no recupera la fila de encabezado como datos de salida. </p> <p>Los encabezados llaman a los nombres de variables en la salida.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>El módulo también recupera la primera fila de la tabla</p> <p>Los nombres de las variables en la salida se denominan A, B, C, D, etc.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Values] </td> 
   <td> <p>Introduzca o asigne las celdas deseadas de la fila que desee añadir.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opción de entrada de valor]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Usuario introducido]</strong></p> <p>Los valores se analizan como si el usuario los escribiera en la interfaz de usuario. Los números siguen siendo números, pero las cadenas se pueden convertir en números, fechas u otros formatos según las mismas reglas que se aplican al introducir texto en una celda mediante el [!DNL Google Sheets] IU.</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> Los valores que introduce el usuario no se analizan y se almacenan tal cual. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opción Insertar datos]</td> 
   <td> <p>Especifique cómo se cambian los datos existentes al introducir nuevos datos. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Insertar filas]</strong></p> <p>Las filas se insertan para los nuevos datos.</p> </li> 
     <li> <p><strong>[!UICONTROL Sobrescribir]</strong> </p> <p>Los nuevos datos sobrescriben los datos existentes en las áreas en las que se escriben. Al agregar datos al final de la hoja, se insertan nuevas filas o columnas para que se puedan escribir los datos.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Actualizar una fila]

Este módulo le permite cambiar el contenido de la celda en una fila seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Sheets] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mode]</td> 
   <td> <p>Seleccione si desea seleccionar la hoja de cálculo manualmente o mediante asignación.</p> <p>Nota: La asignación manual es útil, por ejemplo, cuando se crea una nueva hoja de cálculo en el escenario [!UICONTROL Workfront Fusion] y se desea agregar datos a la hoja de cálculo recién creada directamente en el escenario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja de cálculo] </td> 
   <td> <p>Seleccione el [!DNL Google] hoja de cálculo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Seleccione la hoja en la que desea actualizar una fila.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número de fila]</td> 
   <td> <p> Introduzca el número de la fila que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL La tabla contiene encabezados]</td> 
   <td> <p> Seleccione si la hoja de cálculo contiene la fila de encabezado.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Sí]</strong> </p> <p>El módulo no recupera la fila de encabezado como datos de salida. </p> <p>Los encabezados llaman a los nombres de variables en la salida.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>El módulo también recupera la primera fila de la tabla</p> <p>Los nombres de las variables en la salida se denominan A, B, C, D, etc.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Values] </td> 
   <td> <p>Introduzca o asigne los valores a las celdas deseadas de la fila que desee cambiar (actualizar).</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opción de entrada de valor]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Usuario introducido]</strong></p> <p>Los valores se analizan como si el usuario los escribiera en la interfaz de usuario. Los números siguen siendo números, pero las cadenas se pueden convertir en números, fechas u otros formatos según las mismas reglas que se aplican al introducir texto en una celda mediante el [!DNL Google Sheets] IU.</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> Los valores que introduce el usuario no se analizan y se almacenan tal cual. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Borrar una fila]

Elimina los valores de una fila especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Sheets] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja de cálculo] </td> 
   <td> <p>Seleccione el [!DNL Google] hoja de cálculo que contiene la hoja desde la que desea borrar una fila.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p> Seleccione la hoja desde la que desea borrar los datos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número de fila]</td> 
   <td> <p>Introduzca el número de la fila desde la que desea borrar los datos. Por ejemplo, <code> 23</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eliminar una fila]

Elimina una fila especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Sheets] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja de cálculo] </td> 
   <td> <p>Seleccione la hoja de cálculo de Google que contiene la hoja desde la que desea eliminar una fila.</p> </td> 
  </tr> 
  <tr> 
   <td>Hoja </td> 
   <td> <p>Seleccione la hoja desde la que desea eliminar una fila.</p> </td> 
  </tr> 
  <tr> 
   <td>Número de fila</td> 
   <td> <p>Introduzca el número de la fila que desea eliminar. Ejemplo: <code>23</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obtener una celda]

Recupera un valor de una celda seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Sheets] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja de cálculo] </td> 
   <td> <p>Seleccione el [!DNL Google] hoja de cálculo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Seleccione la hoja que contiene la celda desde la que desea recuperar los datos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cell] </td> 
   <td> <p>Introduzca el ID de la celda desde la que desea recuperar los datos. Ejemplo: <code>A6</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valor render option]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Valor con formato]</p> <p>Los valores se calculan y se les da formato en la respuesta según el formato de la celda. El formato se basa en la configuración regional de la hoja de cálculo, no en la configuración regional del usuario solicitante. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y formateado como moneda, <code>A2</code> devuelve <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Unformatted value]</p> <p>Los valores se calcularán, pero no se les aplicará formato en la respuesta. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y formateado como moneda, <code>A2</code> devolverá el número <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Formula]</p> <p>Los valores no se calculan. La respuesta incluirá las fórmulas. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y formateado como moneda, <code>A2</code> devuelve <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Date and time render option]</td> 
   <td> <p style="font-weight: bold;">[!DNL Serial number]</p> <p>Indica a los campos de fecha, hora, fecha y hora que se deben generar como dobles en formato de "número de serie", tal y como se rellena en Lotus 1-2-3. La parte numérica completa del valor (a la izquierda del decimal) cuenta los días desde el 30 de diciembre de 1899. La parte fraccionada (derecha del decimal) cuenta el tiempo como una fracción del día. Por ejemplo, el 1 de enero de 1900 al mediodía sería de 2,5, 2 porque son 2 días después del 30 de diciembre de 1899 y 0,5 porque el mediodía es de medio día. El 1 de febrero de 1900 a las 3 pm sería 33.625. Esto trata correctamente al año 1900 como un año bisiesto.</p> <p style="font-weight: bold;">[!DNL Formatted string]</p> <p>Indica a los campos de fecha, hora, fecha y hora que se exporten como cadenas en su formato de número dado (que depende de la configuración regional de la hoja de cálculo).</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Actualizar una celda]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Sheets] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja de cálculo] </td> 
   <td> <p>Seleccione el [!DNL Google] hoja de cálculo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cell] </td> 
   <td> <p>Introduzca el ID de la celda que desea actualizar. Ejemplo: <code>A5</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valor]</td> 
   <td> <p>Introduzca el nuevo valor de la celda.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opción de entrada de valor]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Usuario introducido]</strong></p> <p>Los valores se analizan como si el usuario los escribiera en la interfaz de usuario. Los números siguen siendo números, pero las cadenas se pueden convertir en números, fechas u otros formatos según las mismas reglas que se aplican al introducir texto en una celda mediante el [!DNL Google Sheets] IU.</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> Los valores que introduce el usuario no se analizan y se almacenan tal cual. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Borrar una celda]

Elimina un valor de una celda especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Sheets] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja de cálculo] </td> 
   <td> <p>Seleccione la hoja de cálculo de Google que contiene la hoja desde la que desea borrar una celda.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Seleccione la hoja desde la que desea borrar una celda.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cell] </td> 
   <td> <p>Introduzca el ID de la celda que desea borrar. Ejemplo: <code>A5</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Agregar una hoja]

Crea una hoja nueva en una hoja de cálculo seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Sheets] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja de cálculo] </td> 
   <td> <p>Seleccione la hoja de cálculo de Google donde desee agregar una hoja.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Propiedades]</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">[!UICONTROL Title]</p> <p>Introduzca el nombre de la nueva hoja.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Index]</p> <p>Introduzca la posición de la hoja. El valor predeterminado es 0 (coloca la hoja en primer lugar)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Creación de una hoja de cálculo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Sheets] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title] </td> 
   <td> <p>Introduzca el nombre de una nueva hoja de cálculo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Configuración regional]</td> 
   <td> <p>Introduzca la configuración regional de la hoja de cálculo en uno de los siguientes formatos:</p> 
    <ul> 
     <li>un código de idioma ISO 639-1 como <code>en</code></li> 
     <li>un código de idioma ISO 639-2 como <code>haw</code>, si no existe ningún código 639-1</li> 
     <li>una combinación del código de idioma ISO y el código de país, como <code>en_US</code></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Intervalo de cálculo]</td> 
   <td> <p>Cantidad de tiempo de espera antes de que se recalculen las funciones volátiles:</p> <p style="font-weight: bold;">[!UICONTROL On change]</p> <p>Las funciones volátiles se actualizan en cada cambio.</p> <p style="font-weight: bold;">[!UICONTROL On change and every minute]</p> <p>Las funciones volátiles se actualizan cada cambio y cada minuto.</p> <p style="font-weight: bold;">[!UICONTROL En caso de cambio y por hora]</p> <p>Las funciones volátiles se actualizan con cada cambio y cada hora.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Time zone]</td> 
   <td> <p> Seleccione la zona horaria de la hoja de cálculo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Formato de número]</td> 
   <td> <p>Seleccione el formato predeterminado de todas las celdas de la hoja de cálculo.</p> <p><strong>[!UICONTROL Texto]</strong>: Formato de texto. Ejemplo: <code>1000. 12</code></p> <p><strong>[!UICONTROL Number]</strong>: Formato de número. Ejemplo: <code>1,000.12</code></p> <p><strong>[!UICONTROL Porcentaje]</strong>: Formato porcentual. Ejemplo: <code>10. 12%</code></p> <p><strong>[!UICONTROL Moneda]</strong>: Formato de moneda. Ejemplo: <code>$1,000.12</code></p> <p><strong>[!UICONTROL Date]</strong>: Formato de fecha. Ejemplo: <code>9/26/2008</code></p> <p><strong>[!UICONTROL Time]</strong>: Formato de hora. Ejemplo: <code>3:59:00 PM</code></p> <p><strong>[!UICONTROL Fecha y hora]</strong>: Formato de fecha y hora. Ejemplo: <code>9/26/08 15:59:00</code> </p> <p><strong>[!UICONTROL Científico]</strong>Formato científico de números. Ejemplo: <code>1. 01E+03</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheets] </td> 
   <td> <p>Haga clic en <strong>[!UICONTROL Agregar]</strong> para agregar una hoja a la hoja de cálculo. Para cada hoja, introduzca o asigne un título para la hoja y el índice de la hoja. Un índice de 0 representa la primera hoja.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eliminar una hoja]

Elimina una hoja específica.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Sheets] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja de cálculo] </td> 
   <td> <p>Seleccione el [!DNL Google] hoja de cálculo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Seleccione la hoja que desee eliminar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Realizar una llamada de API]

Este módulo de acción le permite realizar una llamada API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [aplicación de fusión] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>Especifique una ruta relativa a <code>https://sheets.googleapis.com/v4/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada a la API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de un objeto JSON estándar. Por ejemplo, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] añade los encabezados de autorización por usted.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p> Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:   <p>Al utilizar afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Búsquedas

* [[!UICONTROL Buscar filas]](#search-rows)
* [[!UICONTROL Filas de búsqueda (avanzadas)]](#search-rows-advanced)
* [[!UICONTROL Obtener valores de rango]](#get-range-values)
* [[!UICONTROL Hojas de lista]](#list-sheets)

### [!UICONTROL Buscar filas]

Busca filas mediante las opciones de filtro.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [aplicación de fusión] a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja de cálculo] </td> 
   <td> <p>Seleccione el [!DNL Google] hoja de cálculo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Seleccione la hoja en la que desea buscar las filas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL La tabla contiene encabezados]</td> 
   <td> <p> Seleccione si la hoja de cálculo contiene la fila de encabezado. Si la opción [!UICONTROL Yes] está seleccionada, el módulo no recupera la fila del encabezado, ya que los encabezados llaman a los datos de salida y los nombres de variables en la salida. Si la opción [!UICONTROL No] está seleccionada, el módulo también recupera la primera fila de la tabla y los nombres de las variables en la salida se llaman simplemente A, B, C, D, etc.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Intervalo de columnas]</td> 
   <td>Seleccione el rango de columnas con el que trabajar. Ejemplo: <code>A-F</code></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Filtro]</td> 
   <td> <p>Establezca el filtro para la fila que desea buscar.</p> <p>Para obtener más información sobre los filtros, consulte <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Añadir un filtro a un escenario en [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Orden]</td> 
   <td>Seleccione si desea ordenar ascendente o descendente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Order by]</td> 
   <td>Elija la columna por la que desea ordenar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valor render option]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Valor con formato]</p> <p>Los valores se calculan y se les da formato en la respuesta según el formato de la celda. El formato se basa en la configuración regional de la hoja de cálculo, no en la configuración regional del usuario solicitante. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y formateado como moneda, <code>A2</code> devuelve <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Valor sin formato]</p> <p>Los valores se calcularán, pero no se les aplicará formato en la respuesta. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y formateado como moneda, <code>A2</code> devolverá el número <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Formula]</p> <p>Los valores no se calculan. La respuesta incluirá las fórmulas. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y formateado como moneda, <code>A2</code> devuelve <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opción de representación de fecha y hora]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Número de serie]</p> <p>Indica a los campos de fecha, hora, fecha y hora que se emitan como dobles en formato de "número de serie", tal como se populariza en Lotus 1-2-3. La parte numérica completa del valor (a la izquierda del decimal) cuenta los días desde el 30 de diciembre de 1899. La parte fraccionada (derecha del decimal) cuenta el tiempo como una fracción del día. Por ejemplo, el 1 de enero de 1900 al mediodía sería de 2,5, 2 porque son 2 días después del 30 de diciembre de 1899 y 0,5 porque el mediodía es de medio día. El 1 de febrero de 1900 a las 3 pm sería 33.625. Esto trata correctamente al año 1900 como un año bisiesto.</p> <p style="font-weight: bold;">[!UICONTROL Cadena con formato]</p> <p>Indica a los campos de fecha, hora, fecha y hora que se exporten como cadenas en su formato de número dado (que depende de la configuración regional de la hoja de cálculo).</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de filas devueltas]</td> 
   <td>Establezca el número máximo de filas que [!DNL Workfront Fusion] volverá durante un ciclo de ejecución.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Filas de búsqueda (avanzadas)]

Devuelve los resultados que coinciden con los criterios dados.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Sheets] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja de cálculo] </td> 
   <td> <p>Seleccione la hoja de cálculo de Google que contiene la hoja que desea buscar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Seleccione la hoja que contiene las filas que desea buscar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query]</td> 
   <td> <p>Utilice la variable [!DNL Google Charts Query Language]. Ejemplo: <code>select * where B = "John"</code></p> <p>Para obtener más información, consulte [!DNL Google Charts Query Language], consulte <a href="https://developers.google.com/chart/interactive/docs/querylanguage">Referencia del lenguaje de consulta</a> en el [!DNL Google] documentación.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obtener valores de rango]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Sheets] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja de cálculo] </td> 
   <td> <p>Seleccione el [!DNL Google] hoja de cálculo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Seleccione la hoja desde la que desea obtener el contenido del rango.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Range] </td> 
   <td> <p>Introduzca el rango que desea obtener. Ejemplo: <code>A1:D25</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL La tabla contiene encabezados]</td> 
   <td> <p>Marque esta casilla si la hoja tiene una fila de encabezado</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fila con encabezados]</td> 
   <td>Introduzca el rango de los encabezados de tabla. Ejemplo <code>A1:F1</code>. Si deja vacío el campo, [!DNL Workfront Fusion] supondrá que el encabezado está en la primera fila del intervalo especificado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valor render option]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Valor con formato]</p> <p>Los valores se calculan y se les da formato en la respuesta según el formato de la celda. El formato se basa en la configuración regional de la hoja de cálculo, no en la configuración regional del usuario solicitante. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y formateado como moneda, <code>A2</code> devuelve <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Valor sin formato]</p> <p>Los valores se calcularán, pero no se les aplicará formato en la respuesta. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y formateado como moneda, <code>A2</code> devolverá el número <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Formula]</p> <p>Los valores no se calculan. La respuesta incluirá las fórmulas. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y formateado como moneda, <code>A2</code> devuelve <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opción de representación de fecha y hora]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Número de serie]</p> <p>Indica a los campos de fecha, hora, fecha y hora que se emitan como dobles en formato de "número de serie", tal como se populariza en Lotus 1-2-3. La parte numérica completa del valor (a la izquierda del decimal) cuenta los días desde el 30 de diciembre de 1899. La parte fraccionada (derecha del decimal) cuenta el tiempo como una fracción del día. Por ejemplo, el 1 de enero de 1900 al mediodía sería de 2,5, 2 porque son 2 días después del 30 de diciembre de 1899 y 0,5 porque el mediodía es de medio día. El 1 de febrero de 1900 a las 3 pm sería 33.625. Esto trata correctamente al año 1900 como un año bisiesto.</p> <p style="font-weight: bold;">[!UICONTROL Cadena con formato]</p> <p>Indica a los campos de fecha, hora, fecha y hora que se exporten como cadenas en su formato de número dado (que depende de la configuración regional de la hoja de cálculo).</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Hojas de lista]

Este módulo devuelve una lista de todas las hojas de una hoja de cálculo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Sheets] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja de cálculo] </td> 
   <td> <p>Seleccione el [!DNL Google] hoja de cálculo que contiene las hojas que desea enumerar.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Límites de uso

Si el error `429: RESOURCE_EXHAUSTED` se produce, ha superado el límite de velocidad de API.

La variable [!DNL Google Sheets] La API tiene un límite de 500 solicitudes por 100 segundos por proyecto y 100 solicitudes por 100 segundos por usuario. Los límites de las lecturas y escrituras se rastrean por separado. No hay límite de uso diario.

Consulte más detalles en [developers.google.com/sheets/api/limits](https://developers.google.com/sheets/api/limits).

## Sugerencias y trucos

* [Cómo obtener celdas vacías de una [!DNL Google] Hoja](#how-to-get-empty-cells-from-a-google-sheet)
* [Añadir un botón en una hoja para ejecutar un escenario](#add-a-button-in-a-sheet-to-run-a-scenario)

### Cómo obtener celdas vacías de una [!DNL Google Sheet]

Utilice la variable [!UICONTROL Filas de búsqueda (avanzadas)] módulo y utilice esta fórmula para obtener las columnas que están vacías.
<pre>seleccione * [!UICONTROL donde E es nulo ​]</pre>Aquí "E" es la columna y "es nulo" es la condición. Puede crear una consulta más avanzada utilizando [Google Query Lang.](https://developers.google.com/chart/interactive/docs/querylanguage)

### Añadir un botón en una hoja para ejecutar un escenario

1. En [!DNL Workfront Fusion], inserte el **[!UICONTROL Weblock]** > **[!UICONTROL Enlaces web personalizados]** módulo/déclencheur en el escenario y configúrelo (consulte [Enlaces web](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md)).

1. Copie la URL del vínculo web.
1. Ejecute el escenario.
1. En hojas de Google, elija **[!UICONTROL Insertar]** > **[!UICONTROL Dibujo]**... en la barra de menús principal.

1. En el [!UICONTROL Dibujo] , haga clic en el botón **[!UICONTROL Cuadro de texto]** icono ![](assets/text-box.png) cerca de la parte superior de la ventana.
1. Diseñe un botón y haga clic en el botón **[!UICONTROL Guardar y cerrar]** en la esquina superior derecha:
1. El botón se colocará en la hoja de cálculo. Haga clic en los tres puntos verticales en la esquina superior derecha del botón:
1. Choose **[!UICONTROL Asignar secuencia de comandos.].** del menú .
1. Introduzca el nombre de la secuencia de comandos (función), por ejemplo `runScenario` y haga clic en **[!UICONTROL OK]**:
1. Choose **[!UICONTROL Herramientas]** > **[!UICONTROL Editor de secuencias de comandos]** en la barra de menús principal.

1. Inserte el siguiente código:

   * El nombre de la función debe corresponder al nombre especificado en el paso 9.
   * Reemplace la URL con la URL del enlace web que copió en el paso 2.

      <pre>function runScenario() {</pre><pre>UrlFetchApp.fetch("<webhook you copied>")</pre><pre>}</pre>

1. Press **[!UICONTROL Ctrl + S]** para guardar el archivo de secuencia de comandos, introduzca un nombre de proyecto y haga clic en **[!UICONTROL OK]**.

1. Vuelva a cambiar a [!DNL Google Sheets] y haga clic en el botón nuevo.
1. Conceda la autorización necesaria a la secuencia de comandos:
1. En [!DNL Workfront Fusion], compruebe que el escenario se haya ejecutado correctamente.

## Almacenamiento de fechas en una hoja de cálculo

Si almacena un valor Fecha en una hoja de cálculo sin ningún formato, aparecerá en la hoja de cálculo como texto en formato ISO 8601. Sin embargo, [!DNL Google Sheets] fórmulas o funciones que funcionan con fechas que no comprenden este texto (ejemplo: fórmula `=A1+10`) mostrará el siguiente error:

![](assets/mceclip6-350x87.png)

Para ayudar a permitir [!DNL Google Sheets] para comprender la fecha, aplique el formato con la variable [[!UICONTROL formatDate] (fecha; formato; [zona horaria]](../../workfront-fusion/functions/date-and-time-functions.md#formatda) función. El formato correcto pasado a la función como segundo argumento depende de la configuración regional de la hoja de cálculo.

Para determinar el formato correcto:

1. Choose **[!UICONTROL Archivo]** > **[!UICONTROL Hoja de cálculo]** en el menú principal para comprobar/establecer la configuración regional.

1. Una vez que haya comprobado/establecido la configuración regional adecuada, determine el formato de fecha y hora correspondiente eligiendo **[!UICONTROL Formato]** > **[!UICONTROL Número]** del menú principal. El formato se muestra junto al elemento de menú Fecha y hora :

1. Para componer el formato correcto que debe pasarse al [!UICONTROL formatDate()] , consulte la lista de [Tokens para el formato de fecha y hora en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md).

**Ejemplo:** El uso de `MM/DD/YYYY HH:mm:ss` para la configuración regional de Estados Unidos:

![](assets/locale-time-350x83.png)

## Explotación [!DNL Google Sheets] funciones

Si se pierde una función integrada, pero esta función la presenta [!DNL Google Sheets], puede explotarlo. Para obtener más información, consulte [Uso [!DNL Google Sheets] funciones](../../workfront-fusion/functions/map-using-functions.md#exploiti) en [Asignación de elementos mediante funciones en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md) .

## Keep [!DNL Google Sheets] de cambiar números a fechas

Podría encontrar que una cadena de números que está utilizando como texto se está interpretando como una fecha en un [!DNL Google] hoja de cálculo. Por ejemplo, escriba 1-2019, con la intención de que sea texto, pero Google lo interpretará como una fecha. Puede predar formato al número como texto sin formato para evitarlo.

1. En [!DNL Google Sheets], resalte la columna o celda que contiene el número o los números.
1. Haga clic en **[!UICONTROL Formato]** > **[!UICONTROL Número]** > **[!UICONTROL Texto sin formato]**.

Otra solución alternativa a [!DNL Workfront Fusion] es escribir un apóstrofo (&#39;) antes de un número, por ejemplo, &quot;1-2019 o &quot;1/47&quot;. El apóstrofo no se muestra en la celda después de enviar los datos desde [!DNL Workfront Fusion].
