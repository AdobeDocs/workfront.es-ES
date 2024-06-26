---
title: Servicios de Adobe PDF
description: Servicios de Adobe PDF
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: e0a5736b-dbdb-43c6-83ff-e88a5625a5bf
source-git-commit: ba161761acfc57e271f8593f534a5f7510187559
workflow-type: tm+mt
source-wordcount: '3719'
ht-degree: 0%

---

# [!DNL Adobe PDF Services]

Con el [!DNL Adobe Workfront Fusion] [!DNL Adobe PDF Services], puede extraer datos de un archivo de PDF o generar un nuevo archivo de PDF a partir de los datos proporcionados. Además, puede convertir distintos tipos de archivo en PDF o PDF en otros tipos de archivo. Los servicios de PDF también permiten combinar, comprimir o leer metadatos de un archivo de PDF, así como controlar la protección con contraseña del archivo.

Si necesita instrucciones sobre cómo crear un escenario, consulte [Creación de un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

Para obtener información sobre la API utilizada para los servicios de PDF, consulte [API de generación de documentos de Adobe](https://www.adobe.io/apis/documentcloud/dcsdk/doc-generation.html).

## Consideraciones de seguridad al utilizar [!DNL Adobe PDF Services]

<!--

* [You do not need an [!DNL Adobe] account](#you-do-not-need-an-adobe-account) 
* [[!DNL Workfront Fusion] does not store your files](#workfront-fusion-does-not-store-your-files)

### You do not need an [!DNL Adobe] account 

Because [!DNL Workfront Fusion] is part of the [!DNL Adobe] product suite, you don't need a separate [!DNL Adobe] account to use these tools. Each tool accesses [!DNL Adobe] PDF functionality without using a connection.

Although [!DNL Workfront Fusion] does not require an [!DNL Adobe] account to use the PDF Services, the modules do require a connection. There are no credentials involved in this connection, and you provide only a name for the connection itself.

### [!DNL Workfront Fusion] does not store your files 

-->

El [!DNL Adobe PDF Services] puede leer, convertir o modificar sus archivos, pero ninguno de los dos [!DNL Adobe] ni [!DNL Workfront Fusion] almacene sus archivos o datos. Esto significa lo siguiente:

* Usted mantiene el control sobre sus archivos, incluyendo su seguridad
* No es necesario que tenga un [!UICONTROL Adobe] Cuenta de almacenamiento o almacenamiento en la nube para utilizar los servicios de PDF.

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

Para crear un servidor a servidor OAuth, debe agregar la API de servicios de Adobe PDF a la consola de desarrolladores de Adobe. Al agregar la API, seleccione la opción Servidor a servidor OAuth.

Para obtener instrucciones, consulte [Agregar una API al proyecto mediante OAuth](https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/) En la documentación para desarrolladores de Adobe.

## Cree una conexión con [!DNL Adobe PDF Services]

Para crear una conexión para su [!DNL Adobe PDF Services] módulos:

1. En cualquier [!DNL Adobe PDF Services] , haga clic en **[!UICONTROL Añadir]** situado junto al cuadro Conexión.

1. Rellene los campos siguientes:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Tipo de conexión]</td>
          <td>
            <p>Seleccione si desea crear una conexión servidor a servidor o una conexión JWT.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Nombre de conexión]</td>
          <td>
            <p>Escriba un nombre para esta conexión.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID de cliente]</td>
          <td>Introduzca su [!DNL Adobe] [!UICONTROL ID de cliente]. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].<p>Para obtener instrucciones sobre cómo localizar las credenciales, consulte <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Credenciales</a> en la documentación para desarrolladores de Adobe.</p></td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Secreto de cliente]</td>
          <td>Introduzca su [!DNL Adobe] [!UICONTROL Secreto de cliente]. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].<p>Para obtener instrucciones sobre cómo localizar las credenciales, consulte <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Credenciales</a> en la documentación para desarrolladores de Adobe.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID de cuenta técnica] (solo JWT)</td>
          <td>Introduzca su [!DNL Adobe] [!UICONTROL ID de cuenta técnica]. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].<p>Para obtener instrucciones sobre cómo localizar las credenciales, consulte <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Credenciales</a> en la documentación para desarrolladores de Adobe.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Organization ID] (solo JWT)</td>
          <td>Introduzca su [!DNL Adobe] [!UICONTROL ID de organización]. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].<p>Para obtener instrucciones sobre cómo localizar las credenciales, consulte <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >Credenciales</a> en la documentación para desarrolladores de Adobe.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL MetaÁmbitos] (solo JWT)</td>
          <td>
            Escriba los metaámbitos necesarios para la conexión.
          </td>
        </tr>
       </tbody>
    </table>
1. Clic **[!UICONTROL Continuar]** para guardar la conexión y volver al módulo.


## [!DNL Adobe PDF Services] módulos y sus campos

Al configurar [!DNL PDF Services], [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, pueden mostrarse campos adicionales en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Generar documento]](#generate-document)
* [[!UICONTROL Extraer texto/tabla]](#extract-text--table)
* [[!UICONTROL Combinación de archivos de PDF]](#combine-pdf-files)
* [[!UICONTROL Comprimir archivos del PDF]](#compress-pdf-files)
* [[!UICONTROL Convertir documento en archivo PDF]](#convert-document-to-pdf-file)
* [[!UICONTROL Convertir HTML en archivo de PDF]](#convert-html-to-pdf-file)
* [[!UICONTROL Convertir imagen a archivo de PDF]](#convert-image-to-pdf-file)
* [[!UICONTROL Convertir PDF en documento]](#convert-pdf-to-document)
* [[!UICONTROL Convertir PDF en imagen]](#convert-pdf-to-image)
* [[!UICONTROL Linealización de un archivo de PDF]](#linearize-a-pdf-file)
* [[!UICONTROL OCR para archivo de PDF]](#ocr-for-pdf-file)
* [[!UICONTROL Manipulación de páginas]](#page-manipulation)
* [[!UICONTROL Etiquetado automático de accesibilidad de PDF]](#pdf-accessibility-auto-tag)
* [[!UICONTROL Propiedades del archivo del PDF]](#pdf-file-properties)
* [[!UICONTROL Archivo de PDF de Protect]](#protect-pdf-file)
* [[!UICONTROL Eliminación de la protección de un archivo de PDF]](#remove-protection-of-a-pdf-file)
* [División de un archivo de PDF](#split-a-pdf-file)

### [!UICONTROL Generar documento]

El [!UICONTROL Generar documento] El módulo es una forma eficaz de crear un PDF que contenga los datos seleccionados. Puede aplicarle formato mediante una [!DNL Microsoft Word] o proporcionando datos en formato JSON.

Para obtener más información sobre [!UICONTROL [!DNL Adobe PDF Services] Generar documento] funcionalidad, consulte la [Información general sobre la generación de documentos](https://www.adobe.io/apis/documentcloud/dcsdk/docs.html) en el [!DNL Adobe Document Services] documentación.

* [Utilice el [!UICONTROL Generar documento] módulo con un [!DNL Microsoft Word] plantilla](#use-the-generate-document-module-with-a-microsoft-word-template)
* [Utilice el [!UICONTROL Generar documento] módulo con JSON](#use-the-generate-document-module-with-json)

#### Utilice el [!UICONTROL Generar documento] módulo con un [!DNL Microsoft Word] plantilla

<!--
>[!NOTE]
>
>For a discussion of Microsoft Word templates, see [Microsoft Word Template modules](../../workfront-fusion/apps-and-their-modules/microsoft-word-templates-modules.md). 
>
>You do not need to use Microsoft Word template modules to use a Microsoft Word template with the PDF Services Generate document module.
-->

Para usar la variable [!UICONTROL Generar documento] módulo con un [!UICONTROL Microsoft Word] plantilla, primero debe crear la plantilla. Para obtener instrucciones, busque &quot;Crear una plantilla&quot; en la [!DNL Microsoft Office] documentación.

Rellene el [!UICONTROL Generar documento] Campos de módulo de la siguiente manera:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Seleccione la conexión que se utilizará para este módulo.</p> Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe PDF Services], consulte <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Cree una conexión con [!DNL Adobe PDF Services]</a> en este artículo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> <p>Este archivo de origen es el [!DNL Microsoft Word ]plantilla que utiliza el módulo para generar el nuevo PDF.</p> <p>Se recomienda crear un proyecto en [!DNL Workfront] para el [!DNL Microsoft Word] plantillas que utiliza en [!DNL Workfront Fusion]. A continuación, puede utilizar la variable [!DNL Workfront] &gt; Módulo [!UICONTROL Descargar documento] para extraer la plantilla adecuada a su escenario.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Datos para combinar]</td> 
   <td> <p>Para cada etiqueta de valor de la plantilla que desee reemplazar con texto, rellene el siguiente cuadro:</p> 
    <ul> 
     <li> <p>[!UICONTROL Key]</p> <p>Introduzca una clave. En la plantilla, la clave es el texto que se muestra en la etiqueta de valor. Por ejemplo, si desea colocar texto en la etiqueta de valor <code>&#123;&#123;name&#125;&#125;</code>, introduzca <code>name </code>en el campo clave.</p> </li> 
     <li> <p>Tipo de valor</p> <p>Seleccione si los datos del campo de valor son un valor, un objeto o una matriz de objetos.</p> </li> 
     <li> <p>[!UICONTROL Valor]</p> <p>Introduzca o asigne el texto que desea que aparezca en el documento generado en lugar de la etiqueta de valor.</p> </li> 
    </ul> <p> <img src="assets/generate-with-template-350x241.png" style="width: 350;height: 241;"> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Utilice el [!UICONTROL Generar documento] módulo con JSON

Para usar la variable [!UICONTROL Generar documento] con JSON, rellene los campos de la siguiente manera:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Seleccione la conexión que se utilizará para este módulo.</p> Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe PDF Services], consulte <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Cree una conexión con [!DNL Adobe PDF Services]</a> en este artículo. </td> 
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
   <td role="rowheader">[!UICONTROL Datos para combinar]</td> 
   <td> <p>Para utilizar JSON en este módulo, debe habilitar la asignación en este campo.</p> <p>Introduzca o asigne el JSON desde el que generar el documento. </p> <p>Puede escribir JSON directamente en este campo o asignar la salida JSON desde un módulo JSON.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Extraer texto/tabla]

Este módulo de acción le permite extraer datos de un archivo de PDF. El módulo genera elementos de texto individuales, como un párrafo o el texto en una sola celda de una tabla.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Seleccione la conexión que se utilizará para este módulo.</p> Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe PDF Services], consulte <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Cree una conexión con [!DNL Adobe PDF Services]</a> en este artículo. </td> 
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
   <td role="rowheader">[!UICONTROL ¿Desea incluir información de estilo para la salida?]</td> 
   <td>Active esta opción para añadir información de estilo al JSON de salida.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Combinación de archivos de PDF]

Este módulo de acción toma varios archivos de PDF y los combina en un solo archivo de PDF. Por ejemplo, este módulo podría combinar todos los documentos de una [!UICONTROL Workfront] proyecto en un único PDF al finalizar el proyecto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Seleccione la conexión que se utilizará para este módulo.</p> Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe PDF Services], consulte <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Cree una conexión con [!DNL Adobe PDF Services]</a> en este artículo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Documentos]</td> 
   <td> <p>Puede utilizar un módulo de acumulador para recopilar documentos para combinarlos en un PDF o puede agregar los documentos manualmente. </p> <p>Se recomienda utilizar un módulo [!UICONTROL Array Aggregator] para agregar los resultados de un módulo anterior. Al utilizar un agregador, no es necesario conocer los nombres, ubicaciones o números de archivos que se van a combinar. Por lo tanto, el uso de un agregador es mucho más flexible y escalable que la introducción manual de los documentos que se van a combinar.</p> <p>Para utilizar el módulo de archivos de [!UICONTROL Combine PDF] con un agregador, debe habilitar la asignación en el campo [!UICONTROL Documents]. </p> <p>En este ejemplo, el módulo [!UICONTROL Leer registros relacionados] identifica los documentos asociados a un proyecto y el módulo [!UICONTROL Descargar documentos] descarga cada uno de ellos. Todos los PDF se agregan en una matriz, que se pasa al módulo de archivos de [!UICONTROL Combinar PDF].</p> <p> <img src="assets/combine-example-350x104.png" style="width: 350;height: 104;"> </p> <p>También puede introducir documentos manualmente.</p> <p>Para que cada documento incluya en el PDF combinado:</p> 
    <ol> 
     <li value="1"> <p>Haga clic en [!UICONTROL Agregar documento]</p> </li> 
     <li value="2"> <p>En el campo [!UICONTROL Archivo de origen], seleccione el módulo que genera el documento que desea incluir o asigne el nombre y los datos del archivo de origen. </p> </li> 
     <li value="3"> <p>(Opcional) Si desea incluir solo determinadas páginas del archivo de origen, haga clic en para cada intervalo de páginas que desee agregar <strong>[!UICONTROL Agregar elemento]</strong> en el campo [!UICONTROL Pages], introduzca la primera y la última página del intervalo de páginas que desea incluir y haga clic en <strong>[!UICONTROL Agregar]</strong>. Puede incluir más de un intervalo de páginas de un solo documento.</p> </li> 
     <li value="4"> <p>Clic <strong>[!UICONTROL Agregar]</strong>. </p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Comprimir archivos del PDF]

Este módulo de acción toma un archivo de PDF y lo comprime. Esto puede resultar útil para conservar ancho de banda o memoria.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Seleccione la conexión que se utilizará para este módulo.</p> Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe PDF Services], consulte <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Cree una conexión con [!DNL Adobe PDF Services]</a> en este artículo. </td> 
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

### [!UICONTROL Convertir documento en archivo PDF]

Esta herramienta convierte un documento en un archivo de PDF. El archivo de origen debe tener uno de los siguientes formatos de documento:

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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Seleccione la conexión que se utilizará para este módulo.</p> Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe PDF Services], consulte <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Cree una conexión con [!DNL Adobe PDF Services]</a> en este artículo. </td> 
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
   <td role="rowheader">[!UICONTROL Idioma]</td> 
   <td> <p>Seleccione el idioma predeterminado para el documento de origen. Esto permite al módulo seleccionar una fuente adecuada, si no se incluye en el archivo de origen.</p> <p>Seleccione entre los siguientes idiomas:</p> 
    <ul> 
     <li> <p>en-US (predeterminado): inglés (Estados Unidos de América)</p> </li> 
     <li> <p>ca-ES: Catalán (España)</p> </li> 
     <li> <p>cs-CZ: Checo (República Checa)</p> </li> 
     <li> <p>da-DK: Danés (Dinamarca)</p> </li> 
     <li> <p>de-DE: Alemán (Alemania)</p> </li> 
     <li> <p>en-AE: Inglés (Emiratos Árabes Unidos)</p> </li> 
     <li> <p>en-GB: inglés (Reino Unido)</p> </li> 
     <li> <p>en-IL: Inglés (Israel)</p> </li> 
     <li> <p>en-US: Inglés (Estados Unidos de América)</p> </li> 
     <li> <p>es-ES: Español (España)</p> </li> 
     <li> <p>es-MX: Español (México)</p> </li> 
     <li> <p>eu-ES: Vasco (España)</p> </li> 
     <li> <p>fi-FI: finés (Finlandia)</p> </li> 
     <li> <p>fr-CA: Francés (Canadá)</p> </li> 
     <li> <p>fr-FR: Francés (Francia)</p> </li> 
     <li> <p>fr-MA: Francés (Marruecos)</p> </li> 
     <li> <p>hr-HR: Croata (Croacia)</p> </li> 
     <li> <p>hu-HU: húngaro (Hungría)</p> </li> 
     <li> <p>it-IT: italiano (Italia)</p> </li> 
     <li> <p>ja-JP: Japonés (Japón)</p> </li> 
     <li> <p>kr-KR: Coreano (Corea del Sur)</p> </li> 
     <li> <p>nb-NO: Noruego Bokmål (Noruega)</p> </li> 
     <li> <p>nl-NL: Neerlandés (Países Bajos)</p> </li> 
     <li> <p>pl-PL: polaco (Polonia)</p> </li> 
     <li> <p>pt-BR: portugués (Brasil)</p> </li> 
     <li> <p>pt-PT: portugués (Portugal)</p> </li> 
     <li> <p>ro-RO: Rumano (Rumanía)</p> </li> 
     <li> <p>ru-RU: Ruso (Rusia)</p> </li> 
     <li> <p>sk-SK: Eslovaco (Eslovaquia)</p> </li> 
     <li> <p>sl-SI: Esloveno (Eslovenia)</p> </li> 
     <li> <p>sv-SE: Sueco (Suecia)</p> </li> 
     <li> <p>tr-TR: Turco (Turquía)</p> </li> 
     <li> <p>uk-UA: Ucraniano (Ucrania)</p> </li> 
     <li> <p>zh-CN: chino (China continental)</p> </li> 
     <li> <p>zh-TW: Chino (Taiwán)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convertir HTML en archivo de PDF]

Esta herramienta convierte un archivo de HTML en un archivo de PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Seleccione la conexión que se utilizará para este módulo.</p> Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe PDF Services], consulte <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Cree una conexión con [!DNL Adobe PDF Services]</a> en este artículo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> <p>Importante: El archivo de origen debe estar en formato HTML o ZIP. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON]</td> 
   <td> <p>Si el HTML hace referencia a variables de JavaScript, puede incluir dichas variables aquí. </p> <p>Haga clic en cada variable <strong>[!UICONTROL Agregar elemento]</strong> e incluir la clave y el valor de la variable.</p> <p>Nota:   
     <ul> 
      <li> <p>Al crear un PDF a partir de un archivo ZIP, el material colateral de origen debe incluir un elemento de secuencia de comandos como: <code> &lt;script src='./json.js' type='text/javascript'&gt;&lt;/script&gt;</code> </p> </li> 
      <li> <p>Al crear un PDF a partir de una dirección URL, el contenido de este objeto JSON se inserta en la máquina virtual del explorador antes de que se procese la página. </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Incluir encabezado y pie de página]</td> 
   <td> <p>Active esta opción para crear encabezados y pies de página para el documento de PDF.</p> 
    <ul> 
     <li> <p>El encabezado incluye una fecha y el título del documento.</p> </li> 
     <li> <p>El pie de página incluye el nombre del archivo y un número de página.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anchura de página]</td> 
   <td>Escriba la anchura del papel, en pulgadas. El módulo utiliza esta información para dar formato a las páginas en el archivo de PDF creado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Altura de página]</td> 
   <td>Escriba la altura del papel, en pulgadas. El módulo utiliza esta información para dar formato a las páginas en el archivo de PDF creado.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convertir imagen a archivo de PDF]

Esta herramienta convierte una imagen en un archivo de PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Seleccione la conexión que se utilizará para este módulo.</p> Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe PDF Services], consulte <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Cree una conexión con [!DNL Adobe PDF Services]</a> en este artículo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y el archivo de imagen del archivo de origen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convertir PDF en documento]

Esta herramienta convierte un archivo de PDF en un documento. Puede seleccionar uno de los siguientes formatos para el archivo de salida.

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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Seleccione la conexión que se utilizará para este módulo.</p> Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe PDF Services], consulte <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Cree una conexión con [!DNL Adobe PDF Services]</a> en este artículo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> <p>El archivo de origen debe tener el formato de PDF. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de archivos de salida]</td> 
   <td> <p>Seleccione el formato con el que desea que se emitan los archivos:</p> 
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

Esta herramienta convierte un PDF en una imagen en formato PNG o de JPEG., que a continuación se muestra como un ZIP. El PDF se convierte en una imagen por página y cada imagen termina con el número de página. A continuación, los archivos de imagen se combinan en un archivo ZIP.

Por ejemplo, un archivo denominado &quot;TestFile&quot; con 8 páginas produciría 8 imágenes, denominadas &quot;TestFile_1&quot; a &quot;TestFile_8&quot;. La salida del módulo es un archivo ZIP que contiene las 8 imágenes.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Seleccione la conexión que se utilizará para este módulo.</p> Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe PDF Services], consulte <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Cree una conexión con [!DNL Adobe PDF Services]</a> en este artículo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> <p>El archivo de origen debe tener el formato de PDF. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de archivos de salida]</td> 
   <td> <p>Seleccione el formato con el que desea que se emitan los archivos:</p> 
    <ul> 
     <li>PNG</li> 
     <li>JPEG</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Linealización de un archivo de PDF]

Esta herramienta linealiza un documento de PDF para crear un documento de PDF optimizado para la web. Un documento PDF linealizado se puede ver página por página sin necesidad de descargar todo el documento.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Seleccione la conexión que se utilizará para este módulo.</p> Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe PDF Services], consulte <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Cree una conexión con [!DNL Adobe PDF Services]</a> en este artículo. </td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Seleccione la conexión que se utilizará para este módulo.</p> Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe PDF Services], consulte <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Cree una conexión con [!DNL Adobe PDF Services]</a> en este artículo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL OCR type]</td> 
   <td> 
    <ul> 
     <li> <p>El tipo [!UICONTROL Imagen original modificada] garantiza que el texto se pueda buscar y seleccionar, pero modifica la imagen original durante el proceso de limpieza (por ejemplo, la recorta) antes de colocar una capa de texto invisible sobre ella. Este tipo elimina los artefactos no deseados y puede resultar en un documento más legible en algunos casos. </p> </li> 
     <li> <p>El tipo [!UICONTROL Imagen original sin modificar] también superpone una capa de texto en la que se puede buscar sobre la imagen original, pero en este caso, la imagen original no cambia. Este tipo produce la máxima fidelidad a la imagen original.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Idioma]</td> 
   <td>Seleccione el idioma de este documento.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Manipulación de páginas]

Este módulo le permite rotar o eliminar selectivamente páginas de un documento de PDF. Por ejemplo, puede cambiar la vista vertical a la horizontal o quitar determinadas páginas del documento de PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Seleccione la conexión que se utilizará para este módulo.</p> Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe PDF Services], consulte <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Cree una conexión con [!DNL Adobe PDF Services]</a> en este artículo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Acción]</td> 
   <td> <p>Seleccione la acción que desea realizar en el archivo.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Eliminar]</b> </p> <p>Seleccione esta opción para eliminar páginas del documento.</p> </li> 
     <li> <p><b>[!UICONTROL Rotar]</b> </p> <p>Seleccione esta opción para girar las páginas y, a continuación, introduzca el ángulo, en grados en el sentido de las agujas del reloj, que desea que giren las páginas del documento en relación con su orientación inicial.</p> <p>Para girar de vertical a horizontal o viceversa, gire la página 90 o 270 grados.</p> <p>Si una página está al revés, gírela 180 grados.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Páginas]</td> 
   <td> <p>Para cada intervalo de páginas que desee eliminar, haga clic en <strong>[!UICONTROL Agregar]</strong> y, a continuación, introduzca la primera y la última página del intervalo de páginas. </p> <p>Nota:   
     <ul> 
      <li> <p>Puede utilizar números negativos para contar desde el final del documento. La última página de un documento es -1, la segunda a la última página es -2, y así sucesivamente.</p> </li> 
      <li> <p>Para eliminar una sola página, establezca el mismo número de página que el inicio y el final del intervalo.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros con los que desea que trabaje el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Etiquetado automático de accesibilidad de PDF]

Este módulo de acción crea un PDF etiquetado para casos de uso de accesibilidad. También crea un informe opcional de Microsoft Excel que enumera los problemas y sugiere correcciones.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Seleccione la conexión que se utilizará para este módulo.</p> Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe PDF Services], consulte <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Cree una conexión con [!DNL Adobe PDF Services]</a> en este artículo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados de cambio]</td> 
   <td> <p>Active esta opción para cambiar los encabezados del documento.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Generar informe]</b> </p> <p>Active esta opción para generar un informe que enumere los problemas de accesibilidad en el PDF junto con su ubicación y proporcione sugerencias para solucionarlos.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Propiedades del archivo del PDF]

Esta herramienta extrae información básica sobre el documento, como:

* Recuento de páginas
* Versión del PDF
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Seleccione la conexión que se utilizará para este módulo.</p> Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe PDF Services], consulte <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Cree una conexión con [!DNL Adobe PDF Services]</a> en este artículo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Archivo de PDF de Protect]

Esta herramienta asegura un documento de PDF con una contraseña de usuario o de propietario. También establece restricciones en determinadas funciones, como imprimir, editar y copiar en el documento de PDF. Se selecciona el tipo de contenido que se va a cifrar y el algoritmo de cifrado.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Seleccione la conexión que se utilizará para este módulo.</p> Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe PDF Services], consulte <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Cree una conexión con [!DNL Adobe PDF Services]</a> en este artículo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> <p>El archivo de origen debe tener el formato de PDF. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de protección por contraseña]</td> 
   <td> <p>Active esta opción para utilizar contraseñas para cifrar el documento del PDF de entrada. Si activa esta opción, debe especificar e introducir un valor para una o ambas de las siguientes opciones: </p> 
    <ul> 
     <li> <p>[!UICONTROL userPassword]</p> </li> 
     <li> <p>[!UICONTROL ownerPassword] </p> </li> 
    </ul> <p>Cada contraseña puede tener hasta 128 caracteres de longitud.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Algoritmo de cifrado]</td> 
   <td> <p>Seleccione el algoritmo de cifrado. </p> 
    <ul> 
     <li> <p>[!UICONTROL AES-128 cifrado]</p> <p>La contraseña solo admite caracteres LATIN-I. </p> </li> 
     <li> <p>[!UICONTROL AES-256 cifrado]</p> <p>La contraseña admite conjuntos de caracteres Unicode</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenido para cifrar]</td> 
   <td> <p>Seleccione el tipo de contenido que desea cifrar.</p> 
    <ul> 
     <li> <p>[!UICONTROL Todo el contenido]</p> </li> 
     <li> <p>[!UICONTROL Todo el contenido excepto los metadatos]</p> </li> 
     <li> <p>[!UICONTROL Solo datos incrustados] </p> </li> 
    </ul> <p>Si selecciona "[!UICONTROL Solo datos incrustados]", los permisos de acceso proporcionados se considerarán ineficaces.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Permisos]</td> 
   <td> <p>Seleccione los permisos que desee incluir para permitir la impresión, edición o copia de contenido.</p> <p>La configuración de permisos sólo se utiliza si [!UICONTROL ownerPassword] está establecida en el campo [!UICONTROL Password Protection Type].</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eliminación de la protección de un archivo de PDF]

Esta herramienta elimina la seguridad (protección con contraseña) de un documento de PDF.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Seleccione la conexión que se utilizará para este módulo.</p> Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe PDF Services], consulte <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Cree una conexión con [!DNL Adobe PDF Services]</a> en este artículo. </td> 
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

### [!UICONTROL División de un archivo de PDF]

Este módulo de acción divide un documento de PDF en varios documentos más pequeños. Especifique si desea dividirlo por número de archivos, páginas por archivo o intervalos de páginas.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Seleccione la conexión que se utilizará para este módulo.</p> Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe PDF Services], consulte <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Cree una conexión con [!DNL Adobe PDF Services]</a> en este artículo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> <p>El archivo de origen debe tener el formato de PDF.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Opción [!UICONTROL Split]</td> 
   <td>Seleccione cómo desea dividir el archivo. 
   <ul>
   <li><p><b>Intervalos de página</b></p><p>Para cada intervalo de páginas que desee dividir en un documento independiente, haga clic en <b>Añadir</b> e introduzca la página en la que desea comenzar y la página en la que desea finalizar.</p></li>
   <li><p><b>Recuento de páginas</b></p><p>Introduzca el número de páginas que desea incluir en los nuevos documentos.</p></li>
   <li><p><b>Número de archivos</b></p><p>Introduzca el número de archivos de tamaño uniforme en los que desea dividir el documento.</p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>

## Realizar una llamada de API personalizada

Este módulo de acción envía una solicitud HTTP personalizada a la API de servicios de PDF.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Seleccione la conexión que se utilizará para este módulo.</p> Para obtener instrucciones sobre cómo crear una conexión con [!DNL Adobe PDF Services], consulte <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >Cree una conexión con [!DNL Adobe PDF Services]</a> en este artículo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> Introduzca una ruta relativa o una dirección URL. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion añade los encabezados de autorización automáticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos]</td> 
   <td> <p>Para cada campo que desee añadir a la llamada de API, haga clic en <b>Añadir elemento</b> e introduzca la clave y el valor opcional del campo.</p> <p>Nota:  <p>Cuando se utilizan afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera del enunciado condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

