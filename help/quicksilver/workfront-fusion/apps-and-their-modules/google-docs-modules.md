---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos Google Docs
description: Adobe Workfront Fusion [!DNL Google Docs] los módulos le permiten monitorizar, crear, editar y recuperar documentos en su [!DNL Google Docs] y [!DNL Google Docs] (para usuarios de [!DNL G Suite]).
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: fbe7d628-d833-43ce-83b8-8e4e6a812fd1
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '4042'
ht-degree: 0%

---

# [!DNL Google Docs] módulos

La variable [!DNL Adobe Workfront Fusion] [!DNL Google Docs] los módulos le permiten monitorizar, crear, editar y recuperar documentos en su [!DNL Google Docs] y [!DNL Google Docs] (para [!DNL G Suite] usuarios).

Para usar [!DNL Google Docs] con [!DNL Adobe Workfront Fusion], es necesario tener un [!DNL Google] cuenta. Si no tiene un [!DNL Google] todavía puede crear una en la [!DNL Google] Página de ayuda de la cuenta.

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

Para usar [!DNL Google Docs] , debe tener una cuenta de Google.

## [!DNL Google Docs] módulos y sus campos

Al configurar [!DNL Google Docs] módulos, [!UICONTROL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL Google Docs] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Documento

* [[!UICONTROL Documentos de Watch]](#watch-documents)
* [[!UICONTROL Documentos de lista]](#list-documents)
* [[!UICONTROL Obtener contenido de un documento]](#get-content-of-a-document)
* [[!UICONTROL Crear un documento]](#create-a-document)
* [[!UICONTROL Crear un documento a partir de una plantilla]](#create-a-document-from-a-template)
* [[!UICONTROL Insertar un párrafo en un documento]](#insert-a-paragraph-to-a-document)
* [[!UICONTROL Insertar una imagen en un documento]](#insert-an-image-to-a-document)
* [[!UICONTROL Reemplazar una imagen por una nueva imagen]](#replace-an-image-with-a-new-image)
* [[!UICONTROL Reemplazar texto en un documento]](#replace-text-in-a-document)
* [[!UICONTROL Descargar un documento]](#download-a-document)
* [[!UICONTROL Eliminar un documento]](#delete-a-document)

#### [!UICONTROL Documentos de Watch]

Este módulo de déclencheur devuelve los detalles del documento cuando se crea o modifica un nuevo documento en la carpeta seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch Documents]</td> 
   <td> <p style="color: #000000;">Seleccione si desea ver los documentos creados ([!UICONTROL By Created Date]) o modificados ([!UICONTROL By Modified Date]).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad que desea monitorizar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta que desea ver para los documentos creados o modificados.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta que desea ver para los documentos creados o modificados.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible para [!DNL G Suite] solo usuarios)</p> <p>Seleccione si desea [!UICONTROL Usar acceso de administrador de dominio]. Si selecciona [!UICONTROL Sí], la solicitud se emite como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida que desee ver.</p> <p>Nota: Si ha seleccionado la variable [!DNL Google Shared Drive] en este campo y no es [!DNL G Suite] usuario, el error <code>[400] Invalid Value</code> se devuelve.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td> <p>Establezca el número máximo de documentos que Workfront Fusion devuelve en un ciclo de ejecución.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Documentos de lista]

Este módulo de acción recupera una lista de documentos de la carpeta seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad desde la que desea enumerar los documentos.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta desde la que desea enumerar los documentos.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta desde la que desea enumerar los documentos.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible para [!DNL G Suite] solo usuarios)</p> <p>Seleccione si desea [!UICONTROL Usar acceso de administrador de dominio]. Si selecciona [!UICONTROL Sí], la solicitud se emite como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida de la que desea enumerar los documentos.</p> <p>Nota: Si ha seleccionado la variable [!DNL Google Docs] en este campo y no es [!DNL G Suite] usuario, el error <code>[400] Invalid Value</code> se devuelve.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td> <p>Configurar el número máximo de documentos [!DNL Workfront Fusion] devuelve en un ciclo de ejecución.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener contenido de un documento]

Este módulo de acción recupera un documento especificado.

Es posible que deba ampliar los permisos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtener contenido de un documento]</td> 
   <td> <p>Seleccione si desea asignar el ID del documento o seleccione el documento en el menú desplegable manualmente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad que contiene el documento que desea recuperar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta que contiene el documento que desea recuperar.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta que contiene el documento que desea recuperar.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible para [!DNL G Suite] solo usuarios)</p> <p>Seleccione si desea [!UICONTROL Usar acceso de administrador de dominio]. Si selecciona [!UICONTROL Sí], la solicitud se emite como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida que contiene el documento que desea recuperar.</p> <p>Nota: Si ha seleccionado la variable [!DNL Google Docs] en este campo y no es [!DNL G Suite] usuario, el error <code>[400] Invalid Value</code> se devuelve.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filtro]</p> </td> 
   <td> <p>Seleccione el objeto que desea que se devuelva en la salida del módulo.</p> 
    <ul> 
     <li>[!UICONTROL Image] (predeterminado)</li> 
     <li>[!UICONTROL Dibujo]</li> 
     <li>[!UICONTROL Chart]</li> 
    </ul> <p>Nota:  <p>Para obtener más asignación de estos objetos, utilice el valor [!UICONTROL Inline Objects Array] en la salida de este módulo (en lugar de [!UICONTROL inlineObjects]).</p> <p>Los objetos [!UICONTROL Inline Objects Array] se ordenan en el mismo orden en que aparecen en el documento. Facilitará el procesamiento posterior.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un documento]

Este módulo de acción permite crear un nuevo documento en la carpeta seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Introduzca el nombre del documento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content]</td> 
   <td> <p>Introduzca el contenido del documento. HTML compatible.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad en la que desea crear un documento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta en la que desea crear un documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta en la que desea crear un documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible para [!DNL G Suite] solo usuarios)</p> <p>Seleccione si desea [!UICONTROL Usar acceso de administrador de dominio]. Si selecciona [!UICONTROL Sí], la solicitud se emite como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida en la que desea crear un documento.</p> <p>Nota: Si ha seleccionado la variable [!DNL Google Docs] en este campo y no es [!DNL G Suite] usuario, el error <code>[400] Invalid Value</code> se devuelve.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Insertar un encabezado]</td> 
   <td> <p> Active esta opción para insertar el encabezado al documento y, a continuación, introduzca o asigne el texto del encabezado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Insertar un pie de página] </td> 
   <td> <p>Active esta opción para insertar el pie de página en el documento y, a continuación, introduzca o asigne el texto del encabezado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un documento a partir de una plantilla]

Este módulo de acción crea una copia de un documento de plantilla existente y reemplaza cualquier etiqueta. Este módulo también permite a los usuarios reemplazar imágenes con nuevas imágenes por dirección URL.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Crear un documento a partir de una plantilla]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Por Asignación]</strong> <br>Seleccione esta opción para asignar la plantilla de documento.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br>Seleccione esta opción para elegir la plantilla de documento en el menú desplegable.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad en la que se encuentra la plantilla. Esta opción está disponible si ha seleccionado [!UICONTROL By Dropdown] en el campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta en la que se encuentra la plantilla.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta en la que se encuentra la plantilla.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible para [!DNL G Suite] solo usuarios)</p> <p>Seleccione si desea [!UICONTROL Usar acceso de administrador de dominio]. Si selecciona [!UICONTROL Sí], la solicitud se emite como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida en la que se encuentra la plantilla.</p> <p>Nota: Si ha seleccionado la variable [!DNL Google Docs] en este campo y no es [!DNL G Suite] usuario, el error <code>[400] Invalid Value</code> se devuelve.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Values]</p> </td> 
   <td> <p>Introduzca los valores que se introducen en lugar de las variables en el nuevo documento.</p> 
    <ul> 
     <li><strong>[!UICONTROL Etiquetas]</strong> <br>Introduzca las etiquetas incluidas en la plantilla de documento. No use <code>&#123;&#123;&#125;&#125;</code>. Ejemplo: use <code>name</code> en lugar de <code>&#123;&#123;name&#125;&#125;</code>.</li> 
     <li><strong>[!UICONTROL Valor reemplazado]</strong><br>Introduzca el valor de la etiqueta.</li> 
    </ul> <p>Por ejemplo, la variable<code> &#123;&#123;name&#125;&#125;</code> en el documento de origen se mostrará como el campo de nombre aquí, donde se puede insertar el valor, como <code>John</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sustitución de imágenes]</p> </td> 
   <td> <p>Introduzca el vínculo a [!UICONTROL Image Object ID] y [!UICONTROL Image URL] que sustituirá a la imagen actual.</p> <p>Nota: Puede recuperar los ID de imagen utilizando el módulo [!UICONTROL Obtener un documento], donde los ID están contenidos en la matriz [!UICONTROL matriz de objetos en línea].</p> <p>Le recomendamos que agregue texto ALT a las imágenes de su [!DNL Google] documento. </p> <p>Para agregar un texto ALT al [!DNL Google Docs] imagen:</p> 
    <ol> 
     <li value="1">Haga clic con el botón derecho en la imagen.</li> 
     <li value="2">Seleccione la opción [!UICONTROL ALT text].</li> 
     <li value="3">Introduzca el [!UICONTROL ALT text] en el campo [!UICONTROL Title] y haga clic en [!UICONTROL OK].</li> 
    </ol> <p>Después de agregar el texto ALT a la imagen, el texto ALT se muestra entre paréntesis en el nombre del campo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title] </td> 
   <td> <p>Introduzca el nombre del nuevo documento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad en la que se encuentra la plantilla. Esta opción está disponible si ha seleccionado [!UICONTROL By Dropdown] en el campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta en la que desea crear el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta en la que desea crear el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible para [!DNL G Suite] solo usuarios)</p> <p>Seleccione si desea [!UICONTROL Usar acceso de administrador de dominio]. Si selecciona [!UICONTROL Sí], la solicitud se emite como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida en la que desea crear el documento.</p> <p>Nota: Si ha seleccionado la variable [!DNL Google Docs] en este campo y no es [!DNL G Suite] usuario, el error <code>[400] Invalid Value</code> se devuelve.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Insertar un párrafo en un documento]

Este módulo de acción anexa o inserta un nuevo párrafo en un documento existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Seleccionar un documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Por Asignación]</strong> <br>Seleccione esta opción para asignar el documento.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Seleccione esta opción para elegir el documento en el menú desplegable.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad en la que se encuentra el documento al que desea agregar un párrafo. Esta opción está disponible si ha seleccionado [!UICONTROL By Dropdown] en el campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta en la que se encuentra el documento al que desea agregar un párrafo y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta en la que se encuentra el documento al que desea agregar un párrafo y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible para [!DNL G Suite] solo usuarios)</p> <p>Seleccione si desea [!UICONTROL Usar acceso de administrador de dominio]. Si selecciona [!UICONTROL Sí], la solicitud se emite como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida en la que se encuentra el documento al que desea agregar un párrafo y, a continuación, seleccione el documento.</p> <p>Nota: Si ha seleccionado la variable [!DNL Google Docs] en este campo y no es [!DNL G Suite] usuario, el error <code>[400] Invalid Value</code> se devuelve.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Insertar un párrafo]</p> </td> 
   <td> <p>Seleccione cómo desea que el nuevo texto se inserte en el documento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Por especificación de ubicación]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL By index]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Index]</strong> </p> <p>Introduzca el número de índice en el que desea insertar el texto. Puede utilizar el módulo [!UICONTROL Get a Document] para recuperar el número de índice.</p> <p>Para mostrar todos los caracteres (incluido el oculto) del documento, puede utilizar el complemento [!UICONTROL Show]. Puede encontrar el complemento en [!UICONTROL Add-ons] &gt; [!UICONTROL Get add-ons]. Busque [!UICONTROL Show] e instale el complemento [!UICONTROL Show].</p> </li> 
         <li> <p><strong>[!UICONTROL Texto insertado]</strong> </p> <p>Escriba el texto que desee insertar en el documento.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL Por ID de segmento]</strong> </p> <p>Seleccione el encabezado y pie de página al que desee insertar el contenido de texto e introduzca el texto que desee insertar en los campos correspondientes.</p> <p>Si el encabezado o pie de página ya contiene texto, el nuevo texto se agregará antes del texto existente.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Anexando al cuerpo del documento]</strong> </p> <p>Anexa el texto introducido al final del contenido del cuerpo del documento.</p> <p>El estilo del nuevo párrafo se copiará del párrafo en el índice de inserción actual, incluidas las listas y las viñetas.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Anexando al final del segmento (Encabezado y pie de página)]</strong> </p> <p>Seleccione el encabezado y pie de página al que desee insertar el contenido de texto e introduzca el texto que desee insertar en los campos correspondientes.</p> <p>Si el encabezado o pie de página ya contiene texto, el nuevo texto se agregará después del texto existente.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Texto anexado]</td> 
   <td>Escriba o asigne el texto que desee anexar al documento</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Insertar una imagen en un documento]

Este módulo de acción inserta una imagen de la dirección URL en el documento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Seleccionar un documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Por Asignación]</strong> <br>Seleccione esta opción para asignar la plantilla de documento.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Seleccione esta opción para elegir el documento en el menú desplegable.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad en la que se encuentra el documento al que desea agregar una imagen. Esta opción está disponible si ha seleccionado [!UICONTROL By Dropdown] en el campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta en la que se encuentra el documento al que desea agregar una imagen y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta en la que se encuentra el documento al que desea agregar una imagen y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible para [!DNL G Suite] solo usuarios)</p> <p>Seleccione si desea [!UICONTROL Usar acceso de administrador de dominio]. Si selecciona [!UICONTROL Sí], la solicitud se emite como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida en la que se encuentra el documento al que desea agregar una imagen y, a continuación, seleccione el documento.</p> <p>Nota: Si ha seleccionado la variable [!DNL Google Docs] en este campo y no es [!DNL G Suite] usuario, el error <code>[400] Invalid Value</code> se devuelve.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Insertar una imagen]</p> </td> 
   <td> <p>Seleccione cómo desea que la nueva imagen se inserte en el documento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Por especificación de ubicación]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL By index]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Index]</strong> </p> <p>Introduzca el número de índice en el que desea insertar la imagen. Puede utilizar el módulo [!UICONTROL Get a Document] recuperar [!UICONTROL Index number].</p> <p>Para mostrar todos los caracteres (incluido el oculto) del documento, puede utilizar el complemento [!UICONTROL Show]. Puede encontrar el complemento en [!UICONTROL Add-ons] &gt; [!UICONTROL Get add-ons]. Busque [!UICONTROL Show] e instale el complemento [!UICONTROL Show].</p> </li> 
         <li> <p><strong>[!UICONTROL Image URL]</strong> </p> <p>Introduzca la dirección URL de la imagen que desea insertar en el documento.</p> <p>El tamaño máximo de la imagen es de 50 MB. No debe superar los 25 megapíxeles. Solo se admite formato PNG, JPEG o GIF.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL Por ID de segmento]</strong> </p> <p>Seleccione el encabezado y pie de página al que desee insertar la imagen e introduzca la URL de la imagen en los campos correspondientes.</p> <p>El tamaño máximo de la imagen es de 50 MB. La imagen no debe superar los 25 megapíxeles. Solo se admite el formato PNG, JPEG o GIF.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Anexando al cuerpo del documento]</strong> </p> <p>Anexa una imagen específica al final del contenido del cuerpo del documento.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Anexando al final del segmento (Encabezado y pie de página)]</strong> </p> <p>Seleccione el encabezado y pie de página al que desea insertar una imagen e introduzca la URL de la imagen que desea insertar en los campos correspondientes.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Magnitud de altura en puntos/anchura en puntos]</p> </td> 
   <td> <p>Defina el tamaño de la imagen insertada. Se mantendrá la relación de aspecto.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Reemplazar una imagen por una nueva imagen]

Este módulo de acción reemplaza una imagen existente. Se mantendrá la relación de aspecto de la imagen original.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Seleccionar un documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Por Asignación]</strong> <br>Seleccione esta opción para asignar la plantilla de documento.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Seleccione esta opción para elegir el documento en el menú desplegable.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad donde se encuentra el documento que desea reemplazar en una imagen. Esta opción está disponible si ha seleccionado [!UICONTROL By Dropdown] en el campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta donde se encuentra el documento que desea reemplazar a una imagen y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta donde se encuentra el documento que desea reemplazar a una imagen y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible para [!DNL G Suite] solo usuarios)</p> <p>Seleccione si desea [!UICONTROL Usar acceso de administrador de dominio]. Si selecciona [!UICONTROL Sí], la solicitud se emite como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida en la que se encuentra el documento que desea reemplazar con una imagen y, a continuación, seleccione el documento.</p> <p>Nota: Si ha seleccionado la variable [!DNL Google Docs] en este campo y no es [!DNL G Suite] usuario, el error <code>[400] Invalid Value</code> se devuelve.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Image URL]</p> </td> 
   <td> <p>Introduzca o asigne la URL de la nueva imagen que reemplazará a la imagen existente.</p> <p>Las imágenes se muestran en el orden en que aparecen en el documento. Por ejemplo, <code>Body: Image No. 1</code> es la primera imagen del documento.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Reemplazar texto en un documento]

Este módulo de acción reemplaza el texto de un documento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Seleccionar un documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Por Asignación]</strong> <br>Seleccione esta opción para asignar la plantilla de documento.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Seleccione esta opción para elegir el documento en el menú desplegable.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad en la que se encuentra el documento al que desea agregar texto. Esta opción está disponible si ha seleccionado [!UICONTROL By Dropdown] en el campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta en la que se encuentra el documento al que desea agregar texto y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta en la que se encuentra el documento al que desea agregar texto y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible para [!DNL G Suite] solo usuarios)</p> <p>Seleccione si desea [!UICONTROL Usar acceso de administrador de dominio]. Si selecciona [!UICONTROL Sí], la solicitud se emite como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida en la que se encuentra el documento al que desea agregar texto y, a continuación, seleccione el documento.</p> <p>Nota: Si ha seleccionado la variable [!DNL Google Docs] en este campo y no es [!DNL G Suite] usuario, el error <code>[400] Invalid Value</code> se devuelve.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Reemplazar un texto]</p> </td> 
   <td> <p>Agregue cada texto que desee reemplazar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Texto antiguo que se va a reemplazar]</strong> </p> <p>Escriba el texto que desee reemplazar.</p> </li> 
     <li> <p><strong>[!UICONTROL Nuevo texto que se va a insertar]</strong> </p> <p>Introduzca el nuevo texto.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Descargar un documento]

Este módulo de acción convierte y descarga el documento seleccionado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad en la que se encuentra el documento que desea descargar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta donde se encuentra el documento que desea descargar y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta donde se encuentra el documento que desea descargar y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible para [!DNL G Suite] solo usuarios)</p> <p>Seleccione si desea [!UICONTROL Usar acceso de administrador de dominio]. Si selecciona [!UICONTROL Sí], la solicitud se emite como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida en la que se encuentra el documento que desea descargar y, a continuación, seleccione el documento.</p> <p>Nota: Si ha seleccionado la variable [!DNL Google Docs] en este campo y no es [!DNL G Suite] usuario, el error <code>[400] Invalid Value</code> se devuelve.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type] </p> </td> 
   <td> <p>Seleccione el formato de archivo de destino del documento descargado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un documento]

Este módulo de acción elimina un documento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad donde se encuentra el documento que desea eliminar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta donde se encuentra el documento que desea eliminar y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta donde se encuentra el documento que desea eliminar y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible para [!DNL G Suite] solo usuarios)</p> <p>Seleccione si desea [!UICONTROL Usar acceso de administrador de dominio]. Si selecciona [!UICONTROL Sí], la solicitud se emite como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida en la que se encuentra el documento que desea eliminar y, a continuación, seleccione el documento.</p> <p>Nota: Si ha seleccionado la variable [!DNL Google Docs] en este campo y no es [!DNL G Suite] usuario, el error <code>[400] Invalid Value</code> se devuelve.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Unidad compartida]</td> 
   <td> <p>Seleccione la unidad que contiene el documento que desea descargar y, a continuación, seleccione un documento. Esta opción está disponible si ha seleccionado [!DNL Google Docs] en el campo [!UICONTROL Elegir una unidad].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Document ID]</td> 
   <td> <p> Seleccione o asigne el documento en el que desea reemplazar una o más imágenes.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Otro

* [[!UICONTROL Realizar una llamada de API]](#make-an-api-call)
* [[!UICONTROL Hacer clic en todos los vínculos de un documento]](#make-all-links-in-a-document-clickable)

#### [!UICONTROL Realizar una llamada de API]

Este módulo de acción le permite realizar una llamada API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Especifique una ruta relativa a <code>https://docs.googleapis.com/</code>. Ejemplo: <code>/v1/documents/{presentationID}</code>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada a la API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de un objeto JSON estándar. Por ejemplo, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] añade los encabezados de autorización por usted.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p> Introduzca la cadena de consulta de solicitud.</p> </td> 
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

**Ejemplo:** La siguiente llamada de API recupera los detalles del documento especificado en los documentos de Google:

**Dirección URL:**

/v1/documents/1ujkf-GDgB0TQSYPrxbCSK4Uso54tHVMqHZEVZZxB6aY

**Método:**

[!UICONTROL GET]

![](assets/api-call-example.png)

Los detalles del documento recuperado se encuentran en la sección Output del módulo, en [!UICONTROL Paquete] > [!UICONTROL Cuerpo].

![](assets/api-output.png)

#### [!UICONTROL Hacer clic en todos los vínculos de un documento]

Este módulo de acción encuentra todos los vínculos en el documento y los hace seleccionables.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Google] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conecte la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Crear todos los vínculos en un documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Por Asignación]</strong> <br>Seleccione esta opción para asignar la plantilla de documento.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Seleccione esta opción para elegir el documento en el menú desplegable.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad en la que se encuentra el documento en el que desea hacer clic en los vínculos. Esta opción está disponible si ha seleccionado [!UICONTROL By Dropdown] en el campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta en la que se encuentra el documento en el que desea hacer clic en los vínculos y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta en la que se encuentra el documento en el que desea hacer clic en los vínculos y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible para [!DNL G Suite] solo usuarios)</p> <p>Seleccione si desea [!UICONTROL Usar acceso de administrador de dominio]. Si selecciona [!UICONTROL Sí], la solicitud se emite como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida en la que se encuentra el documento en el que desea hacer clic en los vínculos y, a continuación, seleccione el documento.</p> <p>Nota: Si ha seleccionado la variable [!DNL Google Docs] en este campo y no es [!DNL G Suite] usuario, el error <code>[400] Invalid Value</code> se devuelve.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Unidad compartida]</td> 
   <td> <p>Seleccione la unidad que contiene el documento en el que desea actualizar los vínculos y, a continuación, seleccione un documento. Esta opción está disponible si ha seleccionado [!DNL Google Docs] en el campo [!UICONTROL Elija una unidad].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Document ID]</td> 
   <td> <p> Seleccione o asigne el documento en el que desea actualizar los vínculos.</p> </td> 
  </tr> 
 </tbody> 
</table>
