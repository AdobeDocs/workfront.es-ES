---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de diapositivas de Google
description: Los módulos de diapositivas de Adobe Workfront Fusion Google le permiten crear, actualizar, mostrar en lista o eliminar presentaciones y cargar imágenes en presentaciones en su cuenta de diapositivas de Google.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 680a5328-1d50-4434-beda-7a4670a6e458
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1618'
ht-degree: 0%

---

# [!DNL Google Slides] módulos

Los módulos [!DNL Adobe Workfront Fusion] [!DNL Google Slides] le permiten crear, actualizar, mostrar en lista o eliminar presentaciones y cargar imágenes en presentaciones de su cuenta de [!DNL Google Slides].

Para usar [!DNL Google Slides] con [!DNL Workfront Fusion], es necesario tener una cuenta de [!DNL Google]. Si todavía no tiene una cuenta [!DNL Google], puede crearla en la página de ayuda de la cuenta [!DNL Google].

También necesita [!DNL Google Slides] en su [!DNL Google Drive].

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

Para usar módulos de [!DNL Google Slides], debe tener una cuenta de [!DNL Google].

## [!DNL Google Slides] módulos y sus campos

Al configurar [!DNL Google Slides] módulos, Workfront Fusion muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Google Slides] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Presentación](#presentation)
* [Otro](#other)

### Presentación

* [[!UICONTROL Ver Presentations]](#watch-presentations)
* [[!UICONTROL Lista de Presentations]](#list-presentations)
* [[!UICONTROL Obtener una presentación]](#get-a-presentation)
* [[!UICONTROL Obtener una página o miniatura]](#get-a-pagethumbnail)
* [[!UICONTROL Crear una presentación a partir de una plantilla]](#create-a-presentation-from-a-template)
* [[!UICONTROL Cargar una imagen en una presentación]](#upload-an-image-to-a-presentation)
* [[!UICONTROL Actualizar un gráfico]](#refresh-a-chart)
* [[!UICONTROL Agregar o eliminar una diapositiva]](#adddelete-a-slide)

#### [!UICONTROL Ver Presentations]

Déclencheur cuando se crea o actualiza una nueva presentación.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Slides] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch] </td> 
   <td> <p>Seleccione la opción para ver las presentaciones:</p> 
    <ul> 
     <li> <p>[!UICONTROL Fecha de creación]</p> </li> 
     <li> <p>[!UICONTROL Fecha de modificación]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Número máximo de presentaciones que Workfront Fusion debe devolver durante un ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Lista de Presentations]

Recupera una lista de todas las presentaciones.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Slides] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija una ubicación de unidad]</td> 
   <td> <p>Seleccione el(la) [!DNL Google Drive] donde se encuentran las presentaciones que desea enumerar:</p> 
    <ul> 
     <li>[!UICONTROL Mi unidad]</li> 
     <li>[!UICONTROL Compartido Conmigo]</li> 
     <li>Unidad compartida [!UICONTROL [!DNL Google]]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de carpeta]</td> 
   <td> <p>Elija la ubicación de la carpeta de las presentaciones que desea enumerar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Se debe devolver el número máximo de presentaciones [!DNL Workfront Fusion] durante un ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener una presentación]

Obtiene la última versión de una presentación especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Slides] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija una unidad]</td> 
   <td> <p>Seleccione el(la) [!DNL Google Drive] donde se encuentran las presentaciones que desea enumerar:</p> 
    <ul> 
     <li>[!UICONTROL Mi unidad]</li> 
     <li>[!UICONTROL Compartido Conmigo]</li> 
     <li>Unidad compartida [!UICONTROL [!DNL Google]]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de presentación]</td> 
   <td> <p> Seleccione la presentación que desea recuperar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener una página o miniatura]

Obtiene la última versión de la página especificada o de la miniatura de una página de la presentación.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Slides] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de presentación]</td> 
   <td> <p> Seleccione el ID de presentación que desee recuperar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Page Object ID]</td> 
   <td> <p> Seleccione la diapositiva para la que desea ver los detalles del objeto de página.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mostrar miniatura de página]</td> 
   <td> <p> Seleccione la casilla de verificación si desea ver la información de la miniatura de la página.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear una presentación a partir de una plantilla]

Crea una nueva presentación reemplazando todas las etiquetas como `{{Name}}`, `{{Email}}` en una plantilla con los datos proporcionados.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Slides] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Título] </td> 
   <td> <p>Escriba un nombre para la nueva presentación.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copiar una presentación]</td> 
   <td> <p> Seleccione la opción si está copiando una presentación existente:</p> 
    <ul> 
     <li>[!UICONTROL Por Asignación]</li> 
     <li>[!UICONTROL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copia de ID de presentación existente]</td> 
   <td> <p> Introduzca la ruta o el ID de presentación de una presentación existente que desee copiar. Este campo aparece si está creando la presentación [!UICONTROL By Mapping].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija una unidad]</td> 
   <td> <p>Seleccione el(la) [!DNL Google Drive] donde se encuentran las presentaciones que desea enumerar:</p> 
    <ul> 
     <li>[!UICONTROL Mi unidad]</li> 
     <li>[!UICONTROL Compartido Conmigo]</li> 
     <li>Unidad compartida [!UICONTROL [!DNL Google]]</li> 
    </ul> <p>Este campo aparece si está creando la presentación [!UICONTROL By Dropdown].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de presentación]</td> 
   <td> <p> Seleccione el ID de presentación de la presentación que desee utilizar como plantilla.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valores] </td> 
   <td> <p>Añada los valores:</p> 
    <ul> 
     <li><strong>[!UICONTROL Tag]</strong>: Escriba la etiqueta que desee reemplazar en la presentación. Por ejemplo, <code>&#123;&#123;Name&#125;&#125;</code></li> 
     <li><strong>[!UICONTROL Valor reemplazado]</strong>: escriba el valor con el que se reemplazará la etiqueta existente. Por ejemplo, si una cadena <tr><ul><tr><tr><tr><code>&#123;&#123;Name&#125;&#125;/code> in the presentation and the replaced value is Sample, then the <code>&#123;&#123;Name}}</code> will be replaced by <code>Sample</code>.</li> 
    </ul> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL New Drive Location]</td> 
   <td> <p>Select the [!DNL Google Drive] where you want to store or add the new presentation:</p> 
     
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared With Me]</li> 
     <li>[!UICONTROL [!DNL Google] Shared Drive]</li> 
    </ul> </td> 
  </tr> 
   
   <td role="rowheader"> <p>[!UICONTROL New Document's Location]</p> </td> 
   <td> <p>Select the folder where you want to store or add the presentation.</p> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL Shared] </td> 
   <td> <p>Select if you want to share the presentation.</p> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL Sharing with Other's Email Address]</td> 
   <td> <p> Enter the email address with whom you want to share the presentation. If you are not entering an email address and selecting only shared field, the presentation is shareable to anyone.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cargar una imagen en una presentación]

Carga una imagen con los datos proporcionados.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Slides] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una presentación]</td> 
   <td> <p>Elija cómo desea seleccionar la presentación en la que está cargando una imagen.</p> 
    <ul> 
     <li>[!UICONTROL Por Asignación]</li> 
     <li>[!DNL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija una unidad]</td> 
   <td> <p>Seleccione el(la) [!DNL Google Drive] donde se encuentran las presentaciones que desea enumerar:</p> 
    <ul> 
     <li>[!UICONTROL Mi unidad]</li> 
     <li>[!UICONTROL Compartido Conmigo]</li> 
     <li>Unidad compartida [!UICONTROL [!DNL Google]]</li> 
    </ul> <p>Este campo aparece si está creando la presentación [!UICONTROL By Dropdown].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de presentación]</td> 
   <td> <p> Seleccione el ID de presentación de la presentación en la que está cargando la imagen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valores]</td> 
   <td> <p>Valores Agregue los valores:</p> 
    <ul> 
     <li><strong>[!UICONTROL Tag]</strong>: escriba la etiqueta a la que desea agregar la dirección URL.</li> 
     <li><strong>[!UICONTROL Image URL]</strong>: escriba la ruta de acceso o la dirección URL de la imagen que desea cargar.</li> 
    </ul> <p>Nota: Las imágenes deben tener un tamaño inferior a 50 MB, no pueden superar los 25 megapíxeles y deben estar en formato PNG, JPEG o GIF.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar un gráfico]

Actualiza los datos del gráfico almacenados en una presentación especificada por el identificador.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Slides] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija una unidad]</td> 
   <td> <p>Seleccione el(la) [!DNL Google Drive] donde se encuentran las presentaciones que desea enumerar:</p> 
    <ul> 
     <li>[!UICONTROL Mi unidad]</li> 
     <li>[!UICONTROL Compartido Conmigo]</li> 
     <li>Unidad compartida [!UICONTROL [!DNL Google]]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de presentación]</td> 
   <td> <p>Seleccione el ID de presentación de la presentación que incluye el gráfico que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de objeto de gráfico]</td> 
   <td> <p> Seleccione el gráfico que desea actualizar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Agregar o eliminar una diapositiva]

Crea una diapositiva vacía o elimina una diapositiva existente de la presentación especificada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Slides] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccione el método]</td> 
   <td> <p>Elija si desea agregar o eliminar una diapositiva nueva.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Presentation ID]</td> 
   <td> <p>Seleccione el ID. de presentación de la presentación para la que desea agregar o eliminar una diapositiva.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de diseño predefinido]</td> 
   <td> <p> Seleccione el diseño de diapositiva predefinido que desea que utilice la diapositiva agregada. Especifique valores para cualquier campo adicional (como [!UICONTROL Title]).</p> 
    <ul> 
     <li>[!UICONTROL Diseño en blanco, sin marcadores de posición]</li> 
     <li>[!UICONTROL Diseño con un título en la parte inferior]</li> 
     <li>[!UICONTROL Diseño con título y subtítulo]</li> 
     <li>[!UICONTROL Diseño con título y cuerpo]</li> 
     <li>[!UICONTROL Diseño con un título y dos columnas]</li> 
     <li>[!UICONTROL Diseño con solo un título]</li> 
     <li>[!UICONTROL Diseño con título de sección]</li> 
     <li>[!UICONTROL Diseño con título y subtítulo en una cara y descripción en la otra]</li> 
     <li>[!UICONTROL Diseño con un título y un cuerpo, organizados en una sola columna]</li> 
     <li>[!UICONTROL Diseño con punto principal]</li> 
     <li>[!DNL Layout with a big number heading]</li> 
    </ul> <p>Este campo está disponible si ha seleccionado añadir una diapositiva.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Otro

* [[!UICONTROL Realizar una llamada API]](#make-an-api-call)
* [[!UICONTROL Insertar vínculos en una presentación]](#insert-links-in-a-presentation)

#### [!UICONTROL Realizar una llamada API]

Realiza una llamada de API autorizada arbitraria.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Slides] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Escriba una ruta relativa a https://developers.google.com/slides/. Por ejemplo, Presentación.</p> <p>Para obtener la lista de extremos disponibles, consulte la <a href="https://developers.google.com/slides/reference/rest">[!DNL Google Slides] Documentación de la API </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Introduzca los encabezados de solicitud deseados. No es necesario agregar encabezados de autorización.</p> </td> 
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

>[!INFO]
>
>**Ejemplo:** Con una llamada de API, puede obtener los detalles de presentación del identificador de presentación que ha especificado. Puede encontrar el identificador de presentación en la dirección URL cuando abra la presentación en [!DNL Google Slides].
>
>![](assets/api-call-350x13.png)
>
>La siguiente llamada de API devuelve los detalles de la presentación:
>
>![](assets/presentation-details.png)
>
>Las coincidencias de la búsqueda se encuentran en la salida del módulo en [!UICONTROL Paquete] > [!UICONTROL Cuerpo] > [!UICONTROL presentationId].
>
>En nuestro ejemplo, se han devuelto los detalles de presentación solicitados:
>
>![](assets/presentation-details-2.png)

#### [!UICONTROL Insertar vínculos en una presentación]

Este módulo permite hacer clic en todos los vínculos de una presentación o inserta un vínculo en todos los textos de entrada coincidentes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión] </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Google Slides] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elegir una presentación]</td> 
   <td> <p>Elija cómo desea seleccionar la presentación en la que está cargando una imagen.</p> 
    <ul> 
     <li>[!UICONTROL Por Asignación]</li> 
     <li>[!UICONTROL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Elija una unidad]</td> 
   <td> <p>Seleccione el(la) [!DNL Google Drive] donde se encuentran las presentaciones que desea enumerar:</p> 
    <ul> 
     <li>[!UICONTROL Mi unidad]</li> 
     <li>[!UICONTROL Compartido Conmigo]</li> 
     <li>Unidad compartida [!UICONTROL [!DNL Google]]</li> 
    </ul> <p>Este campo aparece si está creando la presentación [!UICONTROL By Dropdown].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de presentación]</td> 
   <td> <p>Elija la ubicación de la carpeta de las presentaciones que desea enumerar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar]</td> 
   <td> <p>Seleccione si desea que todos los vínculos de una presentación se puedan seleccionar o si desea insertar un vínculo en todos los textos de entrada coincidentes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entradas de texto]</td> 
   <td>Para cada elemento de texto para el que desee agregar un vínculo, agregue a la lista el elemento y su vínculo asociado. Cada vez que el elemento aparece en la presentación, se vinculará automáticamente al sitio especificado.</td> 
  </tr> 
 </tbody> 
</table>
