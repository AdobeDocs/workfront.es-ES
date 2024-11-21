---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Google Drive
description: Los módulos  [!DNL Adobe Workfront Fusion Google Drive] le permiten supervisar, buscar, crear, actualizar, eliminar y administrar sus archivos, carpetas o unidades compartidas en su [!DNL Google Drive].
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d620c93-d1bf-4451-9f76-1d6fd850cec9
source-git-commit: 2e91e9a4c691430f3c98e3cbddb30706ea57f84a
workflow-type: tm+mt
source-wordcount: '2958'
ht-degree: 0%

---

# [!DNL Google Drive] módulos

Los módulos [!DNL Adobe Workfront Fusion] [!DNL Google Drive] le permiten supervisar, buscar, crear, actualizar, eliminar y administrar sus archivos, carpetas o unidades compartidas en su [!DNL Google Drive].

En un escenario de [!DNL Adobe Workfront Fusion], puede conectar su cuenta de [!DNL Google Drive] a varias aplicaciones y servicios de terceros.

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

## Información de API de Google Drive

El conector de Google Drive utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL básica</td> 
   <td> https://www.googleapis.com/drive/v3</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Versión de API</td> 
   <td> v3 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>v4.1.22</td> 
  </tr>
 </tbody> 
 </table>



## Conectando [!DNL Google Drive] a [!DNL Workfront Fusion]

Si es un usuario de [!DNL @gmail.com] o [!DNL @googlemail.com], debe crear un cliente de OAuth en [the [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) para obtener [!UICONTROL ID de cliente] y [!UICONTROL Secreto de cliente].

Para obtener instrucciones paso a paso sobre cómo crear el cliente OAuth (y obtener [!UICONTROL ID de cliente] y [!UICONTROL Secreto de cliente]), consulte [Conectarse [!DNL Adobe Workfront Fusion] a [!DNL Google Services] con un cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Para obtener instrucciones sobre cómo conectar tu cuenta de [!DNL Google Drive] a [!UICONTROL Workfront Fusion], consulta [Crear una conexión a [!UICONTROL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Google Drive] módulos y sus campos

Al configurar [!DNL Google Drive] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Google Drive] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)



* [Déclencheur](#triggers)
* [Acciones](#actions)

### Déclencheur

* [[!UICONTROL Ver Archivos En La Carpeta]](#watch-files-in-folder)
* [[!UICONTROL Ver todos los archivos]](#watch-all-files)
* [[!UICONTROL Ver archivos compartidos]](#watch-shared-files)
* [[!UICONTROL Observar comentarios]](#watch-comments)

#### [!UICONTROL Ver Archivos En La Carpeta]

Recupera detalles del archivo cuando se agrega o modifica un archivo en la carpeta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Conexión] </td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Drive] a [!DNL Workfront Fusion], vea <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Seleccione la carpeta que desea ver]</td>
    <td >Seleccione la carpeta de la unidad en la que desea inspeccionar los archivos.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL Qué archivos observar]</td>
   <td> <p>Seleccione el tipo de archivos que desea inspeccionar.</p> 
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
    <td>Seleccione el formato de archivo al que desea convertir [!DNL Google Documents].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir [!DNL Google Spreadsheets] archivos a formato]</td>
    <td>Seleccione el formato de archivo al que desea convertir [!DNL Google Spreadsheets].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir [!DNL Google Slides] archivos a formato]</td>
    <td>Seleccione el formato de archivo al que desea convertir [!DNL Google Slides].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir [!DNL Google Drawings] archivos a formato]</td>
    <td>Seleccione el formato de archivo al que desea convertir [!DNL Google Drawings].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Watch]</td>
    <td>Seleccione si desea inspeccionar los nuevos archivos y todos los cambios, o sólo los nuevos.</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL Número máximo de archivos descargados]</td>
    <td>Establezca el número máximo de resultados que [!DNL Workfront Fusion] descargará durante un ciclo (el número de repeticiones por ejecución de escenario).</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ver todos los archivos]

Recupera detalles del archivo cuando se agrega o modifica un archivo de su [!DNL Google Drive].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Drive] a [!DNL Workfront Fusion], vea <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Qué archivos observar]</td> 
   <td> <p>Seleccione el tipo de archivos que desea inspeccionar.</p> 
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
    <td>Seleccione el formato de archivo al que desea convertir [!DNL Google Documents].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir [!DNL Google Spreadsheets] archivos a formato]</td>
    <td>Seleccione el formato de archivo al que desea convertir [!DNL Google Spreadsheets].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir [!DNL Google Slides] archivos a formato]</td>
    <td>Seleccione el formato de archivo al que desea convertir [!DNL Google Slides].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir [!DNL Google Drawings] archivos a formato]</td>
    <td>Seleccione el formato de archivo al que desea convertir [!DNL Google Drawings].</td>
  </tr>  
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>Seleccione si desea inspeccionar los nuevos archivos y todos los cambios, o sólo los nuevos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de archivos descargados]</td> 
   <td>Establezca el número máximo de resultados que [!DNL Workfront Fusion] descargará durante un ciclo (el número de repeticiones por ejecución de escenario).</td> 
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
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Drive] a [!DNL Workfront Fusion], vea <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Seleccione la carpeta que desea ver]</td> 
   <td>Seleccione la carpeta compartida en la que desea inspeccionar los archivos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Qué archivos observar]</td> 
   <td> <p>Seleccione el tipo de archivos que desea inspeccionar.</p> 
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
    <td>Seleccione el formato de archivo al que desea convertir [!DNL Google Documents].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir [!DNL Google Spreadsheets] archivos a formato]</td>
    <td>Seleccione el formato de archivo al que desea convertir [!DNL Google Spreadsheets].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir [!DNL Google Slides] archivos a formato]</td>
    <td>Seleccione el formato de archivo al que desea convertir [!DNL Google Slides].</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convertir [!DNL Google Drawings] archivos a formato]</td>
    <td>Seleccione el formato de archivo al que desea convertir [!DNL Google Drawings].</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>Seleccione si desea inspeccionar los nuevos archivos y todos los cambios, o sólo los nuevos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de archivos descargados]</td> 
   <td>Establezca el número máximo de resultados que [!DNL Workfront Fusion] descargará durante un ciclo (el número de repeticiones por ejecución de escenario).</td> 
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
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Drive] a [!DNL Workfront Fusion], vea <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archivo]</td> 
   <td>Seleccione el archivo que desea inspeccionar en busca de comentarios.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>Seleccione si desea inspeccionar todos los cambios o sólo los comentarios nuevos</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de comentarios devueltos]</td> 
   <td>Establezca el número máximo de comentarios que [!DNL Workfront Fusion] devolverá durante un ciclo (el número de repeticiones por ejecución de escenario).</td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Cargar un archivo]](#upload-a-file)
* [[!UICONTROL Actualizar un archivo]](#update-a-file)
* [[!UICONTROL Copiar un archivo]](#copy-a-file)
* [[!UICONTROL Eliminar un archivo]](#delete-a-file)
* [[!UICONTROL Mover un archivo o carpeta a la papelera]](#move-a-filefolder-to-trash)
* [[!UICONTROL Obtener un archivo]](#get-a-file)
* [[!UICONTROL Buscar archivos/carpetas]](#search-for-filesfolders)
* [[!UICONTROL Crear una carpeta]](#create-a-folder)
* [[!UICONTROL Obtener un vínculo compartido]](#get-a-share-link)

#### [!UICONTROL Cargar un archivo]

Sube un archivo a su [!DNL Google Drive].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Drive] a [!DNL Workfront Fusion], vea <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Destination]</td> 
   <td> <p>Seleccione el destino en el que desea cargar un archivo.</p> 
    <ul> 
     <li>[!DNL My Drive]</li> 
     <li>[!DNL Shared with Me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta de destino]</td> 
   <td>Seleccione la carpeta en la que desea cargar un archivo. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL archivo Source]</td> 
   <td>Seleccione si desea utilizar un archivo transferido desde un módulo anterior o si desea asignar el archivo manualmente.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre de archivo]</td> 
   <td>Seleccione el nombre del archivo. Esta opción está disponible si selecciona "[!UICONTROL Map]" en el campo [!UICONTROL archivo de origen].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datos]</td> 
   <td>Seleccione el archivo de datos que desea cargar. Esta opción está disponible si selecciona "[!UICONTROL Map]" en el campo [!UICONTROL archivo de origen].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Título]</td> 
   <td>Escriba un título para el nuevo archivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir un archivo]</td> 
   <td>Al habilitar esta opción, el módulo podrá convertir archivos al formato [!DNL Google] correspondiente.</td> 
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
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Drive] a [!DNL Workfront Fusion], vea <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destino]</td> 
   <td> <p>Seleccione el destino en el que desea cargar un archivo.</p> 
    <ul> 
     <li>[!UICONTROL Mi unidad]</li> 
     <li>[!UICONTROL compartido conmigo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mover a una carpeta]</td> 
   <td>Si desea mover el archivo a una carpeta diferente, seleccione la carpeta en la que desea mover el archivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de archivo]</td> 
   <td>Asigne el ID del archivo que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Título]</td> 
   <td>Escriba un título para el archivo actualizado.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cambiar el contenido de un archivo]</td> 
   <td>Seleccione si desea reemplazar el contenido del archivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL archivo Source]</td> 
   <td>Seleccione si desea utilizar un archivo transferido desde un módulo anterior o si desea asignar el archivo manualmente. Este campo está disponible si ha seleccionado cambiar el contenido del archivo en el campo anterior.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nombre de archivo]</td> 
   <td>Seleccione el nombre del archivo. Esta opción está disponible si selecciona "[!UICONTROL Map]" en el campo [!UICONTROL archivo de origen].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datos]</td> 
   <td>Seleccione el archivo de datos que desea cargar. Esta opción está disponible si selecciona "[!UICONTROL Map]" en el campo [!UICONTROL archivo de origen].</td> 
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
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Drive] a [!DNL Workfront Fusion], vea <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destino]</td> 
   <td> <p>Seleccione el destino en el que desea cargar un archivo.</p> 
    <ul> 
     <li>[!UICONTROL Mi unidad]</li> 
     <li>[!UICONTROL compartido conmigo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta de destino]</td> 
   <td>Seleccione la carpeta donde se encuentra el archivo que desea copiar/</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de archivo]</td> 
   <td>Asigne el ID del archivo que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL El nombre de la copia]</td> 
   <td>Escriba un título para el nuevo archivo. Deje este campo en blanco si no desea cambiar el nombre del archivo original.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un archivo]

Elimina permanentemente un archivo o carpeta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Drive] a [!DNL Workfront Fusion], vea <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de archivo]</td> 
   <td>Asigne el ID del archivo que desea eliminar.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover un archivo o carpeta a la papelera]

Mueve un archivo o una carpeta a la papelera.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Drive] a [!DNL Workfront Fusion], vea <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de archivo]</td> 
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
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Drive] a [!DNL Workfront Fusion], vea <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Documents] archivos a formato]</td> 
   <td>Seleccione el formato de archivo al que desea convertir [!DNL Google Documents].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Spreadsheets] archivos a formato]</td> 
   <td>Seleccione el formato de archivo al que desea convertir [!DNL Google Spreadsheets].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Slides] archivos a formato]</td> 
   <td>Seleccione el formato de archivo al que desea convertir [!DNL Google Slides].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Drawings] archivos a formato]</td> 
   <td>Seleccione el formato de archivo al que desea convertir [!DNL Google Drawings].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de archivo]</td> 
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
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Drive] a [!DNL Workfront Fusion], vea <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destino]</td> 
   <td> <p>Seleccione el destino en el que desea buscar.</p> 
    <ul> 
     <li>[!UICONTROL Mi unidad]</li> 
     <li>[!UICONTROL compartido conmigo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mostrar una carpeta]</td> 
   <td>Desplácese hasta la carpeta en la que desee buscar los archivos o carpetas.</td> 
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
       <li> <p><strong>[!UICONTROL Consulta]</strong> </p> <p>Introduzca una parte del nombre de archivo o el nombre completo del archivo (incluido el sufijo) que desee buscar.</p> </li> 
       <li> <p><strong>[!UICONTROL Opciones de búsqueda]</strong> </p> <p>Seleccione si desea buscar el término exacto o si desea buscar nombres que contengan el término de búsqueda.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Texto completo] buscar</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Consulta]</strong> </p> <p>Escriba cualquier término de búsqueda que quiera buscar en su [!DNL Google Drive].</p> </li> 
      </ul> </li> 
     <li> <p><strong>Introducir consulta de búsqueda personalizada</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Consulta]</strong> </p> <p>Introduzca la consulta de búsqueda personalizada. Para obtener más información, consulte la sección [!UICONTROL Buscar archivos] de este artículo.</p> </li> 
       <li> <p><strong>Agregar la carpeta seleccionada arriba a la consulta</strong> </p> <p>Busca la carpeta en la colección primaria. Esto encuentra todos los archivos y carpetas ubicados directamente en la carpeta seleccionada anteriormente.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de resultados devueltos]</td> 
   <td>Establezca el número máximo de archivos o carpetas que devolverá [!DNL Workfront Fusion] durante un ciclo de ejecución.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continuar la ejecución de la ruta aunque el módulo no devuelva resultados]</td> 
   <td>Active esta opción para asegurarse de que el escenario no se detiene si el módulo no devuelve resultados.</td> 
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
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Drive] a [!DNL Workfront Fusion], vea <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destino]</td> 
   <td> <p>Seleccione el destino en el que desea cargar un archivo.</p> 
    <ul> 
     <li>[!UICONTROL Mi unidad]</li> 
     <li>[!UICONTROL compartido conmigo]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nueva ubicación de carpeta]</td> 
   <td>Vaya a la ubicación en la que desea crear una carpeta nueva.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL El nombre de la nueva carpeta]</td> 
   <td>Escriba un nombre para la carpeta que está creando.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Compartir carpeta]</td> 
   <td>Seleccione esta opción si desea compartir la carpeta con alguien que tenga el vínculo [!UICONTROL Compartir]. De lo contrario, el vínculo compartido solo es para el propietario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un vínculo compartido]

Recupera el vínculo compartido de un archivo en Google Drive.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Drive] a [!DNL Workfront Fusion], vea <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Google Drive] a [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de archivo]</td> 
   <td>Asigne el ID del archivo para el que desea obtener el vínculo compartido.</td> 
  </tr> 
 </tbody> 
</table>

## Resolución de problemas

### No se puede cargar o actualizar un archivo

Cuando falla la carga o actualización de un archivo, se dan varias situaciones:

* El archivo cargado es demasiado grande y supera el límite máximo de tamaño de archivo permitido para el plan [!DNL Google Drive] o ha excedido el límite de almacenamiento de [!DNL Google Drive]. Puede actualizar su plan de almacenamiento o eliminar los archivos existentes del servicio [!DNL Google Drive].
* La carpeta seleccionada en la que se iba a cargar el archivo ya no existe. El escenario se detiene y es necesario volver a seleccionar una carpeta de destino.

## Buscar archivos

En el módulo Mostrar archivos en una carpeta puede utilizar su propia consulta, que consta de estas partes:

* **[!UICONTROL Campo]** - Atributo del archivo que se está buscando, por ejemplo, el atributo `name` del archivo.

* **[!UICONTROL Operador]**: prueba que se realiza en los datos para proporcionar una coincidencia, por ejemplo, `contains`.

* **[!UICONTROL Valor]** - El contenido del atributo que se prueba, por ejemplo, el nombre del archivo `My cool document`.

Combine cláusulas con las conjunciones `and` o `or` y anule la consulta con `not`.

* [Campos](#fields)
* [Tipos de valor](#value-types)
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
   <td>cadena</td> 
   <td><code>contains</code><sup>1</sup>, <code>=</code>, <code>!=</code></td> 
   <td> <p> Nombre del archivo.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL fullText]</code> </td> 
   <td>cadena </td> 
   <td><code>contains</code><sup>2, 3</sup> </td> 
   <td> <p> Texto completo del archivo, incluido el nombre, la descripción, el contenido y el texto indexable.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL mimeType]</code> </td> 
   <td> cadena</td> 
   <td><code>contains</code>, <code>=</code>, <code>!=</code></td> 
   <td> <p> Tipo MIME del archivo.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL modifiedDate]</code> </td> 
   <td> fecha<sup>4</sup></td> 
   <td><code> &lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> Fecha de la última modificación del archivo.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL lastViewedByMeDate]</code> </td> 
   <td> fecha<sup>4</sup></td> 
   <td><code>&lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> Fecha en la que el usuario vio un archivo por última vez.</p> </td> 
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
   <td> <p>Si el archivo está marcado con estrellas o no.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL parents]</code></td> 
   <td>colección </td> 
   <td><code>in </code> </td> 
   <td> <p>Si la colección [!UICONTROL parent] contiene el identificador especificado.</p> </td> 
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
   <td> <p> Archivos que se encuentran en la colección "Compartido conmigo" del usuario.</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL properties] </code> </td> 
   <td>colección</td> 
   <td><code>has </code> </td> 
   <td> <p> Propiedades públicas del archivo personalizado.</p> </td> 
  </tr> 
 </tbody> 
</table>

Tenga en cuenta lo siguiente sobre los operadores en estos campos:

* El operador `contains` solo realiza la coincidencia de prefijos para `title`.

  Por ejemplo, el título &quot;HelloWorld&quot; coincide con `title contains 'Hello'` pero no con `title contains 'World'`.

* El operador `contains` solo realiza coincidencias en tokens de cadena completos para `fullText`.

  Por ejemplo, si el texto completo de un documento contiene la cadena &quot;HelloWorld&quot;, solo la consulta `fullText contains 'HelloWorld'` devuelve un resultado. Consultas como `fullText contains 'Hello'` no arrojarían resultados en este escenario.

* El operador `contains` coincide con una frase alfanumérica exacta si está entre comillas dobles.

  Por ejemplo, si el `fullText` de un documento contiene la cadena &quot;Hello there world&quot;, la consulta `fullText contains '"Hello there"'` devuelve un resultado, pero la consulta `fullText contains '"Hello world"'` no.

  Además, como la búsqueda es alfanumérica, si el `fullText` de un documento contiene la cadena &quot;Hello_world&quot;, la consulta `fullText contains '"Hello world"'` devuelve un resultado.

* Actualmente, los campos de fecha `type` no son comparables entre sí, solo con fechas constantes.

### Tipos de valor

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
   <td> <p>Rodear con comillas simples '. Omitir comillas simples en consultas con <code>\'</code>, p. ej.,<code> 'Valentine\'s Day'</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Booleano </td> 
   <td> <p><code>true </code>o <code>false</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Fecha </td> 
   <td> <p>formato RFC 3339, la zona horaria predeterminada es UTC; p. ej., <code>2012-06-04T12:00:00-08:00</code>.</p> </td> 
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
   <td> <p>Un elemento está contenido dentro de una colección.</p> </td> 
  </tr> 
  <tr> 
   <td><code>and </code> </td> 
   <td> <p>Devuelve archivos que coinciden con ambas cláusulas.</p> </td> 
  </tr> 
  <tr> 
   <td><code>or </code> </td> 
   <td> <p>Devolver archivos que coincidan con cualquiera de las cláusulas.</p> </td> 
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

En el caso de las cláusulas compuestas, puede utilizar paréntesis para agrupar cláusulas. Por ejemplo:
`modifiedDate > '2012-06-04T12:00:00' and (mimeType contains 'image/' or mimeType contains 'video/')` Esta búsqueda devuelve todos los archivos con un tipo MIME de imagen o vídeo cuya última modificación fue después del 4 de junio de 2012. Dado que los operadores `and` y `or` se evalúan de izquierda a derecha, sin paréntesis, el ejemplo anterior devuelve solamente las imágenes modificadas después del 4 de junio de 2012, pero devuelve todos los vídeos, incluso los anteriores al 4 de junio de 2012.

### Ejemplos

Todos los ejemplos de esta página muestran el parámetro sin codificar `<q>q</q>`, donde `title = 'hello'` está codificado como `title+%3d+%27hello%27`. Las bibliotecas de cliente gestionan esta codificación automáticamente.

* Buscar archivos con el nombre &quot;hello&quot;
  <pre>title = 'hello'</pre>
* Buscar carpetas utilizando el tipo MIME específico de la carpeta
  <pre>mimeType = 'application/vnd.google-apps.folder'</pre>
* Buscar archivos que no sean carpetas
  <pre>mimeType!= 'application/vnd.google-apps.folder'</pre>
* Busque archivos con un nombre que contenga las palabras &quot;hello&quot; y &quot;bye&quot;
  <pre>el título contiene 'hello' y [!UICONTROL name] contiene 'bye'</pre>
* Busque archivos con un nombre que no contenga la palabra &quot;hello&quot;
  <pre>no el título contiene 'hello'</pre>
* Busque archivos que contengan la palabra &quot;hello&quot; en el contenido
  <pre>fullText contiene 'hello'</pre>
* Busque archivos que no contengan la palabra &quot;hello&quot; en el contenido
  <pre>no fullText contiene 'hello'</pre>
* Busque archivos que contengan la frase exacta &quot;hello world&quot; en el contenido
  <pre>fullText contiene 'hello world''fullText contiene 'hello_world'</pre>
* Busque archivos con una consulta que contenga el carácter &quot;\&quot; (por ejemplo, &quot;\authors&quot;)
  <pre>fullText contiene '\\authors'</pre>
* Buscar archivos que pueda escribir el usuario `test@example.org`
  <pre>'test@example.org' en [!DNL writers]</pre>
* Busque el identificador `1234567` en la colección `parents`. Esto encuentra todos los archivos y carpetas ubicados directamente en la carpeta cuyo identificador es `1234567`.
  <pre>'1234567' en [!UICONTROL parent]</pre>
* Busque el ID de alias `appDataFolder` en la colección `parents`. Esto encuentra todos los archivos y carpetas ubicados directamente bajo la [carpeta de datos de la aplicación](https://developers.google.com/drive/api/v2/appdata).
  <pre>'appDataFolder' en elementos primarios</pre>
* Busque archivos que puedan escribir los usuarios `test@example.org` y `test2@example.org`
  <pre>'test@example.org' en escritores y 'test2@example.org' en escritores</pre>
* Busque archivos que contengan el texto &quot;importante&quot; y que se encuentren en la papelera
  <pre>fullText contiene 'important' y trashed = true</pre>
* Buscar archivos modificados después del 4 de junio de 2012
  <pre>modifiedDate &gt; '2012-06-04T12:00:00' // La zona horaria predeterminada es UTC</pre><pre>modifiedDate &gt; '2012-06-04T12:00:00-08:00'</pre>
* Busque archivos compartidos con el usuario autorizado con &quot;hello&quot; en el nombre
  <pre>sharedWithMe y el título contiene 'hello'</pre>
* Busque archivos con una [propiedad de archivo personalizada](https://developers.google.com/drive/api/v2/properties) denominada `additionalID` con el valor `8e8aceg2af2ge72e78`.
  <pre>properties tiene { key='additionalID' and value='8e8aceg2af2ge72e78' and visibility='PRIVATE' }</pre>

El Source de esta guía es [[!DNL Google Drive] documentation](https://developers.google.com/drive/api/v2/search-shareddrives).
