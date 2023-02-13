---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: módulos Dropbox
description: En un [!DNL Adobe Workfront Fusion] en este caso, puede automatizar los flujos de trabajo que utilizan Dropbox, así como conectarlos a varias aplicaciones y servicios de terceros. Esto le permite automatizar actividades como monitorizar, buscar, recuperar, enumerar, crear y editar archivos y carpetas en su Dropbox.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: a35631d7-40ac-4e7f-9a37-ad3879c0b6a2
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3013'
ht-degree: 0%

---

# [!DNL Dropbox] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!UICONTROL Dropbox], así como conectarlo a varias aplicaciones y servicios de terceros. Esto le permite automatizar actividades como monitorizar, buscar, recuperar, listar, crear y editar archivos y carpetas en su [!UICONTROL Dropbox].

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

Para usar [!DNL Dropbox] módulos, debe tener un [!DNL Dropbox] cuenta.

## [!DNL Dropbox] módulos y sus campos

Al configurar [!DNL Dropbox] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL Dropbox] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [módulos de déclencheur](#trigger-modules)
* [Módulos para obtener [!DNL Dropbox] archivos y carpetas](#modules-for-getting-dropbox-files-and-folders)
* [Módulos para crear y editar [!DNL Dropbox] archivos y carpetas](#modules-for-creating-and-editing-dropbox-files-and-folders)
* [Otros módulos](#other-modules)

### módulos de déclencheur

#### [!UICONTROL Archivos de Watch]

Este módulo de tipo Déclencheur devuelve detalles del archivo cuando se modifica el archivo en una carpeta especificada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Dropbox] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleccione la carpeta que desee ver para ver los cambios.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch también subcarpetas]</td> 
   <td> <p> Active esta opción para controlar también las subcarpetas de la carpeta seleccionada para los archivos modificados.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Límite] </td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Módulos para obtener [!DNL Dropbox] archivos y carpetas

* [[!UICONTROL Buscar archivos/carpetas]](#search-filesfolders)
* [[!UICONTROL Descargar un archivo]](#download-a-file)
* [[!UICONTROL Obtener metadatos de una carpeta]](#get-a-folder-metadata)
* [[!UICONTROL Enumerar todos los archivos/subcarpetas en una carpeta]](#list-all-filessubfolders-in-a-folder)
* [[!UICONTROL Enumerar revisiones de archivos]](#list-file-revisions)

#### [!UICONTROL Buscar archivos/carpetas]

Este módulo de búsqueda busca registros en un objeto de [!DNL Dropbox] que coinciden con la consulta de búsqueda especificada.

Puede asignar esta información en módulos posteriores en el escenario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Dropbox] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Buscar] </td> 
   <td> <p>Introduzca el término de búsqueda.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleccione la carpeta que desee buscar. Este módulo busca todo [!DNL Dropbox] si no selecciona ninguna carpeta.</p> </td> 
  </tr> 
  <tr> 
   <td>Estado del archivo</td> 
   <td> <p> Seleccione el estado del archivo para restringir la búsqueda al estado del archivo seleccionado.</p> </td> 
  </tr> 
  <tr> 
   <td>Categorías de archivos</td> 
   <td> <p> Seleccione las categorías de archivos para restringir la búsqueda a las categorías seleccionadas.</p> </td> 
  </tr> 
  <tr> 
   <td>Extensiones de archivo</td> 
   <td> <p> Elija las extensiones de archivo que desea buscar.</p> </td> 
  </tr> 
  <tr> 
   <td>Límite </td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Descargar un archivo]

Este módulo de acción descarga un archivo de una carpeta.

Especifique el archivo y su ubicación.

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
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Dropbox] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>Forma de seleccionar archivos</td> 
   <td> <p> Seleccione si desea asignar la ruta del archivo o seleccione el archivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ruta del archivo/Archivo</p> </td> 
   <td> <p style="font-weight: bold;">Ruta de archivo</p> <p>Introduzca o asigne la ruta de destino al archivo.</p> <p style="font-weight: bold;">Archivo</p> <p>Seleccione el archivo en el menú .</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener metadatos de una carpeta]

Este módulo de acción recupera los detalles de las carpetas compartidas.

Especifique el ID de la carpeta.

El módulo devuelve el ID de la carpeta y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Dropbox] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>ID de carpeta compartida</td> 
   <td> <p> Introduzca o asigne el ID de la carpeta de la que desea recuperar los detalles.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enumerar todos los archivos/subcarpetas en una carpeta]

Este módulo de acción enumera los archivos o carpetas de una carpeta concreta.

Especifique el ID de la carpeta.

El módulo devuelve los ID de los archivos o carpetas y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Dropbox] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>Lista </td> 
   <td> <p>Seleccione si desea recuperar archivos o carpetas.</p> </td> 
  </tr> 
  <tr> 
   <td>Mostrar solo archivos descargables</td> 
   <td> <p> Active esta opción para devolver solo los archivos descargables. Algunos tipos de archivos, como Google Docs, no se pueden descargar.</p> </td> 
  </tr> 
  <tr> 
   <td>Carpeta </td> 
   <td> <p>Introduzca o asigne la carpeta desde la que desea recuperar archivos o carpetas.</p> </td> 
  </tr> 
  <tr> 
   <td>Límite </td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo enumere durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Enumerar revisiones de archivos]

Este módulo de acción recupera todas las revisiones de archivos (un historial de versiones) de un archivo en particular.\
Especifique el ID del archivo.

El módulo devuelve todos los campos estándar asociados con el registro, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Dropbox] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>Forma de seleccionar archivos</td> 
   <td> <p> Seleccione si desea asignar la ruta del archivo o seleccione el archivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ruta del archivo/Archivo</p> </td> 
   <td> <p style="font-weight: bold;">Ruta de archivo</p> <p>Introduzca o asigne la ruta de destino al archivo.</p> <p style="font-weight: bold;">Archivo</p> <p>Seleccione el archivo en el menú .</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Límite</p> </td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo enumere durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Módulos para crear y editar [!DNL Dropbox] archivos y carpetas

* [[!UICONTROL Cargar] un archivo](#upload-a-file)
* [[!UICONTROL Crear una carpeta]](#create-a-folder)
* [[!UICONTROL Crear/sobrescribir un archivo de texto]](#createoverwrite-a-text-file)
* [[!UICONTROL Crear/actualizar un vínculo compartido]](#createupdate-a-share-link)
* [[!UICONTROL Restaurar un archivo]](#restore-a-file)
* [[!UICONTROL Mover un archivo/carpeta]](#move-a-filefolder)
* [[!UICONTROL Cambiar el nombre de un archivo o carpeta]](#rename-a-filefolder)
* [[!UICONTROL Eliminar un archivo/carpeta]](#delete-a-filefolder)

#### [!UICONTROL Cargar un archivo]

Este módulo de acción carga un archivo en una carpeta.

Especifique información como la ubicación del archivo, el archivo que desea cargar y un nombre nuevo opcional para el archivo.

El módulo devuelve el ID del archivo y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Dropbox] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td> <p> Seleccione la carpeta de [!DNL Dropbox] desea cargar el archivo en .</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Archivo de origen]</p> </td> 
   <td> <p>Introduzca o asigne el archivo que desea agregar a la variable [!DNL Dropbox] carpeta seleccionada arriba.</p> <p style="font-weight: bold;">[!UICONTROL File name]</p> <p>Introduzca o asigne el nombre de archivo, incluida la extensión de archivo.</p> <p style="font-weight: bold;">[!UICONTROL Datos de archivo]</p> <p>Introduzca o asigne los datos del archivo (del módulo anterior, como [!UICONTROL Google Drive] &gt;[!UICONTROL Get a File)].</p> <p>Nota: El tamaño máximo del archivo cargado es de 150 MB.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sobrescribir un archivo existente]</td> 
   <td> <p> Active esta opción para reemplazar el archivo existente por el nuevo archivo. Si esta opción se deja desactivada, se cambia el nombre del archivo cargado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear una carpeta]

Este módulo de acción crea una nueva carpeta.

Especifique la ruta y un nombre para la carpeta.

El módulo devuelve el ID de la carpeta y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Dropbox] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder Name] </td> 
   <td> <p>Introduzca el nombre de la nueva carpeta.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Folder]</p> </td> 
   <td> <p>Introduzca o asigne la ruta en la que desea crear una carpeta nueva.</p> <p>Nota:   <p>Si está utilizando un [!DNL Dropbox Business] cuenta (con espacios de equipo), debe eliminar la barra diagonal <code>/</code>o no haga clic en <strong>[!UICONTROL Haga clic aquí] para elegir la carpeta</strong> para crear una carpeta de equipo en la raíz.</p> <p>Si la barra diagonal no se elimina, se produce un error <code>[409] path/malformed_path/..</code> se devuelve.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cambio de nombre automático]</td> 
   <td> <p> Active esta opción para cambiar el nombre de la nueva carpeta si ya existe una carpeta con el mismo nombre en la ubicación de destino.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear/sobrescribir un archivo de texto]

Este módulo de acción crea un archivo DOC o sobrescribe el contenido de uno existente.

Especifique el archivo de origen y la carpeta.

El módulo devuelve el ID de la carpeta y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Dropbox] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Seleccionar a]</td> 
   <td> <p> Seleccione si desea crear o sobrescribir un archivo DOC.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Seleccione la ubicación de destino en la que desea crear un archivo.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Archivo de origen]</p> </td> 
   <td> <p>Introduzca o asigne el archivo que desea agregar a la variable [!DNL Dropbox] carpeta.</p> <p style="font-weight: bold;">Nombre del archivo</p> <p>Introduzca el nombre de archivo del nuevo archivo DOC (sin extensión).</p> <p style="font-weight: bold;">Contenido del archivo</p> <p>Introduzca el contenido de texto del archivo DOC.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear/actualizar un vínculo compartido]

Este módulo de acción crea un vínculo público a un archivo.

Especifique el archivo y la información sobre el vínculo.

El módulo devuelve el ID del vínculo y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Dropbox] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Forma de seleccionar archivos]</td> 
   <td> <p> Seleccione si desea asignar o introducir la ruta del archivo, o seleccione el archivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Ruta del archivo / Archivo]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Ruta de archivo]</p> <p>Introduzca o asigne la ruta de destino al archivo.</p> <p style="font-weight: bold;">[!UICONTROL Archivo]</p> <p>Seleccione el archivo en el menú .</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Visibilidad solicitada]</p> </td> 
   <td> <p>Seleccione si el vínculo es público, para equipo o si la contraseña está restringida.</p> <p>Nota: Las opciones [!UICONTROL Team only] y [!UICONTROL Access with password] solo están disponibles para los usuarios que tengan [!DNL Dropbox Pro] o una versión posterior.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fecha de caducidad del vínculo]</td> 
   <td> <p> Introduzca la fecha y la hora en que caducará el vínculo y este dejará de ser accesible. Si este campo se deja vacío, el vínculo no caducará. Para obtener una lista de los formatos de fecha y hora admitidos, consulte <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Coerción de tipo en [!DNL Adobe Workfront Fusion]</a>.</p> <p>Nota: Las opciones [!UICONTROL Team only] y [!UICONTROL Access with password] solo están disponibles para los usuarios que tengan [!UICONTROL Dropbox Pro] o versiones posteriores.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Nivel de acceso del vínculo]</p> </td> 
   <td> <p>Establezca el permiso para el destinatario del vínculo.</p> <p><strong>[!UICONTROL Viewer]</strong> Los usuarios que utilicen el vínculo pueden ver y comentar el contenido.</p> <p><strong>[!UICONTROL Editor]</strong> Los usuarios que utilicen el vínculo pueden editar, ver y comentar el contenido.</p> <p><strong>[!UICONTROL Max]</strong> Los usuarios que utilicen el vínculo reciben el nivel de acceso máximo al que puede establecer el vínculo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Restaurar un archivo]

Este módulo de acción restaura una versión anterior de un archivo.

Especifique el archivo y el número de la revisión que desee.

El módulo devuelve el ID de la versión y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Dropbox] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Forma de seleccionar archivos]</td> 
   <td> <p> Seleccione si desea asignar o introducir la ruta del archivo, o seleccione el archivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File Path] / [!UICONTROL File]</p> </td> 
   <td> <p><strong>[!UICONTROL Ruta de archivo]</strong> </p> <p>Introduzca o asigne la ruta de destino al archivo.</p> <p><strong>[!UICONTROL Archivo]</strong> </p> <p>Seleccione el archivo en el menú .</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Revisión]</p> </td> 
   <td> <p>Introduzca o asigne el número de revisión de la revisión que desea restaurar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover un archivo/carpeta]

Este módulo de acción mueve un archivo o carpeta a una ubicación diferente.

Usted especifica el archivo o la carpeta y cómo y dónde desea moverlo.

El módulo devuelve el ID del archivo o la carpeta y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Dropbox] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Forma de seleccionar archivos] </td> 
   <td> <p>Seleccione si desea asignar o introducir la ruta del archivo, o seleccione el archivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File/Folder Path] / [!UICONTROL File/Folder]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Archivo/Ruta de carpeta]</p> <p>Introduzca o asigne la ruta de destino al archivo o carpeta.</p> <p style="font-weight: bold;">[!UICONTROL Archivo/Carpeta]</p> <p>Seleccione el archivo o la carpeta en el menú .</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL To Folder]</p> </td> 
   <td> <p>Introduzca o asigne la ubicación de destino del archivo o carpeta.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Nuevo nombre]</p> </td> 
   <td> <p>Introduzca el nuevo nombre del archivo o carpeta en la nueva ubicación.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Cambio de nombre automático]</p> </td> 
   <td> <p>Active esta opción para asegurarse de que si existe un archivo o carpeta con el mismo nombre, el módulo cambia el nombre del nuevo archivo o carpeta agregando ([!UICONTROL NUMBER]) después del nombre del archivo o carpeta. De lo contrario, se sobrescribe el archivo o la carpeta en la ubicación de destino.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permitir transferencia de propiedad]</p> </td> 
   <td> <p>Active esta opción para permitir movimientos por propietario, incluso si resultaría en una transferencia de propiedad para el contenido que se está moviendo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cambiar el nombre de un archivo o carpeta]

Este módulo de acción cambia el nombre de un archivo o carpeta.

Especifique el archivo o la carpeta y el nuevo nombre.

El módulo devuelve el ID del archivo o la carpeta y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Dropbox] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>Forma de seleccionar archivos</td> 
   <td> <p> Seleccione si desea asignar o introducir la ruta del archivo, o seleccione el archivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ruta de archivo/carpeta/Archivo/Carpeta</p> </td> 
   <td> <p style="font-weight: bold;">Ruta de archivo/carpeta</p> <p>Introduzca o asigne la ruta de destino al archivo o carpeta.</p> <p style="font-weight: bold;">Archivo/Carpeta</p> <p>Seleccione el archivo o la carpeta en el menú .</p> </td> 
  </tr> 
  <tr> 
   <td>Cambiar nombre </td> 
   <td> <p>Introduzca el [!UICONTROL target name] para el archivo, incluida la extensión de archivo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un archivo/carpeta]

Este módulo de acción elimina un archivo o una carpeta.

Especifique el archivo o la carpeta.

El módulo devuelve el ID del registro y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Dropbox] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Forma de seleccionar archivos]</td> 
   <td> <p> Seleccione si desea asignar o introducir la ruta del archivo, o seleccione el archivo manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File Path] / [!UICONTROL File]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Ruta de archivo]</p> <p>Introduzca o asigne la ruta de destino al archivo.</p> <p style="font-weight: bold;">[!UICONTROL Archivo]</p> <p>Seleccione el archivo en el menú .</p> </td> 
  </tr> 
 </tbody> 
</table>

### Otros módulos

#### [!UICONTROL Realizar una llamada de API]

Este módulo de acción le permite realizar una llamada autenticada personalizada al [!DNL Dropbox] API. De este modo, puede crear una automatización del flujo de datos que no se pueda lograr con la otra [!DNL Dropbox] módulos.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Dropbox] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Introduzca una ruta relativa a Introducir una ruta relativa a <code>https://api.dropboxapi.com</code>. Por ejemplo, <code>/2/files/list_folder</code></p> <p>Nota: Para ver la lista de extremos disponibles, consulte la <a href="https://www.dropbox.com/developers/documentation/http/documentation">Documentación de la API v2 del Dropbox</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada a la API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Encabezados] </td> 
   <td> <p>Introduzca los encabezados de solicitud deseados. [!DNL Workfront Fusion] añade encabezados de autorización automáticamente.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cadena de consulta]</td> 
   <td> <p> Introduzca la cadena de consulta de solicitud.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body] </td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:   <p>Al utilizar afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Ejemplo:** La siguiente llamada de API devuelve los primeros 10 archivos de la variable [!DNL /Text files] en su [!DNL Dropbox] cuenta:
>
>Dirección URL: `/2/files/list_folder`
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
>En nuestro ejemplo, se devolvieron 10 entradas:

## Problemas comunes

* [No se puede cargar o actualizar un archivo](#unable-to-upload-or-update-a-file)
* [La imagen a la que se hace referencia mediante un vínculo compartido no se renderiza](#image-referenced-via-a-shared-link-does-not-render)

### No se puede cargar o actualizar un archivo

Existen varias situaciones en las que se produce un error al cargar o actualizar un archivo:

* El archivo cargado es demasiado grande y supera el tamaño máximo de archivo permitido para su [!DNL Dropbox] o ha usado todo su [!DNL Dropbox] cuota de almacenamiento de la cuenta. Debe eliminar los archivos existentes de su [!DNL Dropbox] o actualice su plan.
* La carpeta seleccionada anteriormente, a la que se está cargando el archivo, ya no existe. El escenario se detiene y debe seleccionar de nuevo la carpeta de destino.

### La imagen a la que se hace referencia mediante un vínculo compartido no se renderiza

La URL devuelta por la variable [!UICONTROL Dropbox] >[!UICONTROL Crear un vínculo compartido] no se vincula directamente a una imagen, sino a una [!DNL Dropbox] página. Para forzar la descarga de la imagen, reemplace la `?dl=0` con `?dl=1`. Para forzar la representación de la imagen (por ejemplo, en un navegador web o en Facebook Messenger), anexe `&raw=1` a la dirección URL.

Si necesita obtener el vínculo directo o sin procesar de la imagen para su sitio web u otro [!DNL Workfront Fusion] , debe modificar la URL compartida inicial de la siguiente manera:

URL original:

`https://www.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png?dl=0`

1. Reemplazar `www` con `dl`.
1. Eliminar `?dl=0`.

URL final:

`https://dl.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png`

Para modificar automáticamente la dirección URL, puede usar la variable `replace()` función dos veces:

* Reemplazar www con dl

   ![](assets/www-to-dl-350x32.png)

* Y para eliminar ?dl=0

   ![](assets/remove-dl0-350x33.png)

Para hacerlo en un solo paso, combine estas funciones:

![](assets/replace-both-350x47.png)

También puede copiarlo y pegarlo en el campo . Reemplazar `1.url` con la dirección URL.

```
{{replace(replace(1.url; "?dl=0"; ""); "www"; "dl")}}
```
