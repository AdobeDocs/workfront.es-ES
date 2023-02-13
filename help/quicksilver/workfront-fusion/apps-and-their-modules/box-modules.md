---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos de caja
description: En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan Box, así como conectarlos a varias aplicaciones y servicios de terceros. supervisa una carpeta especificada para comprobar los cambios en el archivo, modificar y eliminar archivos existentes o cargar nuevos archivos a una carpeta.
author: Becky
feature: Workfront Fusion
exl-id: 965ce570-40bf-474d-b318-0d2de8be6b9d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 0%

---

# Módulos de caja

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Box], así como conectarlo a varias aplicaciones y servicios de terceros. supervisa una carpeta especificada para comprobar los cambios en el archivo, modificar y eliminar archivos existentes o cargar nuevos archivos a una carpeta.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Para usar [!DNL Box] módulos, debe tener un [!DNL Box] cuenta.

## [!DNL Box] módulos y sus campos

Al configurar [!DNL Box] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL Box] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Déclencheur

* [[!UICONTROL Nuevo evento]](#new-event)
* [[!UICONTROL Archivos de Watch]](#watch-files)

#### [!UICONTROL Nuevo evento]

Este módulo de déclencheur instantáneo inicia un escenario cuando se agrega, mueve, copia, elimina, bloquea o desbloquea un archivo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Weblock]</td> 
   <td> <p>Seleccione el vínculo web que desea utilizar para ver los mensajes salientes. Para añadir un vínculo web, haga clic en <strong>[!UICONTROL Agregar]</strong> e introduzca el nombre y la conexión del vínculo web.</p> <p> Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Box] a [!UICONTROL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!UICONTROL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Número máximo de eventos devueltos]</p> </td> 
   <td> <p>Introduzca el número más alto de eventos que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Archivos de Watch]

Este módulo de déclencheur inicia un escenario cuando se agrega un nuevo archivo o se actualiza un archivo existente en una carpeta que se está viendo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Box] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  <tr> 
   <td role="rowheader">Watch</td> 
   <td> <p>Seleccione el tipo de archivos que desea ver.</p> 
    <ul> 
     <li> <p><strong>Solo archivos nuevos</strong> </p> <p>El escenario se iniciará cuando se añada un nuevo archivo.</p> </li> 
     <li> <p><strong>Nuevos archivos y todos los cambios</strong> </p> <p>El escenario se inicia cuando se agrega un archivo, o cuando se modifica el contenido del archivo o un atributo de archivo (como su nombre).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Número máximo de archivos descargados</p> </td> 
   <td> <p>Introduzca el número más alto de archivos que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Cargar] un archivo](#upload-a-file)
* [[!UICONTROL Actualizar un archivo]](#update-a-file)
* [[!UICONTROL Eliminar un archivo]](#delete-a-file)
* [[!UICONTROL Obtener un archivo]](#get-a-file)

#### [!UICONTROL Cargar un archivo]

Este módulo de acción carga un archivo.

El archivo se especifica. También puede proporcionar un nuevo nombre de archivo para el archivo.

El módulo devuelve el ID del archivo y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Box] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Si este módulo no se ejecuta correctamente, tenga en cuenta lo siguiente:
>
>* El tamaño del archivo puede superar el límite máximo de tamaño de archivo para su [!DNL Box] o puede que haya usado todo su [!DNL Box] cuota de almacenamiento de la cuenta. Para obtener más espacio de almacenamiento, elimine los archivos existentes de [!DNL Box] o actualice su [!DNL Box] cuenta.
>* [!DNL Box] no carga más de un archivo con el mismo nombre en una sola carpeta. Si la carpeta de destino contiene un archivo con el mismo nombre que el archivo que se está cargando, la ejecución del escenario termina con un error. Para evitarlo, cambie el nombre del archivo . Si desea actualizar el archivo, utilice la variable **[!UICONTROL Actualizar un archivo]** módulo.


#### [!UICONTROL Actualizar un archivo]

Este módulo de acción actualiza un archivo.

Especifique el ID del archivo.

El módulo devuelve el ID del archivo y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Box] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td>Introduzca o asigne el ID exclusivo del archivo que desea que actualice el módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un archivo]

Este módulo de acción elimina un archivo.

Especifique el ID del archivo.

El módulo devuelve el ID del archivo y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Box] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td>Introduzca o asigne el ID exclusivo del archivo que desea que actualice el módulo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un archivo]

Este módulo de acción descarga un archivo.

Especifique el ID del archivo.

El módulo devuelve el ID del archivo y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

>[!NOTE]
>
>Este módulo es útil para proporcionar archivos a módulos posteriores.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Box] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td>Introduzca o asigne el ID exclusivo del archivo que desea que actualice el módulo.</td> 
  </tr> 
 </tbody> 
</table>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Possible problems</h2>
-->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This is drafted out because we don't have a download module for Box yet</p>
-->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Watch files trigger module doesn't download a file contained in the folder.</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">There are several situations when downloading a file fails:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The current file lock setting does not allow the file to be downloaded or the downloading of the file is disabled. In this case, the file is ignored.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">When the scenario started, the file was being uploaded to the server and was not ready to be downloaded. The scenario run gets stopped and Workfront Fusion tries downloading the file again during the next execution of the scenario.</li>
  -->
