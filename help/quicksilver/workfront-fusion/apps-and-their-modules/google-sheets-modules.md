---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de hojas de Google
description: Para usar [!DNL Google Sheets] con [!DNL Adobe Workfront Fusion],you need the [!UICONTROL Workfront Fusion Google Sheets] extensión (opcional, pero necesaria para déclencheur instantáneos).
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 11d62222-df34-472d-93d7-f0d53eb95c9b
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '4023'
ht-degree: 0%

---

# [!DNL Google Sheets] módulos

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!DNL Google Sheets], así como conectarlo a varias aplicaciones y servicios de terceros.

Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Sheets] a [!DNL Workfront Fusion], vea [Crear una conexión a [!DNL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

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
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
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

Para usar módulos de [!UICONTROL Google Sheets], debes tener una cuenta de [!UICONTROL Google].

## Información de API de hojas de Google

El conector de Google Sheets utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL básica</td> 
   <td> https://sheets.googleapis.com/v4</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Versión de API</td> 
   <td> v4 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 2.5.7</td> 
  </tr>
 </tbody> 
 </table>

## Déclencheur

### [!UICONTROL Filas de inspección]

Recupera valores de cada fila recién agregada en la hoja de cálculo.

El módulo recupera únicamente las filas nuevas que no se hayan rellenado anteriormente. El déclencheur no procesará una fila sobrescrita.

>[!IMPORTANT]
>
>Si la hoja de cálculo contiene una fila en blanco, no se procesará ninguna fila después de la fila en blanco.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Sheets] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Hoja de cálculo de [!UICONTROL] </td> 
   <td> <p>Seleccione la hoja de cálculo que contiene la hoja que desea inspeccionar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Hoja] </td> 
   <td> <p>Seleccione la hoja que desee inspeccionar para buscar una fila nueva.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL La tabla contiene encabezados]</td> 
   <td> <p> Seleccione si la hoja de cálculo contiene la fila de encabezado.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Sí]</strong> </p> <p>El módulo no recupera la fila de encabezado como datos de salida. </p> <p>Los encabezados llaman a los nombres de las variables en la salida.</p> </li> 
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
   <td role="rowheader"> <p>[!UICONTROL Opción de procesamiento de valor]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Valor con formato]</p> <p>Los valores se calculan y se les aplica formato en la respuesta según el formato de la celda. El formato se basa en la configuración regional de la hoja de cálculo, no en la del usuario solicitante. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devolvería <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Valor sin formato]</p> <p>Los valores se calculan, pero no se les aplica formato en la respuesta. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devolvería el número <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Fórmula]</p> <p>Los valores no se calculan. La respuesta incluirá las fórmulas. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devolvería <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Opción de procesamiento de fecha y hora]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Número de serie]</p> <p>Indica a los campos de fecha, hora, fecha y hora que deben aparecer como valores dobles en formato de "número de serie", tal como lo ha popularizado Lotus 1-2-3. La parte del número entero del valor (a la izquierda del decimal) cuenta los días transcurridos desde el 30 de diciembre de 1899. La parte fraccionaria (a la derecha del decimal) cuenta la hora como una fracción del día. Por ejemplo, el 1 de enero de 1900 al mediodía sería 2,5, 2 porque son 2 días después del 30 de diciembre de 1899 y 0,5 porque el mediodía es medio día. El 1 de febrero de 1900 a las 3 de la tarde sería 33.625. Esto trata correctamente el año 1900 como un año no bisiesto.</p> <p style="font-weight: bold;">[!UICONTROL Cadena con formato]</p> <p>Indica a los campos de fecha, hora, fecha y hora que se muestren como cadenas en el formato de número especificado (que depende de la configuración regional de la hoja de cálculo).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td> <p>Establezca el número máximo de resultados con los que trabajará [!DNL Workfront Fusion] durante un ciclo de ejecución.</p> </td> 
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
* [[!UICONTROL Crear una hoja de cálculo]](#create-a-spreadsheet)
* [[!UICONTROL Eliminar una hoja]](#delete-a-sheet)
* [[!UICONTROL Realizar una llamada API]](#make-an-api-call)

### [!UICONTROL Agregar una fila]

Este módulo anexa una fila a una hoja.

Al configurar [!DNL Google Sheets] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Google Sheets] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Sheets] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modo]</td> 
   <td> <p>Seleccione si desea seleccionar la hoja de cálculo y la hoja manualmente o mediante asignación.</p> <p>Nota: La asignación manual resulta útil, por ejemplo, cuando se crea una hoja de cálculo nueva en un escenario de [!DNL Workfront Fusion] y desea agregar datos directamente en el escenario a la hoja de cálculo recién creada.</p> </td> 
  </tr> 
  <tr> 
   <td>Hoja de cálculo de [!UICONTROL] </td> 
   <td> <p>Seleccione la hoja de cálculo [!DNL Google].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja] </td> 
   <td> <p>Seleccione la hoja a la que desee agregar una fila.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rango de columnas]</td> 
   <td>Seleccione el rango de columnas con el que desea trabajar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL La tabla contiene encabezados]</td> 
   <td> <p> Seleccione si la hoja de cálculo contiene la fila de encabezado.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Sí]</strong> </p> <p>El módulo no recupera la fila de encabezado como datos de salida. </p> <p>Los encabezados llaman a los nombres de las variables en la salida.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>El módulo también recupera la primera fila de la tabla</p> <p>Los nombres de las variables en la salida se denominan A, B, C, D, etc.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valores] </td> 
   <td> <p>Introduzca o asigne las celdas deseadas de la fila que desee añadir.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opción de entrada de valor]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Usuario introducido]</strong></p> <p>Los valores se analizan como si el usuario los hubiera escrito en la interfaz de usuario. Los números siguen siendo números, pero las cadenas se pueden convertir en números, fechas u otros formatos siguiendo las mismas reglas que se aplican al escribir texto en una celda a través de la interfaz de usuario de [!DNL Google Sheets].</p> </li> 
     <li> <p><strong>[!UICONTROL RAW]</strong> </p> <p> Los valores que introduce el usuario no se analizan y se almacenan tal cual. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Insertar opción de datos]</td> 
   <td> <p>Especifique cómo se cambian los datos existentes al introducir nuevos datos. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Insertar filas]</strong></p> <p>Las filas se insertan para los nuevos datos.</p> </li> 
     <li> <p><strong>[!UICONTROL Sobrescribir]</strong> </p> <p>Los nuevos datos sobrescriben los datos existentes en las áreas en las que se escriben. Al agregar datos al final de la hoja, se insertan nuevas filas o columnas para poder escribir los datos.</p> </li> 
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
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Sheets] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Modo]</td> 
   <td> <p>Seleccione si desea seleccionar la hoja de cálculo y la hoja manualmente o mediante asignación.</p> <p>Nota: La asignación manual resulta útil, por ejemplo, cuando se crea una nueva hoja de cálculo en el escenario [!UICONTROL Workfront Fusion] y se desea agregar datos a la hoja de cálculo recién creada directamente en el escenario.</p> </td> 
  </tr> 
  <tr> 
   <td>Hoja de cálculo de [!UICONTROL] </td> 
   <td> <p>Seleccione la hoja de cálculo [!DNL Google].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja] </td> 
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
     <li> <p><strong>[!UICONTROL Sí]</strong> </p> <p>El módulo no recupera la fila de encabezado como datos de salida. </p> <p>Los encabezados llaman a los nombres de las variables en la salida.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>El módulo también recupera la primera fila de la tabla</p> <p>Los nombres de las variables en la salida se denominan A, B, C, D, etc.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valores] </td> 
   <td> <p>Introduzca o asigne los valores a las celdas deseadas de la fila que desea cambiar (actualizar).</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opción de entrada de valor]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Usuario introducido]</strong></p> <p>Los valores se analizan como si el usuario los hubiera escrito en la interfaz de usuario. Los números siguen siendo números, pero las cadenas se pueden convertir en números, fechas u otros formatos siguiendo las mismas reglas que se aplican al escribir texto en una celda a través de la interfaz de usuario de [!DNL Google Sheets].</p> </li> 
     <li> <p><strong>[!UICONTROL RAW]</strong> </p> <p> Los valores que introduce el usuario no se analizan y se almacenan tal cual. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Borrar una fila]

Elimina valores de una fila especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Sheets] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Hoja de cálculo de [!UICONTROL] </td> 
   <td> <p>Seleccione la hoja de cálculo [!DNL Google] que contiene la hoja de cálculo de la que desea borrar una fila.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja] </td> 
   <td> <p> Seleccione la hoja de la que desea borrar los datos.</p> </td> 
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
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Sheets] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Hoja de cálculo de [!UICONTROL] </td> 
   <td> <p>Seleccione la hoja de cálculo de Google que contiene la hoja en la que desea eliminar una fila.</p> </td> 
  </tr> 
  <tr> 
   <td>Hoja </td> 
   <td> <p>Seleccione la hoja de la que desea eliminar una fila.</p> </td> 
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
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Sheets] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Hoja de cálculo de [!UICONTROL] </td> 
   <td> <p>Seleccione la hoja de cálculo [!DNL Google].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja] </td> 
   <td> <p>Seleccione la hoja que contiene la celda de la que desea recuperar los datos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Celda] </td> 
   <td> <p>Introduzca el ID de la celda desde la que desea recuperar los datos. Ejemplo: <code>A6</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opción de procesamiento de valor]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Valor con formato]</p> <p>Los valores se calculan y se les aplica formato en la respuesta según el formato de la celda. El formato se basa en la configuración regional de la hoja de cálculo, no en la del usuario solicitante. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devolvería <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Unformatted value]</p> <p>Los valores se calculan, pero no se les aplica formato en la respuesta. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devolvería el número <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Formula]</p> <p>Los valores no se calculan. La respuesta incluirá las fórmulas. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devolvería <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Date and time render option]</td> 
   <td> <p style="font-weight: bold;">[!DNL Serial number]</p> <p>Indica a los campos de fecha, hora, fecha y hora que deben aparecer como valores dobles en formato de "número de serie", tal como lo ha popularizado Lotus 1-2-3. La parte del número entero del valor (a la izquierda del decimal) cuenta los días transcurridos desde el 30 de diciembre de 1899. La parte fraccionaria (a la derecha del decimal) cuenta la hora como una fracción del día. Por ejemplo, el 1 de enero de 1900 al mediodía sería 2,5, 2 porque son 2 días después del 30 de diciembre de 1899 y 0,5 porque el mediodía es medio día. El 1 de febrero de 1900 a las 3 de la tarde sería 33.625. Esto trata correctamente el año 1900 como un año no bisiesto.</p> <p style="font-weight: bold;">[!DNL Formatted string]</p> <p>Indica a los campos de fecha, hora, fecha y hora que se muestren como cadenas en el formato de número especificado (que depende de la configuración regional de la hoja de cálculo).</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Actualizar una celda]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Sheets] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Hoja de cálculo de [!UICONTROL] </td> 
   <td> <p>Seleccione la hoja de cálculo [!DNL Google].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Celda] </td> 
   <td> <p>Introduzca el ID de la celda que desea actualizar. Ejemplo: <code>A5</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valor]</td> 
   <td> <p>Introduzca el nuevo valor para la celda.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opción de entrada de valor]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Usuario introducido]</strong></p> <p>Los valores se analizan como si el usuario los hubiera escrito en la interfaz de usuario. Los números siguen siendo números, pero las cadenas se pueden convertir en números, fechas u otros formatos siguiendo las mismas reglas que se aplican al escribir texto en una celda a través de la interfaz de usuario de [!DNL Google Sheets].</p> </li> 
     <li> <p><strong>[!UICONTROL RAW]</strong> </p> <p> Los valores que introduce el usuario no se analizan y se almacenan tal cual. </p> </li> 
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
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Sheets] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Hoja de cálculo de [!UICONTROL] </td> 
   <td> <p>Seleccione la hoja de cálculo de Google que contiene la hoja en la que desea borrar una celda.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja] </td> 
   <td> <p>Seleccione la hoja en la que desea borrar una celda.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Celda] </td> 
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
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Sheets] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Hoja de cálculo de [!UICONTROL] </td> 
   <td> <p>Seleccione la hoja de cálculo de Google en la que desea agregar una hoja.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Propiedades]</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">[!UICONTROL Título]</p> <p>Introduzca el nombre de la nueva hoja.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Índice]</p> <p>Introduzca la posición de la hoja. El valor predeterminado es 0 (coloca la hoja en primer lugar)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Crear una hoja de cálculo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Sheets] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Título] </td> 
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
   <td> <p>Cantidad de tiempo de espera antes de volver a calcular las funciones volátiles:</p> <p style="font-weight: bold;">[!UICONTROL Al cambiar]</p> <p>Las funciones volátiles se actualizan con cada cambio.</p> <p style="font-weight: bold;">[!UICONTROL Al cambiar y cada minuto]</p> <p>Las funciones volátiles se actualizan en cada cambio y cada minuto.</p> <p style="font-weight: bold;">[!UICONTROL Al cambiar y por hora]</p> <p>Las funciones volátiles se actualizan con cada cambio y cada hora.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zona horaria]</td> 
   <td> <p> Seleccione la zona horaria de la hoja de cálculo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Formato de número]</td> 
   <td> <p>Seleccione el formato predeterminado de todas las celdas de la hoja de cálculo.</p> <p><strong>[!UICONTROL Text]</strong>: formato de texto. Ejemplo: <code>1000. 12</code></p> <p><strong>[!UICONTROL Número]</strong>: formato de número. Ejemplo: <code>1,000.12</code></p> <p><strong>[!UICONTROL Percent]</strong>: formato de porcentaje. Ejemplo: <code>10. 12%</code></p> <p><strong>[!UICONTROL Currency]</strong>: Formato de moneda. Ejemplo: <code>$1,000.12</code></p> <p><strong>[!UICONTROL Fecha]</strong>: formato de fecha. Ejemplo: <code>9/26/2008</code></p> <p><strong>[!UICONTROL Time]</strong>: formato de hora. Ejemplo: <code>3:59:00 PM</code></p> <p><strong>[!UICONTROL Fecha y hora]</strong>: formato de fecha y hora. Ejemplo: <code>9/26/08 15:59:00</code> </p> <p><strong>[!UICONTROL Scientific]</strong>Formato de número científico. Ejemplo: <code>1. 01E+03</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hojas] </td> 
   <td> <p>Haga clic en <strong>[!UICONTROL Add]</strong> para agregar una hoja a la hoja de cálculo. Para cada hoja, introduzca o asigne un título para la hoja y su índice. Un índice de 0 representa la primera hoja.</p> </td> 
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
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Sheets] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Hoja de cálculo de [!UICONTROL] </td> 
   <td> <p>Seleccione la hoja de cálculo [!DNL Google].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja] </td> 
   <td> <p>Seleccione la hoja que desee eliminar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Realizar una llamada API]

Este módulo de acción le permite realizar una llamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [Fusion App] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Crear una conexión a [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>Escriba una ruta relativa a <code>https://sheets.googleapis.com/v4/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Agregue los encabezados de la solicitud en forma de objeto JSON estándar. Por ejemplo, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] agrega los encabezados de autorización por usted.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p> Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuerpo]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:   <p>Cuando utilice afirmaciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Búsquedas

* [[!UICONTROL Buscar filas]](#search-rows)
* [[!UICONTROL Buscar filas (avanzadas)]](#search-rows-advanced)
* [[!UICONTROL Obtener valores de rango]](#get-range-values)
* [[!UICONTROL Hojas de lista]](#list-sheets)

### [!UICONTROL Buscar filas]

Busca filas utilizando las opciones de filtro.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [Fusion App] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Crear una conexión a [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Hoja de cálculo de [!UICONTROL] </td> 
   <td> <p>Seleccione la hoja de cálculo [!DNL Google].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja] </td> 
   <td> <p>Seleccione la hoja en la que desea buscar las filas.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL La tabla contiene encabezados]</td> 
   <td> <p> Seleccione si la hoja de cálculo contiene la fila de encabezado. Si se selecciona la opción [!UICONTROL Yes], el módulo no recupera la fila de encabezado, ya que los encabezados llaman a los datos de salida y a los nombres de las variables en la salida. Si se selecciona la opción [!UICONTROL No], el módulo también recupera la primera fila de tabla y los nombres de variables en la salida se llaman solo A, B, C, D, etc.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rango de columnas]</td> 
   <td>Seleccione el rango de columnas con el que desea trabajar. Ejemplo: <code>A-F</code></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Filtro]</td> 
   <td> <p>Establezca el filtro para la fila por la que desea buscar.</p> <p>Para obtener más información sobre los filtros, consulte <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Agregar un filtro a un escenario en [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Orden]</td> 
   <td>Seleccione si desea ordenar de forma ascendente o descendente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordenar por]</td> 
   <td>Elija la columna por la que desea ordenar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opción de procesamiento de valor]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Valor con formato]</p> <p>Los valores se calculan y se les aplica formato en la respuesta según el formato de la celda. El formato se basa en la configuración regional de la hoja de cálculo, no en la del usuario solicitante. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devolvería <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Valor sin formato]</p> <p>Los valores se calculan, pero no se les aplica formato en la respuesta. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devolvería el número <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Fórmula]</p> <p>Los valores no se calculan. La respuesta incluirá las fórmulas. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devolvería <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opción de procesamiento de fecha y hora]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Número de serie]</p> <p>Indica a los campos de fecha, hora, fecha y hora que se deben mostrar como valores dobles en formato de "número de serie", tal como lo popularizó Lotus 1-2-3. La parte del número entero del valor (a la izquierda del decimal) cuenta los días transcurridos desde el 30 de diciembre de 1899. La parte fraccionaria (a la derecha del decimal) cuenta la hora como una fracción del día. Por ejemplo, el 1 de enero de 1900 al mediodía sería 2,5, 2 porque son 2 días después del 30 de diciembre de 1899 y 0,5 porque el mediodía es medio día. El 1 de febrero de 1900 a las 3 de la tarde sería 33.625. Esto trata correctamente el año 1900 como un año no bisiesto.</p> <p style="font-weight: bold;">[!UICONTROL Cadena con formato]</p> <p>Indica a los campos de fecha, hora, fecha y hora que se muestren como cadenas en el formato de número especificado (que depende de la configuración regional de la hoja de cálculo).</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de filas devueltas]</td> 
   <td>Establezca el número máximo de filas que [!DNL Workfront Fusion] devolverá durante un ciclo de ejecución.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Buscar filas (avanzadas)]

Devuelve los resultados que coinciden con los criterios dados.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Sheets] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Hoja de cálculo de [!UICONTROL] </td> 
   <td> <p>Seleccione la hoja de cálculo de Google que contiene la hoja que desea buscar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja] </td> 
   <td> <p>Seleccione la hoja que contiene las filas que desea buscar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Consulta]</td> 
   <td> <p>Usar [!DNL Google Charts Query Language]. Ejemplo: <code>select * where B = "John"</code></p> <p>Para obtener más información sobre [!DNL Google Charts Query Language], consulte <a href="https://developers.google.com/chart/interactive/docs/querylanguage">Referencia del lenguaje de consulta</a> en la documentación de [!DNL Google].</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Obtener valores de rango]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Sheets] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Hoja de cálculo de [!UICONTROL] </td> 
   <td> <p>Seleccione la hoja de cálculo [!DNL Google].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Hoja] </td> 
   <td> <p>Seleccione la hoja de la que desee obtener el contenido del intervalo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rango] </td> 
   <td> <p>Introduzca el rango que desea obtener. Ejemplo: <code>A1:D25</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL La tabla contiene encabezados]</td> 
   <td> <p>Marque esta casilla si la hoja tiene una fila de encabezado</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fila con encabezados]</td> 
   <td>Introduzca el rango de los encabezados de tabla. Ejemplo <code>A1:F1</code>. Si deja el campo vacío, [!DNL Workfront Fusion] supondrá que el encabezado se encuentra en la primera fila del rango especificado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opción de procesamiento de valor]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Valor con formato]</p> <p>Los valores se calculan y se les aplica formato en la respuesta según el formato de la celda. El formato se basa en la configuración regional de la hoja de cálculo, no en la del usuario solicitante. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devolvería <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Valor sin formato]</p> <p>Los valores se calculan, pero no se les aplica formato en la respuesta. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devolvería el número <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Fórmula]</p> <p>Los valores no se calculan. La respuesta incluirá las fórmulas. Por ejemplo, si <code>A1</code> es <code>1.23</code> y <code>A2</code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devolvería <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Opción de procesamiento de fecha y hora]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Número de serie]</p> <p>Indica a los campos de fecha, hora, fecha y hora que se deben mostrar como valores dobles en formato de "número de serie", tal como lo popularizó Lotus 1-2-3. La parte del número entero del valor (a la izquierda del decimal) cuenta los días transcurridos desde el 30 de diciembre de 1899. La parte fraccionaria (a la derecha del decimal) cuenta la hora como una fracción del día. Por ejemplo, el 1 de enero de 1900 al mediodía sería 2,5, 2 porque son 2 días después del 30 de diciembre de 1899 y 0,5 porque el mediodía es medio día. El 1 de febrero de 1900 a las 3 de la tarde sería 33.625. Esto trata correctamente el año 1900 como un año no bisiesto.</p> <p style="font-weight: bold;">[!UICONTROL Cadena con formato]</p> <p>Indica a los campos de fecha, hora, fecha y hora que se muestren como cadenas en el formato de número especificado (que depende de la configuración regional de la hoja de cálculo).</p> </td> 
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
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Sheets] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Hoja de cálculo de [!UICONTROL] </td> 
   <td> <p>Seleccione la hoja de cálculo [!DNL Google] que contiene las hojas que desea enumerar.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Límites de uso

Si se produce el error `429: RESOURCE_EXHAUSTED`, ha excedido el límite de tasa de API.

La API [!DNL Google Sheets] tiene un límite de 500 solicitudes por 100 segundos por proyecto y de 100 solicitudes por 100 segundos por usuario. Los límites para lecturas y escrituras se rastrean por separado. No hay límite de uso diario.

Ver más detalles en [developers.google.com/sheets/api/limits](https://developers.google.com/sheets/api/limits).

## Sugerencias y trucos

* [Cómo obtener celdas vacías de una  [!DNL Google] hoja](#how-to-get-empty-cells-from-a-google-sheet)
* [Agregar un botón en una hoja para ejecutar un escenario](#add-a-button-in-a-sheet-to-run-a-scenario)

### Cómo obtener celdas vacías de un(a) [!DNL Google Sheet]

Use el módulo [!UICONTROL Buscar filas (avanzadas)] y use esta fórmula para obtener las columnas que están vacías.
<pre>seleccione * donde E es nulo</pre>Aquí, "E" es la columna y "es nulo" es la condición. Puede crear una consulta más avanzada con [Google Query Lang](https://developers.google.com/chart/interactive/docs/querylanguage).

### Agregar un botón en una hoja para ejecutar un escenario

1. En [!DNL Workfront Fusion], inserte el módulo/déclencheur **[!UICONTROL Webhook]** > **[!UICONTROL Webhooks personalizados]** en el escenario y configúrelo (consulte [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md)).

1. Copie la URL del gancho web.
1. Ejecute el escenario.
1. En Hojas de cálculo de Google, elija **[!UICONTROL Insertar]** > **[!UICONTROL Dibujo]**... en la barra de menús principal.

1. En la ventana [!UICONTROL Dibujo], haga clic en el icono **[!UICONTROL Cuadro de texto]** ![](assets/text-box.png) cerca de la parte superior de la ventana.
1. Diseñe un botón y haga clic en el botón **[!UICONTROL Guardar y cerrar]** en la esquina superior derecha:
1. El botón se colocará en la hoja de cálculo. Haga clic en los tres puntos verticales de la esquina superior derecha del botón:
1. Elija **[!UICONTROL Asignar script..].** del menú.
1. Escriba el nombre del script (función), por ejemplo `runScenario` y haga clic en **[!UICONTROL Aceptar]**:
1. Elija **[!UICONTROL Herramientas]** > **[!UICONTROL Editor de scripts]** en la barra de menús principal.

1. Inserte el siguiente código:

   * El nombre de la función debe corresponder al nombre especificado en el paso 9.
   * Reemplace la URL con la URL del webhook que copió en el paso 2.

     <pre>function runScenario() {</pre><pre>UrlFetchApp.fetch("&lt;webhook que copió&gt;");</pre><pre>}</pre>

1. Presione **[!UICONTROL Ctrl+S]** para guardar el archivo de script, ingrese un nombre de proyecto y haga clic en **[!UICONTROL Aceptar]**.

1. Vuelva a [!DNL Google Sheets] y haga clic en el nuevo botón.
1. Conceda la autorización necesaria al script:
1. En [!DNL Workfront Fusion], compruebe que el escenario se haya ejecutado correctamente.

## Almacenamiento de fechas en una hoja de cálculo

Si almacena un valor de fecha en una hoja de cálculo sin ningún formato, aparecerá en la hoja de cálculo como texto en formato ISO 8601. Sin embargo, [!DNL Google Sheets] fórmulas o funciones que funcionan con fechas que no comprenden este texto (Ejemplo: fórmula `=A1+10`) mostrarán el siguiente error:

![](assets/mceclip6-350x87.png)

Para permitir que [!DNL Google Sheets] entienda la fecha, asígnele el formato con la función [[!UICONTROL formatDate] (date; format; [timezone])](../../workfront-fusion/functions/date-and-time-functions.md#formatda). El formato correcto pasado a la función como segundo argumento depende de la configuración regional de la hoja de cálculo.

Para determinar el formato correcto:

1. Elija la configuración de **[!UICONTROL Archivo]** > **[!UICONTROL Hoja de cálculo]** en el menú principal para comprobar o establecer la configuración regional.

1. Una vez que haya verificado/establecido la configuración regional adecuada, determine el formato de fecha y hora correspondiente eligiendo **[!UICONTROL Formato]** > **[!UICONTROL Número]** en el menú principal. El formato se muestra junto al elemento de menú Fecha y hora:

1. Para componer el formato correcto que se debe pasar a la función [!UICONTROL formatDate()], consulte la lista de [tokens para el formato de fecha y hora en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md).

**Ejemplo:** Uso del formato `MM/DD/YYYY HH:mm:ss` para la configuración regional de Estados Unidos:

![](assets/locale-time-350x83.png)

## Explotando [!DNL Google Sheets] funciones

Si se le pasa por alto una función integrada, pero [!DNL Google Sheets] la presenta, puede aprovecharla. Para obtener más información, vea [Usar [!DNL Google Sheets] funciones](../../workfront-fusion/functions/map-using-functions.md#exploiti) en [Asignar elementos usando funciones en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md) .

## Evitar que [!DNL Google Sheets] cambie números a fechas

Es posible que descubra que una cadena de números que está utilizando como texto se interpreta como una fecha en una hoja de cálculo [!DNL Google]. Por ejemplo, se escribe 1-2019 con la intención de que sea texto, pero Google lo interpreta como una fecha. Puede dar formato previo al número como texto sin formato para evitarlo.

1. En [!DNL Google Sheets], resalte la columna o celda que contenga el número o los números.
1. Haga clic en **[!UICONTROL Formato]** > **[!UICONTROL Número]** > **[!UICONTROL Texto sin formato]**.

Otra solución en [!DNL Workfront Fusion] es escribir un apóstrofo (&#39;) antes de un número, por ejemplo, &#39;1-2019 o &#39;1/47. El apóstrofo no se muestra en la celda después de enviar los datos desde [!DNL Workfront Fusion].
