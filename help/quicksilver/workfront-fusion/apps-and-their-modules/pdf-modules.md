---
title: Servicios de Adobe PDF
description: Servicios de Adobe PDF
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: e0a5736b-dbdb-43c6-83ff-e88a5625a5bf
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3213'
ht-degree: 0%

---

# [!DNL Adobe PDF Services]

Con la variable [!DNL Adobe Workfront Fusion] [!DNL Adobe PDF Services], puede extraer datos de un archivo de PDF o generar un nuevo archivo de PDF a partir de los datos que proporcione. Además, puede convertir varios tipos de archivo a PDF o PDF a otros tipos de archivo. Los servicios de PDF también le permiten combinar, comprimir o leer metadatos de un archivo de PDF, así como controlar la protección con contraseña del archivo.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

Para obtener información sobre la API utilizada para los servicios de PDF, consulte [API de generación de documentos de Adobe](https://www.adobe.io/apis/documentcloud/dcsdk/doc-generation.html).

## Consideraciones al utilizar [!DNL Adobe PDF Services]

* [No necesita un [!DNL Adobe] account](#you-do-not-need-an-adobe-account)
* [[!DNL Workfront Fusion] no almacena sus archivos](#workfront-fusion-does-not-store-your-files)

### No necesita un [!DNL Adobe] account

Porque [!DNL Workfront Fusion] forma parte del [!DNL Adobe] grupo de productos, no necesita una [!DNL Adobe] para utilizar estas herramientas. Cada herramienta accede a [!DNL Adobe] funcionalidad de PDF sin utilizar una conexión.

Aunque [!DNL Workfront Fusion] no requiere un [!DNL Adobe] para utilizar los servicios de PDF, los módulos requieren una conexión. No hay credenciales involucradas en esta conexión y usted sólo proporciona un nombre para la conexión misma.

### [!DNL Workfront Fusion] no almacena sus archivos

La variable [!DNL Adobe PDF Services] puede leer, convertir o modificar sus archivos, pero ninguno de los dos [!DNL Adobe] nor [!DNL Workfront Fusion] almacene sus archivos o datos. Esto significa que:

* Usted mantiene el control sobre sus archivos, incluida su seguridad
* No es necesario que tenga un [!UICONTROL Adobe] cuenta de almacenamiento en la nube o de almacenamiento en la nube para utilizar los servicios de PDF.

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

## [!DNL Adobe PDF Services] módulos y sus campos

Al configurar [!DNL PDF Services], [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Junto con estos, podrían mostrarse campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. El título en negrita de un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Generar documento]](#generate-document)
* [[!UICONTROL Extraer texto/tabla]](#extract-text--table)
* [[!UICONTROL Combinación de archivos PDF]](#combine-pdf-files)
* [[!UICONTROL Comprimir archivos del PDF]](#compress-pdf-files)
* [[!UICONTROL Convertir documento a archivo PDF]](#convert-document-to-pdf-file)
* [[!UICONTROL Convertir HTML en archivo PDF]](#convert-html-to-pdf-file)
* [[!UICONTROL Convertir imagen en archivo PDF]](#convert-image-to-pdf-file)
* [[!UICONTROL Convertir PDF en documento]](#convert-pdf-to-document)
* [[!UICONTROL Convertir PDF en imagen]](#convert-pdf-to-image)
* [[!UICONTROL Vinculación de un archivo de PDF]](#linearize-a-pdf-file)
* [[!UICONTROL OCR para archivo de PDF]](#ocr-for-pdf-file)
* [[!UICONTROL Manipulación de página del PDF]](#pdf-page-manipulation)
* [[!UICONTROL Propiedades del archivo PDF]](#pdf-file-properties)
* [[!UICONTROL Archivo de PDF de Protect]](#protect-pdf-file)
* [[!UICONTROL Eliminación de la protección de un archivo PDF]](#remove-protection-of-a-pdf-file)

### [!UICONTROL Generar documento]

La variable [!UICONTROL Generar documento] es una forma eficaz de crear un PDF que contenga los datos que seleccione. Puede aplicarle formato utilizando un [!DNL Microsoft Word] o proporcionando datos en formato JSON.

Para obtener más información sobre [!UICONTROL [!DNL Adobe PDF Services] Generar documento] , consulte la [Descripción general de la generación de documentos](https://www.adobe.io/apis/documentcloud/dcsdk/docs.html) en el [!DNL Adobe Document Services] documentación.

* [Utilice la variable [!UICONTROL Generar documento] módulo con un [!DNL Microsoft Word] plantilla](#use-the-generate-document-module-with-a-microsoft-word-template)
* [Utilice la variable [!UICONTROL Generar documento] módulo con JSON](#use-the-generate-document-module-with-json)

#### Utilice la variable [!UICONTROL Generar documento] módulo con un [!DNL Microsoft Word] plantilla

<!--
>[!NOTE]
>
>For a discussion of Microsoft Word templates, see [Microsoft Word Template modules](../../workfront-fusion/apps-and-their-modules/microsoft-word-templates-modules.md). 
>
>You do not need to use Microsoft Word template modules to use a Microsoft Word template with the PDF Services Generate document module.
-->

Para usar la variable [!UICONTROL Generar documento] módulo con un [!UICONTROL Microsoft Word] plantilla, primero debe crear la plantilla. Para obtener instrucciones, busque &quot;Crear una plantilla&quot; en la [!DNL Microsoft Office] documentación.

Complete la variable [!UICONTROL Generar documento] campos de módulo como se indica a continuación:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Seleccione la conexión que desea utilizar para este módulo.</p> <p>No necesita un [!DNL Adobe] para crear una conexión de servicios de PDF. Para obtener más información, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">No necesita un [!DNL Adobe] account</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> <p>Este archivo de origen es el [!DNL Microsoft Word ]plantilla que utiliza el módulo para generar el nuevo PDF.</p> <p>Se recomienda crear un proyecto en [!DNL Workfront] para el [!DNL Microsoft Word] plantillas que utilice en [!DNL Workfront Fusion]. A continuación, puede usar la variable [!DNL Workfront] &gt; Módulo [!UICONTROL Descargar documento] para extraer la plantilla adecuada en el escenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de salida]</td> 
   <td> <p>Seleccione el formato del documento generado.</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data for merge]</td> 
   <td> <p>Para cada etiqueta de valor de la plantilla que desee reemplazar por texto, rellene lo siguiente:</p> 
    <ul> 
     <li> <p>[!UICONTROL Key]</p> <p>Introduzca una clave. En la plantilla, la clave es el texto que se muestra en la etiqueta value . Por ejemplo, si desea colocar texto en la etiqueta de valor <code>&#123;&#123;name&#125;&#125;</code>, introduzca <code>name </code>en el campo key .</p> </li> 
     <li> <p>Tipo de valor</p> <p>Seleccione si los datos del campo de valor son un valor, un objeto o una matriz de objetos.</p> </li> 
     <li> <p>[!UICONTROL Valor]</p> <p>Introduzca o asigne el texto que desea que aparezca en el documento generado en lugar de la etiqueta value .</p> </li> 
    </ul> <p> <img src="assets/generate-with-template-350x241.png" style="width: 350;height: 241;"> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Utilice la variable [!UICONTROL Generar documento] módulo con JSON

Para usar la variable [!UICONTROL Generar documento] con JSON, rellene los campos de la siguiente manera:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Seleccione la conexión que desea utilizar para este módulo.</p> <p>No necesita un [!DNL Adobe] para crear una conexión de servicios de PDF. Para obtener más información, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">No necesita un [!DNL Adobe] account</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de salida]</td> 
   <td> <p>Seleccione el formato del documento generado.</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data for merge]</td> 
   <td> <p>Para utilizar JSON en este módulo, debe habilitar la asignación en este campo.</p> <p>Introduzca o asigne el JSON desde el que desea generar el documento. </p> <p>Puede escribir JSON directamente en este campo o asignar la salida JSON de un módulo JSON.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Extraer texto/tabla]

Este módulo de acción permite extraer datos de un archivo PDF. El módulo genera elementos de texto individuales, como un párrafo o el texto en una sola celda de una tabla.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Seleccione la conexión que desea utilizar para este módulo.</p> <p>No necesita un [!DNL Adobe] para crear una conexión de servicios de PDF. Para obtener más información, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">No necesita un [!DNL Adobe] account</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elementos que deben extraerse como JSON]</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Texto]</p> </li> 
     <li> <p>[!UICONTROL Tablas]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Extraer cuadros delimitadores?]</td> 
   <td>Active esta opción para extraer datos sobre el cuadro delimitador del texto.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Incluir información de estilo para la salida?]</td> 
   <td>Active esta opción para añadir información de estilo al JSON de salida.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Combinación de archivos PDF]

Este módulo de acción toma varios archivos de PDF y los combina en un solo archivo de PDF. Por ejemplo, este módulo puede combinar todos los documentos en un [!UICONTROL Workfront] proyectar en un solo PDF una vez finalizado el proyecto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Seleccione la conexión que desea utilizar para este módulo.</p> <p>No necesita un [!DNL Adobe] para crear una conexión de servicios de PDF. Para obtener más información, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">No necesita un [!DNL Adobe] account</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Documents]</td> 
   <td> <p>Puede utilizar un módulo de agregador para recopilar documentos y combinarlos en un PDF, o puede agregar los documentos manualmente. </p> <p>Se recomienda utilizar un módulo [!UICONTROL Array Aggregator] para agregar resultados de un módulo anterior. Al utilizar un agregador, no es necesario conocer los nombres, ubicaciones o números de archivos que se van a combinar. Por lo tanto, el uso de un agregador es mucho más flexible y escalable que la introducción manual de los documentos que se van a combinar.</p> <p>Para utilizar el módulo de archivos [!UICONTROL Combinar PDF] con un agregador, debe habilitar la asignación en el campo [!UICONTROL Documentos]. </p> <p>En este ejemplo, el módulo [!UICONTROL Leer registros relacionados] identifica los documentos asociados a un proyecto y el módulo [!UICONTROL Descargar documentos] descarga cada uno de ellos. Todos los PDF se agregan a una matriz, que se pasa al módulo de archivos [!UICONTROL Combinar PDF].</p> <p> <img src="assets/combine-example-350x104.png" style="width: 350;height: 104;"> </p> <p>También puede introducir documentos manualmente.</p> <p>Para que cada documento se incluya en el PDF combinado:</p> 
    <ol> 
     <li value="1"> <p>Haga clic en [!UICONTROL Agregar un documento]</p> </li> 
     <li value="2"> <p>En el campo [!UICONTROL Source file], seleccione el módulo que envíe el documento que desea incluir o asigne el nombre y los datos del archivo de origen. </p> </li> 
     <li value="3"> <p>(Opcional) Si desea incluir solo determinadas páginas del archivo de origen, haga clic en cada intervalo de páginas que desee agregar <strong>[!UICONTROL Agregar elemento]</strong> en el campo [!UICONTROL Páginas] , introduzca la primera y la última página del rango de páginas que desea incluir y haga clic en <strong>[!UICONTROL Agregar]</strong>. Puede incluir más de un rango de páginas de un solo documento.</p> </li> 
     <li value="4"> <p>Haga clic en <strong>[!UICONTROL Agregar]</strong>. </p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Comprimir archivos del PDF]

Este módulo de acción toma un archivo PDF y lo comprime. Esto puede resultar útil para conservar el ancho de banda o la memoria.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Seleccione la conexión que desea utilizar para este módulo.</p> <p>No necesita un [!DNL Adobe] para crear una conexión de servicios de PDF. Para obtener más información, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">No necesita un [!DNL Adobe] account</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> <p>El archivo de origen debe tener el formato de PDF. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nivel de compresión]</td> 
   <td>Seleccione el nivel de compresión que desee utilizar.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convertir documento a archivo PDF]

Esta herramienta convierte un documento en un archivo PDF. El archivo de origen debe tener uno de los siguientes formatos de documento:

* DOC
* XLS
* PPT
* TXT
* RTF

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Seleccione la conexión que desea utilizar para este módulo.</p> <p>No necesita un [!DNL Adobe] para crear una conexión de servicios de PDF. Para obtener más información, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">No necesita un [!DNL Adobe] account</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> <p>El archivo de origen debe tener uno de los siguientes formatos:</p> 
    <ul> 
     <li> <p>DOC</p> </li> 
     <li> <p>XLS</p> </li> 
     <li> <p>PPT</p> </li> 
     <li> <p>TXT</p> </li> 
     <li> <p>RTF</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td> <p>Seleccione el idioma predeterminado para el documento de origen. Esto permite que el módulo seleccione una fuente adecuada si no se incluye la fuente en el archivo de origen.</p> <p>Seleccione entre los siguientes idiomas:</p> 
    <ul> 
     <li> <p>en-US (predeterminado): Inglés (Estados Unidos de América)</p> </li> 
     <li> <p>ca-ES: Catalán (España)</p> </li> 
     <li> <p>cs-CZ: Checo (República Checa)</p> </li> 
     <li> <p>da-DK: Danés (Dinamarca)</p> </li> 
     <li> <p>de-DE: Alemán (Alemania)</p> </li> 
     <li> <p>en-AE: Inglés (Emiratos Árabes Unidos)</p> </li> 
     <li> <p>en-GB: Inglés (Reino Unido)</p> </li> 
     <li> <p>en-IL: Inglés (Israel)</p> </li> 
     <li> <p>en-US: Inglés (Estados Unidos de América)</p> </li> 
     <li> <p>es-ES: Español (España)</p> </li> 
     <li> <p>es-MX: Español (México)</p> </li> 
     <li> <p>ue-ES: Vasco (España)</p> </li> 
     <li> <p>fi-FI: Finés (Finlandia)</p> </li> 
     <li> <p>fr-CA: Francés (Canadá)</p> </li> 
     <li> <p>fr-FR: Francés (Francia)</p> </li> 
     <li> <p>fr-MA: Francés (Marruecos)</p> </li> 
     <li> <p>hr-HR: Croata (Croacia)</p> </li> 
     <li> <p>hu-HU: Húngaro (Hungría)</p> </li> 
     <li> <p>IT: Italiano (Italia)</p> </li> 
     <li> <p>ja-JP: Japonés (Japón)</p> </li> 
     <li> <p>kr-KR: Coreano (Corea del Sur)</p> </li> 
     <li> <p>nb-NO: Noruego Bokmål (Noruega)</p> </li> 
     <li> <p>nl-NL: Holandés (Países Bajos)</p> </li> 
     <li> <p>pl-PL: Polaco (Polonia)</p> </li> 
     <li> <p>pt-BR: Portugués (Brasil)</p> </li> 
     <li> <p>pt-PT: Portugués (Portugal)</p> </li> 
     <li> <p>RO: Rumano (Rumania)</p> </li> 
     <li> <p>ru-RU: Ruso (Rusia)</p> </li> 
     <li> <p>sk-SK: Eslovaco (Eslovaquia)</p> </li> 
     <li> <p>sl-SI: Esloveno (Eslovenia)</p> </li> 
     <li> <p>sv-SE: Sueco (Suecia)</p> </li> 
     <li> <p>tr-TR: Turco (Turquía)</p> </li> 
     <li> <p>uk-UA: Ucraniano (Ucrania)</p> </li> 
     <li> <p>zh-CN: Chino (China continental)</p> </li> 
     <li> <p>zh-TW: Chino (Taiwán)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convertir HTML en archivo PDF]

Esta herramienta convierte un archivo HTML en un archivo PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Seleccione la conexión que desea utilizar para este módulo.</p> <p>No necesita un [!DNL Adobe] para crear una conexión de servicios de PDF. Para obtener más información, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">No necesita un [!DNL Adobe] account</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> <p>Importante: El archivo de origen debe tener el formato HTML o ZIP. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON]</td> 
   <td> <p>Si el HTML hace referencia a variables JavaScript, puede incluir estas variables aquí. </p> <p>Para cada variable, haga clic en <strong>[!UICONTROL Agregar elemento]</strong> e incluya la clave y el valor de la variable.</p> <p>Nota:   
     <ul> 
      <li> <p>Al crear un PDF desde un archivo ZIP, el material colateral de origen debe incluir un elemento de secuencia de comandos como: <code> &lt;script src='./json.js' type='text/javascript'&gt;&lt;/script&gt;</code> </p> </li> 
      <li> <p>Al crear un PDF a partir de una URL, el contenido de este objeto JSON se inserta en la VM del explorador antes de que se procese la página. </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Incluir encabezado y pie de página]</td> 
   <td> <p>Active esta opción para crear encabezados y pies de página para el documento del PDF.</p> 
    <ul> 
     <li> <p>El encabezado incluye una fecha y el título del documento.</p> </li> 
     <li> <p>El pie de página incluye el nombre del archivo y un número de página.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ancho de página]</td> 
   <td>Introduzca la anchura del papel, en pulgadas. El módulo utiliza esta información para dar formato a las páginas del archivo PDF creado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Altura de la página]</td> 
   <td>Introduzca la altura del papel, en pulgadas. El módulo utiliza esta información para dar formato a las páginas del archivo PDF creado.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convertir imagen en archivo PDF]

Esta herramienta convierte una imagen en un archivo PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Seleccione la conexión que desea utilizar para este módulo.</p> <p>No necesita un [!DNL Adobe] para crear una conexión de servicios de PDF. Para obtener más información, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">No necesita un [!DNL Adobe] account</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y el archivo de imagen del archivo de origen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convertir PDF en documento]

Esta herramienta convierte un archivo PDF en un documento. Puede seleccionar uno de los siguientes formatos para el archivo de salida.

* DOC
* DOCX
* PPTX
* XLSX
* RTF

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Seleccione la conexión que desea utilizar para este módulo.</p> <p>No necesita un [!DNL Adobe] para crear una conexión de servicios de PDF. Para obtener más información, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">No necesita un [!DNL Adobe] account</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> <p>El archivo de origen debe tener el formato de PDF. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de archivos de salida]</td> 
   <td> <p>Seleccione el formato en el que desea que se muestren los archivos:</p> 
    <ul> 
     <li> <p>DOC</p> </li> 
     <li> <p>DOCX</p> </li> 
     <li> <p>PPTX</p> </li> 
     <li> <p>XLSX</p> </li> 
     <li> <p>RTF</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convertir PDF en imagen]

Esta herramienta convierte un PDF en una imagen en formato PNG o JPEG, que luego se genera como ZIP. El PDF se convierte en una imagen por página y cada imagen termina con el número de página. A continuación, los archivos de imagen se combinan en un archivo ZIP.

Por ejemplo, un archivo llamado &quot;TestFile&quot; con 8 páginas produciría 8 imágenes con el nombre &quot;TestFile_1&quot; hasta &quot;TestFile_8&quot;. La salida del módulo es un archivo ZIP que contiene las 8 imágenes.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Seleccione la conexión que desea utilizar para este módulo.</p> <p>No necesita un [!DNL Adobe] para crear una conexión de servicios de PDF. Para obtener más información, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">No necesita un [!DNL Adobe] account</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> <p>El archivo de origen debe tener el formato de PDF. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de archivos de salida]</td> 
   <td> <p>Seleccione el formato en el que desea que se muestren los archivos:</p> 
    <ul> 
     <li>PNG</li> 
     <li>JPEG</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Vinculación de un archivo de PDF]

Esta herramienta linealiza un documento de PDF para crear un documento de PDF optimizado para la web. Un documento PDF linealizado puede verse página por página sin necesidad de descargar todo el documento.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Seleccione la conexión que desea utilizar para este módulo.</p> <p>No necesita un [!DNL Adobe] para crear una conexión de servicios de PDF. Para obtener más información, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">No necesita un [!DNL Adobe] account</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL OCR para archivo de PDF]

Esta herramienta realiza el reconocimiento óptico de caracteres (OCR) en un archivo y produce un PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Seleccione la conexión que desea utilizar para este módulo.</p> <p>No necesita un [!DNL Adobe] para crear una conexión de servicios de PDF. Para obtener más información, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">No necesita un [!DNL Adobe] account</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo OCR]</td> 
   <td> 
    <ul> 
     <li> <p>El tipo de [!UICONTROL Imagen original modificada] garantiza que el texto se pueda buscar y seleccionar, pero modifica la imagen original durante el proceso de limpieza (por ejemplo, la muestra a su escritorio) antes de colocar una capa de texto invisible sobre ella. Este tipo elimina los artefactos no deseados y puede resultar en un documento más legible en algunos casos. </p> </li> 
     <li> <p>El tipo [!UICONTROL Imagen original sin cambiar] también superpone una capa de texto con capacidad de búsqueda sobre la imagen original, pero en este caso, la imagen original no cambia. Este tipo produce la máxima fidelidad a la imagen original.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td>Seleccione el idioma de este documento.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Manipulación de página del PDF]

Este módulo le permite rotar o eliminar páginas de forma selectiva en un documento de PDF. Por ejemplo, puede cambiar la vista vertical a la vista horizontal o eliminar ciertas páginas del documento del PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Seleccione la conexión que desea utilizar para este módulo.</p> <p>No necesita un [!DNL Adobe] para crear una conexión de servicios de PDF. Para obtener más información, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">No necesita un [!DNL Adobe] account</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td> <p>Seleccione la acción que desee realizar en el archivo.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Eliminar]</b> </p> <p>Seleccione esta opción para eliminar páginas del documento.</p> </li> 
     <li> <p><b>[!UICONTROL Rotar]</b> </p> <p>Seleccione esta opción para girar las páginas e introduzca el ángulo, en grados en el sentido de las agujas del reloj, que desea rotar las páginas del documento en relación con su orientación inicial.</p> <p>Para girar de vertical a horizontal o viceversa, gire la página 90 o 270 grados.</p> <p>Si una página está al revés, gírela 180 grados.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Páginas]</td> 
   <td> <p>Para cada intervalo de páginas que desee eliminar, haga clic en <strong>[!UICONTROL Agregar]</strong> y, a continuación, introduzca la primera y la última página del intervalo de páginas. </p> <p>Nota:   
     <ul> 
      <li> <p>Puede utilizar números negativos para contar desde el final del documento. La última página de un documento es -1, la segunda página es -2, etc.</p> </li> 
      <li> <p>Para eliminar una sola página, defina el mismo número de página que el inicio y el final del intervalo.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros con los que desea que funcione el módulo durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Propiedades del archivo PDF]

Esta herramienta extrae información básica sobre el documento, como:

* Recuento de páginas
* versión del PDF
* Si el archivo está cifrado
* Si el archivo está linearizado
* Si el archivo contiene archivos incrustados

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Seleccione la conexión que desea utilizar para este módulo.</p> <p>No necesita un [!DNL Adobe] para crear una conexión de servicios de PDF. Para obtener más información, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">No necesita un [!DNL Adobe] account</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Archivo de PDF de Protect]

Esta herramienta asegura un documento PDF con una contraseña de usuario o de propietario. También establece restricciones sobre determinadas funciones, como imprimir, editar y copiar en el documento del PDF. Seleccione el tipo de contenido que desea codificar y el algoritmo de codificación.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Seleccione la conexión que desea utilizar para este módulo.</p> <p>No necesita un [!DNL Adobe] para crear una conexión de servicios de PDF. Para obtener más información, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">No necesita un [!DNL Adobe] account</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> <p>El archivo de origen debe tener el formato de PDF. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de protección de contraseña]</td> 
   <td> <p>Active esta opción para utilizar contraseñas para cifrar el documento del PDF de entrada. Si activa esta opción, debe especificar e introducir un valor para una de las siguientes opciones o ambas: </p> 
    <ul> 
     <li> <p>[!UICONTROL userPassword]</p> </li> 
     <li> <p>[!UICONTROL ownerPassword] </p> </li> 
    </ul> <p>Cada contraseña puede tener hasta 128 caracteres de longitud.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Algoritmo de codificación]</td> 
   <td> <p>Seleccione el algoritmo de codificación. </p> 
    <ul> 
     <li> <p>[!UICONTROL AES-128 encryption]</p> <p>La contraseña solo admite caracteres LATIN-I. </p> </li> 
     <li> <p>[!UICONTROL AES-256 encryption]</p> <p>La contraseña admite el conjunto de caracteres Unicode</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenido que codificar]</td> 
   <td> <p>Seleccione el tipo de contenido que desea codificar.</p> 
    <ul> 
     <li> <p>[!UICONTROL Todo el contenido]</p> </li> 
     <li> <p>[!UICONTROL Todo el contenido excepto los metadatos]</p> </li> 
     <li> <p>[!UICONTROL Solo datos incrustados] </p> </li> 
    </ul> <p>Al seleccionar "[!UICONTROL Solo datos incrustados]", los permisos de acceso proporcionados se vuelven ineficaces.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Permisos]</td> 
   <td> <p>Seleccione los permisos que desee incluir para permitir la impresión, edición o copia de contenido.</p> <p>La configuración de permisos solo se utiliza si [!UICONTROL ownerPassword] está establecido en el campo [!UICONTROL Password Protection Type].</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eliminación de la protección de un archivo PDF]

Esta herramienta elimina la seguridad (protección con contraseña) de un documento de PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Seleccione la conexión que desea utilizar para este módulo.</p> <p>No necesita un [!DNL Adobe] para crear una conexión de servicios de PDF. Para obtener más información, consulte <a href="#you-do-not-need-an-adobe-account" class="MCXref xref">No necesita un [!DNL Adobe] account</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> <p>El archivo de origen debe tener el formato de PDF.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contraseña]</td> 
   <td>Introduzca la contraseña que protege actualmente el archivo.</td> 
  </tr> 
 </tbody> 
</table>
