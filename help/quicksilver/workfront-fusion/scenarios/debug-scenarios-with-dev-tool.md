---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Situaciones de depuración con la herramienta de desarrollo de Adobe Workfront Fusion
description: La herramienta de desarrollo de Adobe Workfront Fusion le permite comprender y solucionar problemas de escenarios. DevTool agrega un panel adicional a las herramientas para desarrolladores de Chrome. Con este panel de depuración, puede comprobar todas las ejecuciones manuales del escenario, revisar todas las operaciones realizadas y ver los detalles de cada llamada de API realizada. Puede ver qué módulo, operación o respuesta única causaron el error y utilizar ese conocimiento para restringir el escenario.
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1665'
ht-degree: 0%

---

# Situaciones de depuración con la variable [!DNL Adobe Workfront Fusion] Herramienta de desarrollo

La variable [!DNL Adobe Workfront Fusion] DevTool permite comprender y solucionar problemas de escenarios. La herramienta de desarrollo agrega un panel adicional al [!DNL Chrome Developer Tools]. Con este panel de depuración, puede comprobar todas las ejecuciones manuales del escenario, revisar todas las operaciones realizadas y ver los detalles de cada llamada de API realizada. Puede ver qué módulo, operación o respuesta única causaron el error y utilizar ese conocimiento para restringir el escenario.

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p><p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Instale el [!DNL Chrome] Extensión DevTool

Para usar la variable [!DNL Workfront Fusion] DevTool, primero debe instalarla.

1. Haga clic en [este vínculo](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/workfront-fusion-devtool.zip) para descargar la extensión de .
1. Una vez descargados los archivos, extráigalos a la carpeta que elija.
1. Abra una ficha en [!DNL Chrome]
1. En la barra de búsqueda de la pestaña , introduzca `chrome://extensions`.
1. Haga clic en el **[!UICONTROL Modo de desarrollador]** alterne en la parte superior derecha de la pantalla para habilitar el modo Desarrollador . Si se activa la opción a la derecha, el modo de desarrollador está activado.
1. Haga clic en **[!UICONTROL Cargar sin empaquetar]**.
1. Seleccione la carpeta que contiene la herramienta de desarrollo (donde extrajo los archivos en el paso 2).

   Una vez desempaquetado, DevTool aparece entre las demás extensiones de Chrome.

## Busque la variable [!DNL Workfront Fusion] Herramienta de desarrollo

Para usar la variable [!DNL Workfront Fusion] DevTool, debe agregar la variable [!DNL Workfront Fusion] Extensión de DevTool a su [!DNL Chrome] como se describe en [Instalación de la extensión DevTool de Chrome](#install-the-chrome-devtool-extension).

1. Abra su [!DNL Workfront Fusion] escenario.
1. Abrir [!DNL Chrome Developer Tools]:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Mac]</td> 
      <td>Comando + Opción + I</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Windows]</td> 
      <td> <p>Control + Mayús + I</p> <p> O </p> <p>F12</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Se recomienda acoplar el [!DNL Chrome Developer Console] en la parte inferior para mantener una mejor vista de sus módulos.

1. Haga clic en el **[!DNL Workfront Fusion]** en [!DNL Chrome Dev Tools].

## Utilice la variable [!DNL Workfront Fusion] Herramienta de desarrollo

Workfront Fusion DevTool se divide en 3 secciones principales. Puede encontrarlos en el panel izquierdo de la ventana DevTool.

* [Emisión en directo](#live-stream)
* [Depurador de escenarios](#scenario-debugger)
* [Herramientas](#tools)

### Emisión en directo

Transmisión en directo muestra lo que está sucediendo en segundo plano cuando hace clic en Ejecutar una vez en el escenario.

1. Haga clic en el **[!UICONTROL Emisión en directo]** icono ![](assets/live-stream-icon.png) para abrir la sección Transmisión en directo .
1. Realice una de las siguientes acciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Acción</th> 
      <th>Instrucciones</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ver información de solicitud</td> 
      <td> <p>Puede ver la siguiente información para cada módulo en su situación</p> 
       <ul> 
        <li> <p>Encabezados de solicitud (URL de extremo de API, método http, hora y fecha en que se llamó a la solicitud, encabezados de solicitud y cadena de consulta)</p> </li> 
        <li> <p>Cuerpo de la solicitud</p> </li> 
        <li> <p>Encabezados de respuesta</p> </li> 
        <li> <p>Cuerpo de respuesta</p> </li> 
       </ul> <p>Para ver esta información, haga clic en la pestaña correspondiente del panel derecho del [!DNL Workfront Fusion] Herramienta de desarrollo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Solicitudes de búsqueda y respuestas</p> </td> 
      <td> <p>Introduzca el término de búsqueda en el campo de búsqueda del panel izquierdo del [!DNL Workfront Fusion] DevTool para mostrar solo las solicitudes que contienen el término de búsqueda.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Eliminar lista de solicitudes </p> </td> 
      <td> <p>Haga clic en el icono de papelera en la esquina superior derecha del panel izquierdo de DevTool para borrar la lista de solicitudes registradas por el [!DNL Workfront Fusion] Herramienta de desarrollo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Habilitar el registro de consola</p> </td> 
      <td> <p>Haga clic en el icono del equipo <img src="assets/console-computer-icon.png"> en la esquina superior derecha del panel izquierdo de DevTool.</p> <p>El inicio de sesión en la consola se habilita cuando el icono del equipo está en verde.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Recupere la solicitud en formato JSON sin procesar o cURL</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong>JSON sin procesar</strong> </p> <p>Haga clic en <strong>[!UICONTROL Copiar RAW]</strong> en la esquina superior derecha del panel derecho de DevTool.</p> </li> 
        <li> <p><strong>cURL</strong> </p> <p>Haga clic en <strong>[!UICONTROL Copiar cURL]</strong> en la esquina superior derecha del panel derecho de DevTool.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Depurador de escenarios

El Depurador de escenarios es útil para escenarios más complejos. Muestra el historial de las ejecuciones del escenario y le permite buscar módulos por su nombre o ID.

1. Haga clic en el **[!UICONTROL Depurador de escenarios]** icono ![](assets/scenario-debugger-icon.png) para abrir Scenario Debugger.
1. (Opcional) Introduzca el término de búsqueda (nombre o ID de módulo) en el campo de búsqueda del panel izquierdo de [!DNL Workfront Fusion] DevTool en el [!UICONTROL Depurador de escenarios] para obtener más información.
1. Haga doble clic en el nombre del módulo para abrir su configuración en el editor de escenarios.
1. Para ver los detalles de la solicitud, haga clic en la operación deseada.

### Herramientas

La variable [!DNL Workfront Fusion] DevTool cuenta con herramientas que facilitan la configuración del escenario.

1. Haga clic en el **[!UICONTROL Herramientas]** icono ![](assets/console-tools-icon.png) para abrir Herramientas.
1. Seleccione la herramienta que desee utilizar
1. Configure los campos como se detalla a continuación.
1. Haga clic en **[!UICONTROL Ejecutar]**.

Herramientas y sus campos:

* [Enfoque en un módulo](#focus-a-module)
* [Buscar módulos por asignación](#find-modules-by-mapping)
* [Obtener metadatos de la aplicación](#get-app-metadata)
* [Copiar asignación](#copy-mapping)
* [Copiar filtro](#copy-filter)
* [Intercambiar conexión](#swap-connection)
* [Intercambiar variable](#swap-variable)
* [Intercambiar aplicación](#swap-app)
* [Base 64](#base-64)
* [Copiar nombre de módulo](#copy-module-name)
* [Origen de reasignación](#remap-source)
* [Resaltar aplicación](#highlight-app)
* [Migración de GS](#migrate-gs)

#### [!UICONTROL Enfoque en un módulo]

Abre la configuración del módulo especificado por ID.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Module ID]</td>
        <td>Introduzca el ID del módulo cuya configuración desea abrir.</td>
    </tr>
</table>

#### [!UICONTROL Buscar módulos por asignación]

Permite buscar los valores de los módulos para un término especificado. El resultado contiene ID de módulos que contienen el término que ha buscado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Palabra clave]</td> 
   <td> <p> Escriba el término que desee buscar. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Usar solo valores]</p> </td> 
   <td> <p>Active esta opción para buscar solo en los valores de los campos del módulo.</p> <p>Desactive esta opción para buscar también en los nombres de los campos del módulo.</p> <p>La búsqueda se realiza mediante los parámetros name y label .</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener metadatos de la aplicación]

Recupera los metadatos de la aplicación por el nombre o ID del módulo de la aplicación. Esto resulta útil, por ejemplo, cuando necesita conocer la versión de la aplicación utilizada en su escenario.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Seleccione el módulo para el que desea recuperar metadatos.</td>
    </tr>
</table>

#### [!UICONTROL Copiar asignación]

Copia valores del módulo de origen al módulo de destino.

>[!CAUTION]
>
>Asegúrese de establecer los módulos de origen y destino correctos. Si selecciona un tipo diferente de módulo, se eliminarán los valores del módulo de destino.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Seleccione el módulo o introduzca el ID del módulo desde el que desea copiar los valores de campo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Seleccione el módulo o introduzca el ID del módulo en el que desea insertar los valores del módulo de origen.</p> <p>Importante: Se sobrescribirán los valores del módulo de destino.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar filtro]

Copia la configuración del filtro del módulo de origen al módulo de destino.

>[!NOTE]
>
>La acción de copia se realiza en el filtro colocado en el lado izquierdo del módulo seleccionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Seleccione el módulo o introduzca el ID del módulo desde el que desea copiar los valores de filtro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Seleccione el módulo o introduzca el ID del módulo en el que desea insertar los valores de filtro del módulo de origen.</p> <p>Importante: Se sobrescribirán los valores del módulo de destino.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conservar configuración de ruta de reserva]</p> </td> 
   <td> <p>El filtro de origen se establece como la ruta de reserva. Active esta opción para establecer también que el filtro de destino se establece como ruta de reserva.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Intercambiar conexión]

Duplica una conexión del módulo de origen a cada módulo en el escenario de la misma aplicación.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Seleccione el módulo o introduzca el ID del módulo desde el que desea duplicar la conexión.</td>
    </tr>
</table>

#### [!UICONTROL Intercambiar variable]

Busca variables especificadas en el escenario y las reemplaza por una nueva variable.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variable que buscar]</td> 
   <td> <p> Busque la píldora de variables que desea reemplazar desde el módulo en su escenario y cópiela en este campo ([!UICONTROL Variable to Find]). En el campo , aparece con dos llaves. Ejemplo: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Reemplazar con]</p> </td> 
   <td> <p>Busque la píldora de variables con la que desea reemplazar la variable en el módulo de su escenario y cópiela en este campo ([!UICONTROL Variable to Find]). En el campo , aparece con dos llaves. Ejemplo: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module]</p> </td> 
   <td> <p>Seleccione el módulo en el que desea reemplazar la variable. Si no hay ningún módulo seleccionado, la variable se reemplazará en todo el escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Intercambiar aplicación]

Reemplaza la versión de la aplicación seleccionada en el escenario por otra versión de la aplicación.

Esto se puede utilizar, por ejemplo, para actualizar los módulos de las aplicaciones de Gmail y Email a la versión más reciente.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aplicación a reemplazar]</td> 
   <td> <p> Seleccione la aplicación que desea reemplazar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Reemplazar con]</p> </td> 
   <td> <p>Seleccione la aplicación con la que desea reemplazarla.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Base 64]

Permite codificar los datos introducidos en Base64 o descodificar Base64. Algunas solicitudes están codificadas en Base64. Esta herramienta puede resultar útil cuando desea buscar datos concretos en la solicitud codificada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Operation] </td> 
   <td> <p>Seleccione si desea codificar los datos del campo [!UICONTROL Datos sin procesar] a Base64 o descodificar Base64 a Datos sin procesar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Datos sin procesar]</p> </td> 
   <td> <p> Introduzca los datos que desea codificar en Base64 o Base64 si desea descodificarlos en datos sin procesar, según la opción seleccionada en el campo [!UICONTROL Operation] anterior.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar nombre de módulo]

Copia el nombre del módulo seleccionado en el portapapeles.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Module] </td> 
   <td> <p>Seleccione el módulo del que desea copiar el nombre.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Origen de reasignación]

Permite cambiar el origen de la asignación de un módulo a otro.

Primero debe agregar el módulo que desea usar como módulo de origen a la ruta en su escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module] </td> 
   <td> <p> Seleccione el módulo que desea reemplazar como fuente de asignación para otros módulos en su escenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Seleccione el módulo que desee utilizar como nuevo origen de asignación.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Módulo que editar]</p> </td> 
   <td> <p>Seleccione el módulo para el que desea cambiar la asignación si no desea cambiar la asignación en todo el escenario. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Resaltar aplicación]

Resalta los módulos de la aplicación especificada en su escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aplicación a resaltar] </td> 
   <td> <p> Seleccione la aplicación que desee resaltar en su escenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Versión] </p> </td> 
   <td> <p>Seleccione la versión de la aplicación que desee resaltar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Color de resaltado]</p> </td> 
   <td> <p> Introduzca el hexadecimal de color que desee utilizar para los módulos de resaltado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Migración de GS]

Esta herramienta se realiza especialmente para la actualización [!DNL Google Sheets] (heredado) de los últimos [!DNL Google Sheets] versión. Añade una nueva versión del módulo justo después de la versión heredada del módulo en la ruta del escenario.

Este módulo no requiere que establezca ningún parámetro.
