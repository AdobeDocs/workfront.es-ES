---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos Microsoft OneDrive
description: En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan OneDrive, así como conectarlos a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 13a25c6c-bdf1-467d-bd90-ebd763c59235
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3934'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL OneDrive], así como conectarlo a varias aplicaciones y servicios de terceros.

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

Para usar [!DNL OneDrive] módulos, debe tener un [!DNL Microsoft OneDrive] cuenta.

## Conexión de [!DNL OneDrive] servicio a [!DNL Workfront Fusion]

Para obtener instrucciones sobre cómo conectar su [!DNL OneDrive] cuenta para [!UICONTROL Workfront Fusion], consulte [Crear una conexión con [!UICONTROL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Microsoft OneDrive] módulos y sus campos

Al configurar [!DNL OneDrive] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL OneDrive] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Archivo/Carpeta](#filefolder)
* [Otro](#other)

### Archivo/Carpeta

* [[!UICONTROL Archivos/carpetas de inspección]](#watch-filesfolders)
* [[!UICONTROL Buscar archivos/carpetas]](#search-filesfolders)
* [[!UICONTROL Obtener un archivo]](#get-a-file)
* [[!UICONTROL Descargar un archivo]](#download-a-file)
* [[!UICONTROL Cargar un archivo]](#upload-a-file)
* [[!UICONTROL Crear una carpeta]](#create-a-folder)
* [[!UICONTROL Obtener un vínculo compartido]](#get-a-share-link)
* [[!UICONTROL Mover un archivo/carpeta]](#move-a-filefolder)
* [[!UICONTROL Copiar un archivo]](#copy-a-file)
* [[!UICONTROL Eliminar un archivo/carpeta]](#delete-a-filefolder)

#### [!UICONTROL Archivos/carpetas de inspección]

Este módulo de déclencheur inicia un escenario cuando se crea o actualiza un archivo o carpeta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obtener instrucciones sobre cómo conectar su [!DNL OneDrive] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivos/Carpetas de inspección]</td> 
   <td> <p>Seleccione cómo desea ver los archivos o carpetas:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Por Hora De Creación]</b> </p> <p>Busque archivos o carpetas nuevos.</p> </li> 
     <li> <p><b>[!UICONTROL Por Tiempo Actualizado]</b> </p> <p>Busque archivos o carpetas existentes actualizados.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su [!DNL OneDrive] ubicación]</td> 
   <td> <p>Seleccione la ubicación que desee ver:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea que el módulo introduzca un ID de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Introduzca el ID de la unidad que desea que vea el módulo.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> <p>Vaya a la carpeta que desea que vea el módulo. También puede introducir una consulta para filtrar los resultados devueltos.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Compartido Conmigo]</b> </p> <p>El módulo observa los archivos que se han compartido con el propietario de la unidad.</p> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el sitio de SharePoint que desea que vea el módulo. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!UICONTROL Unidad del grupo]</b> </p> <p>Seleccione el grupo cuya unidad desee que vea el módulo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir un tipo de elemento]</td> 
   <td> <p>Seleccione si desea ver archivos, carpetas o ambos.</p> <p>Nota: No puede ver carpetas en una unidad [!UICONTROL compartido conmigo].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>



#### [!UICONTROL Buscar archivos/carpetas]

Este módulo de búsqueda devuelve archivos y carpetas según los criterios establecidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obtener instrucciones sobre cómo conectar su [!DNL OneDrive] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su [!DNL OneDrive] ubicación]</td> 
   <td> <p>Seleccione la ubicación que desee buscar:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea que el módulo introduzca un ID de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Introduzca el ID de la unidad que desea que busque el módulo.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> <p>Vaya a la carpeta en la que desea que busque el módulo. También puede introducir una consulta para filtrar los resultados devueltos.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Compartido Conmigo]</b> </p> <p>El módulo busca los archivos que se han compartido con el propietario de la unidad.</p> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el [!DNL SharePoint] Sitio que desea que busque el módulo. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!UICONTROL Unidad del grupo]</b> </p> <p>Seleccione el grupo cuya unidad desee que busque el módulo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir un tipo de elemento]</td> 
   <td> <p>Seleccione si desea buscar archivos, carpetas o ambos.</p> <p>Nota: No puede buscar carpetas en una unidad [!UICONTROL Compartido conmigo].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un archivo]

Este módulo de acción obtiene los metadatos de un archivo especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obtener instrucciones sobre cómo conectar su [!DNL OneDrive] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrar (ID de archivo y ruta de archivo)]</td> 
   <td>Seleccione si desea identificar el archivo por ID de archivo o por la ruta de archivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir un ID de archivo] / [!UICONTROL Ruta de archivo]</td> 
   <td> <p>Seleccione cómo desea introducir el ID de archivo o la ruta de archivo:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Entrar manualmente]</b> </p> <p>Seleccione esta opción si desea introducir el ID o la ruta directamente, o asignarla desde un módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Seleccionar de una lista]</b> </p> <p>Seleccione esta opción si desea seleccionarla de una lista de archivos o rutas disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su [!DNL OneDrive] ubicación]</td> 
   <td> <p>Seleccione la ubicación que desee buscar:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea que el módulo introduzca un ID de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Introduzca el ID de la unidad que contiene el archivo que desea obtener.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el sitio de SharePoint que contiene el archivo que desea obtener. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!UICONTROL Unidad del grupo]</b> </p> <p>Seleccione el grupo cuya unidad contiene el archivo que desea obtener.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de unidad]</td> 
   <td> <p>Seleccione o asigne la unidad que contiene el archivo que desea obtener. Este campo no está disponible si ha seleccionado [!UICONTROL No] en el campo [!UICONTROL Habilitar para introducir un ID de unidad].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td> 
   <td> <p>Si ha seleccionado [!UICONTROL Entrar manualmente], introduzca o asigne el ID de archivo o la ruta del archivo que desea obtener.</p> <p>Si ha seleccionado [!UICONTROL Seleccionar de la lista], seleccione el archivo que desea obtener.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Descargar un archivo]

Este módulo de acción descarga el archivo especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obtener instrucciones sobre cómo conectar su [!DNL OneDrive] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrar (ID de archivo y ruta de archivo)]</td> 
   <td>Seleccione si desea identificar el archivo por ID de archivo o por la ruta de archivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Especifique un ID de archivo/ruta de archivo</td> 
   <td> <p>Seleccione cómo desea introducir el ID de archivo o la ruta de archivo:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Entrar manualmente]</b> </p> <p>Seleccione esta opción si desea introducir el ID o la ruta directamente, o asignarla desde un módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Seleccionar de una lista]</b> </p> <p>Seleccione esta opción si desea seleccionarla de una lista de archivos o rutas disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su [!DNL OneDrive] ubicación]</td> 
   <td> <p>Seleccione la ubicación que desee que contenga el archivo que desea descargar:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea que el módulo introduzca un ID de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Introduzca el ID de la unidad que contiene el archivo que desea descargar.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el sitio de SharePoint que contiene el archivo que desea descargar. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!UICONTROL Unidad del grupo]</b> </p> <p>Seleccione el grupo cuya unidad contiene el archivo que desea descargar.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de unidad]</td> 
   <td> <p>Seleccione o asigne la unidad que contiene el archivo que desea descargar. Este campo no está disponible si ha seleccionado [!UICONTROL No] en el campo [!UICONTROL Habilitar para introducir un ID de unidad].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td>
   <td> <p>Si ha seleccionado [!UICONTROL Entrar manualmente], introduzca o asigne el ID de archivo o la ruta del archivo que desea descargar.</p> <p>Si ha seleccionado [!UICONTROL Seleccionar de la lista], seleccione el archivo que desea descargar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Convertir en PDF]</td> 
   <td> <p>Active esta opción para convertir el archivo a un archivo PDF. Puede convertir desde los siguientes tipos de archivo:</p> 
    <table style="table-layout:auto"> 
     <col> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td> 
        <ul> 
         <li> <p> <p>CSV</p> </p> </li> 
         <li> <p> <p>DOC</p> </p> </li> 
         <li> <p> <p>DOCX</p> </p> </li> 
         <li> <p> <p>ODP</p> </p> </li> 
         <li> <p> <p>ODS</p> </p> </li> 
         <li> <p> <p>ODT</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p> <p>POT</p> </p> </li> 
         <li> <p> <p>POTM</p> </p> </li> 
         <li> <p> <p>POTX</p> </p> </li> 
         <li> <p> <p>PPS</p> </p> </li> 
         <li> <p> <p>PPSX</p> </p> </li> 
         <li> <p> <p>PPSXM</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p>PPT</p> </li> 
         <li> <p>PPTM</p> </li> 
         <li> <p>PPTX</p> </li> 
         <li> <p>RTF</p> </li> 
         <li> <p>XLS</p> </li> 
         <li> <p>XLSX</p> </li> 
        </ul> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cargar un archivo]

Este módulo de acción carga un archivo en la carpeta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obtener instrucciones sobre cómo conectar su [!DNL OneDrive] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Intro (ID y ruta de ubicación de carpeta)</td> 
   <td>Seleccione si desea identificar la carpeta de destino por ID o por una ruta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su [!DNL OneDrive] ubicación]</td> 
   <td> <p>Seleccione la ubicación en la que desea cargar un archivo:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea que el módulo introduzca un ID de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Seleccione la unidad que contiene el archivo que desea obtener.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el [!DNL SharePoint] Sitio que contiene la carpeta donde desea cargar un archivo. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!UICONTROL Unidad del grupo]</b> </p> <p>Seleccione el grupo cuya unidad contiene la carpeta donde desea cargar un archivo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de unidad]</td> 
   <td> <p>Seleccione la unidad que contiene la carpeta donde desea cargar un archivo. Este campo no está disponible si ha seleccionado [!UICONTROL No] en el campo [!UICONTROL Habilitar para introducir un ID de unidad].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Si existe el archivo con el mismo nombre]</td> 
   <td>Seleccione cómo continuar si ya existe un archivo con el mismo nombre.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descripción]</td> 
   <td>Añada una descripción al archivo cargado.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear una carpeta]

Este módulo de acción crea una nueva carpeta en la unidad especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obtener instrucciones sobre cómo conectar su [!DNL OneDrive] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su [!DNL OneDrive] ubicación]</td> 
   <td> <p>Seleccione la ubicación en la que desea crear una carpeta:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea que el módulo introduzca un ID de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Seleccione la unidad en la que desea crear una carpeta.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el [!DNL SharePoint] Sitio en el que desea crear una carpeta. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!UICONTROL Unidad del grupo]</b> </p> <p>Seleccione el grupo propietario del controlador en el que desea crear una carpeta.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de unidad]</td> 
   <td> <p>Seleccione la unidad en la que desea crear una carpeta. Este campo no está disponible si ha seleccionado [!UICONTROL No] en el campo [!UICONTROL Habilitar para introducir un ID de unidad].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Si desea que la nueva carpeta sea una subcarpeta, vaya a la carpeta en la que desea que sea una subcarpeta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuevo nombre de carpeta]</td> 
   <td> <p>Introduzca o asigne un nombre para la nueva carpeta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Si existe la carpeta con el mismo nombre]</td> 
   <td>Seleccione cómo continuar si ya existe un archivo con el mismo nombre.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un vínculo compartido]

Este módulo de acción devuelve un vínculo compartido para el archivo especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obtener instrucciones sobre cómo conectar su [!DNL OneDrive] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrar (ID de archivo y ruta de archivo)]</td> 
   <td>Seleccione si desea identificar el archivo por ID de archivo o por la ruta de archivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir un ID de archivo] / [!UICONTROL Ruta de archivo]</td> 
   <td> <p>Seleccione cómo desea introducir el ID de archivo o la ruta de archivo:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Entrar manualmente]</b> </p> <p>Seleccione esta opción si desea introducir el ID o la ruta directamente, o asignarla desde un módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Seleccionar de una lista]</b> </p> <p>Seleccione esta opción si desea seleccionarla de una lista de archivos o rutas disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su [!DNL OneDrive] ubicación]</td> 
   <td> <p>Seleccione la ubicación para la que desea recuperar un vínculo compartido:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea que el módulo introduzca un ID de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Introduzca el ID de la unidad que contiene el archivo para el que desea recuperar un vínculo compartido.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el sitio de SharePoint que contiene el archivo para el que desea recuperar un vínculo compartido. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!UICONTROL Unidad del grupo]</b> </p> <p>Seleccione el grupo cuya unidad contiene el archivo para el que desea recuperar un vínculo compartido.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de unidad]</td> 
   <td> <p>Seleccione o asigne la unidad que contiene el archivo para el que desea recuperar un vínculo compartido. Este campo no está disponible si ha seleccionado [!UICONTROL No] en el campo [!UICONTROL Habilitar para introducir un ID de unidad].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td> 
   <td> <p>Si ha seleccionado [!UICONTROL Entrar manualmente], introduzca o asigne el ID de archivo o la ruta del archivo para el que desea recuperar un vínculo compartido.</p> <p>Si ha seleccionado [!UICONTROL Seleccionar] en la lista, seleccione el archivo para el que desea recuperar un vínculo compartido.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de permiso]</td> 
   <td> <p>Seleccione si desea que las personas con el vínculo puedan leer y escribir en el archivo o leer solamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ámbito]</td> 
   <td>Seleccione si desea que el archivo esté disponible para cualquiera que tenga el vínculo o solo para los miembros de su organización que lo tengan.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover un archivo/carpeta]

Este módulo de acción mueve un archivo o carpeta a una nueva ubicación de carpeta

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obtener instrucciones sobre cómo conectar su [!DNL OneDrive] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrar (ID de archivo y ruta de archivo)]</td> 
   <td>Seleccione si desea identificar el archivo por ID de archivo o por la ruta de archivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir un ID de archivo/ruta de archivo]</td> 
   <td> <p>Seleccione cómo desea introducir el ID de archivo o la ruta de archivo:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Entrar manualmente]</b> </p> <p>Seleccione esta opción si desea introducir el ID o la ruta directamente, o asignarla desde un módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Seleccionar de una lista]</b> </p> <p>Seleccione esta opción si desea seleccionarla de una lista de archivos o rutas disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su [!DNL OneDrive] ubicación]</td> 
   <td> <p>Seleccione la ubicación que contiene el archivo o la carpeta que desea mover:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea que el módulo introduzca un ID de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Introduzca el ID de la unidad que contiene el archivo o la carpeta que desea mover.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el [!DNL SharePoint] Sitio que contiene el archivo o la carpeta que desea mover. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!UICONTROL Unidad del grupo]</b> </p> <p>Seleccione el grupo cuya unidad contiene el archivo o la carpeta que desea mover.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de unidad]</td> 
   <td> <p>Seleccione o asigne la unidad que contiene el archivo o carpeta que desea mover. Este campo no está disponible si ha seleccionado [!UICONTROL No] en el campo [!UICONTROL Habilitar para introducir un ID de unidad].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Seleccionar [!UICONTROL Archivo/Carpeta]</td> 
   <td>Seleccione si desea mover un archivo o una carpeta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</p> <p role="rowheader">[!UICONTROL Folder] / [!UICONTROL Folder ID] / [!UICONTROL Folder Path]</p> </td> 
   <td> <p>Si ha seleccionado [!UICONTROL Entrar manualmente], introduzca o asigne el ID o la ruta del archivo o carpeta que desea mover.</p> <p>Si ha seleccionado [!UICONTROL Seleccionar] en la lista, seleccione el archivo o la carpeta que desee mover.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir una nueva ubicación de carpeta]</td> 
   <td> <p>Seleccione cómo desea introducir la ubicación a la que desea mover el archivo o la carpeta:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Entrar manualmente]</b> </p> <p>Seleccione esta opción si desea introducir el ID o la ruta directamente, o asignarla desde un módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Seleccionar de una lista]</b> </p> <p>Seleccione esta opción si desea seleccionarla de una lista de archivos o rutas disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su [!DNL OneDrive] ubicación]</td> 
   <td> <p>Seleccione la ubicación a la que desea mover el archivo o la carpeta:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea que el módulo introduzca un ID de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Introduzca el ID de la unidad a la que desea mover el archivo o la carpeta.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el [!DNL SharePoint] Sitio al que desea mover el archivo o la carpeta. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!UICONTROL Unidad del grupo]</b> </p> <p>Seleccione el grupo a cuya unidad desea mover el archivo o la carpeta.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de unidad]</td> 
   <td> <p>Seleccione o asigne la unidad que contiene la carpeta a la que desea mover el archivo o la carpeta. Este campo no está disponible si ha seleccionado [!UICONTROL No] en el campo [!UICONTROL Habilitar para introducir un ID de unidad].</p> <p>Si deja esto en blanco, el archivo o la carpeta solo se pueden mover dentro del mismo [!DNL OneDrive].</p> <p>Puede mover archivos y carpetas de [!UICONTROL My Drive] a una [!UICONTROL Site's Drive] o a una unidad de [!UICONTROL Group]. </p> <p>Puede mover archivos de una unidad de [!UICONTROL Site's Drive] solo a la misma unidad en el mismo sitio.</p> <p>Puede mover archivos de una unidad de [!UICONTROL Group] solo a la misma unidad del mismo grupo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Introduzca o asigne la carpeta a la que desea mover el archivo o la carpeta.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar un archivo]

Este módulo de acción copia un archivo en una nueva ubicación de carpeta

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obtener instrucciones sobre cómo conectar su [!DNL OneDrive] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrar (ID de archivo y ruta de archivo)]</td> 
   <td>Seleccione si desea identificar el archivo por ID de archivo o por la ruta de archivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir un ID de archivo] / [!UICONTROL Ruta de archivo]</td> 
   <td> <p>Seleccione cómo desea introducir el ID de archivo o la ruta de archivo:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Entrar manualmente]</b> </p> <p>Seleccione esta opción si desea introducir el ID o la ruta directamente, o asignarla desde un módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Seleccionar de una lista]</b> </p> <p>Seleccione esta opción si desea seleccionarla de una lista de archivos o rutas disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su [!DNL OneDrive] ubicación]</td> 
   <td> <p>Seleccione la ubicación que contiene el archivo que desea copiar:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea que el módulo introduzca un ID de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Introduzca el ID de la unidad que contiene el archivo o la carpeta que desea copiar.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el sitio de SharePoint que contiene el archivo que desea mover. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!UICONTROL Unidad del grupo]</b> </p> <p>Seleccione el grupo cuya unidad contiene el archivo que desea copiar.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de unidad]</td> 
   <td> <p>Seleccione o asigne la unidad que contiene el archivo que desea copiar. Este campo no está disponible si ha seleccionado [!UICONTROL No] en el campo [!UICONTROL Habilitar para introducir un ID de unidad].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</p> </td> 
   <td> <p>Si ha seleccionado [!UICONTROL Entrar manualmente], introduzca o asigne el ID o la ruta del archivo que desea copiar.</p> <p>Si ha seleccionado [!UICONTROL Seleccionar] en la lista, seleccione el archivo que desea copiar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introducir una nueva ubicación de carpeta]</td> 
   <td> <p>Seleccione cómo desea introducir la ubicación en la que desea copiar el archivo o:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Entrar manualmente]</b> </p> <p>Seleccione esta opción si desea introducir el ID o la ruta directamente, o asignarla desde un módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Seleccionar de una lista]</b> </p> <p>Seleccione esta opción si desea seleccionarla en una lista de carpetas disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nueva ubicación de OneDrive]</td> 
   <td> <p>Seleccione la ubicación donde desea copiar el filtro. Esta opción está disponible si elige seleccionar la nueva ubicación de carpeta de una lista.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea que el módulo introduzca un ID de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Introduzca el ID de la unidad en la que desea copiar el archivo.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el [!DNL SharePoint] Sitio en el que desea copiar el archivo. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!UICONTROL Unidad del grupo]</b> </p> <p>Seleccione el grupo en cuya unidad desee copiar el archivo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de unidad]</td> 
   <td> <p>Seleccione o asigne la unidad que contiene la carpeta en la que desea copiar el archivo. Este campo no está disponible si ha seleccionado [!UICONTROL No] en el campo [!UICONTROL Habilitar para introducir un ID de unidad].</p> <p>Si deja esto en blanco, el archivo o la carpeta solo se pueden copiar dentro de la misma [!UICONTROL OneDrive].</p> <p>Puede copiar archivos y carpetas de [!UICONTROL My Drive] a una [!UICONTROL Site's Drive] o a una unidad de [!UICONTROL Group]. </p> <p>Puede copiar archivos de una unidad de [!UICONTROL Site's Drive] solo en la misma unidad del mismo sitio.</p> <p>Puede copiar archivos de una unidad de [!UICONTROL Group] solo en la misma unidad del mismo grupo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Introduzca o asigne la carpeta a la que desea mover la copia o carpeta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuevo nombre de archivo copiado]</td> 
   <td> <p>Introduzca o asigne un nombre para la nueva copia del archivo. Puede dejarlo en blanco si no desea cambiar el nombre del archivo original.</p> <p>El nombre debe incluir la extensión de archivo. Ejemplo:<code> file.txt</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un archivo/carpeta]

Este módulo de acción elimina el archivo seleccionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obtener instrucciones sobre cómo conectar su [!DNL OneDrive] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrar (ID de archivo/carpeta y ruta)]</td> 
   <td>Seleccione si desea identificar el archivo por ID de archivo o por la ruta de archivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Introduzca un ID de archivo/carpeta /Introduzca una ruta de archivo/carpeta]</td> 
   <td> <p>Seleccione cómo desea introducir el ID de archivo o la ruta de archivo:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Entrar manualmente]</b> </p> <p>Seleccione esta opción si desea introducir el ID o la ruta directamente, o asignarla desde un módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Seleccionar de una lista]</b> </p> <p>Seleccione esta opción si desea seleccionarla de una lista de archivos o rutas disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su [!DNL OneDrive] ubicación]</td> 
   <td> <p>Seleccione la ubicación que desee buscar:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea que el módulo introduzca un ID de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Introduzca el ID de la unidad que contiene el archivo o la carpeta que desea eliminar.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el [!DNL SharePoint] Sitio que contiene el archivo o la carpeta que desea eliminar. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!UICONTROL Unidad del grupo]</b> </p> <p>Seleccione el grupo cuya unidad contenga el archivo o la carpeta que desee eliminar.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de unidad]</td> 
   <td> <p>Seleccione o asigne la unidad que contiene el archivo o la carpeta que desea eliminar. Este campo no está disponible si ha seleccionado [!UICONTROL No] en el campo [!UICONTROL Habilitar para introducir un ID de unidad].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Seleccionar [!UICONTROL Archivo/Carpeta]</td> 
   <td>Seleccione si desea eliminar un archivo o una carpeta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td>
   <td> <p>Si ha seleccionado [!UICONTROL Entrar manualmente], introduzca o asigne el ID de archivo o la ruta del archivo que desea eliminar.</p> <p>Si ha seleccionado [!UICONTROL Seleccionar] en la lista, seleccione el archivo que desea eliminar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Otro

#### [!UICONTROL Realizar una llamada de API]

Este módulo realiza una llamada API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obtener instrucciones sobre cómo conectar su [!DNL OneDrive] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Especifique una ruta relativa a <code>https://graph.microsoft.com</code>. Ejemplo:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   td&gt; <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada a la API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Al utilizar afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>



## Si no puede cargar o actualizar un archivo

Existen varios problemas posibles al cargar o actualizar un archivo con errores:

* El archivo cargado es demasiado grande y supera el límite de tamaño máximo de archivo para [!DNL OneDrive] o ha usado todo su [!DNL OneDrive] cuota de almacenamiento de la cuenta. Para obtener más espacio de almacenamiento, elimine los archivos existentes de [!DNL OneDrive] o actualice su [!DNL OneDrive] cuenta.
* OneDrive no permite cargar dos archivos con el mismo nombre en una sola carpeta. Si la carpeta de destino contiene un archivo con el mismo nombre que el archivo que se está cargando, la ejecución del escenario termina con un error. La solución es simplemente cambiar el nombre del archivo que se está cargando. Si su objetivo es actualizar un archivo, use la función [!UICONTROL Actualizar un archivo] acción.
* La carpeta seleccionada anteriormente, a la que se está cargando el archivo, ya no existe. El escenario se detiene y tendrá que seleccionar de nuevo la carpeta de destino.
