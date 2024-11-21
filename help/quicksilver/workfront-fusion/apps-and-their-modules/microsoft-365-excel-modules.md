---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Excel de Microsoft Office 365
description: En un escenario  [!DNL Adobe Workfront Fusion] puede automatizar los flujos de trabajo que utilizan Microsoft 365 Excel, así como conectarlos a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 9aa3739d-6800-4eb1-a17f-32fdfd8ed0f2
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '2768'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Excel] módulos

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!DNL Microsoft 365 Excel], así como conectarlo a varias aplicaciones y servicios de terceros.

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

Para usar [!DNL Microsoft office 365 Excel], debe tener una cuenta de Microsoft.

## Información de la API de Excel de Microsoft Office 365

El conector de Excel de Microsoft Office 365 utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL básica</td> 
   <td> https://graph.microsoft.com/v1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Versión de API</td> 
   <td> Versión 1.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 2.0.16</td> 
  </tr>
 </tbody> 
 </table>



## Conectando el servicio [!DNL Office 365 Excel] a [!DNL Workfront Fusion]

Para obtener instrucciones sobre cómo conectar tu cuenta de [!DNL Office 365 Excel] a [!UICONTROL Workfront Fusion], consulta [Crear una conexión a [!UICONTROL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Algunas aplicaciones de Microsoft utilizan la misma conexión, que está vinculada a permisos de usuario individuales. Por lo tanto, al crear una conexión, la pantalla de consentimiento de permisos muestra todos los permisos que se hayan concedido anteriormente a la conexión de este usuario, además de los nuevos permisos necesarios para la aplicación actual.
>
>Por ejemplo, si un usuario tiene permisos de &quot;Leer tabla&quot; concedidos a través del conector de Excel y, a continuación, crea una conexión en el conector de Outlook para leer correos electrónicos, la pantalla de consentimiento de permisos mostrará tanto el permiso de &quot;Leer tabla&quot; ya concedido como el permiso de &quot;Escribir correo electrónico&quot; recién requerido.

## [!DNL Microsoft Office 365 Excel] módulos y sus campos

Al configurar [!DNL Microsoft 365 Excel] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Microsoft 365 Excel] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Libro](#workbook)
* [Hoja de cálculo](#worksheet)
* [Tabla](#table)
* [Otro](#other)

### Libro

* [Ver libros](#watch-workbooks)
* [Buscar libros](#search-workbooks)
* [Descargar un libro](#download-a-workbook)

#### [!UICONTROL Ver libros]

Este módulo de déclencheur inicia un escenario cuando se crea un libro.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carpeta]</td> 
   <td> <p>Seleccione la carpeta en la que desea buscar nuevos libros.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filtro]</p> </td> 
   <td> <p>Puede definir un filtro para inspeccionar sólo los libros que cumplan los criterios seleccionados.</p> <p>Para cada filtro, introduzca el campo que desea que evalúe el filtro, el operador y el valor que desea que permita el filtro. Puede utilizar más de un filtro añadiendo reglas AND u OR.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de libros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Buscar libros]

Este módulo de acción busca [!DNL Excel] libros.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carpeta]</td> 
   <td> <p>Seleccione la carpeta en la que desea buscar libros.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filtro]</p> </td> 
   <td> <p>Puede definir un filtro para buscar sólo libros que cumplan los criterios seleccionados.</p> <p>Para cada filtro, introduzca el campo que desea que evalúe el filtro, el operador y el valor que desea que permita el filtro. Puede utilizar más de un filtro añadiendo reglas AND u OR.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de hojas de cálculo que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Descargar un libro]

Este módulo de acción descarga el contenido del libro de Excel especificado.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descargar un libro]</td> 
   <td> <p>Seleccione cómo desea identificar el libro para que el módulo lo descargue.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Al escribir un ID manualmente]</strong> </p> <p>En el campo [!UICONTROL Workbook ID], escriba o asigne el identificador del libro específico que desea que descargue el módulo.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccionando desde la ruta]</strong> </p> <p>En el campo [!UICONTROL Workbook], seleccione el libro que desea que descargue el módulo.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Hoja de cálculo

* [[!UICONTROL Observar filas de hoja de cálculo]](#watch-worksheet-rows)
* [[!UICONTROL Enumerar hojas de cálculo]](#list-worksheets)
* [[!UICONTROL Enumerar filas de hoja de cálculo]](#list-worksheet-rows)
* [[!UICONTROL Agregar hoja de cálculo]](#add-a-worksheet)
* [[!UICONTROL Agregar una fila de hoja de cálculo]](#add-a-worksheet-row)
* [[!UICONTROL Actualizar una fila de hoja de cálculo]](#update-a-worksheet-row)
* [[!UICONTROL Eliminar una fila de hoja de cálculo]](#delete-a-worksheet-row)

#### [!UICONTROL Observar filas de hoja de cálculo]

Este módulo de déclencheur inicia un escenario cuando se agrega una nueva fila a la hoja.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Libro] </td>
   <td> <p>Seleccione el libro que contiene la hoja de cálculo que desea inspeccionar para buscar nuevas filas.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >Hoja de cálculo de [!UICONTROL] </td>
   <td> <p>Seleccione la hoja de Excel que desea inspeccionar para buscar nuevas filas.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Límite]</td>
   <td> <p>Introduzca o asigne el número máximo de filas de hoja de cálculo que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enumerar hojas de cálculo]

Este módulo de acción recupera una lista de hojas de cálculo del libro especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Libro] </td>
   <td> <p>Seleccione el libro que contiene las hojas de cálculo que desea que muestre el módulo.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Límite]</td>
   <td> <p>Introduzca o asigne el número máximo de hojas de cálculo que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enumerar filas de hoja de cálculo]

Este módulo de acción recupera una lista de filas de la hoja de cálculo especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Libro] </td>
   <td> <p>Seleccione el libro que contiene la hoja de cálculo que incluye las filas que desea enumerar.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >Hoja de cálculo de [!UICONTROL] </td>
   <td> <p>Seleccione la hoja de cálculo que contiene las filas que desea enumerar.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Límite]</td>
   <td> <p>Introduzca o asigne el número máximo de filas de hoja de cálculo que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Agregar hoja de cálculo]

Este módulo de acción crea una nueva hoja de cálculo dentro del libro seleccionado.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Libro] </td>
   <td> <p>Seleccione el libro en el que desea agregar una hoja de cálculo.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Nombre] </td>
   <td> <p>Introduzca o asigne un nombre para la nueva hoja de cálculo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Agregar una fila de hoja de cálculo]

Este módulo de acción agrega una nueva fila a la hoja de cálculo seleccionada.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Libro] </td>
   <td> <p>Seleccione el libro que contiene la hoja de cálculo donde desea agregar una fila.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >Hoja de cálculo de [!UICONTROL] </td>
   <td> <p>Seleccione la hoja de cálculo donde desea agregar una fila.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de valores introducidos]</p> </td> 
   <td> <p>Seleccione el tipo de valor que se va a introducir en la hoja de cálculo. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Fórmulas]</strong> </p> <p> Excel intenta evaluar la expresión especificada. Los nombres de las funciones de una fórmula están en inglés. Ejemplo: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Fórmulas locales]</strong> </p> <p>Excel intenta evaluar la expresión especificada. Los nombres de las funciones están en el idioma de la aplicación de Excel. Ejemplo: <code>=SUM(A1, 1.5)</code> frente a <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL Valor]</strong> </p> <p>Excel no evalúa el valor. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Fila]</td>
    <td>Para cada columna, introduzca el valor que desea que tenga la columna en la nueva fila.</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar una fila de hoja de cálculo]

Este módulo de acción actualiza una fila de hoja de cálculo existente.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Libro] </td>
   <td> <p>Seleccione el libro que contiene la hoja que incluye la fila que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >Hoja de cálculo de [!UICONTROL] </td>
   <td> <p>Seleccione la hoja que contiene la fila que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de valores introducidos]</p> </td> 
   <td> <p>Seleccione el tipo de valor que se va a introducir en la hoja de cálculo. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Fórmulas]</strong> </p> <p> Excel intenta evaluar la expresión especificada. Los nombres de las funciones de una fórmula están en inglés. Ejemplo: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Fórmulas locales]</strong> </p> <p>Excel intenta evaluar la expresión especificada. Los nombres de las funciones están en el idioma de la aplicación de Excel. Ejemplo: <code>=SUM(A1, 1.5)</code> frente a <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL Valor]</strong> </p> <p>Excel no evalúa el valor. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de fila]</td> 
   <td>Seleccione el número de la fila que desea actualizar.</td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Fila]</td>
    <td>Para cada columna, introduzca el valor que desea que tenga la columna en la nueva fila.</td>
   --&gt; 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar una fila de hoja de cálculo]

Este módulo de acción elimina una fila de una hoja de cálculo.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Libro] </td>
   <td> <p>Seleccione el libro que contiene la hoja de cálculo que incluye la fila que desea eliminar.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >Hoja de cálculo de [!UICONTROL]</td>
   <td> <p> Seleccione la hoja de cálculo que contiene la fila que desea eliminar.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL ID de fila]</td>
   <td>Introduzca o asigne el ID de la fila que desea eliminar.</td> 
  </tr> 
 </tbody> 
</table>

### Tabla

* [[!UICONTROL Observar filas de tabla]](#watch-table-rows)
* [[!UICONTROL Tablas de lista]](#list-tables)
* [[!UICONTROL Enumerar filas de tabla]](#list-table-rows)
* [[!UICONTROL Obtener una tabla]](#get-a-table)
* [[!UICONTROL Agregar una tabla]](#add-a-table)
* [[!UICONTROL Agregar una fila de tabla]](#add-a-table-row)
* [[!UICONTROL Actualizar una tabla]](#update-a-table)
* [[!UICONTROL Eliminar una tabla]](#delete-a-table)

#### [!UICONTROL Observar filas de tabla]

Este déclencheur inicia un escenario cuando se agrega una nueva fila a una tabla.

>[!NOTE]
>
>La tabla aquí hace referencia al elemento de tabla incrustado en el libro. No toda la tabla (libro/hoja).

![](assets/embedded-table-350x420.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Libro]</p> </td> 
   <td> <p>Seleccione el libro que contiene la tabla que desea inspeccionar.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >Hoja de cálculo de [!UICONTROL] </td>
   <td> <p> Seleccione la hoja de cálculo que contiene la tabla que desea inspeccionar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tabla]</p> </td> 
   <td> <p>Seleccione la tabla que desee ver.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Límite]</td>
   <td> <p>Introduzca o asigne el número máximo de filas que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Tablas de lista]

Este módulo de búsqueda recupera una lista de todos los objetos de tabla.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Libro] </td>
   <td> <p>Seleccione el libro que contiene las tablas que desea enumerar.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >Hoja de cálculo de [!UICONTROL] </td>
   <td> <p>Seleccione la hoja de cálculo que contiene las tablas que desea enumerar</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Límite]</td>
   <td> <p>Introduzca o asigne el número máximo de tablas que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enumerar filas de tabla]

Este módulo de búsqueda recupera una lista de todas las filas de tabla de un libro.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Libro] </td>
   <td> <p>Seleccione el libro que contiene la tabla que incluye las filas que desea enumerar.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >Hoja de cálculo de [!UICONTROL] </td>
   <td> <p>Seleccione la hoja de cálculo que contiene la tabla que incluye las filas que desea enumerar</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Tabla] </td>
   <td> <p>Seleccione la tabla que contiene las filas que desea enumerar.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Límite]</td>
   <td> <p>Introduzca o asigne el número máximo de filas de tabla que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener una tabla]

Este módulo de acción recupera los metadatos de la tabla especificada.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
     <p >[!UICONTROL Conexión]</p>
   </td> 
   <td> 
     <p>Para obtener instrucciones acerca de cómo conectar su cuenta de Office 365 a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p>
    --&gt; </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtener una tabla]</td> 
   <td> <p>Seleccione cómo desea identificar la tabla que desea recuperar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el campo [!UICONTROL Workbook ID], escriba o asigne el identificador del libro que contiene la tabla que desea recuperar.</p> <p>En el campo [!UICONTROL Table Name], escriba o asigne el nombre de la tabla que desea recuperar.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione de la lista]</strong> </p> <p>Seleccione el libro y la hoja de cálculo que contienen la tabla que desea recuperar y, a continuación, seleccione la tabla.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Agregar una tabla]

Este módulo de acción crea un elemento de tabla en la hoja de cálculo de Excel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Libro] </td> 
   <td> <p>Seleccione el libro que contiene la hoja de cálculo en la que desea agregar una tabla.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Hoja de cálculo de [!UICONTROL] </td> 
   <td> <p>Seleccione la hoja de cálculo donde desea agregar una tabla.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tiene encabezados]</td> 
   <td> <p>Active esta opción para definir la primera fila como encabezados de tabla.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Dirección]</p> </td> 
   <td> <p>Establezca el tamaño de la tabla indicando las celdas superior izquierda e inferior derecha. Ejemplo: <code>A1:C10</code> crea una tabla con 3 columnas y 10 filas.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Agregar una fila de tabla]

Este módulo de acción modifica una tabla existente.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Libro] </td>
   <td> <p>Seleccione el libro que contiene la tabla en la que desea agregar una fila.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >Hoja de cálculo de [!UICONTROL] </td>
   <td> <p>Seleccione la hoja de cálculo que contiene la tabla en la que desea agregar una fila.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Tabla]</td>
   <td>Seleccione la tabla en la que desea agregar una fila.</td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Fila]</td>
    <td>Para cada columna, introduzca el valor que desea que tenga la columna en la nueva fila.</td>
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ID de fila]</p> </td> 
   <td> <p>Para agregar una fila en una ubicación específica de la tabla, escriba o asigne un número de fila. El módulo inserta la nueva fila después de esta fila.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar una tabla]

Este módulo de acción actualiza una tabla existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Actualizar una tabla]</td> 
   <td> <p>Seleccione cómo desea identificar la tabla que desea actualizar.</p> 
    <ul> 
     <li> <p><strong>Introducir manualmente</strong> </p> <p>En el campo [!UICONTROL Workbook ID], escriba o asigne el identificador del libro que contiene la tabla que desea actualizar.</p> <p>En el campo [!UICONTROL Table Name], escriba o asigne el nombre de la tabla que desea actualizar.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione de la lista]</strong> </p> <p>Seleccione el libro y la hoja de cálculo que contienen la tabla que desea actualizar y, a continuación, seleccione la tabla.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabla] </td> 
   <td> <p>Seleccione la tabla que desee actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre]</td> 
   <td> <p>Si desea cambiar el nombre de la tabla, escriba o asigne un nombre nuevo para la tabla.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar encabezados]</td> 
   <td> <p>Active esta opción para mostrar los encabezados de la tabla actualizada.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar totales]</td> 
   <td>Active esta opción para mostrar los valores totales de la tabla.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Style]</td> 
   <td>Elija un estilo para la nueva tabla.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar una tabla]

Este módulo de acción elimina la tabla especificada de una hoja de cálculo [!DNL Excel].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtener una tabla]</td> 
   <td> <p>Seleccione cómo desea identificar la tabla que desea eliminar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Entrar manualmente]</strong> </p> <p>En el campo [!UICONTROL Workbook ID], escriba o asigne el identificador del libro que contiene la tabla que desea eliminar.</p> <p>En el campo [!UICONTROL Table Name], escriba o asigne el nombre de la tabla que desea eliminar.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleccione de la lista]</strong> </p> <p>Seleccione el libro y la hoja de cálculo que contienen la tabla que desea eliminar y, a continuación, seleccione la tabla.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Otro

* [[!UICONTROL Recuperar datos]](#retrieve-data)
* [[!UICONTROL Realizar una llamada API]](#make-an-api-call)

#### [!UICONTROL Recuperar datos]

Esta acción recupera datos del rango de hoja de cálculo definido y devuelve un paquete para cada fila.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Libro] </td> 
   <td> <p>Seleccione el libro que contiene los datos que desea recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Hoja de cálculo de [!UICONTROL] </td> 
   <td> <p>Seleccione la hoja de cálculo que contiene los datos que desea recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rango] </td> 
   <td> <p>Especifique el área de la hoja de la que desea recuperar datos indicando las celdas superior izquierda e inferior derecha. Ejemplo: <code>A1:D10</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Realizar una llamada API]

Este módulo de acción le permite realizar una llamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Office 365] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Escriba una ruta relativa a <code>https://graph.microsoft.com</code>. Ejemplo:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   td&gt; <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion añade los encabezados de autorización por usted.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p> </td> 
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
