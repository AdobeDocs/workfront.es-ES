---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Google Forms
description: Los  [!DNL Adobe Workfront Fusion Google Forms] módulos le permiten supervisar, seleccionar, agregar, actualizar o eliminar respuestas en su Forms de Google.
author: Becky
feature: Workfront Fusion
exl-id: 45c86879-bc4e-4134-b63c-02410b9de43b
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1435'
ht-degree: 0%

---

# [!DNL Google Forms] módulos

Los módulos [!DNL Adobe Workfront Fusion] [!DNL Google Forms] le permiten supervisar, seleccionar, agregar, actualizar o eliminar respuestas en su [!DNL Google Forms].

Para usar [!DNL Google Docs] con [!DNL Adobe Workfront Fusion], es necesario tener una cuenta de [!DNL Google]. Si todavía no tiene una cuenta [!DNL Google], puede crearla en la página de ayuda de la cuenta [!DNL Google].

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información acerca de los módulos, vea [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Para usar módulos de [!DNL Google Forms], debe tener una cuenta de [!DNL Google].

## Información de la API de Google Forms

El conector Forms de Google utiliza lo siguiente:

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

## Crear una hoja de cálculo a partir de un formulario

Para trabajar con las respuestas del formulario, se debe crear la hoja de cálculo de las respuestas.

1. Abra el formulario.
1. Vaya a la pestaña **[!UICONTROL Respuestas]**.
1. Haga clic en el icono **[!UICONTROL Crear hoja de cálculo]** ![](assets/spreadsheet-icon.png).

1. Seleccione si desea crear una hoja de cálculo nueva o una existente
1. Haga clic en **[!UICONTROL Crear]**.

## [!DNL Google Forms] módulos y sus campos

Al configurar [!DNL Google Forms] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Google Forms] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheur](#triggers)
* [Acciones](#actions)
* [Búsquedas](#searches)

### Déclencheur

#### [!UICONTROL Respuestas de inspección]

Inspecciona el formulario en busca de nuevas respuestas.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Hoja de cálculo de [!UICONTROL]</td> 
   <td> <p>Seleccione la hoja de cálculo que contiene las respuestas del formulario que desea inspeccionar en busca de nuevas respuestas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Hoja]</td> 
   <td> <p> Seleccione la hoja que contiene las respuestas del formulario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fila con encabezados]</td> 
   <td>Especifique la fila de encabezado de la tabla. La fila predeterminada es <code>A1:Z1</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Opción de procesamiento de valores]</td> 
   <td> <p>Especifique cómo desea que se representen los valores en la salida.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Valor con formato]</strong> </p> <p>Los valores se calculan y se les aplica formato en la respuesta según el formato de la celda. El formato se basa en la configuración regional de la hoja de cálculo, no en la del usuario solicitante. Por ejemplo, si <code>A1</code> es <code>1. 23</code> y <code>A2 </code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devuelve <code>$1. 23</code></p> </li> 
     <li> <p><strong>[!UICONTROL Valor sin formato]</strong> </p> <p>Los valores se calculan, pero no se les aplica formato en la respuesta. Por ejemplo, si <code>A1</code> es <code>1. 23</code> y <code>A2 </code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devuelve el número <code>1. 23</code></p> </li> 
     <li> <p><strong>[!UICONTROL Fórmula]</strong> </p> <p>Los valores no se calculan. La respuesta incluye las fórmulas. Por ejemplo, si <code>A1</code> es <code>1. 23</code> y <code>A2 </code>es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devuelve <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Opción de procesamiento de fecha y hora]</td> 
   <td>Seleccione cómo desea que se representen las fechas, las horas y la duración en la salida. Este campo se omite si [!UICONTROL Opción de procesamiento de valores] se establece en [!UICONTROL Valor con formato].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p> Establezca el número máximo de respuestas con las que trabaja [!DNL Workfront Fusion] durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Agregar una respuesta]](#add-a-response)
* [[!UICONTROL Actualizar una respuesta]](#update-a-response)
* [[!UICONTROL Eliminar una respuesta]](#delete-a-response)

#### [!UICONTROL Agregar una respuesta]

Este módulo anexa una nueva respuesta a la parte inferior de la hoja de cálculo del formulario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Hoja de cálculo de [!UICONTROL]</td> 
   <td> <p>Seleccione la hoja de cálculo que contiene la hoja a la que desea agregar una respuesta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Hoja]</td> 
   <td> <p> Seleccione la hoja que contiene las respuestas del formulario.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Valores]</p> </td> 
   <td> <p>Introduzca los valores deseados en las columnas de la hoja.</p> <p>Para la columna [!UICONTROL Timestamp] con el formato correcto, utilice el siguiente valor:</p><pre>formatDate(now;DD/MM/AAAA HH:mm;UTC)</pre> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Opción de entrada de valor]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL RAW]</strong> </p> <p> Los valores que introduce el usuario no se analizan y se almacenan tal cual. </p> </li> 
     <li> <p><strong>[!UICONTROL Usuario introducido]</strong></p> <p>Los valores se analizan como si el usuario los hubiera escrito en la interfaz de usuario. Los números siguen siendo números, pero las cadenas se pueden convertir en números, fechas u otros formatos siguiendo las mismas reglas que se aplican al escribir texto en una celda a través de la interfaz de usuario de [!DNL Google Sheets].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Insertar opción de datos]</td> 
   <td> <p>Especifique cómo se cambian los datos existentes al introducir nuevos datos. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Sobrescribir]</strong> </p> <p>Los nuevos datos sobrescriben los datos existentes en las áreas en las que se escriben. Al agregar datos al final de la hoja, se insertan nuevas filas o columnas para poder escribir los datos.</p> </li> 
     <li> <p><strong>[!UICONTROL Insertar filas]</strong></p> <p>Las filas se insertan para los nuevos datos.</p> </li> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Hoja de cálculo de [!UICONTROL]</td> 
   <td> <p>Seleccione la hoja de cálculo que contiene la hoja en la que desea actualizar una respuesta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Hoja]</td> 
   <td> <p> Seleccione la hoja que contiene las respuestas del formulario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Número de fila]</p> </td> 
   <td> <p>Introduzca o asigne el número de la fila que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Valores]</p> </td> 
   <td> <p>Introduzca los nuevos valores en las columnas deseadas.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Opción de entrada de valor]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL RAW]</strong> </p> <p> Los valores que introduce el usuario no se analizan y se almacenan tal cual. </p> </li> 
     <li> <p><strong>[!UICONTROL Usuario introducido]</strong></p> <p>Los valores se analizan como si el usuario los hubiera escrito en la interfaz de usuario. Los números siguen siendo números, pero las cadenas se pueden convertir en números, fechas u otros formatos siguiendo las mismas reglas que se aplican al escribir texto en una celda a través de la interfaz de usuario de [!DNL Google Sheets].</p> </li> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Hoja de cálculo de [!UICONTROL]</td> 
   <td> <p>Seleccione la hoja de cálculo que contiene la hoja en la que desea eliminar una respuesta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Hoja]</td> 
   <td> <p> Seleccione la hoja que contiene las respuestas del formulario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Número de fila]</p> </td> 
   <td> <p>Introduzca o asigne el número de la fila que desea eliminar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

* [[!UICONTROL Respuestas de búsqueda]](#search-responses)
* [[!UICONTROL Respuestas de búsqueda (avanzadas])](#search-responses-advanced)

#### [!UICONTROL Respuestas de búsqueda]

Este módulo devuelve respuestas que coinciden con los criterios dados.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
    <td>Conexión</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>Hoja de cálculo de [!UICONTROL]</td>
   <td> <p>Seleccione el formulario en el que desea buscar.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Hoja] </td>
   <td> <p>Seleccione la hoja que contiene las respuestas del formulario.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Rango de columnas]</td>
   <td> <p> Seleccione el rango de columnas que desea buscar.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Defina el filtro por el que desea buscar respuestas.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Orden] </td>
   <td> <p>Seleccione si desea ordenar las respuestas devueltas en orden ascendente o descendente.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Ordenar por]</td>
   <td> <p> Seleccione la columna por la que desea ordenar las respuestas devueltas.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Opción de procesamiento de valores]</td> 
   <td> <p>Especifique cómo desea que se representen los valores en la salida.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Valor con formato]</strong></p> <p>Los valores se calculan y se les aplica formato en la respuesta según el formato de la celda. El formato se basa en la configuración regional de la hoja de cálculo, no en la del usuario solicitante. Por ejemplo, si <code>A1</code> es <code>1. 23</code> y <code>A2 </code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devuelve <code>$1. 23</code></p> </li> 
     <li> <p><strong>[!UICONTROL Valor sin formato]</strong> </p> <p>Los valores se calculan, pero no se les aplica formato en la respuesta. Por ejemplo, si <code>A1</code> es <code>1. 23</code> y <code>A2 </code> es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devuelve el número <code>1. 23</code></p> </li> 
     <li> <p><strong>[!UICONTROL Fórmula]</strong> </p> <p>Los valores no se calculan. La respuesta incluye las fórmulas. Por ejemplo, si <code>A1</code> es <code>1. 23</code> y <code>A2 </code>es <code>=A1</code> y tiene formato de moneda, <code>A2</code> devuelve <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Opción de procesamiento de fecha y hora]</td>
    <td>Seleccione cómo desea que se representen las fechas, las horas y la duración en la salida. Este campo se omite si la opción [!UICONTROL Value Render] está establecida en Valor con formato. </td>
  </tr> 
  <tr>
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Número máximo de respuestas devueltas]</td>
   <td> <p> Establezca el número máximo de respuestas que [!DNL Workfront Fusion] devuelve durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Respuestas de búsqueda (avanzadas)]

Este módulo realiza una búsqueda utilizando [[!DNL Google Charts Query Language]](https://developers.google.com/chart/interactive/docs/querylanguage). Este módulo no devuelve un número de fila.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Conexión]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td>Hoja de cálculo de [!UICONTROL]</td>
   <td> <p>Seleccione la hoja de cálculo que contiene la hoja que desea buscar.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Hoja]</td>
   <td> <p> Seleccione la hoja que contiene las respuestas del formulario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Defina la consulta de búsqueda utilizando <a href="https://developers.google.com/chart/interactive/docs/querylanguage">[!DNL Google Charts Query Language]</a>.</p> <p>Ejemplo: <code>select * where C = "John"</code> recupera todos los valores de la fila donde la columna C es "John".</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Número máximo de filas devueltas]</td>
   <td> <p> Establezca el número máximo de respuestas que [!DNL Workfront Fusion] devuelve durante un ciclo.</p> </td> 
  </tr> 
 </tbody> 
</table>
