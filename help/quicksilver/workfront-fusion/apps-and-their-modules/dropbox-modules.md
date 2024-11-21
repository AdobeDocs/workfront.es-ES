---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Dropbox
description: En un  [!DNL Adobe Workfront Fusion] escenario, puede automatizar los flujos de trabajo que utilizan Dropbox, así como conectarlo a varias aplicaciones y servicios de terceros. Esto le permite automatizar actividades como la supervisión, la búsqueda, la recuperación, la inclusión, la creación y la edición de archivos y carpetas en el Dropbox.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: a35631d7-40ac-4e7f-9a37-ad3879c0b6a2
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '3230'
ht-degree: 0%

---

# [!DNL Dropbox] módulos

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que usan [!UICONTROL Dropbox] o [!DNL Dropbox Business], así como conectarlo a varias aplicaciones y servicios de terceros. Esto le permite automatizar actividades como supervisar, buscar, recuperar, enumerar, crear y editar archivos y carpetas en su [!UICONTROL Dropbox].

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

* Para usar módulos de [!DNL Dropbox], debe tener una cuenta de [!DNL Dropbox].

>[!IMPORTANT]
>
>El Dropbox debe aprobar las aplicaciones con más de 50 usuarios.
>
>Para obtener más información, busque &quot;Aprobación de producción&quot; en la guía para desarrolladores de Dropbox.

## Información de API del Dropbox

El conector del Dropbox utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL básica</td> 
   <td> https://api.dropboxapi.com/2    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Versión de API</td> 
   <td> 2 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td><ul><li><p>Dropbox</p><p>Versión 5.3.9</p></li><li><p>Dropbox Empresa</p><p>Versión 1.0.12</p></li></ul></td> 
  </tr>
 </tbody> 
 </table>


## Crear una conexión con [!DNL Dropbox]

Para crear una conexión para los módulos de [!DNL Dropbox]:

1. Haga clic en **[!UICONTROL Agregar]** junto al cuadro Conexión.

1. Rellene los campos siguientes:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[!UICONTROL Nombre de conexión]</td>
        <td>
          <p>Escriba un nombre para esta conexión.</p>
        </td>
        <tr>
        <td role="rowheader">[!UICONTROL Entorno]</td>
        <td>Seleccione si esta conexión es para un entorno de producción o de no producción.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Tipo]</td>
        <td>Seleccione si desea conectarse a una cuenta de servicio o a una cuenta personal.</td>
        </tr>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL ID de cliente]</td>
        <td>Introduzca el [!UICONTROL Dropbox] [!UICONTROL ID de cliente] de [!UICONTROL]. </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Secreto de cliente]</td>
        <td>Escriba su [!UICONTROL Secreto de cliente] [!DNL Dropbox]. </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Tipo de cuenta]</td>
        <td>Seleccione si desea conectarse a una cuenta de Dropbox personal o a una cuenta de empresa (Dropbox Business).</td>
        </tr>
      </tbody>
    </table>

1. Haga clic en **[!UICONTROL Continuar]** para guardar la conexión y volver al módulo.## [!DNL Dropbox] módulos y sus campos

## [!DNL Dropbox] módulos y sus campos

Al configurar [!DNL Dropbox] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Dropbox] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Módulos de activador](#trigger-modules)
* [Módulos para obtener  [!DNL Dropbox] archivos y carpetas](#modules-for-getting-dropbox-files-and-folders)
* [Módulos para crear y editar  [!DNL Dropbox] archivos y carpetas](#modules-for-creating-and-editing-dropbox-files-and-folders)
* [Otros módulos](#other-modules)

### Módulos de activador

#### [!UICONTROL Observar archivos]

Este módulo de tipo de Déclencheur devuelve los detalles del archivo cuando se modifica el archivo de una carpeta especificada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Dropbox] a [!DNL Workfront Fusion], vea <a href="#create-a-connection-to-dropbox" class="MCXref xref">Crear una conexión con [!DNL Dropbox]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione la carpeta en la que desee inspeccionar los cambios.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ver también subcarpetas]</td> 
   <td> <p> Habilite esta opción para supervisar también las subcarpetas de la carpeta seleccionada en busca de archivos modificados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Límite] </td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Módulos para obtener [!DNL Dropbox] archivos y carpetas

* [[!UICONTROL Archivos/carpetas de búsqueda]](#search-filesfolders)
* [[!UICONTROL Descargar un archivo]](#download-a-file)
* [[!UICONTROL Obtener metadatos de carpeta]](#get-a-folder-metadata)
* [[!UICONTROL Enumerar todos los archivos/subcarpetas de una carpeta]](#list-all-filessubfolders-in-a-folder)
* [[!UICONTROL Revisiones de archivos de lista]](#list-file-revisions)

#### [!UICONTROL Archivos/carpetas de búsqueda]

Este módulo de búsqueda busca registros en un objeto de [!DNL Dropbox] que coincidan con la consulta de búsqueda especificada.

Puede asignar esta información en módulos subsiguientes en el escenario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Dropbox] a [!DNL Workfront Fusion], vea <a href="#create-a-connection-to-dropbox" class="MCXref xref">Crear una conexión con [!DNL Dropbox]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Buscar] </td> 
   <td> <p>Introduzca el término de búsqueda.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione la carpeta en la que desea buscar. Este módulo busca en todo el [!DNL Dropbox] si no selecciona ninguna carpeta.</p> </td> 
  </tr> 
  <tr> 
   <td>Estado del archivo</td> 
   <td> <p> Seleccione el estado del archivo para restringir la búsqueda al estado del archivo seleccionado.</p> </td> 
  </tr> 
  <tr> 
   <td>Categorías de archivo</td> 
   <td> <p> Seleccione las categorías de archivo para restringir la búsqueda a las categorías seleccionadas.</p> </td> 
  </tr> 
  <tr> 
   <td>Extensiones de archivo</td> 
   <td> <p> Elija las extensiones de archivo que desea buscar.</p> </td> 
  </tr> 
  <tr> 
   <td>Límite </td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Descargar un archivo]

Este módulo de acción descarga un archivo de una carpeta.

Especifique el archivo y su ubicación.

El módulo devuelve el ID del archivo y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

>[!NOTE]
>
>Este módulo es útil para proporcionar archivos a módulos subsiguientes.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Dropbox] a [!DNL Workfront Fusion], vea <a href="#create-a-connection-to-dropbox" class="MCXref xref">Crear una conexión con [!DNL Dropbox]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>Forma de seleccionar archivos</td> 
   <td> <p> Seleccione si desea asignar la ruta de acceso del archivo o seleccione el archivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ruta de archivo / Archivo</p> </td> 
   <td> <p style="font-weight: bold;">Ruta de archivo</p> <p>Introduzca o asigne la ruta de destino al archivo.</p> <p style="font-weight: bold;">Archivo</p> <p>Seleccione el archivo en el menú.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener metadatos de carpeta]

Este módulo de acción recupera los detalles de la carpeta compartida.

Especifique el ID de la carpeta.

El módulo devuelve el ID de la carpeta y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Dropbox] a [!DNL Workfront Fusion], vea <a href="#create-a-connection-to-dropbox" class="MCXref xref">Crear una conexión con [!DNL Dropbox]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>Identificador de carpeta compartida</td> 
   <td> <p> Introduzca o asigne el ID de la carpeta sobre la que desea recuperar los detalles.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enumerar todos los archivos/subcarpetas de una carpeta]

Este módulo de acción enumera los archivos o carpetas de una carpeta concreta.

Especifique el ID de la carpeta.

El módulo devuelve los ID de los archivos o carpetas y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Dropbox] a [!DNL Workfront Fusion], vea <a href="#create-a-connection-to-dropbox" class="MCXref xref">Crear una conexión con [!DNL Dropbox]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>Lista </td> 
   <td> <p>Seleccione si desea recuperar archivos o carpetas.</p> </td> 
  </tr> 
  <tr> 
   <td>Mostrar solo los archivos descargables</td> 
   <td> <p> Active esta opción para devolver solo los archivos descargables. Algunos tipos de archivos, como los documentos de Google, no se pueden descargar.</p> </td> 
  </tr> 
  <tr> 
   <td>Carpeta </td> 
   <td> <p>Introduzca o asigne la carpeta de la que desea recuperar archivos o carpetas.</p> </td> 
  </tr> 
  <tr> 
   <td>Límite </td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo enumere durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Revisiones de archivos de lista]

Este módulo de acción recupera todas las revisiones de archivo (un historial de versiones) de un archivo concreto.\
Especifique el ID del archivo.

El módulo devuelve cualquier campo estándar asociado con el registro, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Dropbox] a [!DNL Workfront Fusion], vea <a href="#create-a-connection-to-dropbox" class="MCXref xref">Crear una conexión con [!DNL Dropbox]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>Forma de seleccionar archivos</td> 
   <td> <p> Seleccione si desea asignar la ruta de acceso del archivo o seleccione el archivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ruta de archivo / Archivo</p> </td> 
   <td> <p style="font-weight: bold;">Ruta de archivo</p> <p>Introduzca o asigne la ruta de destino al archivo.</p> <p style="font-weight: bold;">Archivo</p> <p>Seleccione el archivo en el menú.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Límite</p> </td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo enumere durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Módulos para crear y editar [!DNL Dropbox] archivos y carpetas

* [[!UICONTROL Cargar] un archivo](#upload-a-file)
* [[!UICONTROL Crear una carpeta]](#create-a-folder)
* [[!UICONTROL Crear o sobrescribir un archivo de texto]](#createoverwrite-a-text-file)
* [[!UICONTROL Crear/actualizar un vínculo compartido]](#createupdate-a-share-link)
* [[!UICONTROL Restaurar un archivo]](#restore-a-file)
* [[!UICONTROL Mover un archivo/carpeta]](#move-a-filefolder)
* [[!UICONTROL Cambiar el nombre de un archivo o carpeta]](#rename-a-filefolder)
* [[!UICONTROL Eliminar un archivo o carpeta]](#delete-a-filefolder)

#### [!UICONTROL Cargar un archivo]

Este módulo de acción carga un archivo en una carpeta.

Especifique información como la ubicación del archivo, el archivo que desea cargar y un nuevo nombre opcional para el archivo.

El módulo devuelve el ID del archivo y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Dropbox] a [!DNL Workfront Fusion], vea <a href="#create-a-connection-to-dropbox" class="MCXref xref">Crear una conexión con [!DNL Dropbox]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta]</td> 
   <td> <p> Seleccione la carpeta de su [!DNL Dropbox] en la que desee cargar el archivo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Archivo Source]</p> </td> 
   <td> <p>Escriba o asigne el archivo que desea agregar a la carpeta [!DNL Dropbox] seleccionada anteriormente.</p> <p style="font-weight: bold;">[!UICONTROL Nombre de archivo]</p> <p>Introduzca o asigne el nombre del archivo, incluida su extensión.</p> <p style="font-weight: bold;">[!UICONTROL Datos de archivo]</p> <p>Introduzca o asigne los datos del archivo (del módulo anterior, como [!UICONTROL Google Drive] &gt;[!UICONTROL Get a File)].</p> <p>Nota: El tamaño máximo del archivo cargado es de 150 MB.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sobrescribir un archivo existente]</td> 
   <td> <p> Active esta opción para reemplazar el archivo existente con el nuevo archivo. Si esta opción se deja deshabilitada, se cambiará el nombre del archivo cargado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear una carpeta]

Este módulo de acción crea una carpeta nueva.

Especifique la ruta y el nombre de la carpeta.

El módulo devuelve el ID de la carpeta y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Dropbox] a [!DNL Workfront Fusion], vea <a href="#create-a-connection-to-dropbox" class="MCXref xref">Crear una conexión con [!DNL Dropbox]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre de carpeta] </td> 
   <td> <p>Introduzca el nombre de la nueva carpeta.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Carpeta]</p> </td> 
   <td> <p>Introduzca o asigne la ruta donde desea crear una nueva carpeta.</p> <p>Nota:   <p>Si usa una cuenta de [!DNL Dropbox Business] (con espacios de equipo), debe quitar la barra <code>/</code> o no hacer clic en <strong>[!UICONTROL Haga clic aquí] para elegir la carpeta </strong> y crear una carpeta de equipo en la raíz.</p> <p>Si no se quita la barra oblicua, se devuelve un error <code>[409] path/malformed_path/..</code>.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cambiar nombre automáticamente]</td> 
   <td> <p> Active esta opción para cambiar el nombre de la nueva carpeta, si ya existe una carpeta con el mismo nombre en la ubicación de destino.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear o sobrescribir un archivo de texto]

Este módulo de acción crea un archivo DOC o sobrescribe el contenido de uno existente.

Especifique el archivo de origen y la carpeta.

El módulo devuelve el ID de la carpeta y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Dropbox] a [!DNL Workfront Fusion], vea <a href="#create-a-connection-to-dropbox" class="MCXref xref">Crear una conexión con [!DNL Dropbox]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Seleccionar para]</td> 
   <td> <p> Seleccione si desea crear o sobrescribir un archivo DOC.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione la ubicación de destino en la que desea crear un archivo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Archivo Source]</p> </td> 
   <td> <p>Escriba o asigne el archivo que desea agregar a la carpeta [!DNL Dropbox].</p> <p style="font-weight: bold;">Nombre del archivo</p> <p>Introduzca el nombre del nuevo archivo DOC (sin extensión).</p> <p style="font-weight: bold;">Contenido de archivo</p> <p>Introduzca el contenido de texto del archivo DOC.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear/actualizar un vínculo compartido]

Este módulo de acción crea un vínculo público a un archivo.

Especifique el archivo y la información sobre el vínculo.

El módulo devuelve el ID del vínculo y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Dropbox] a [!DNL Workfront Fusion], vea <a href="#create-a-connection-to-dropbox" class="MCXref xref">Crear una conexión con [!DNL Dropbox]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Forma de seleccionar archivos]</td> 
   <td> <p> Seleccione si desea asignar o introducir la ruta del archivo, o seleccione el archivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Ruta de archivo / Archivo]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Ruta de archivo]</p> <p>Introduzca o asigne la ruta de destino al archivo.</p> <p style="font-weight: bold;">[!UICONTROL Archivo]</p> <p>Seleccione el archivo en el menú.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Visibilidad solicitada]</p> </td> 
   <td> <p>Seleccione si el vínculo es público, de equipo o si está restringido con contraseña.</p> <p>Nota: Las opciones [!UICONTROL Team only] y [!UICONTROL Access with password] solo están disponibles para los usuarios que tengan [!DNL Dropbox Pro] o una versión superior.</p> </td> 
  </tr> 
  <tr> 
   <td>Fecha de caducidad del vínculo [!UICONTROL]</td> 
   <td> <p> Introduzca la fecha y la hora en que caducará el vínculo y dejará de ser accesible. Si este campo se deja vacío, el vínculo no caducará. Para obtener una lista de los formatos de fecha y hora admitidos, vea <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Coerción de tipos en [!DNL Adobe Workfront Fusion]</a>.</p> <p>Nota: Las opciones [!UICONTROL Team only] y [!UICONTROL Access with password] solo están disponibles para los usuarios que tengan [!UICONTROL Dropbox Pro] o versiones posteriores.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Nivel de acceso de [!UICONTROL Link]</p> </td> 
   <td> <p>Establezca el permiso para el destinatario del vínculo.</p> <p><strong>[!UICONTROL Viewer]</strong> Los usuarios que usen el vínculo pueden ver el contenido y realizar comentarios sobre él.</p> <p><strong>[!UICONTROL Editor]</strong> Los usuarios que usen el vínculo pueden editar, ver y comentar el contenido.</p> <p><strong>[!UICONTROL Max]</strong> Los usuarios que usen el vínculo reciben el nivel de acceso máximo al que puede establecer el vínculo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Restaurar un archivo]

Este módulo de acción restaura una versión anterior de un archivo.

Especifique el fichero y el número de revisión que desee.

El módulo devuelve el ID de la versión y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Dropbox] a [!DNL Workfront Fusion], vea <a href="#create-a-connection-to-dropbox" class="MCXref xref">Crear una conexión con [!DNL Dropbox]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Forma de seleccionar archivos]</td> 
   <td> <p> Seleccione si desea asignar o introducir la ruta del archivo, o seleccione el archivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Ruta de archivo] / [!UICONTROL Archivo]</p> </td> 
   <td> <p><strong>[!UICONTROL Ruta de archivo]</strong> </p> <p>Introduzca o asigne la ruta de destino al archivo.</p> <p><strong>[!UICONTROL Archivo]</strong> </p> <p>Seleccione el archivo en el menú.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Revisión]</p> </td> 
   <td> <p>Introduzca o asigne el número de revisión de la revisión que desea restaurar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover un archivo/carpeta]

Este módulo de acción mueve un archivo o carpeta a una ubicación diferente.

Usted especifica el archivo o carpeta y cómo y dónde desea moverlo.

El módulo devuelve el ID del archivo o la carpeta y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Dropbox] a [!DNL Workfront Fusion], vea <a href="#create-a-connection-to-dropbox" class="MCXref xref">Crear una conexión con [!DNL Dropbox]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Forma de seleccionar archivos] </td> 
   <td> <p>Seleccione si desea asignar o introducir la ruta del archivo, o seleccione el archivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Ruta de archivo/carpeta] / [!UICONTROL Archivo/carpeta]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Ruta de archivo/carpeta]</p> <p>Introduzca o asigne la ruta de destino al archivo o carpeta.</p> <p style="font-weight: bold;">[!UICONTROL Archivo/Carpeta]</p> <p>Seleccione el archivo o la carpeta en el menú.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL A Carpeta]</p> </td> 
   <td> <p>Introduzca o asigne la ubicación de destino del archivo o carpeta.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Nuevo nombre]</p> </td> 
   <td> <p>Introduzca el nuevo nombre del archivo o la carpeta en la nueva ubicación.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Cambiar nombre automáticamente]</p> </td> 
   <td> <p>Habilite esta opción para asegurarse de que si existe un archivo o una carpeta con el mismo nombre, el módulo cambia el nombre del nuevo archivo o carpeta agregando ([!UICONTROL NUMBER]) después del nombre del archivo o carpeta. De lo contrario, se sobrescribe el archivo o la carpeta de la ubicación de destino.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permitir transferencia de propiedad]</p> </td> 
   <td> <p>Active esta opción para permitir movimientos por propietario, incluso si esto resultara en una transferencia de propiedad del contenido que se está moviendo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cambiar el nombre de un archivo o carpeta]

Este módulo de acción cambia el nombre de un archivo o carpeta.

Especifique el archivo o la carpeta y el nuevo nombre.

El módulo devuelve el ID del archivo o la carpeta y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Dropbox] a [!DNL Workfront Fusion], vea <a href="#create-a-connection-to-dropbox" class="MCXref xref">Crear una conexión con [!DNL Dropbox]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>Forma de seleccionar archivos</td> 
   <td> <p> Seleccione si desea asignar o introducir la ruta del archivo, o seleccione el archivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ruta de archivo/carpeta / Archivo/carpeta</p> </td> 
   <td> <p style="font-weight: bold;">Ruta de archivo/carpeta</p> <p>Introduzca o asigne la ruta de destino al archivo o carpeta.</p> <p style="font-weight: bold;">Archivo/Carpeta</p> <p>Seleccione el archivo o la carpeta en el menú.</p> </td> 
  </tr> 
  <tr> 
   <td>Cambiar nombre </td> 
   <td> <p>Escriba el [!UICONTROL nombre de destino] para el archivo, incluida la extensión de archivo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un archivo o carpeta]

Este módulo de acción elimina un archivo o una carpeta.

Especifique el archivo o la carpeta.

El módulo devuelve el ID del registro y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Dropbox] a [!DNL Workfront Fusion], vea <a href="#create-a-connection-to-dropbox" class="MCXref xref">Crear una conexión con [!DNL Dropbox]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Forma de seleccionar archivos]</td> 
   <td> <p> Seleccione si desea asignar o introducir la ruta del archivo, o seleccione el archivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Ruta de archivo] / [!UICONTROL Archivo]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Ruta de archivo]</p> <p>Introduzca o asigne la ruta de destino al archivo.</p> <p style="font-weight: bold;">[!UICONTROL Archivo]</p> <p>Seleccione el archivo en el menú.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Otros módulos

#### [!UICONTROL Realizar una llamada API]

Este módulo de acción le permite realizar una llamada autenticada personalizada a la API [!DNL Dropbox]. De este modo, puede crear una automatización del flujo de datos que no puedan realizar los otros [!DNL Dropbox] módulos.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Dropbox] a [!DNL Workfront Fusion], vea <a href="#create-a-connection-to-dropbox" class="MCXref xref">Crear una conexión con [!DNL Dropbox]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Escriba una ruta relativa a Escriba una ruta relativa a <code>https://api.dropboxapi.com</code>. Por ejemplo, <code>/2/files/list_folder</code></p> <p>Nota: Para obtener la lista de extremos disponibles, consulte la <a href="https://www.dropbox.com/developers/documentation/http/documentation">Documentación de la API de Dropbox v2</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Encabezados] </td> 
   <td> <p>Introduzca los encabezados de solicitud deseados. [!DNL Workfront Fusion] agrega los encabezados de autorización automáticamente.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cadena de consulta]</td> 
   <td> <p> Introduzca la cadena de consulta de solicitud.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cuerpo] </td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:   <p>Cuando utilice afirmaciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Ejemplo:** La siguiente llamada de API devuelve los primeros 10 archivos de la carpeta [!DNL /Text files] de su cuenta de [!DNL Dropbox]:
>
>URL: `/2/files/list_folder`
>
>Cuerpo:
> 
>`{`
>
>`"path": "/Text files",`
>
>`"limit": 10,`
>
>`"recursive": false,`
>
>`"include_deleted": false`
>
>`}`
>
>Las coincidencias de la búsqueda se pueden encontrar en la salida del módulo en [!UICONTROL Paquete] > [!UICONTROL Cuerpo] > entradas.
>
>En nuestro ejemplo, se devolvieron 10 tickets:

## Problemas comunes

* [No se puede cargar o actualizar un archivo](#unable-to-upload-or-update-a-file)
* [La imagen a la que se hace referencia mediante un vínculo compartido no se representa](#image-referenced-via-a-shared-link-does-not-render)

### No se puede cargar o actualizar un archivo

Cuando falla la carga o actualización de un archivo, se dan varias situaciones:

* El archivo cargado es demasiado grande y supera el tamaño máximo de archivo permitido para el plan [!DNL Dropbox], o bien ha utilizado toda la cuota de almacenamiento de la cuenta [!DNL Dropbox]. Debe eliminar los archivos existentes de su cuenta de [!DNL Dropbox] o actualizar su plan.
* La carpeta seleccionada anteriormente en la que se está cargando el archivo ya no existe. El escenario se detiene y debe volver a seleccionar la carpeta de destino.

### La imagen a la que se hace referencia mediante un vínculo compartido no se representa

La dirección URL devuelta por el [!UICONTROL Dropbox] >[!UICONTROL Crear un vínculo compartido] no vincula directamente a una imagen, sino a una página [!DNL Dropbox]. Para forzar la descarga de la imagen, reemplace el `?dl=0` final por `?dl=1`. Para forzar el procesamiento de la imagen (por ejemplo, en un explorador Web o en Facebook Messenger), añada `&raw=1` a la dirección URL.

Si necesita obtener el vínculo directo o sin procesar de la imagen para su sitio web o para otros módulos de [!DNL Workfront Fusion], debe modificar la dirección URL compartida inicial de la siguiente manera:

URL original:

`https://www.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png?dl=0`

1. Reemplazar `www` por `dl`.
1. Quitar `?dl=0`.

URL final:

`https://dl.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png`

Para modificar automáticamente la dirección URL, puede usar la función `replace()` dos veces:

* Reemplazar www por dl

  ![](assets/www-to-dl-350x32.png)

* Y para quitar ?dl=0

  ![](assets/remove-dl0-350x33.png)

Para hacerlo en un solo paso, combine estas funciones:

![](assets/replace-both-350x47.png)

También puede copiarlo y pegarlo en el campo. Reemplazar `1.url` por la URL.

```
{{replace(replace(1.url; "?dl=0"; ""); "www"; "dl")}}
```
