---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Depurar escenarios con Adobe Workfront Fusion Devtool
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1861'
ht-degree: 95%

---

# Depurar escenarios con [!DNL Adobe Workfront Fusion] Devtool

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Depurar un escenario](https://experienceleague.adobe.com/docs/workfront-fusion/using/manage-scenarios/debug-a-scenario.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

[!DNL Adobe Workfront Fusion] Devtool le permite comprender y solucionar problemas de escenarios. Devtool añade un panel adicional a las [!DNL Chrome Developer Tools]. Con este panel del depurador, puede comprobar todas las ejecuciones manuales de su escenario, revisar todas las operaciones realizadas y ver los detalles de cada llamada de API realizada. Puede ver qué módulo, operación o respuesta única causó el error y utilizar ese conocimiento para perfeccionar el escenario.

>[!NOTE]
>
>El inicio de sesión en el panel del depurador estará limitado o no estará disponible en escenarios confidenciales, ejecuciones automáticas y operaciones satisfactorias.

Para ver un vídeo introductorio y un tutorial de Fusion Devtool, consulte

* [Herramienta de desarrollo de Fusion](https://video.tv.adobe.com/v/3427031/){target=_blank}.
* [Tutorial de Devtool](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/troubleshooting-and-error-handling/dev-tool-walkthrough.html)

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

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
   <td role="rowheader">Licencia** de [!UICONTROL Adobe Workfront Fusion]</td> 
  <td>
   <p>Requisito de licencia actual: no se requiere la licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre las licencias de [!DNL Adobe Workfront Fusion], consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Acceder a la herramienta Devtool de Workfront Fusion

El acceso a la herramienta Devtool difiere en función de si está utilizando Fusion en [!DNL Adobe Unified Experience].

* [Acceder a la herramienta Devtool en  [!DNL Adobe Unified Experience]](#access-the-devtool-in-the-adobe-unified-experience)
* [Acceder a la herramienta Devtool en la experiencia clásica de  [!DNL Fusion] ](#access-the-devtool-in-the-classic-fusion-experience)

### Acceder a la herramienta Devtool en [!DNL Adobe Unified Experience] o en la nueva experiencia de Fusion

Si utiliza Fusion en Adobe Unified Shell o ha actualizado a la nueva experiencia de Fusion, podrá acceder a la herramienta Devtool desde el editor de escenarios.

1. Haga clic en el icono **Helper tools** ![Helper tools](assets/debugger-icon.png) cerca de la parte inferior de la pantalla.

O

1. Vaya al editor de escenarios correspondiente al escenario que desea depurar.

   Para localizar el editor de escenarios, consulte [Editor de escenarios](/help/quicksilver/workfront-fusion/scenarios/scenario-editor.md).

1. Haga clic con el botón derecho en un área vacía de la página (no en un módulo).
1. Seleccione **abrir Devtool**.

### Acceder a la herramienta Devtool en la experiencia clásica de [!DNL Fusion]

Para usar la herramienta Devtool en la experiencia clásica de [!DNL Fusion], debe instalar la extensión de [!DNL Chrome]. A continuación, puede usar esta extensión desde las herramientas para desarrolladores de [!DNL Chrome].

* [Instalar la extensión de la herramienta Devtool de  [!DNL Chrome] ](#install-the-chrome-devtool-extension)
* [Localizar la herramienta Devtool de  [!DNL Workfront Fusion] ](#locate-the-workfront-fusion-devtool)

#### Instalación de la extensión de la herramienta Devtool de [!DNL Chrome]

Puede añadir la herramienta Devtool de [!DNL Workfront Fusion] a [!DNL Chrome] a través de la tienda web] de [!UICONTROL [!DNL Chrome].

1. Haga clic en [este vínculo](https://chromewebstore.google.com/u/1/detail/workfront-fusion-devtool/hkimbmkkmmejdnhbhoaefggkpkndfjnn) para ir a la herramienta Devtool de [!DNL Workfront Fusion] en la tienda web] de [!UICONTROL [!DNL Chrome].
1. Haga clic en **[!UICONTROL Añadir columna[!DNL Chrome]]**.
1. En la ventana que se abre, examine los permisos. Si está de acuerdo con los permisos, haga clic en **[!UICONTROL Añadir extensión]**.

La extensión de la herramienta Devtool de [!DNL Workfront Fusion]se ha añadido a las extensiones de [!DNL Chrome].


#### Busque la herramienta Devtool de [!DNL Workfront Fusion]

Para usar la la herramienta Devtool de [!DNL Workfront Fusion], debe añadir la extensión de la herramienta Devtool de [!DNL Workfront Fusion] al explorador de [!DNL Chrome], tal como se describe en [Instalar la extensión Devtool de Chrome](#install-the-chrome-Devtool-extension).

1. Abra el escenario de [!DNL Workfront Fusion].
1. Abra [!DNL Chrome Developer Tools].

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
   >Se recomienda acoplar [!DNL Chrome Developer Console] a la parte inferior para mantener una mejor vista de los módulos.

1. Haga clic en la pestaña **[!DNL Workfront Fusion]** de [!DNL Chrome Dev Tools].

## Uso de herramienta Devtool de [!DNL Workfront Fusion]

La herramienta Devtool de Workfront Fusion se divide en tres secciones principales. Puede encontrarlas en el panel izquierdo de la ventana de Devtool.

* [Live Stream](#live-stream)
* [Depurador de escenario](#scenario-debugger)
* [Herramientas](#tools)

### Live Stream

Live Stream muestra lo que está sucediendo en segundo plano cuando hace clic en Ejecutar una vez en su escenario.

1. Haga clic en el icono **[!UICONTROL Live Stream]** ![](assets/live-stream-icon.png) para abrir la sección Live Stream.
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
      <td> <p>Puede ver la siguiente información para cada módulo de su escenario</p> 
       <ul> 
        <li> <p>Encabezados de solicitud (URL de extremo de API, método HTTP, hora y fecha en que se llamó a la solicitud, encabezados de solicitud y cadena de consulta)</p> </li> 
        <li> <p>Cuerpo de solicitud</p> </li> 
        <li> <p>Encabezados de respuesta</p> </li> 
        <li> <p>Cuerpo de respuesta</p> </li> 
       </ul> <p>Para ver esta información, haga clic en la pestaña correspondiente del panel derecho de la herramienta Devtool de [!DNL Workfront Fusion].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Buscar solicitudes y respuestas</p> </td> 
      <td> <p>Escriba el término de búsqueda en el campo de búsqueda del panel izquierdo de la herramienta Devtool de [!DNL Workfront Fusion] para mostrar solamente las solicitudes que contienen el término de búsqueda.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Eliminar lista de solicitudes </p> </td> 
      <td> <p>Haga clic en el icono de papelera en la esquina superior derecha del panel izquierdo de Devtool para borrar la lista de solicitudes registradas por la herramienta Devtool de [!DNL Workfront Fusion]. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Habilitar registro de consola</p> </td> 
      <td> <p>Haga clic en el icono del equipo <img src="assets/console-computer-icon.png"> en la esquina superior derecha del panel izquierdo de Devtool.</p> <p>El registro en la consola está habilitado cuando el icono del equipo está en verde.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Recuperar la solicitud en formato Raw JSON o cURL</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong>Raw JSON</strong> </p> <p>Haga clic en <strong>[!UICONTROL Copy RAW]</strong> en la esquina superior derecha del panel derecho de Devtool.</p> </li> 
        <li> <p><strong>cURL</strong> </p> <p>Haga clic en <strong>[!UICONTROL Copy cURL]</strong> en la esquina superior derecha del panel derecho de Devtool.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Depurador de escenario

El depurador de escenario resulta útil para escenarios más complejos. Muestra el historial de ejecuciones de escenarios y le permite buscar módulos por su nombre o ID.

1. Haga clic en el icono **[!UICONTROL Depurador de escenario]** ![](assets/scenario-debugger-icon.png) para abrir el Depurador de escenario.
1. (Opcional) Introduzca el término de búsqueda (nombre o ID de módulo) en el campo de búsqueda del panel izquierdo de [!DNL Workfront Fusion] Devtool en la sección [!UICONTROL Depurador de escenario].
1. Haga doble clic en el nombre del módulo para abrir su configuración en el editor de escenarios.
1. Vea los detalles de la solicitud haciendo clic en la operación deseada.

### Herramientas

[!DNL Workfront Fusion] Devtool incluye herramientas que facilitan la configuración del escenario.

1. Haga clic en el icono **[!UICONTROL Herramientas]** ![](assets/console-tools-icon.png) para abrir las herramientas.
1. Seleccione la herramienta que desee utilizar.
1. Configure los campos como se indica a continuación.
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
* [Reasignar origen](#remap-source)
* [Resaltar aplicación](#highlight-app)
* [Migrar GS](#migrate-gs)

#### [!UICONTROL Enfoque en un módulo]

Abre la configuración del módulo especificado por identificador.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Module ID]</td>
        <td>Introduzca el ID del módulo cuya configuración desea abrir.</td>
    </tr>
</table>

#### [!UICONTROL Buscar módulos por asignación]

Permite buscar los valores de los módulos para el término especificado. La salida contiene los ID de los módulos que contienen el término que se ha buscado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Keyword]</td> 
   <td> <p> Introduzca el término que desea buscar. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Use Only Values]</p> </td> 
   <td> <p>Active esta opción para buscar únicamente en los valores de los campos del módulo.</p> <p>Deshabilite esta opción para buscar también en los nombres de los campos del módulo.</p> <p>La búsqueda se realiza mediante los parámetros de nombre y etiqueta.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener metadatos de la aplicación]

Recupera los metadatos de la aplicación por el nombre o ID del módulo de la aplicación. Esto resulta útil, por ejemplo, cuando necesita saber la versión de la aplicación utilizada en su escenario.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Seleccione el módulo cuyos metadatos desea recuperar.</td>
    </tr>
</table>

#### [!UICONTROL Copiar asignación]

Copia los valores del módulo de origen en el módulo de destino.

>[!CAUTION]
>
>Asegúrese de establecer los módulos de origen y de destino correctos. Si selecciona un tipo de módulo diferente, se eliminarán los valores del módulo de destino.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Seleccione el módulo o introduzca el ID del módulo cuyos valores de campo desea copiar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Seleccione el módulo o introduzca el ID del módulo en el que desea insertar los valores del módulo de origen.</p> <p>Importante: los valores del módulo de destino se sobrescribirán.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar filtro]

Copia la configuración del filtro del módulo de origen al módulo de destino.

>[!NOTE]
>
>La acción de copiar se realiza en el filtro colocado en el lado izquierdo del módulo seleccionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Seleccione el módulo o introduzca el ID del módulo del que desea copiar los valores de filtro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Seleccione el módulo o introduzca el ID del módulo en el que desea insertar los valores de filtro desde el módulo de origen.</p> <p>Importante: los valores del módulo de destino se sobrescribirán.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Preserve Fallback Route setting]</p> </td> 
   <td> <p>El filtro de origen se establece como ruta de reserva. Active esta opción para establecer también que el filtro de destino se establezca como ruta de reserva.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Intercambiar conexión]

Duplica una conexión desde el módulo de origen a cada uno de los módulos en el escenario de la misma aplicación.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Seleccione el módulo o introduzca el ID del módulo del que desea duplicar la conexión.</td>
    </tr>
</table>

#### [!UICONTROL Intercambiar variable]

Busca las variables especificadas en el escenario y las reemplaza por una variable nueva.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variable to Find]</td> 
   <td> <p> Localice la píldora de variables que desea reemplazar desde el módulo en su escenario y cópiela en este campo ([!UICONTROL Variable to Find]). En el campo, aparece entre corchetes dobles. Ejemplo: <code>&#123;&#123;5.value&#125;&#125;</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Replace With]</p> </td> 
   <td> <p>Localice la píldora de variables por la que desea reemplazar la variable desde el módulo en su escenario y cópiela en el campo ([!UICONTROL Variable to Find]). En el campo, aparece entre corchetes dobles. Ejemplo: <code>&#123;&#123;5.value&#125;&#125;</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module]</p> </td> 
   <td> <p>Seleccione el módulo en el que desea reemplazar la variable. Si no se selecciona ningún módulo, la variable se reemplazará en todo el escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Intercambiar aplicación]

Reemplaza la versión de la aplicación seleccionada en su escenario por otra versión de la aplicación.

Esto se puede utilizar, por ejemplo, para actualizar los módulos de las aplicaciones de Gmail y de correo electrónico a la versión más reciente.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL App to be Replaced]</td> 
   <td> <p> Seleccione la aplicación que desea reemplazar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Replace with]</p> </td> 
   <td> <p>Seleccione la aplicación por la que desea reemplazarla.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Base 64]

Le permite codificar los datos introducidos en Base64 o descodificar Base64. Algunas solicitudes se codifican en Base64. Esta herramienta puede resultar útil cuando desea buscar datos concretos en la solicitud codificada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Operation] </td> 
   <td> <p>Seleccione si desea codificar los datos del campo [!UICONTROL Raw Data] a Base64 o descodificar Base64 a Raw Data.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Raw Data]</p> </td> 
   <td> <p> Introduzca los datos que desea codificar a Base64 o Base64 si desea descodificarlos a datos sin procesar, según la opción seleccionada en el campo [!UICONTROL Operation] anterior.</p> </td> 
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
   <td> <p>Seleccione el módulo del que desea copiar el nombre. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Reasignar origen]

Le permite cambiar el origen de la asignación de un módulo a otro.

Primero debe añadir el módulo para utilizarlo como módulo de origen para la ruta en un escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module] </td> 
   <td> <p> Seleccione el módulo que desea reemplazar como origen de asignación para otros módulos de su escenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Seleccione el módulo que desee utilizar como nuevo origen de asignación.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module to Edit]</p> </td> 
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
   <td role="rowheader">[!UICONTROL App to be Highlighted] </td> 
   <td> <p> Seleccione la aplicación que desea que aparezca resaltada en su escenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Version] </p> </td> 
   <td> <p>Seleccione la versión de la aplicación que desea resaltar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Highlight Color]</p> </td> 
   <td> <p> Introduzca el hexadecimal de color que desee utilizar para resaltar módulos.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Migrar GS]

Esta herramienta está diseñada especialmente para actualizar módulos (heredados) de [!DNL Google Sheets] a la última versión de [!DNL Google Sheets]. Añade una nueva versión del módulo justo después de la versión heredada del módulo en la ruta del escenario.

Este módulo no requiere que establezca ningún parámetro.
