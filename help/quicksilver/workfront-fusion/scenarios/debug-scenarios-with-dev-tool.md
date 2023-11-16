---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Depuración de escenarios con Adobe Workfront Fusion Developer
description: La herramienta de desarrollo de Adobe Workfront Fusion le permite comprender y solucionar problemas de escenarios. La herramienta de desarrollo añade un panel adicional a las herramientas para desarrolladores de Chrome. Con este panel del depurador, puede comprobar todas las ejecuciones manuales de su escenario, revisar todas las operaciones realizadas y ver los detalles de cada llamada de API realizada. Puede ver qué módulo, operación o respuesta única causó el error y utilizar ese conocimiento para refinar el escenario.
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
source-git-commit: 27117543df0d2ba0a5c5035c71a3105d7a855345
workflow-type: tm+mt
source-wordcount: '1845'
ht-degree: 1%

---

# Depurar escenarios con [!DNL Adobe Workfront Fusion] Devtool

El [!DNL Adobe Workfront Fusion] Devtool le permite comprender y solucionar problemas de escenarios. Devtool añade un panel adicional a [!DNL Chrome Developer Tools]. Con este panel del depurador, puede comprobar todas las ejecuciones manuales de su escenario, revisar todas las operaciones realizadas y ver los detalles de cada llamada de API realizada. Puede ver qué módulo, operación o respuesta única causó el error y utilizar ese conocimiento para refinar el escenario.

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo], [!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]</p>
   </td>    </tr> 
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

## Acceso a Workfront Fusion DevTool

El acceso a Devtool difiere en función de si utiliza Fusion en la [!DNL Adobe Unified Experience].

* [Acceda a la herramienta Desarrollo en la [!DNL Adobe Unified Experience]](#access-the-devtool-in-the-adobe-unified-experience)
* [Acceda a la herramienta de desarrollo en el clásico [!DNL Fusion] experiencia](#access-the-devtool-in-the-classic-fusion-experience)

### Acceda a la herramienta Desarrollo en la [!DNL Adobe Unified Experience]

Si utiliza Fusion en el shell unificado de Adobe, puede acceder a la herramienta de desarrollo desde el editor de escenarios.

1. Vaya al Editor de escenarios para el escenario que desea depurar.

   Para localizar el Editor de escenarios, consulte [Editor de escenarios](/help/quicksilver/workfront-fusion/scenarios/scenario-editor.md).

1. Haga clic con el botón derecho en un área vacía de la página (no en un módulo).
1. Seleccionar **Abrir Devtool**.

>[!NOTE]
>
>Actualmente, solo la variable **Emisión en directo** y **Depurador de escenarios** Las áreas de la herramienta de desarrollo están disponibles para los usuarios en la experiencia unificada. El **Herramientas** Esta área no está disponible en la experiencia unificada en este momento.

### Acceda a la herramienta de desarrollo en el clásico [!DNL Fusion] experiencia

Para utilizar Devtool en el clásico [!DNL Fusion] experiencia, debe instalar un [!DNL Chrome] extensión. A continuación, puede utilizar esta extensión desde el [!DNL Chrome] Herramientas para desarrolladores.

* [Instale el Instale el [!DNL Chrome] Extensión Devtool](#install-the-chrome-devtool-extension)
* [Busque el [!DNL Workfront Fusion] Devtool](#locate-the-workfront-fusion-devtool)

#### Instale el [!DNL Chrome] Extensión Devtool

Puede añadir la variable [!DNL Workfront Fusion] Devtool a [!DNL Chrome] a través de [!UICONTROL [!DNL Chrome] Tienda web].

1. Clic [este vínculo](https://chrome.google.com/webstore/detail/workfront-fusion-Devtool/hkimbmkkmmejdnhbhoaefggkpkndfjnn/related) para ir a [!DNL Workfront Fusion] Devtool en el [!UICONTROL [!DNL Chrome] Tienda web].
1. Clic **[!UICONTROL Añadir a[!DNL Chrome]]**.
1. En la ventana que se abre, examine los permisos. Si acepta los permisos, haga clic en **[!UICONTROL Añadir extensión]**.

El [!DNL Workfront Fusion] La extensión Devtool se añade a su [!DNL Chrome] extensiones.


#### Busque el [!DNL Workfront Fusion] Devtool

Para usar la variable [!DNL Workfront Fusion] Devtool, debe añadir el [!DNL Workfront Fusion] Extensión Devtool a su [!DNL Chrome] explorador, tal como se describe en [Instale la extensión de Chrome DevTool](#install-the-chrome-Devtool-extension).

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
   >Se recomienda acoplar el [!DNL Chrome Developer Console] hasta la parte inferior para mantener una mejor vista de sus módulos.

1. Haga clic en **[!DNL Workfront Fusion]** pestaña en [!DNL Chrome Dev Tools].

## Utilice el [!DNL Workfront Fusion] Devtool

Workfront Fusion Devtool se divide en 3 secciones principales. Puede encontrarlas en el panel izquierdo de la ventana de Devtool.

* [Emisión en directo](#live-stream)
* [Depurador de escenarios](#scenario-debugger)
* [Herramientas](#tools)

### Emisión en directo

La emisión en directo muestra lo que está sucediendo en segundo plano cuando hace clic en Ejecutar una vez en su escenario.

1. Haga clic en **[!UICONTROL Emisión en directo]** icono ![](assets/live-stream-icon.png) para abrir la sección Emisión en directo.
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
        <li> <p>Encabezados de solicitud (URL de extremo de API, método http, hora y fecha en que se llamó a la solicitud, encabezados de solicitud y cadena de consulta)</p> </li> 
        <li> <p>Cuerpo de solicitud</p> </li> 
        <li> <p>Encabezados de respuesta</p> </li> 
        <li> <p>Cuerpo de respuesta</p> </li> 
       </ul> <p>Para ver esta información, haga clic en la pestaña adecuada en el panel derecho del [!DNL Workfront Fusion] Devtool.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Solicitudes de búsqueda y respuestas</p> </td> 
      <td> <p>Introduzca el término de búsqueda en el campo de búsqueda del panel izquierdo del [!DNL Workfront Fusion] Devtool para mostrar solo las solicitudes que contienen el término de búsqueda.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Eliminar lista de solicitudes </p> </td> 
      <td> <p>Haga clic en el icono de la papelera en la esquina superior derecha del panel izquierdo de Devtool para borrar la lista de solicitudes registradas por. [!DNL Workfront Fusion] Devtool. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Activar registro de consola</p> </td> 
      <td> <p>Haga clic en el icono del equipo <img src="assets/console-computer-icon.png"> en la esquina superior derecha del panel izquierdo de Devtool.</p> <p>El inicio de sesión en la consola está habilitado cuando el icono del equipo está en verde.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Recuperar la solicitud en formato JSON sin procesar o cURL</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong>JSON sin procesar</strong> </p> <p>Clic <strong>[!UICONTROL Copiar RAW]</strong> en la esquina superior derecha del panel derecho de Devtool.</p> </li> 
        <li> <p><strong>cURL</strong> </p> <p>Clic <strong>[!UICONTROL Copiar cURL]</strong> en la esquina superior derecha del panel derecho de Devtool.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Depurador de escenarios

El depurador de escenarios resulta útil para escenarios más complejos. Muestra el historial de ejecuciones de escenarios y le permite buscar módulos por su nombre o ID.

1. Haga clic en **[!UICONTROL Depurador de escenarios]** icono ![](assets/scenario-debugger-icon.png) para abrir Scenario Debugger.
1. (Opcional) Introduzca el término de búsqueda (nombre o ID de módulo) en el campo de búsqueda del panel izquierdo de [!DNL Workfront Fusion] Devtool en la [!UICONTROL Depurador de escenarios] sección.
1. Haga doble clic en el nombre del módulo para abrir su configuración en el editor de escenarios.
1. Vea los detalles de la solicitud haciendo clic en la operación deseada.

### Herramientas

>[!NOTE]
>
>Actualmente, esta área no está disponible para los usuarios de la experiencia unificada de Adobe.

El [!DNL Workfront Fusion] Devtool incluye herramientas que facilitan la configuración de su escenario.

1. Haga clic en **[!UICONTROL Herramientas]** icono ![](assets/console-tools-icon.png) para abrir las herramientas.
1. Seleccione la herramienta que desee utilizar
1. Configure los campos como se detalla a continuación.
1. Clic **[!UICONTROL Ejecutar]**.

Herramientas y sus campos:

* [Enfoque de un módulo](#focus-a-module)
* [Buscar módulos por asignación](#find-modules-by-mapping)
* [Obtener metadatos de aplicación](#get-app-metadata)
* [Copiar asignación](#copy-mapping)
* [Copiar filtro](#copy-filter)
* [Intercambiar conexión](#swap-connection)
* [Intercambiar variable](#swap-variable)
* [Intercambiar aplicación](#swap-app)
* [Base 64](#base-64)
* [Copiar nombre de módulo](#copy-module-name)
* [Origen de reasignación](#remap-source)
* [Resaltar aplicación](#highlight-app)
* [Migrar GS](#migrate-gs)

#### [!UICONTROL Enfoque de un módulo]

Abre la configuración del módulo especificado por identificador.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL ID de módulo]</td>
        <td>Introduzca el ID del módulo cuya configuración desea abrir.</td>
    </tr>
</table>

#### [!UICONTROL Buscar módulos por asignación]

Permite buscar los valores de los módulos para un término especificado. La salida contiene los ID de los módulos que contienen el término que ha buscado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Palabra clave [!UICONTROL]</td> 
   <td> <p> Introduzca el término que desea buscar. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Utilizar sólo valores]</p> </td> 
   <td> <p>Active esta opción para buscar únicamente en los valores de los campos del módulo.</p> <p>Deshabilite esta opción para buscar también en los nombres de los campos de módulo.</p> <p>La búsqueda se realiza mediante los parámetros name y label.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener metadatos de aplicación]

Recupera los metadatos de la aplicación por el nombre o ID del módulo de la aplicación. Esto resulta útil, por ejemplo, cuando necesita saber la versión de la aplicación utilizada en su escenario.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Módulo de origen]</td>
        <td>Seleccione el módulo para el que desea recuperar metadatos.</td>
    </tr>
</table>

#### [!UICONTROL Copiar asignación]

Copia los valores del módulo de origen en el módulo de destino.

>[!CAUTION]
>
>Asegúrese de establecer los módulos de origen y destino correctos. Si selecciona un tipo de módulo diferente, se eliminarán los valores del módulo de destino.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Módulo de origen]</td> 
   <td> <p> Seleccione el módulo o introduzca el ID del módulo desde el que desea copiar los valores de campo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Módulo de destino]</p> </td> 
   <td> <p>Seleccione el módulo o introduzca el ID del módulo en el que desea insertar los valores del módulo de origen.</p> <p>Importante: Los valores del módulo de destino se sobrescribirán.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Módulo de origen]</td> 
   <td> <p> Seleccione el módulo o introduzca el ID del módulo desde el que desea copiar los valores de filtro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Módulo de destino]</p> </td> 
   <td> <p>Seleccione el módulo o introduzca el ID del módulo en el que desea insertar los valores de filtro desde el módulo de origen.</p> <p>Importante: Los valores del módulo de destino se sobrescribirán.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conservar configuración de ruta de reserva]</p> </td> 
   <td> <p>El filtro de origen se establece como ruta de reserva. Active esta opción para establecer también que el filtro de destino se establezca como ruta de reserva.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Intercambiar conexión]

Duplica una conexión desde el módulo de origen a cada módulo en el escenario de la misma aplicación.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Módulo de origen]</td>
        <td>Seleccione el módulo o introduzca el ID del módulo desde el que desea duplicar la conexión.</td>
    </tr>
</table>

#### [!UICONTROL Intercambiar variable]

Busca variables especificadas en el escenario y las reemplaza por una variable nueva.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variable que buscar]</td> 
   <td> <p> Busque la píldora de variables que desee reemplazar desde el módulo en su escenario y cópiela en este campo ([!UICONTROL Variable to Find]). En el campo, aparece con llaves dobles. Ejemplo: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Reemplazar con]</p> </td> 
   <td> <p>Busque la píldora de variables con la que desea reemplazar la variable desde el módulo en su escenario y cópiela en este campo ([!UICONTROL Variable to Find]). En el campo, aparece con llaves dobles. Ejemplo: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Módulo]</p> </td> 
   <td> <p>Seleccione el módulo en el que desea reemplazar la variable. Si no se selecciona ningún módulo, la variable se reemplazará en todo el escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Intercambiar aplicación]

Reemplaza la versión de la aplicación seleccionada en su escenario con otra versión de la aplicación.

Esto se puede utilizar, por ejemplo, para actualizar los módulos de las aplicaciones de Gmail y de correo electrónico a la versión más reciente.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Aplicación [!UICONTROL para reemplazar]</td> 
   <td> <p> Seleccione la aplicación que desea reemplazar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Reemplazar con]</p> </td> 
   <td> <p>Seleccione la aplicación con la que desea reemplazarla.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Base 64]

Permite codificar los datos introducidos en Base64 o descodificar Base64. Algunas solicitudes se codifican en Base64. Esta herramienta puede resultar útil cuando desea buscar datos concretos en la solicitud codificada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Operación] </td> 
   <td> <p>Seleccione si desea codificar los datos del campo [!UICONTROL Raw Data] en Base64 o descodificar Base64 en Raw Data.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Módulo] </td> 
   <td> <p>Seleccione el módulo del que desea copiar el nombre.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Origen de reasignación]

Permite cambiar el origen de asignación de un módulo a otro.

Primero debe agregar el módulo que desea usar como módulo de origen a la ruta de su escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Módulo de origen] </td> 
   <td> <p> Seleccione el módulo que desea reemplazar como origen de asignación para otros módulos de su escenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Módulo de destino]</p> </td> 
   <td> <p>Seleccione el módulo que desee utilizar como nuevo origen de asignación.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Módulo [!UICONTROL para editar]</p> </td> 
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
   <td role="rowheader">Aplicación [!UICONTROL para resaltar] </td> 
   <td> <p> Seleccione la aplicación que desea que aparezca resaltada en su escenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Versión] </p> </td> 
   <td> <p>Seleccione la versión de la aplicación que desea resaltar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Color de resaltado]</p> </td> 
   <td> <p> Introduzca el hex de color que desee utilizar para los módulos de resaltado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Migrar GS]

Esta herramienta está diseñada especialmente para actualizar [!DNL Google Sheets] Módulos (heredados) a la última versión [!DNL Google Sheets] versión. Añade una nueva versión del módulo justo después de la versión heredada del módulo en la ruta del escenario.

Este módulo no requiere que establezca ningún parámetro.
