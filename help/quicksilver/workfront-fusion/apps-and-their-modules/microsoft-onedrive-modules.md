---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Microsoft OneDrive
description: En un escenario de  [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan OneDrive, así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 13a25c6c-bdf1-467d-bd90-ebd763c59235
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '4073'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive] módulos

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!DNL OneDrive], así como conectarlo a varias aplicaciones y servicios de terceros.

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
   <td role="rowheader">Product</td> 
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

Para usar módulos de [!DNL OneDrive], debe tener una cuenta de [!DNL Microsoft OneDrive].




## Conectando el servicio [!DNL OneDrive] a [!DNL Workfront Fusion]

Para obtener instrucciones sobre cómo conectar tu cuenta de [!DNL OneDrive] a [!UICONTROL Workfront Fusion], consulta [Crear una conexión a [!UICONTROL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Algunas aplicaciones de Microsoft utilizan la misma conexión, que está vinculada a permisos de usuario individuales. Por lo tanto, al crear una conexión, la pantalla de consentimiento de permisos muestra todos los permisos que se hayan concedido anteriormente a la conexión de este usuario, además de los nuevos permisos necesarios para la aplicación actual.
>
>Por ejemplo, si un usuario tiene permisos de &quot;Leer tabla&quot; concedidos a través del conector de Excel y, a continuación, crea una conexión en el conector de Outlook para leer correos electrónicos, la pantalla de consentimiento de permisos mostrará tanto el permiso de &quot;Leer tabla&quot; ya concedido como el permiso de &quot;Escribir correo electrónico&quot; recién requerido.

## [!DNL Microsoft OneDrive] módulos y sus campos

Al configurar [!DNL OneDrive] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL OneDrive] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Archivo/Carpeta](#filefolder)
* [Otro](#other)

### Archivo/Carpeta

* [[!UICONTROL Archivos/carpetas de inspección]](#watch-filesfolders)
* [[!UICONTROL Archivos/carpetas de búsqueda]](#search-filesfolders)
* [[!UICONTROL Obtener un archivo]](#get-a-file)
* [[!UICONTROL Descargar un archivo]](#download-a-file)
* [[!UICONTROL Cargar un archivo]](#upload-a-file)
* [[!UICONTROL Crear una carpeta]](#create-a-folder)
* [[!UICONTROL Obtener un vínculo compartido]](#get-a-share-link)
* [[!UICONTROL Mover un archivo/carpeta]](#move-a-filefolder)
* [[!UICONTROL Copiar un archivo]](#copy-a-file)
* [[!UICONTROL Eliminar un archivo o carpeta]](#delete-a-filefolder)

#### [!UICONTROL Archivos/carpetas de inspección]

Este módulo de déclencheur inicia un escenario cuando se crea o actualiza un archivo o carpeta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL OneDrive] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Observar archivos/carpetas]</td> 
   <td> <p>Seleccione cómo desea inspeccionar archivos o carpetas:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Por Hora De Creación]</b> </p> <p>Busque nuevos archivos o carpetas.</p> </li> 
     <li> <p><b>[!UICONTROL Por Hora De Actualización]</b> </p> <p>Busque archivos o carpetas existentes actualizados.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su ubicación [!DNL OneDrive]]</td> 
   <td> <p>Seleccione la ubicación que desee ver:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea permitir que el módulo introduzca un identificador de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Escriba el identificador de la unidad que desea que vea el módulo.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> <p>Desplácese hasta la carpeta que desee que vea el módulo. También puede introducir una consulta para filtrar los resultados devueltos.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Compartido Conmigo]</b> </p> <p>El módulo inspecciona los archivos que se han compartido con el propietario de la unidad.</p> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el sitio de SharePoint que desea que vea el módulo. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!Unidad del grupo UICONTROL]</b> </p> <p>Seleccione el grupo cuya unidad desea que vea el módulo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir un tipo de elemento]</td> 
   <td> <p>Seleccione si desea inspeccionar archivos, carpetas o ambos.</p> <p>Nota: No puede inspeccionar carpetas en una unidad de [!UICONTROL compartida conmigo].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>



#### [!UICONTROL Archivos/carpetas de búsqueda]

Este módulo de búsqueda devuelve archivos y carpetas en función de los criterios definidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL OneDrive] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su ubicación [!DNL OneDrive]]</td> 
   <td> <p>Seleccione la ubicación en la que desea buscar:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea permitir que el módulo introduzca un identificador de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Escriba el identificador de la unidad que desea que busque el módulo.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> <p>Desplácese hasta la carpeta en la que desee buscar el módulo. También puede introducir una consulta para filtrar los resultados devueltos.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Compartido Conmigo]</b> </p> <p>El módulo busca los archivos que se han compartido con el propietario de la unidad.</p> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el sitio [!DNL SharePoint] en el que desea que busque el módulo. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!Unidad del grupo UICONTROL]</b> </p> <p>Seleccione el grupo cuya unidad desea que busque el módulo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir un tipo de elemento]</td> 
   <td> <p>Seleccione si desea buscar archivos, carpetas o ambos.</p> <p>Nota: No puede buscar carpetas en una unidad de [!UICONTROL Compartida conmigo].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL OneDrive] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrar (ID de archivo y ruta de archivo)]</td> 
   <td>Seleccione si desea identificar el archivo por ID de archivo o por ruta de archivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escriba un Id. de archivo] / [!UICONTROL Ruta de archivo]</td> 
   <td> <p>Seleccione cómo desea introducir el ID de archivo o la ruta de archivo:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Escribir manualmente]</b> </p> <p>Seleccione esta opción si desea introducir el ID o la ruta directamente o asignarlos desde un módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Seleccionar de una lista]</b> </p> <p>Seleccione esta opción si desea seleccionar de una lista de archivos o rutas disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su ubicación [!DNL OneDrive]]</td> 
   <td> <p>Seleccione la ubicación en la que desea buscar:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea permitir que el módulo introduzca un identificador de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Escriba el identificador de la unidad que contiene el archivo que desea obtener.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el sitio de SharePoint que contiene el archivo que desea obtener. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!Unidad del grupo UICONTROL]</b> </p> <p>Seleccione el grupo cuya unidad contiene el archivo que desea obtener.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de unidad]</td> 
   <td> <p>Seleccione o asigne la unidad que contiene el archivo que desea obtener. Este campo no está disponible si seleccionó [!UICONTROL No] en el campo [!UICONTROL Habilitar para escribir un Id. de unidad].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo] / [!UICONTROL Id. de archivo] / [!UICONTROL Ruta de archivo]</td> 
   <td> <p>Si seleccionó [!UICONTROL Escribir manualmente], escriba o asigne el Id. o la ruta de acceso del archivo que desea obtener.</p> <p>Si seleccionó [!UICONTROL Seleccionar de la lista], seleccione el archivo que desea obtener.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL OneDrive] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrar (ID de archivo y ruta de archivo)]</td> 
   <td>Seleccione si desea identificar el archivo por ID de archivo o por ruta de archivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Introduzca un ID de archivo/ruta de archivo</td> 
   <td> <p>Seleccione cómo desea introducir el ID de archivo o la ruta de archivo:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Escribir manualmente]</b> </p> <p>Seleccione esta opción si desea introducir el ID o la ruta directamente o asignarlos desde un módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Seleccionar de una lista]</b> </p> <p>Seleccione esta opción si desea seleccionar de una lista de archivos o rutas disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su ubicación [!DNL OneDrive]]</td> 
   <td> <p>Seleccione la ubicación que desee que contenga el archivo que desea descargar:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea permitir que el módulo introduzca un identificador de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Escriba el identificador de la unidad que contiene el archivo que desea descargar.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el sitio de SharePoint que contiene el archivo que desea descargar. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!Unidad del grupo UICONTROL]</b> </p> <p>Seleccione el grupo cuya unidad contiene el archivo que desea descargar.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de unidad]</td> 
   <td> <p>Seleccione o asigne la unidad que contiene el archivo que desea descargar. Este campo no está disponible si seleccionó [!UICONTROL No] en el campo [!UICONTROL Habilitar para escribir un Id. de unidad].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo] / [!UICONTROL Id. de archivo] / [!UICONTROL Ruta de archivo]</td>
   <td> <p>Si seleccionó [!UICONTROL Escribir manualmente], escriba o asigne el Id. o la ruta de acceso del archivo que desea descargar.</p> <p>Si seleccionó [!UICONTROL Seleccionar de la lista], seleccione el archivo que desea descargar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Convertir en PDF]</td> 
   <td> <p>Active esta opción para convertir el archivo en un archivo de PDF. Puede convertir desde los siguientes tipos de archivo:</p> 
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
         <li> <p> <p>PUNTO</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p> <p>MACETA</p> </p> </li> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL OneDrive] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Introducir (ID y ruta de ubicación de la carpeta)</td> 
   <td>Seleccione si desea identificar la carpeta de destino por ID o por ruta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su ubicación [!DNL OneDrive]]</td> 
   <td> <p>Seleccione la ubicación donde desea cargar un archivo:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea permitir que el módulo introduzca un identificador de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Seleccione la unidad que contiene el archivo que desea obtener.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el sitio [!DNL SharePoint] que contiene la carpeta donde desea cargar un archivo. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!Unidad del grupo UICONTROL]</b> </p> <p>Seleccione el grupo cuya unidad contiene la carpeta donde desea cargar un archivo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de unidad]</td> 
   <td> <p>Seleccione la unidad que contiene la carpeta donde desea cargar un archivo. Este campo no está disponible si seleccionó [!UICONTROL No] en el campo [!UICONTROL Habilitar para escribir un Id. de unidad].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL archivo Source]</td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL OneDrive] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su ubicación [!DNL OneDrive]]</td> 
   <td> <p>Seleccione la ubicación donde desea crear una carpeta:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea permitir que el módulo introduzca un identificador de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Seleccione la unidad donde desea crear una carpeta.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el sitio [!DNL SharePoint] en el que desea crear una carpeta. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!Unidad del grupo UICONTROL]</b> </p> <p>Seleccione el grupo propietario de la unidad donde desea crear una carpeta.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de unidad]</td> 
   <td> <p>Seleccione la unidad en la que desea crear una carpeta. Este campo no está disponible si seleccionó [!UICONTROL No] en el campo [!UICONTROL Habilitar para escribir un Id. de unidad].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carpeta]</td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL OneDrive] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrar (ID de archivo y ruta de archivo)]</td> 
   <td>Seleccione si desea identificar el archivo por ID de archivo o por ruta de archivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escriba un Id. de archivo] / [!UICONTROL Ruta de archivo]</td> 
   <td> <p>Seleccione cómo desea introducir el ID de archivo o la ruta de archivo:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Escribir manualmente]</b> </p> <p>Seleccione esta opción si desea introducir el ID o la ruta directamente o asignarlos desde un módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Seleccionar de una lista]</b> </p> <p>Seleccione esta opción si desea seleccionar de una lista de archivos o rutas disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su ubicación [!DNL OneDrive]]</td> 
   <td> <p>Seleccione la ubicación para la que desea recuperar un vínculo compartido:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea permitir que el módulo introduzca un identificador de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Escriba el identificador de la unidad que contiene el archivo para el que desea recuperar un vínculo compartido.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el sitio de SharePoint que contiene el archivo para el que desea recuperar un vínculo compartido. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!Unidad del grupo UICONTROL]</b> </p> <p>Seleccione el grupo cuya unidad contiene el archivo para el que desea recuperar un vínculo compartido.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de unidad]</td> 
   <td> <p>Seleccione o asigne la unidad que contiene el archivo para el que desea recuperar un vínculo compartido. Este campo no está disponible si seleccionó [!UICONTROL No] en el campo [!UICONTROL Habilitar para escribir un Id. de unidad].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo] / [!UICONTROL Id. de archivo] / [!UICONTROL Ruta de archivo]</td> 
   <td> <p>Si seleccionó [!UICONTROL Escribir manualmente], escriba o asigne el Id. de archivo o la ruta de acceso del archivo para el que desea recuperar un vínculo compartido.</p> <p>Si seleccionó [!UICONTROL Seleccionar] de la lista, seleccione el archivo para el que desea recuperar un vínculo compartido.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de permiso]</td> 
   <td> <p>Seleccione si desea que las personas con el vínculo puedan leer y escribir en el archivo o sólo leer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ámbito]</td> 
   <td>Seleccione si desea que el archivo esté disponible para cualquier persona que tenga el vínculo o solo para los miembros de su organización que lo tengan.</td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL OneDrive] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrar (ID de archivo y ruta de archivo)]</td> 
   <td>Seleccione si desea identificar el archivo por ID de archivo o por ruta de archivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escriba un Id. de archivo / Ruta de archivo]</td> 
   <td> <p>Seleccione cómo desea introducir el ID de archivo o la ruta de archivo:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Escribir manualmente]</b> </p> <p>Seleccione esta opción si desea introducir el ID o la ruta directamente o asignarlos desde un módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Seleccionar de una lista]</b> </p> <p>Seleccione esta opción si desea seleccionar de una lista de archivos o rutas disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su ubicación [!DNL OneDrive]]</td> 
   <td> <p>Seleccione la ubicación que contiene el archivo o la carpeta que desea mover:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea permitir que el módulo introduzca un identificador de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Escriba el identificador de la unidad que contiene el archivo o la carpeta que desea mover.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el sitio [!DNL SharePoint] que contiene el archivo o la carpeta que desea mover. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!Unidad del grupo UICONTROL]</b> </p> <p>Seleccione el grupo cuya unidad contiene el archivo o la carpeta que desea mover.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de unidad]</td> 
   <td> <p>Seleccione o asigne la unidad que contiene el archivo o la carpeta que desea mover. Este campo no está disponible si seleccionó [!UICONTROL No] en el campo [!UICONTROL Habilitar para escribir un Id. de unidad].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Seleccionar [!UICONTROL Archivo/Carpeta]</td> 
   <td>Seleccione si desea mover un archivo o una carpeta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL Archivo] / [!UICONTROL Id. de archivo] / [!UICONTROL Ruta de archivo]</p> <p role="rowheader">[!UICONTROL Carpeta] / [!UICONTROL Id. de carpeta] / [!UICONTROL Ruta de carpeta]</p> </td> 
   <td> <p>Si seleccionó [!UICONTROL Escribir manualmente], escriba o asigne el Id. o la ruta de acceso del archivo o carpeta que desea mover.</p> <p>Si seleccionó [!UICONTROL Seleccionar] de la lista, seleccione el archivo o la carpeta que desee mover.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escriba una nueva ubicación de carpeta]</td> 
   <td> <p>Seleccione cómo desea introducir la ubicación a la que desea mover el archivo o la carpeta:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Escribir manualmente]</b> </p> <p>Seleccione esta opción si desea introducir el ID o la ruta directamente o asignarlos desde un módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Seleccionar de una lista]</b> </p> <p>Seleccione esta opción si desea seleccionar de una lista de archivos o rutas disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su ubicación [!DNL OneDrive]]</td> 
   <td> <p>Seleccione la ubicación a la que desea mover el archivo o la carpeta:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea permitir que el módulo introduzca un identificador de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Escriba el identificador de la unidad donde desea mover el archivo o la carpeta.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el sitio [!DNL SharePoint] al que desee mover el archivo o la carpeta. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!Unidad del grupo UICONTROL]</b> </p> <p>Seleccione el grupo al que desea mover el archivo o la carpeta.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de unidad]</td> 
   <td> <p>Seleccione o asigne la unidad que contiene la carpeta a la que desea mover el archivo o carpeta. Este campo no está disponible si seleccionó [!UICONTROL No] en el campo [!UICONTROL Habilitar para escribir un Id. de unidad].</p> <p>Si deja esto en blanco, el archivo o la carpeta solamente se podrá mover dentro del mismo [!DNL OneDrive].</p> <p>Puede mover archivos y carpetas de [!UICONTROL Mi unidad] a una unidad de sitio de [!UICONTROL] o a una unidad de grupo de [!UICONTROL]. </p> <p>Solo puede mover archivos de una unidad de [!UICONTROL Site] a la misma unidad del mismo sitio.</p> <p>Solo puede mover archivos de una unidad de [!UICONTROL Group] a la misma unidad del mismo grupo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carpeta]</td> 
   <td>Escriba o asigne la carpeta donde desea mover el archivo o la carpeta.</td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL OneDrive] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrar (ID de archivo y ruta de archivo)]</td> 
   <td>Seleccione si desea identificar el archivo por ID de archivo o por ruta de archivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escriba un Id. de archivo] / [!UICONTROL Ruta de archivo]</td> 
   <td> <p>Seleccione cómo desea introducir el ID de archivo o la ruta de archivo:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Escribir manualmente]</b> </p> <p>Seleccione esta opción si desea introducir el ID o la ruta directamente o asignarlos desde un módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Seleccionar de una lista]</b> </p> <p>Seleccione esta opción si desea seleccionar de una lista de archivos o rutas disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su ubicación [!DNL OneDrive]]</td> 
   <td> <p>Seleccione la ubicación que contiene el archivo que desea copiar:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea permitir que el módulo introduzca un identificador de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Escriba el identificador de la unidad que contiene el archivo o la carpeta que desea copiar.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el sitio de SharePoint que contiene el archivo que desea mover. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!Unidad del grupo UICONTROL]</b> </p> <p>Seleccione el grupo cuya unidad contiene el archivo que desea copiar.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de unidad]</td> 
   <td> <p>Seleccione o asigne la unidad que contiene el archivo que desea copiar. Este campo no está disponible si seleccionó [!UICONTROL No] en el campo [!UICONTROL Habilitar para escribir un Id. de unidad].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL Archivo] / [!UICONTROL Id. de archivo] / [!UICONTROL Ruta de archivo]</p> </td> 
   <td> <p>Si seleccionó [!UICONTROL Escribir manualmente], escriba o asigne el Id. o la ruta de acceso del archivo que desea copiar.</p> <p>Si seleccionó [!UICONTROL Seleccionar] de la lista, seleccione el archivo que desea copiar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escriba una nueva ubicación de carpeta]</td> 
   <td> <p>Seleccione cómo desea introducir la ubicación en la que desea copiar el archivo o:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Escribir manualmente]</b> </p> <p>Seleccione esta opción si desea introducir el ID o la ruta directamente o asignarlos desde un módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Seleccionar de una lista]</b> </p> <p>Seleccione esta opción si desea seleccionar de una lista de carpetas disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nueva ubicación de OneDrive]</td> 
   <td> <p>Seleccione la ubicación donde desea copiar el filtro. Esta opción está disponible si elige seleccionar la nueva ubicación de la carpeta en una lista.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea permitir que el módulo introduzca un identificador de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Escriba el identificador de la unidad donde desea copiar el archivo.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el sitio [!DNL SharePoint] en el que desea copiar el archivo. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!Unidad del grupo UICONTROL]</b> </p> <p>Seleccione el grupo en cuya unidad desee copiar el archivo.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de unidad]</td> 
   <td> <p>Seleccione o asigne la unidad que contiene la carpeta en la que desea copiar el archivo. Este campo no está disponible si seleccionó [!UICONTROL No] en el campo [!UICONTROL Habilitar para escribir un Id. de unidad].</p> <p>Si deja esto en blanco, el archivo o la carpeta sólo se podrán copiar dentro de la misma [!UICONTROL OneDrive].</p> <p>Puede copiar archivos y carpetas de [!UICONTROL Mi unidad] a una unidad de sitio de [!UICONTROL] o a una unidad de grupo de [!UICONTROL]. </p> <p>Solo puede copiar archivos de una unidad de [!UICONTROL Site] en la misma unidad del mismo sitio.</p> <p>Puede copiar archivos de una unidad de [!UICONTROL Group] sólo en la misma unidad del mismo grupo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Carpeta]</td> 
   <td>Introduzca o asigne la carpeta a la que desea mover la copia o carpeta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nuevo nombre de archivo copiado]</td> 
   <td> <p>Introduzca o asigne un nombre para la nueva copia del archivo. Puede dejarlo en blanco si no desea cambiar el nombre del archivo original.</p> <p>El nombre debe incluir la extensión de archivo. Ejemplo:<code> file.txt</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un archivo o carpeta]

Este módulo de acción elimina el archivo seleccionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL OneDrive] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entrar (Archivo/Id. de carpeta y ruta)]</td> 
   <td>Seleccione si desea identificar el archivo por ID de archivo o por ruta de archivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Escriba un Id. de archivo/carpeta /Escriba una ruta de archivo/carpeta]</td> 
   <td> <p>Seleccione cómo desea introducir el ID de archivo o la ruta de archivo:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Escribir manualmente]</b> </p> <p>Seleccione esta opción si desea introducir el ID o la ruta directamente o asignarlos desde un módulo anterior.</p> </li> 
     <li> <p><b>[!UICONTROL Seleccionar de una lista]</b> </p> <p>Seleccione esta opción si desea seleccionar de una lista de archivos o rutas disponibles. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija su ubicación [!DNL OneDrive]]</td> 
   <td> <p>Seleccione la ubicación en la que desea buscar:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Mi unidad]</b> </p> <p>Seleccione si desea permitir que el módulo introduzca un identificador de unidad.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Sí]</b> </p> <p>Escriba el identificador de la unidad que contiene el archivo o la carpeta que desea eliminar.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Unidad del sitio]</b> </p> <p>Seleccione el sitio [!DNL SharePoint] que contiene el archivo o la carpeta que desea eliminar. Los sitios disponibles son sitios seguidos por el usuario que ha iniciado sesión.</p> </li> 
     <li> <p><b>[!Unidad del grupo UICONTROL]</b> </p> <p>Seleccione el grupo cuya unidad contiene el archivo o la carpeta que desea eliminar.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de unidad]</td> 
   <td> <p>Seleccione o asigne la unidad que contiene el archivo o la carpeta que desea eliminar. Este campo no está disponible si seleccionó [!UICONTROL No] en el campo [!UICONTROL Habilitar para escribir un Id. de unidad].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Seleccionar [!UICONTROL Archivo/Carpeta]</td> 
   <td>Seleccione si desea eliminar un archivo o una carpeta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo] / [!UICONTROL Id. de archivo] / [!UICONTROL Ruta de archivo]</td>
   <td> <p>Si seleccionó [!UICONTROL Escribir manualmente], escriba o asigne el Id. o la ruta de acceso del archivo que desea eliminar.</p> <p>Si seleccionó [!UICONTROL Seleccionar] de la lista, seleccione el archivo que desea eliminar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Otro

#### [!UICONTROL Realizar una llamada API]

Este módulo realiza una llamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL OneDrive] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></td> 
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
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando utilice afirmaciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>



## Si no puede cargar o actualizar un archivo

Existen varios problemas posibles cuando falla la carga o actualización de un archivo:

* El archivo cargado es demasiado grande y supera el límite máximo de tamaño de archivo para el plan [!DNL OneDrive] o ha utilizado toda la cuota de almacenamiento de la cuenta [!DNL OneDrive]. Para obtener más espacio de almacenamiento, elimine los archivos existentes de [!DNL OneDrive] o actualice la cuenta de [!DNL OneDrive].
* OneDrive no permite cargar dos archivos con el mismo nombre en una sola carpeta. Si la carpeta de destino contiene un archivo con el mismo nombre que el archivo que se está cargando, la ejecución del escenario finaliza con un error. La solución consiste simplemente en cambiar el nombre del archivo que se está cargando. Si su objetivo es actualizar un archivo, use la acción [!UICONTROL Actualizar un archivo].
* La carpeta seleccionada anteriormente, en la que se está cargando el archivo, ya no existe. El escenario se detiene y tendrá que volver a seleccionar la carpeta de destino.
