---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;agile-and-teams;user-management
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Google Team Drive
description: El [!DNL Adobe Workfront Fusion Google Team Drive] Los módulos de le permiten supervisar, cargar, actualizar, copiar, eliminar o recuperar archivos y crear carpetas en su [!DNL Google Shared] Conduce.
author: Becky
feature: Workfront Fusion
exl-id: 8b4c057f-bb98-44d1-9b71-cbeaa402a1c3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1306'
ht-degree: 0%

---

# [!DNL Google Team Drive] módulos

El [!DNL Adobe Workfront Fusion] [!DNL Google Team Drive] Los módulos de le permiten supervisar, cargar, actualizar, copiar, eliminar o recuperar archivos y crear carpetas en su [!DNL Google Shared Drive].

Para utilizar [!DNL Google Team Drive] con [!DNL Adobe Workfront Fusion], es necesario tener un [!DNL G Suite] cuenta. Si no dispone de uno, puede crear un [!DNL G Suite] cuenta en [[!DNL G Suite] sitio de registro](https://gsuite.google.com/signup/businessstarter/welcome).

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Google Team Drive], así como conectarlo a múltiples aplicaciones y servicios de terceros.

Si necesita instrucciones sobre cómo crear un escenario, consulte [Creación de un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
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

## Requisitos previos

Para usar [!DNL Google Team Drive] módulos, debe tener un [!DNL Google Team Drive].

## [!DNL Google Team Drive] módulos y sus campos

Al configurar [!DNL Google Team Drive] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, se añaden [!DNL Google Team Drive] Los campos pueden mostrarse, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Los campos del cuadro de diálogo del módulo que se muestran en **negrita** (en el [!DNL Workfront Fusion] escenario, **no** en este artículo de documentación) son obligatorios.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Déclencheur

#### [!UICONTROL Observar archivos]

Devuelve detalles del archivo cuando se agrega o modifica un nuevo archivo en la carpeta especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Google Team Drive] cuenta a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Cree una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unidad de equipo]</td> 
   <td> <p> Seleccione la unidad compartida que desee ver.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione la carpeta dentro de la unidad compartida.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Qué archivos observar]</td> 
   <td> <p> Seleccione el tipo de archivos que desea inspeccionar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Documents] archivos para formatear] </td> 
   <td> <p>Seleccione el formato en el que desea que aparezca el objeto visto [!DNL Google Documents] archivos convertidos en.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Sheets] archivos para formatear] </td> 
   <td> <p>Seleccione el formato en el que desea que aparezca el objeto visto [!DNL Google Sheets] archivos convertidos en.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Slides] archivos para formatear] </td> 
   <td> <p>Seleccione el formato en el que desea que aparezca el objeto visto [!DNL Google Slides] archivos convertidos en.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Drawings] archivos para formatear] </td> 
   <td> <p>Seleccione el formato en el que desea que aparezca el objeto visto [!DNL Google Drawings] archivos convertidos en.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p> Seleccione si desea supervisar la carpeta en busca de archivos nuevos y modificados o sólo en busca de archivos nuevos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de archivos descargados]</td> 
   <td> <p> Establecer el número máximo de archivos [!DNL Workfront Fusion] volverá durante un ciclo de ejecución.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Cargar un archivo]](#upload-a-file)
* [[!UICONTROL Actualizar un archivo]](#update-a-file)
* [[!UICONTROL Copiar un archivo]](#copy-a-file)
* [[!UICONTROL Eliminar un archivo]](#delete-a-file)
* [[!UICONTROL Mover un archivo a la papelera]](#move-a-file-to-trash)
* [[!UICONTROL Obtener un archivo]](#get-a-file)
* [[!UICONTROL Obtener una lista de archivos]](#get-a-file-list)
* [[!UICONTROL Crear una carpeta]](#create-a-folder)

#### [!UICONTROL Cargar un archivo]

Carga un archivo en la unidad compartida especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Google Team Drive] cuenta a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Cree una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unidad de equipo] </td> 
   <td> <p>Seleccione la unidad compartida en la que desea cargar un archivo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione la carpeta dentro de la unidad compartida.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Archivo de origen]</p> </td> 
   <td> <p>Especifique el archivo que desea cargar en la unidad compartida.</p> <p>Asigne el archivo que desee cargar desde el módulo anterior (por ejemplo, [!UICONTROL HTTP] &gt;[!UICONTROL Obtener un archivo] o [!UICONTROL Dropbox] &gt;[!UICONTROL Obtener un archivo)], o bien introduzca manualmente el nombre y los datos del archivo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Título]</td> 
   <td> <p> Escriba el título del archivo que se mostrará en la carpeta compartida.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir un archivo]</td> 
   <td> <p> Active esta opción para convertir el archivo al formato de Google correspondiente en la carpeta compartida.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar un archivo]

Permite cambiar el nombre o el contenido del archivo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Google Team Drive] cuenta a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Cree una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unidad de equipo]</td> 
   <td> <p> Seleccione la unidad compartida que contiene el archivo que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione la carpeta dentro de la unidad compartida.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de archivo]</td> 
   <td> <p> Introduzca (asigne) el ID del archivo que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Archivo de origen]</p> </td> 
   <td>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Título] </td> 
   <td> <p>Introduzca el nuevo título del archivo actualizado.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir un archivo]</td> 
   <td> <p> Active esta opción para convertir el archivo al correspondiente [!DNL Google] en la carpeta compartida.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copiar un archivo]

Copia un archivo especificado en la carpeta seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Google Team Drive] cuenta a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Cree una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unidad de equipo]</td> 
   <td> <p> Seleccione la unidad compartida que contiene el archivo que desea copiar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione la carpeta de destino en la que desea copiar el archivo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de archivo]</td> 
   <td> <p> Introduzca (asigne) el ID del archivo que desea copiar.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Nombre del archivo de copia]</p> </td> 
   <td> <p>Introduzca el nuevo nombre de archivo si desea que se cambie en la ubicación de destino.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un archivo]

Elimina un archivo especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Google Team Drive] cuenta a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Cree una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de archivo]</td> 
   <td> <p> Introduzca o asigne el ID del archivo que desea eliminar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mover un archivo a la papelera]

Mueve un archivo especificado a la papelera.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Google Team Drive] cuenta a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Cree una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de archivo]</td> 
   <td> <p> Introduzca o asigne el ID del archivo que desea mover a la papelera.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un archivo]

Recupera detalles acerca del archivo especificado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Google Team Drive] cuenta a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Cree una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Documents] archivos para formatear] </td> 
   <td> <p>Seleccione el formato en el que desee el [!DNL Google Documents] archivos convertidos en.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Sheets] archivos para formatear] </td> 
   <td> <p>Seleccione el formato en el que desee el [!DNL Google Sheets] archivos convertidos en.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Slides] archivos para formatear] </td> 
   <td> <p>Seleccione el formato en el que desee el [!DNL Google Slides] archivos convertidos en.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convertir [!DNL Google Drawings] archivos para formatear] </td> 
   <td> <p>Seleccione el formato en el que desee el [!DNL Google Drawings] archivos convertidos en.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de archivo]</td> 
   <td> <p> Introduzca o asigne el ID del archivo que desea recuperar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener una lista de archivos]

Recupera detalles de archivos o carpetas en función del término de búsqueda.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Google Team Drive] cuenta a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Cree una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unidad de equipo]</td> 
   <td> <p> Seleccione la unidad compartida desde la que desee enumerar los archivos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione la carpeta desde la que desee enumerar los archivos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Buscar] </td> 
   <td> <p>Seleccione el tipo de búsqueda que desea realizar (consulte a continuación).</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Consulta]</p> </td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>[!UICONTROL Buscar en nombres de archivo]</p> <p style="font-weight: normal;">Introduzca el nombre del archivo (incluida la extensión) cuando la opción [!UICONTROL Buscar término exacto] esté seleccionada o introduzca la parte del nombre cuando la opción [!UICONTROL Buscar nombres que contengan el término buscado] esté seleccionada.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Búsqueda de texto completo]</p> <p>Introduzca el término de búsqueda para buscar entre los nombres de archivo, las descripciones y el contenido.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Consulta de búsqueda personalizada]</p> <p>Introduzca el [!DNL Google] término de consulta de búsqueda. Para obtener más información, consulte [!DNL Google]de <a href="https://developers.google.com/drive/api/v2/ref-search-terms">Documentación de consulta de búsqueda</a>. Ejemplo: <code>fullText contains '"Hello world"'</code></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recuperar]</td> 
   <td>Seleccione si desea recuperar archivos, carpetas o ambos.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Número máximo de resultados devueltos]</td> 
   <td> <p> Establecer el número máximo de archivos o carpetas [!DNL Workfront Fusion] volverá durante un ciclo de ejecución.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear una carpeta]

Crea una nueva carpeta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Google Team Drive] cuenta a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Cree una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unidad de equipo]</td> 
   <td> <p> Seleccione la unidad compartida donde desea crear una carpeta.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Carpeta] </td> 
   <td> <p>Seleccione la carpeta en la que desea crear una carpeta.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL El nombre de la nueva carpeta]</td> 
   <td> <p> Introduzca el nombre de la nueva carpeta.</p> </td> 
  </tr> 
 </tbody> 
</table>
