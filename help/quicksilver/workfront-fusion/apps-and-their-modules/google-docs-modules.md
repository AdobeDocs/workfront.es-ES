---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de documentos de Google
description: Los módulos Adobe Workfront Fusion [!DNL Google Docs] le permiten supervisar, crear, editar y recuperar documentos en sus [!DNL Google Docs] y [!DNL Google Docs] (para [!DNL Google Workspace] usuarios).
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: fbe7d628-d833-43ce-83b8-8e4e6a812fd1
source-git-commit: 2e91e9a4c691430f3c98e3cbddb30706ea57f84a
workflow-type: tm+mt
source-wordcount: '4105'
ht-degree: 0%

---

# [!DNL Google Docs] módulos

Los módulos [!DNL Adobe Workfront Fusion] [!DNL Google Docs] le permiten supervisar, crear, editar y recuperar documentos en [!DNL Google Docs] y [!DNL Google Docs] (para [!DNL Google Workspace] usuarios).

Para usar [!DNL Google Docs] con [!DNL Adobe Workfront Fusion], es necesario tener una cuenta de [!DNL Google]. Si todavía no tiene una cuenta [!DNL Google], puede crearla en la página de ayuda de la cuenta [!DNL Google].

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

Para usar módulos de [!DNL Google Docs], debe tener una cuenta de Google.

## Información de API de Google Docs

El conector de documentos de Google utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL básica</td> 
   <td> https://docs.googleapis.com/v1</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Versión de API</td> 
   <td> Versión 1 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 1.4.13</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Google Docs] módulos y sus campos

Al configurar [!DNL Google Docs] módulos, [!UICONTROL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Google Docs] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Documento

* [[!UICONTROL Documentos de inspección]](#watch-documents)
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

#### [!UICONTROL Documentos de inspección]

Este módulo de déclencheur devuelve los detalles del documento cuando se crea o modifica un nuevo documento en la carpeta seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ver documentos]</td> 
   <td> <p style="color: #000000;">Seleccione si desea ver los documentos creados ([!UICONTROL By Created Date]) o modificados ([!UICONTROL By Modified Date]).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad que desea supervisar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta en la que desea inspeccionar documentos creados o modificados.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta en la que desea inspeccionar documentos creados o modificados.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible solo para usuarios de [!DNL Google Workspace])</p> <p>Seleccione si desea [!UICONTROL Utilizar acceso de administrador de dominio]. Al seleccionar [!UICONTROL Sí], se emite la solicitud como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida que desee ver.</p> <p>Nota: Si ha seleccionado la opción [!DNL Google Shared Drive] en este campo y no es un usuario de [!DNL Google Workspace], se devuelve el error <code>[400] Invalid Value</code>.</p> </li> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad desde la que desea enumerar los documentos.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta desde la que desee enumerar los documentos.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta desde la que desee enumerar los documentos.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible solo para usuarios de [!DNL Google Workspace])</p> <p>Seleccione si desea [!UICONTROL Utilizar acceso de administrador de dominio]. Al seleccionar [!UICONTROL Sí], se emite la solicitud como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida desde la que desee enumerar los documentos.</p> <p>Nota: Si ha seleccionado la opción [!DNL Google Docs] en este campo y no es un usuario de [!DNL Google Workspace], se devuelve el error <code>[400] Invalid Value</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td> <p>Establezca el número máximo de documentos que [!DNL Workfront Fusion] devuelve en un ciclo de ejecución.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener contenido de un documento]

Este módulo de acción recupera un documento especificado.

Es posible que tenga que ampliar los permisos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Obtener contenido de un documento]</td> 
   <td> <p>Seleccione si desea asignar el ID del documento o seleccione manualmente el documento en el menú desplegable.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad que contiene el documento que desea recuperar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta que contiene el documento que desea recuperar.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta que contiene el documento que desea recuperar.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible solo para usuarios de [!DNL Google Workspace])</p> <p>Seleccione si desea [!UICONTROL Utilizar acceso de administrador de dominio]. Al seleccionar [!UICONTROL Sí], se emite la solicitud como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida que contiene el documento que desea recuperar.</p> <p>Nota: Si ha seleccionado la opción [!DNL Google Docs] en este campo y no es un usuario de [!DNL Google Workspace], se devuelve el error <code>[400] Invalid Value</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filtro]</p> </td> 
   <td> <p>Seleccione el objeto que desea que se devuelva en la salida del módulo.</p> 
    <ul> 
     <li>[!UICONTROL Image] (predeterminado)</li> 
     <li>[!UICONTROL Dibujo]</li> 
     <li>[!UICONTROL Gráfico]</li> 
    </ul> <p>Nota:  <p>Para obtener más información sobre la asignación de estos objetos, utilice el valor [!UICONTROL Inline Objects Array] en la salida de este módulo (en lugar de [!UICONTROL inlineObjects]).</p> <p>Los objetos [!UICONTROL Inline Objects Array] se ordenan en el mismo orden en que aparecen en el documento. Facilitará cualquier procesamiento posterior.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un documento]

Este módulo de acción le permite crear un nuevo documento en la carpeta seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre] </td> 
   <td> <p>Introduzca el nombre del documento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contenido]</td> 
   <td> <p>Introduzca el contenido del documento. Se admite el HTML.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad donde desea crear un documento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta donde desea crear un documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta donde desea crear un documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible solo para usuarios de [!DNL Google Workspace])</p> <p>Seleccione si desea [!UICONTROL Utilizar acceso de administrador de dominio]. Al seleccionar [!UICONTROL Sí], se emite la solicitud como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida en la que desea crear un documento.</p> <p>Nota: Si ha seleccionado la opción [!DNL Google Docs] en este campo y no es un usuario de [!DNL Google Workspace], se devuelve el error <code>[400] Invalid Value</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Insertar encabezado]</td> 
   <td> <p> Active esta opción para insertar el encabezado en el documento y, a continuación, introduzca o asigne el texto del encabezado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Insertar un pie de página] </td> 
   <td> <p>Active esta opción para insertar el pie de página en el documento y, a continuación, introduzca o asigne el texto del encabezado.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un documento a partir de una plantilla]

Este módulo de acción crea una copia de un documento de plantilla existente y reemplaza las etiquetas. Este módulo también permite a los usuarios reemplazar imágenes con nuevas imágenes por URL.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Crear un documento a partir de una plantilla]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Seleccione esta opción para asignar la plantilla de documento.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br>Seleccione esta opción para elegir la plantilla de documento en el menú desplegable.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad en la que se encuentra la plantilla. Esta opción está disponible si seleccionó [!UICONTROL By Dropdown] en el campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta donde se encuentra la plantilla.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta donde se encuentra la plantilla.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible solo para usuarios de [!DNL Google Workspace])</p> <p>Seleccione si desea [!UICONTROL Utilizar acceso de administrador de dominio]. Al seleccionar [!UICONTROL Sí], se emite la solicitud como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida en la que se encuentra la plantilla.</p> <p>Nota: Si ha seleccionado la opción [!DNL Google Docs] en este campo y no es un usuario de [!DNL Google Workspace], se devuelve el error <code>[400] Invalid Value</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Valores]</p> </td> 
   <td> <p>Introduzca los valores que se introducirán en lugar de las variables en el nuevo documento.</p> 
    <ul> 
     <li><strong>[!UICONTROL Etiquetas]</strong> <br>Escriba las etiquetas que contiene la plantilla de documento. No use <code>&#123;&#123;&#125;&#125;</code>. Ejemplo: use <code>name</code> en lugar de <code>&#123;&#123;name&#125;&#125;</code>.</li> 
     <li><strong>[!UICONTROL Valor reemplazado]</strong><br>Escriba el valor de la etiqueta.</li> 
    </ul> <p>Por ejemplo, la variable <code> &#123;&#123;name&#125;&#125;</code> del documento de origen se mostrará como el campo de nombre aquí, donde se puede insertar el valor, como <code>John</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Images Replacement]</p> </td> 
   <td> <p>Introduzca el vínculo a [!UICONTROL Image Object ID] y [!UICONTROL Image URL] que reemplazarán la imagen actual.</p> <p>Nota: Puede recuperar los ID de imagen utilizando el módulo [!UICONTROL Get a Document], donde los ID se encuentran en la matriz [!UICONTROL Inline Object Array].</p> <p>Le recomendamos que agregue texto ALT a las imágenes de su documento [!DNL Google]. </p> <p>Para agregar un texto ALT a la imagen [!DNL Google Docs]:</p> 
    <ol> 
     <li value="1">Haga clic derecho en la imagen.</li> 
     <li value="2">Seleccione la opción [!UICONTROL ALT text].</li> 
     <li value="3">Introduzca el [!UICONTROL ALT text] en el campo [!UICONTROL Title] y haga clic en [!UICONTROL OK].</li> 
    </ol> <p>Una vez agregado el texto ALT a la imagen, el texto ALT se muestra entre paréntesis en el nombre del campo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Título] </td> 
   <td> <p>Introduzca el nombre del nuevo documento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad en la que se encuentra la plantilla. Esta opción está disponible si seleccionó [!UICONTROL By Dropdown] en el campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta donde desea crear el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta donde desea crear el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible solo para usuarios de [!DNL Google Workspace])</p> <p>Seleccione si desea [!UICONTROL Utilizar acceso de administrador de dominio]. Al seleccionar [!UICONTROL Sí], se emite la solicitud como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida en la que desea crear el documento.</p> <p>Nota: Si ha seleccionado la opción [!DNL Google Docs] en este campo y no es un usuario de [!DNL Google Workspace], se devuelve el error <code>[400] Invalid Value</code>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Insertar un párrafo en un documento]

Este módulo de acción anexa o inserta un párrafo nuevo en un documento existente.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Seleccionar un documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Seleccione esta opción para asignar el documento.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Seleccione esta opción para elegir el documento en el menú desplegable.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad en la que se encuentra el documento al que desea agregar un párrafo. Esta opción está disponible si seleccionó [!UICONTROL By Dropdown] en el campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta donde se encuentra el documento al que desea agregar un párrafo y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta donde se encuentra el documento al que desea agregar un párrafo y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible solo para usuarios de [!DNL Google Workspace])</p> <p>Seleccione si desea [!UICONTROL Utilizar acceso de administrador de dominio]. Al seleccionar [!UICONTROL Sí], se emite la solicitud como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida donde se encuentra el documento al que desea agregar un párrafo y, a continuación, seleccione el documento.</p> <p>Nota: Si ha seleccionado la opción [!DNL Google Docs] en este campo y no es un usuario de [!DNL Google Workspace], se devuelve el error <code>[400] Invalid Value</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Insertar un párrafo]</p> </td> 
   <td> <p>Seleccione cómo desea que se inserte el nuevo texto en el documento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Según especificación de ubicación]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Por índice]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Index]</strong> </p> <p>Introduzca el número de índice donde desea insertar el texto. Puede utilizar el módulo [!UICONTROL Get a Document] para recuperar el número de índice.</p> <p>Para mostrar todos los caracteres (incluidos los ocultos) del documento, puede utilizar el complemento [!UICONTROL Mostrar]. Puede encontrar el complemento en [!UICONTROL Complementos] &gt; [!UICONTROL Obtener complementos]. Busque [!UICONTROL Mostrar] e instale el complemento [!UICONTROL Mostrar].</p> </li> 
         <li> <p><strong>[!UICONTROL Texto insertado]</strong> </p> <p>Escriba el texto que desee insertar en el documento.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL Por ID de segmento]</strong> </p> <p>Seleccione el encabezado y el pie de página en los que desea insertar el contenido de texto e introduzca el texto que desea insertar en los campos correspondientes.</p> <p>Si el encabezado o pie de página ya contiene texto, el nuevo texto se agregará antes del texto existente.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Anexando al cuerpo del documento]</strong> </p> <p>Añade el texto introducido al final del contenido del cuerpo del documento.</p> <p>El estilo del nuevo párrafo se copiará del párrafo en el índice de inserción actual, incluidas las listas y viñetas.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Anexando al final del segmento (Encabezado y pie de página)]</strong> </p> <p>Seleccione el encabezado y el pie de página en los que desea insertar el contenido de texto e introduzca el texto que desea insertar en los campos correspondientes.</p> <p>Si el encabezado o pie de página ya contiene texto, el nuevo texto se agregará después del texto existente.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Texto anexado]</td> 
   <td>Escriba o asigne el texto que desea anexar al documento</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Insertar una imagen en un documento]

Este módulo de acción inserta una imagen desde la dirección URL al documento.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Seleccionar un documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Seleccione esta opción para asignar la plantilla de documento.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Seleccione esta opción para elegir el documento en el menú desplegable.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad donde se encuentra el documento al que desea agregar una imagen. Esta opción está disponible si seleccionó [!UICONTROL By Dropdown] en el campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta donde se encuentra el documento al que desea agregar una imagen y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta donde se encuentra el documento al que desea agregar una imagen y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible solo para usuarios de [!DNL Google Workspace])</p> <p>Seleccione si desea [!UICONTROL Utilizar acceso de administrador de dominio]. Al seleccionar [!UICONTROL Sí], se emite la solicitud como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida donde se encuentra el documento al que desea agregar una imagen y, a continuación, seleccione el documento.</p> <p>Nota: Si ha seleccionado la opción [!DNL Google Docs] en este campo y no es un usuario de [!DNL Google Workspace], se devuelve el error <code>[400] Invalid Value</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Insertar una imagen]</p> </td> 
   <td> <p>Seleccione cómo desea insertar la nueva imagen en el documento.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Según especificación de ubicación]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Por índice]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Index]</strong> </p> <p>Introduzca el número de índice donde desea insertar la imagen. Puede utilizar el módulo [!UICONTROL Obtener un documento] para recuperar [!UICONTROL Número de índice].</p> <p>Para mostrar todos los caracteres (incluidos los ocultos) del documento, puede utilizar el complemento [!UICONTROL Mostrar]. Puede encontrar el complemento en [!UICONTROL Complementos] &gt; [!UICONTROL Obtener complementos]. Busque [!UICONTROL Mostrar] e instale el complemento [!UICONTROL Mostrar].</p> </li> 
         <li> <p><strong>[!UICONTROL Image URL]</strong> </p> <p>Introduzca la dirección URL de la imagen que desea insertar en el documento.</p> <p>El tamaño máximo de imagen es 50 MB. No debe superar los 25 megapíxeles. Solo se admite el formato PNG, JPEG o GIF.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL Por ID de segmento]</strong> </p> <p>Seleccione el encabezado y pie de página en el que desea insertar la imagen e introduzca la URL de la imagen en los campos correspondientes.</p> <p>El tamaño máximo de imagen es 50 MB. La imagen no debe superar los 25 megapíxeles. Solo se admite el formato PNG, JPEG o GIF.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Anexando al cuerpo del documento]</strong> </p> <p>Adjunta una imagen específica al final del contenido del cuerpo del documento.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Anexando al final del segmento (Encabezado y pie de página)]</strong> </p> <p>Seleccione el encabezado y el pie de página en los que desea insertar una imagen e introduzca la URL de la imagen que desea insertar en los campos correspondientes.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Magnitud de altura en puntos/Magnitud de anchura en puntos]</p> </td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Seleccionar un documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Seleccione esta opción para asignar la plantilla de documento.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Seleccione esta opción para elegir el documento en el menú desplegable.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad donde se encuentra el documento que desea reemplazar una imagen. Esta opción está disponible si seleccionó [!UICONTROL By Dropdown] en el campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta en la que se encuentra el documento que desea reemplazar con una imagen y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta en la que se encuentra el documento que desea reemplazar con una imagen y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible solo para usuarios de [!DNL Google Workspace])</p> <p>Seleccione si desea [!UICONTROL Utilizar acceso de administrador de dominio]. Al seleccionar [!UICONTROL Sí], se emite la solicitud como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida en la que se encuentra el documento que desea reemplazar con una imagen y, a continuación, seleccione el documento.</p> <p>Nota: Si ha seleccionado la opción [!DNL Google Docs] en este campo y no es un usuario de [!DNL Google Workspace], se devuelve el error <code>[400] Invalid Value</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Image URL]</p> </td> 
   <td> <p>Introduzca o asigne la dirección URL de la nueva imagen que reemplazará la imagen existente.</p> <p>Las imágenes se muestran en el orden en que aparecen en el documento. Por ejemplo, <code>Body: Image No. 1</code> es la primera imagen del documento.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Seleccionar un documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Seleccione esta opción para asignar la plantilla de documento.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Seleccione esta opción para elegir el documento en el menú desplegable.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad en la que se encuentra el documento al que desea agregar texto. Esta opción está disponible si seleccionó [!UICONTROL By Dropdown] en el campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta donde se encuentra el documento al que desea agregar texto y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta donde se encuentra el documento al que desea agregar texto y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible solo para usuarios de [!DNL Google Workspace])</p> <p>Seleccione si desea [!UICONTROL Utilizar acceso de administrador de dominio]. Al seleccionar [!UICONTROL Sí], se emite la solicitud como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida en la que se encuentra el documento al que desea agregar texto y, a continuación, seleccione el documento.</p> <p>Nota: Si ha seleccionado la opción [!DNL Google Docs] en este campo y no es un usuario de [!DNL Google Workspace], se devuelve el error <code>[400] Invalid Value</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Reemplazar texto]</p> </td> 
   <td> <p>Agregue cada texto que desee reemplazar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Texto antiguo para reemplazar]</strong> </p> <p>Escriba el texto que desee reemplazar.</p> </li> 
     <li> <p><strong>[!UICONTROL Nuevo texto a insertar]</strong> </p> <p>Introduzca el nuevo texto.</p> </li> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad en la que se encuentra el documento que desea descargar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta en la que se encuentra el documento que desea descargar y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta en la que se encuentra el documento que desea descargar y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible solo para usuarios de [!DNL Google Workspace])</p> <p>Seleccione si desea [!UICONTROL Utilizar acceso de administrador de dominio]. Al seleccionar [!UICONTROL Sí], se emite la solicitud como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida en la que se encuentra el documento que desea descargar y, a continuación, seleccione el documento.</p> <p>Nota: Si ha seleccionado la opción [!DNL Google Docs] en este campo y no es un usuario de [!DNL Google Workspace], se devuelve el error <code>[400] Invalid Value</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo] </p> </td> 
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
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad en la que se encuentra el documento que desea eliminar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta en la que se encuentra el documento que desea eliminar y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta en la que se encuentra el documento que desea eliminar y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible solo para usuarios de [!DNL Google Workspace])</p> <p>Seleccione si desea [!UICONTROL Utilizar acceso de administrador de dominio]. Al seleccionar [!UICONTROL Sí], se emite la solicitud como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida en la que se encuentra el documento que desea eliminar y, a continuación, seleccione el documento.</p> <p>Nota: Si ha seleccionado la opción [!DNL Google Docs] en este campo y no es un usuario de [!DNL Google Workspace], se devuelve el error <code>[400] Invalid Value</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Unidad compartida]</td> 
   <td> <p>Seleccione la unidad que contiene el documento que desea descargar y, a continuación, seleccione un documento. Esta opción está disponible si ha seleccionado [!DNL Google Docs] en el campo [!UICONTROL Elegir una unidad].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de documento]</td> 
   <td> <p> Seleccione o asigne el documento en el que desea reemplazar una o varias imágenes.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Otro

* [[!UICONTROL Realizar una llamada API]](#make-an-api-call)
* [[!UICONTROL Hacer que todos los vínculos de un documento se puedan hacer clic]](#make-all-links-in-a-document-clickable)

#### [!UICONTROL Realizar una llamada API]

Este módulo de acción le permite realizar una llamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Escriba una ruta relativa a <code>https://docs.googleapis.com/</code>. Ejemplo: <code>/v1/documents/{presentationID}</code>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Agregue los encabezados de la solicitud en forma de objeto JSON estándar. Por ejemplo, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] agrega los encabezados de autorización por usted.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p> Introduzca la cadena de consulta de solicitud.</p> </td> 
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

**Ejemplo:** La siguiente llamada de API recupera los detalles del documento especificado en los documentos de Google:

**URL:**

/v1/documents/1ujkf-GDgB0TQSYPrxbCSK4Uso54tHVMqHZEVZZxB6aY

**Método:**

[!UICONTROL GET]

![](assets/api-call-example.png)

Los detalles del documento recuperado se encuentran en la salida del módulo en [!UICONTROL Paquete] > [!UICONTROL Cuerpo].

![](assets/api-output.png)

#### [!UICONTROL Hacer que todos los vínculos de un documento se puedan hacer clic]

Este módulo de acción busca todos los vínculos del documento y los hace seleccionables.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Conectar la aplicación o el servicio web del módulo a [!DNL Workfront Fusion]</a> en el artículo <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Hacer todos los vínculos de un documento]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Seleccione esta opción para asignar la plantilla de documento.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Seleccione esta opción para elegir el documento en el menú desplegable.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una unidad]</td> 
   <td> <p>Seleccione el tipo de unidad en la que se encuentra el documento en el que desea hacer clic en los vínculos. Esta opción está disponible si seleccionó [!UICONTROL By Dropdown] en el campo anterior.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mi unidad]</strong> </p> <p>Seleccione la carpeta en la que se encuentra el documento en el que desea hacer clic en los vínculos y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL Compartido Conmigo]</strong> </p> <p>Seleccione la carpeta en la que se encuentra el documento en el que desea hacer clic en los vínculos y, a continuación, seleccione el documento.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Unidad compartida]</strong> (disponible solo para usuarios de [!DNL Google Workspace])</p> <p>Seleccione si desea [!UICONTROL Utilizar acceso de administrador de dominio]. Al seleccionar [!UICONTROL Sí], se emite la solicitud como administrador de dominio y se devuelven todas las unidades compartidas en las que el solicitante es administrador.</p> <p>Seleccione la unidad compartida en la que se encuentra el documento en el que desea que se pueda hacer clic en los vínculos y, a continuación, seleccione el documento.</p> <p>Nota: Si ha seleccionado la opción [!DNL Google Docs] en este campo y no es un usuario de [!DNL Google Workspace], se devuelve el error <code>[400] Invalid Value</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Unidad compartida]</td> 
   <td> <p>Seleccione la unidad que contiene el documento en el que desea actualizar los vínculos y, a continuación, seleccione un documento. Esta opción está disponible si ha seleccionado [!DNL Google Docs] en el campo [!UICONTROL Elegir una unidad].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de documento]</td> 
   <td> <p> Seleccione o asigne el documento en el que desea actualizar los vínculos.</p> </td> 
  </tr> 
 </tbody> 
</table>
