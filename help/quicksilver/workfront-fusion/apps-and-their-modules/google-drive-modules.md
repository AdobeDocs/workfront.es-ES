---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos de Google Drive
description: La variable [!DNL Adobe Workfront Fusion Google Drive] los módulos le permiten supervisar, buscar, crear, actualizar, eliminar y administrar sus archivos, carpetas o unidades compartidas en su [!DNL Google Drive].
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d620c93-d1bf-4451-9f76-1d6fd850cec9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2908'
ht-degree: 0%

---

# [!DNL Google Drive] módulos

La variable [!DNL Adobe Workfront Fusion] [!DNL Google Drive] los módulos le permiten supervisar, buscar, crear, actualizar, eliminar y administrar sus archivos, carpetas o unidades compartidas en su [!DNL Google Drive].

En un [!DNL Adobe Workfront Fusion] , puede conectar su [!DNL Google Drive] a varias aplicaciones y servicios de terceros.

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



## Conexión [!DNL Google Drive] a [!DNL Workfront Fusion]

Si [!DNL @gmail.com] o [!DNL @googlemail.com] usuario que necesita crear un cliente de OAuth en [el [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) para obtener [!UICONTROL ID de cliente] y [!UICONTROL Secreto del cliente].

Para obtener instrucciones paso a paso sobre cómo crear el cliente OAuth (y obtener [!UICONTROL ID de cliente] y [!UICONTROL Secreto del cliente]), consulte [Connect [!DNL Adobe Workfront Fusion] a [!DNL Google Services] uso de un cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Para obtener instrucciones sobre cómo conectar su [!DNL Google Drive] cuenta para [!UICONTROL Workfront Fusion], consulte [Crear una conexión con [!UICONTROL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Google Drive] módulos y sus campos

Al configurar [!DNL Google Drive] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL Google Drive] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)



* [Déclencheur](#triggers)
* [Acciones](#actions)

### Déclencheur

* [[!UICONTROL Archivos de inspección en la carpeta]](#watch-files-in-folder)
* [[!UICONTROL Ver todos los archivos]](#watch-all-files)
* [[!UICONTROL Ver archivos compartidos]](#watch-shared-files)
* [[!UICONTROL Observar comentarios]](#watch-comments)

#### [!UICONTROL Archivos de inspección en la carpeta]

Recupera los detalles del archivo cuando se agrega o modifica un archivo en la carpeta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection] </td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Drive] cuenta para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexión [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Seleccione la carpeta que desea ver]</td>
    <td >Seleccione la carpeta de la unidad en la que desea ver los archivos.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL Qué archivos ver]</td>
   <td> <p>Seleccione el tipo de archivos que desea ver.</p> 
    <ul> 
     <li>[!UICONTROL Todo]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Convertir [!DNL Google Documents] archivos a formato]</td>
    <td>Seleccione el formato de archivo que desea convertir [!DNL Google Documents] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir [!DNL Google Spreadsheets] archivos a formato]</td>
    <td>Seleccione el formato de archivo que desea convertir [!DNL Google Spreadsheets] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir [!DNL Google Slides] archivos a formato]</td>
    <td>Seleccione el formato de archivo que desea convertir [!DNL Google Slides] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir [!DNL Google Drawings] archivos a formato]</td>
    <td>Seleccione el formato de archivo que desea convertir [!DNL Google Drawings] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Watch]</td>
    <td>Seleccione si desea ver nuevos archivos y todos los cambios, o solo archivos nuevos.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL Número máximo de archivos descargados]</td>
    <td>Establezca el número máximo de resultados que [!DNL Workfront Fusion] se descargará durante un ciclo (el número de repeticiones por ejecución de escenario).</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ver todos los archivos]

Recupera los detalles del archivo cuando un archivo de [!DNL Google Drive] se añade o modifica.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Drive] cuenta para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexión [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Qué archivos ver]</td> 
   <td> <p>Seleccione el tipo de archivos que desea ver.</p> 
    <ul> 
     <li>[!UICONTROL Todo]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Convertir [!DNL Google Documents] archivos a formato]</td>
    <td>Seleccione el formato de archivo que desea convertir [!DNL Google Documents] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir [!DNL Google Spreadsheets] archivos a formato]</td>
    <td>Seleccione el formato de archivo que desea convertir [!DNL Google Spreadsheets] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir [!DNL Google Slides] archivos a formato]</td>
    <td>Seleccione el formato de archivo que desea convertir [!DNL Google Slides] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir [!DNL Google Drawings] archivos a formato]</td>
    <td>Seleccione el formato de archivo que desea convertir [!DNL Google Drawings] a.</td>
  </tr>  
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>Seleccione si desea ver nuevos archivos y todos los cambios, o solo archivos nuevos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de archivos descargados]</td> 
   <td>Establezca el número máximo de resultados que [!DNL Workfront Fusion] se descargará durante un ciclo (el número de repeticiones por ejecución de escenario).</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ver archivos compartidos]

Déclencheur cuando se comparte un nuevo archivo con usted o cuando se actualiza un archivo compartido existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Drive] cuenta para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexión [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Seleccione la carpeta que desea ver]</td> 
   <td>Seleccione la carpeta compartida en la que desea ver los archivos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Qué archivos ver]</td> 
   <td> <p>Seleccione el tipo de archivos que desea ver.</p> 
    <ul> 
     <li>[!UICONTROL Todo]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Convertir [!DNL Google Documents] archivos a formato]</td>
    <td>Seleccione el formato de archivo que desea convertir [!DNL Google Documents] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir [!DNL Google Spreadsheets] archivos a formato]</td>
    <td>Seleccione el formato de archivo que desea convertir [!DNL Google Spreadsheets] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir [!DNL Google Slides] archivos a formato]</td>
    <td>Seleccione el formato de archivo que desea convertir [!DNL Google Slides] a.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir [!DNL Google Drawings] archivos a formato]</td>
    <td>Seleccione el formato de archivo que desea convertir [!DNL Google Drawings] a.</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>Seleccione si desea ver nuevos archivos y todos los cambios, o solo archivos nuevos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de archivos descargados]</td> 
   <td>Establezca el número máximo de resultados que [!DNL Workfront Fusion] se descargará durante un ciclo (el número de repeticiones por ejecución de escenario).</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Observar comentarios]

Déclencheur cuando se agrega o modifica un comentario en el archivo seleccionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Drive] cuenta para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexión [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archivo]</td> 
   <td>Seleccione el archivo que desea ver para los comentarios.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>Seleccione si desea ver todos los cambios o solo los comentarios nuevos</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de comentarios devueltos]</td> 
   <td>Establezca el número máximo de comentarios que [!DNL Workfront Fusion] volverá durante un ciclo (el número de repeticiones por ejecución de escenario).</td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Cargar un archivo]](#upload-a-file)
* [[!UICONTROL Actualizar un archivo]](#update-a-file)
* [[!UICONTROL Copiar un archivo]](#copy-a-file)
* [[!UICONTROL Eliminar un archivo]](#delete-a-file)
* [[!UICONTROL Mover un archivo/carpeta a la papelera]](#move-a-filefolder-to-trash)
* [[!UICONTROL Obtener un archivo]](#get-a-file)
* [[!UICONTROL Buscar archivos/carpetas]](#search-for-filesfolders)
* [[!UICONTROL Crear una carpeta]](#create-a-folder)
* [[!UICONTROL Obtener un vínculo compartido]](#get-a-share-link)

#### [!UICONTROL Cargar un archivo]

Carga un archivo en su [!DNL Google Drive].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Drive] cuenta para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexión [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Destination]</td> 
   <td> <p>Seleccione el destino al que desee cargar un archivo.</p> 
    <ul> 
     <li>[!DNL My Drive]</li> 
     <li>[!DNL Shared with Me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Target folder]</td> 
   <td>Seleccione la carpeta en la que desea cargar un archivo. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archivo de origen]</td> 
   <td>Seleccione si desea utilizar un archivo transferido desde un módulo anterior o si desea asignar el archivo manualmente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File name]</td> 
   <td>Seleccione el nombre del archivo. Esta opción está disponible si selecciona "[!UICONTROL Map]" en el campo [!UICONTROL source file].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data]</td> 
   <td>Seleccione el archivo de datos que desea cargar. Esta opción está disponible si selecciona "[!UICONTROL Map]" en el campo [!UICONTROL source file].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title]</td> 
   <td>Introduzca un título para el nuevo archivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir un archivo]</td> 
   <td>Al habilitar esta opción, el módulo puede convertir archivos al [!DNL Google] formato.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar un archivo]

Actualiza los metadatos o el contenido de un archivo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Drive] cuenta para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexión [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destino]</td> 
   <td> <p>Seleccione el destino al que desee cargar un archivo.</p> 
    <ul> 
     <li>[!UICONTROL Mi unidad]</li> 
     <li>[!UICONTROL compartido conmigo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mover a una carpeta]</td> 
   <td>Si desea mover el archivo a otra carpeta, seleccione la carpeta en la que desea mover el archivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td>Asigne el ID del archivo que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title]</td> 
   <td>Introduzca un título para el archivo actualizado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cambiar el contenido de un archivo]</td> 
   <td>Seleccione si desea reemplazar el contenido del archivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archivo de origen]</td> 
   <td>Seleccione si desea utilizar un archivo transferido desde un módulo anterior o si desea asignar el archivo manualmente. Este campo está disponible si ha seleccionado cambiar el contenido del archivo en el campo anterior.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File name]</td> 
   <td>Seleccione el nombre del archivo. Esta opción está disponible si selecciona "[!UICONTROL Map]" en el campo [!UICONTROL source file].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data]</td> 
   <td>Seleccione el archivo de datos que desea cargar. Esta opción está disponible si selecciona "[!UICONTROL Map]" en el campo [!UICONTROL source file].</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar un archivo]

Copia un archivo en la nueva ubicación.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Drive] cuenta para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexión [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destino]</td> 
   <td> <p>Seleccione el destino al que desee cargar un archivo.</p> 
    <ul> 
     <li>[!UICONTROL Mi unidad]</li> 
     <li>[!UICONTROL compartido conmigo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Target folder]</td> 
   <td>Seleccione la carpeta donde se encuentra el archivo que desea copiar/</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td>Asigne el ID del archivo que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL El nombre de la copia]</td> 
   <td>Introduzca un título para el nuevo archivo. Deje este campo vacío si no desea cambiar el nombre del archivo original.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un archivo]

Elimina permanentemente un archivo o una carpeta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Drive] cuenta para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexión [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td>Asigne el ID del archivo que desea eliminar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover un archivo/carpeta a la papelera]

Mueve un archivo o carpeta a la papelera.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Drive] cuenta para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexión [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td>Asigne el ID del archivo que desea mover a la papelera.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un archivo]

Recupera el archivo con el ID especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Drive] cuenta para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexión [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Documents] archivos a formato]</td> 
   <td>Seleccione el formato de archivo que desea convertir [!DNL Google Documents] a.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Spreadsheets] archivos a formato]</td> 
   <td>Seleccione el formato de archivo que desea convertir [!DNL Google Spreadsheets] a.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Slides] archivos a formato]</td> 
   <td>Seleccione el formato de archivo que desea convertir [!DNL Google Slides] a.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Drawings] archivos a formato]</td> 
   <td>Seleccione el formato de archivo que desea convertir [!DNL Google Drawings] a.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td>Asigne el ID del archivo que desea recuperar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Buscar archivos/carpetas]

Busca archivos o carpetas según los criterios de búsqueda.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Drive] cuenta para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexión [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destino]</td> 
   <td> <p>Seleccione el destino que desee buscar.</p> 
    <ul> 
     <li>[!UICONTROL Mi unidad]</li> 
     <li>[!UICONTROL compartido conmigo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lista de una carpeta]</td> 
   <td>Vaya a la carpeta en la que desea buscar los archivos o carpetas.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recuperar]</td> 
   <td> <p> Seleccione si desea buscar archivos, carpetas o ambos.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Buscar]</p> </td> 
   <td> <p>Seleccione el tipo de búsqueda que desea realizar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Buscar en nombres de archivo/carpeta]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>Introduzca una parte del nombre del archivo o del nombre completo del archivo (incluido el sufijo) que desea buscar.</p> </li> 
       <li> <p><strong>[!UICONTROL Opciones de búsqueda]</strong> </p> <p>Seleccione si desea buscar el término exacto o si desea buscar nombres que contengan el término de búsqueda.</p> </li> 
      </ul> </li> 
     <li> <p><strong>Búsqueda de [!UICONTROL Texto completo]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>Escriba cualquier término de búsqueda que desee buscar en su [!DNL Google Drive].</p> </li> 
      </ul> </li> 
     <li> <p><strong>Introducir consulta de búsqueda personalizada</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>Introduzca la consulta de búsqueda personalizada. Para obtener más información, consulte la sección [!UICONTROL Buscar archivos] de este artículo.</p> </li> 
       <li> <p><strong>Añadir la carpeta seleccionada arriba a la consulta</strong> </p> <p>Busca la carpeta en la colección principal. Esto encuentra todos los archivos y carpetas ubicados directamente en la carpeta seleccionada arriba.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de resultados devueltos]</td> 
   <td>Establezca el número máximo de archivos o carpetas [!DNL Workfront Fusion] volverá durante un ciclo de ejecución.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continúe con la ejecución de la ruta aunque el módulo no devuelva ningún resultado]</td> 
   <td>Active esta opción para asegurarse de que el escenario no se detenga si el módulo no devuelve resultados.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear una carpeta]

Crea una carpeta en la ubicación especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Drive] cuenta para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexión [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destino]</td> 
   <td> <p>Seleccione el destino al que desee cargar un archivo.</p> 
    <ul> 
     <li>[!UICONTROL Mi unidad]</li> 
     <li>[!UICONTROL compartido conmigo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nueva ubicación de carpeta]</td> 
   <td>Desplácese a la ubicación en la que desee crear una carpeta nueva.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL El nombre de la nueva carpeta]</td> 
   <td>Escriba un nombre para la carpeta que está creando.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta compartida]</td> 
   <td>Seleccione esta opción si desea compartir la carpeta con cualquier persona que tenga el vínculo [!UICONTROL Compartir]. De lo contrario, el vínculo compartido es solo para el propietario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un vínculo compartido]

Recupera el vínculo de uso compartido de un archivo en Google Drive.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google Drive] cuenta para [!DNL Workfront Fusion], consulte <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conexión [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td>Asigne el ID del archivo para el que desea obtener el vínculo compartido.</td> 
  </tr> 
 </tbody> 
</table>

## Resolución de problemas

### No se puede cargar o actualizar un archivo

Existen varias situaciones en las que se produce un error al cargar o actualizar un archivo:

* El archivo cargado es demasiado grande y supera el límite de tamaño máximo permitido para su [!DNL Google Drive] plan o ha excedido su [!DNL Google Drive] límite de almacenamiento. Puede actualizar su plan de almacenamiento o eliminar los archivos existentes del [!DNL Google Drive] servicio.
* La carpeta seleccionada en la que se iba a cargar el archivo ya no existe. El escenario se detiene y es necesario volver a seleccionar una carpeta de destino.

## Buscar archivos

En el módulo List files in a folder puede utilizar su propia consulta que consta de estas partes:

* **[!UICONTROL Campo]** : Atributo del archivo en el que se está buscando, por ejemplo, el atributo `name` del archivo.

* **[!UICONTROL Operador]** - Prueba que se realiza en los datos para proporcionar una coincidencia, por ejemplo, `contains`.

* **[!UICONTROL Valor]** - El contenido del atributo que se prueba, por ejemplo, el nombre del archivo `My cool document`.

Combinación de cláusulas con las conjunciones `and` o `or`y negar la consulta con `not`.

* [Campos](#fields)
* [Tipos de valores](#value-types)
* [Operadores](#operators)
* [Ejemplos](#examples)

### Campos

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Campo </th> 
   <th>Tipo de valor </th> 
   <th>Operadores</th> 
   <th> <p> Descripción</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>[!UICONTROL title]</code></td> 
   <td>string</td> 
   <td><code>contains</code><sup>1</sup>, <code>=</code>, <code>!=</code></td> 
   <td> <p> Nombre del archivo.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL fullText]</code> </td> 
   <td>string </td> 
   <td><code>contains</code><sup>2, 3</sup> </td> 
   <td> <p> Texto completo del archivo que incluye nombre, descripción, contenido y texto indexable.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL mimeType]</code> </td> 
   <td> string</td> 
   <td><code>contains</code>, <code>=</code>, <code>!=</code></td> 
   <td> <p> Tipo MIME del archivo.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL modifiedDate]</code> </td> 
   <td> date<sup>4</sup></td> 
   <td><code> &lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> Fecha de la última modificación del archivo.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL lastViewedByMeDate]</code> </td> 
   <td> date<sup>4</sup></td> 
   <td><code>&lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> Fecha en la que el usuario vio por última vez un archivo.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL trashed]</code></td> 
   <td>booleano </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> Si el archivo está en la papelera o no.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL starred]</code></td> 
   <td>booleano </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p>Indica si el archivo está iniciado o no.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL parents]</code></td> 
   <td>colección </td> 
   <td><code>in </code> </td> 
   <td> <p>Indica si la colección [!UICONTROL parent] contiene el ID especificado.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL owners]</code></td> 
   <td>colección </td> 
   <td><code>in </code> </td> 
   <td> <p>Usuarios que son propietarios del archivo.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL writers]</code></td> 
   <td>colección </td> 
   <td><code>in </code> </td> 
   <td> <p>Usuarios que tienen permiso para modificar el archivo.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL readers] </code> </td> 
   <td>colección </td> 
   <td><code>in </code> </td> 
   <td> <p>Usuarios que tienen permiso para leer el archivo.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL sharedWithMe]</code> </td> 
   <td>booleano </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> Archivos que están en la colección "Compartidos conmigo" del usuario.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL properties] </code> </td> 
   <td>colección</td> 
   <td><code>has </code> </td> 
   <td> <p> Propiedades de archivo personalizadas públicas.</p> </td> 
  </tr> 
 </tbody> 
</table>

Tenga en cuenta lo siguiente sobre los operadores en estos campos:

* La variable `contains` el operador solo realiza la coincidencia de prefijos en una `title`.

   Por ejemplo, el título &quot;HelloWorld&quot; coincide con el de `title contains 'Hello'` pero no para `title contains 'World'`.

* La variable `contains` el operador solo realiza la coincidencia en tokens de cadena completos para `fullText`.

   Por ejemplo, si el texto completo de un documento contiene la cadena &quot;HelloWorld&quot; solo la consulta `fullText contains 'HelloWorld'` devuelve un resultado. Consultas como `fullText contains 'Hello'` no devolverá resultados en este escenario.

* La variable `contains` coincide con una frase alfanumérica exacta si está rodeada de comillas dobles.

   Por ejemplo, si la variable `fullText` de un documento contiene la cadena &quot;Hello here world&quot;, luego la consulta `fullText contains '"Hello there"'` devuelve un resultado, pero la consulta `fullText contains '"Hello world"'` no.

   Además, porque la búsqueda es alfanumérica, si la variable `fullText` de un documento contiene la cadena &quot;Hello_world&quot;, luego la consulta `fullText contains '"Hello world"'` devuelve un resultado.

* Campos de `type` actualmente no son comparables entre sí, solo para fechas constantes.

### Tipos de valores

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de valor</th> 
   <th> <p> Notas</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Cadena </td> 
   <td> <p>Rodeado de comillas simples ". Omisión de comillas simples en consultas con <code>\'</code>, por ejemplo,<code> 'Valentine\'s Day'</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Booleano </td> 
   <td> <p><code>true </code>o <code>false</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Fecha </td> 
   <td> <p>Formato RFC 3339, la zona horaria predeterminada es UTC, por ejemplo, <code>2012-06-04T12:00:00-08:00</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Operadores

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Operador </th> 
   <th> <p>Notas</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>contains</code></td> 
   <td> <p>El contenido de una cadena está presente en la otra.</p> </td> 
  </tr> 
  <tr> 
   <td><code>=</code> </td> 
   <td> <p> El contenido de una cadena o booleano es igual al otro.</p> </td> 
  </tr> 
  <tr> 
   <td><code>!=</code> </td> 
   <td> <p> El contenido de una cadena o booleano no es igual al otro.</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;</code> </td> 
   <td> <p> Una fecha es anterior a otra.</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;=</code> </td> 
   <td> <p> Una fecha es anterior o igual a otra.</p> </td> 
  </tr> 
  <tr> 
   <td><code>></code> </td> 
   <td> <p> Una fecha es posterior a otra.</p> </td> 
  </tr> 
  <tr> 
   <td><code>>=</code> </td> 
   <td> <p> Una fecha es posterior o igual a otra.</p> </td> 
  </tr> 
  <tr> 
   <td><code>in </code> </td> 
   <td> <p>Un elemento está contenido en una colección.</p> </td> 
  </tr> 
  <tr> 
   <td><code>and </code> </td> 
   <td> <p>Devuelve archivos que coinciden con ambas cláusulas.</p> </td> 
  </tr> 
  <tr> 
   <td><code>or </code> </td> 
   <td> <p>Devuelve archivos que coinciden con cualquiera de las cláusulas.</p> </td> 
  </tr> 
  <tr> 
   <td><code>not </code> </td> 
   <td> <p>Anula una cláusula de búsqueda.</p> </td> 
  </tr> 
  <tr> 
   <td><code>has </code> </td> 
   <td> <p>Una colección contiene un elemento que coincide con los parámetros.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para las cláusulas compuestas, puede utilizar paréntesis para agrupar las cláusulas. Por ejemplo:
`modifiedDate > '2012-06-04T12:00:00' and (mimeType contains 'image/' or mimeType contains 'video/')` Esta búsqueda devuelve todos los archivos con un tipo MIME de imagen o vídeo que su última modificación fue posterior al 4 de junio de 2012. Porque `and` y `or` se evalúan de izquierda a derecha, sin paréntesis; el ejemplo anterior solo devolverá imágenes modificadas después del 4 de junio de 2012, pero devolverá todos los vídeos, incluso los anteriores al 4 de junio de 2012.

### Ejemplos

Todos los ejemplos de esta página muestran el sin codificar `<q>q</q>` , donde `title = 'hello'` se codifica como `title+%3d+%27hello%27`. Las bibliotecas de cliente gestionan esta codificación automáticamente.

* Buscar archivos con el nombre &quot;hello&quot;

   <pre>title = 'hello'</pre>
* Buscar carpetas utilizando el tipo MIME específico de la carpeta

   <pre>mimeType = 'application/vnd.google-apps.folder'</pre>
* Buscar archivos que no sean carpetas

   <pre>mimeType != 'application/vnd.google-apps.folder'</pre>
* Busque archivos con un nombre que contenga las palabras &quot;hello&quot; y &quot;goodbye&quot;

   <pre>el título contiene 'hello' y [!UICONTROL name] contiene 'goodbye'</pre>
* Buscar archivos con un nombre que no contenga la palabra &quot;hello&quot;

   <pre>no el título contiene 'hello'</pre>
* Buscar archivos que contengan la palabra &quot;hello&quot; en el contenido

   <pre>fullText contiene 'hello'</pre>
* Buscar archivos que no contengan la palabra &quot;hello&quot; en el contenido

   <pre>not fullText contains 'hello'</pre>
* Busque archivos que contengan la frase exacta &quot;hello world&quot; en el contenido

   <pre>fullText contiene '"hello world"'fullText contiene '"hello_world"'</pre>
* Busque archivos con una consulta que contenga el carácter &quot;\&quot; (por ejemplo, &quot;\autores&quot;)

   <pre>fullText contiene '\\authors'</pre>
* Busque archivos que pueda escribir el usuario &quot;test@example.org&quot;

   <pre>'test@example.org' en [!DNL writers]</pre>
* Buscar el ID `1234567` en el `parents` colección. Esto encuentra todos los archivos y carpetas ubicados directamente en la carpeta cuyo ID es `1234567`.

   <pre>"1234567" en [!UICONTROL padres]</pre>
* Buscar el ID de alias `appDataFolder` en el `parents` colección. Esto encuentra todos los archivos y carpetas ubicados directamente debajo de la variable [Carpeta de datos de aplicación](https://developers.google.com/drive/api/v2/appdata).

   <pre>"appDataFolder" en padres</pre>
* Busque archivos que puedan escribir los usuarios &quot;test@example.org&quot; y &quot;test2@example.org&quot;

   <pre>'test@example.org' en escritores y 'test2@example.org' en escritores</pre>
* Buscar archivos que contengan el texto &quot;importante&quot; que se encuentra en la papelera

   <pre>fullText contiene 'important' y trashed = true</pre>
* Buscar archivos modificados después del 4 de junio de 2012

   <pre>modifiedDate &gt; '2012-06-04T12:00:00' // la zona horaria predeterminada es UTC</pre><pre>modifiedDate &gt; '2012-06-04T12:00:00-08:00'</pre>
* Buscar archivos compartidos con el usuario autorizado con &quot;hello&quot; en el nombre

   <pre>sharedWithMe y el título contiene 'hello'</pre>
* Busque archivos con un [propiedad de archivo personalizado](https://developers.google.com/drive/api/v2/properties) named `additionalID` con el valor `8e8aceg2af2ge72e78`.

   <pre>properties tiene { key='additionalID' y value='8e8aceg2af2ge72e78' y visibility='PRIVATE' }</pre>

El origen de esta guía es [[!DNL Google Drive] documentación](https://developers.google.com/drive/api/v2/search-shareddrives).
