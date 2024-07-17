---
title: Ampliar módulos
description: En un escenario  [!DNL Adobe Workfront Fusion] puede automatizar los flujos de trabajo que usan [!UICONTROL Widen], así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: d46935bc-4f6c-4502-bd2f-3927f33241e1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1582'
ht-degree: 1%

---

# [!DNL Widen] módulos

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que usan [!UICONTROL Widen], así como conectarlo a varias aplicaciones y servicios de terceros.

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

Para usar módulos [!UICONTROL Widen], debes tener una cuenta de [!UICONTROL Widen].

## Conectar [!DNL Widen] a [!DNL Workfront Fusion] {#connect-widen-to-workfront-fusion}

Puede crear una conexión con su cuenta de [!DNL Widen] directamente desde un módulo de [!DNL Widen].

1. En cualquier módulo de [!DNL Widen], haga clic en **[!UICONTROL Agregar]** junto al campo [!UICONTROL Conexión].
1. Seleccione el dominio [!DNL Widen] al que desea conectarse.
1. Escriba el token para su cuenta de [!DNL Widen]. Para obtener instrucciones sobre cómo localizar este token, consulte las [[!DNL Widen] preguntas frecuentes sobre API](https://community.widen.com/collective/s/article/API-FAQs).
1. Haga clic en **[!UICONTROL Continuar]** para crear la conexión y volver al módulo.

## [!DNL Widen] módulos y sus campos

Al configurar [!DNL Widen] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Widen] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Módulos de activador](#trigger-modules)
* [Módulos de acción](#action-modules)
* [Buscar módulos](#search-modules)

### Módulos de activador

#### [!UICONTROL Observar recursos]

Este módulo de déclencheur inicia un escenario cuando se crea o actualiza un recurso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
  <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Widen] a [!DNL Workfront Fusion], vea <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Widen] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de evento]</td> 
   <td> <p>Seleccione si desea ver recursos nuevos o actualizados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expandir]</td> 
   <td> <p>Seleccione las propiedades que desee incluir en la salida del módulo además de los campos de recurso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td>Seleccione los campos que desea incluir en la salida del módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de recursos con los que desea que trabaje el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Módulos de acción

* [[!UICONTROL Llamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Leer información de recurso]](#read-asset-info)
* [[!UICONTROL Agregar recursos a colecciones]](#add-assets-to-collections)
* [[!UICONTROL Quitar recursos de la colección]](#remove-assets-from-collection)
* [[!UICONTROL Actualizar metadatos de recursos]](#update-asset-metadata)
* [[!UICONTROL Descargar archivo]](#download-file)
* [[!UICONTROL Cargar] un archivo](#upload-a-file)

#### [!UICONTROL Llamada de API personalizada]

Este módulo de acción le permite realizar una llamada autenticada personalizada a la API [!DNL Widen]. De este modo, puede crear una automatización del flujo de datos que no puedan realizar los otros [!DNL Widen] módulos.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Widen] a [!DNL Workfront Fusion], vea <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Widen] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API Version]</td> 
   <td>Seleccione si desea utilizar la última versión de la API [!DNL Widen] o la versión 1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Introduzca o asigne la dirección URL de su llamada de API.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] agrega los encabezados de autorización automáticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p> </td> 
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

#### [!UICONTROL Leer información de recurso]

Este módulo de acción recupera un recurso individual por su ID único.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
  <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Widen] a [!DNL Workfront Fusion], vea <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Widen] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de recurso]</td> 
   <td> <p>Introduzca o asigne el ID del recurso para el que desea leer información.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expandir]</td> 
   <td> <p>Seleccione las propiedades que desee incluir en la salida del módulo además de los campos de recurso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td>Seleccione los campos que desea incluir en la salida del módulo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Agregar recursos a colecciones]

Este módulo de acción añade uno o más recursos a las colecciones.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
  <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Widen] a [!DNL Workfront Fusion], vea <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Widen] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de colecciones]</td> 
   <td> <p>Para cada colección a la que desee agregar los recursos:</p> 
    <ol> 
     <li value="1"> <p> Haga clic en <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Escriba o asigne el [!UICONTROL ID de colección].</p> </li> 
     <li value="3"> <p>Haga clic en <strong>[!UICONTROL Agregar elemento]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assets ID]</td> 
   <td> <p>Para cada recurso que desee agregar a una colección:</p> 
    <ol> 
     <li value="1"> <p> Haga clic en <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Introduzca o asigne el ID de recurso.</p> </li> 
     <li value="3"> <p>Haga clic en <strong>[!UICONTROL Agregar elemento]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de recursos con los que desea que trabaje el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Quitar recursos de la colección]

Este módulo de acción elimina uno o varios recursos de las colecciones.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
  <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Widen] a [!DNL Workfront Fusion], vea <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Widen] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de colecciones]</td> 
   <td> <p>Para cada colección de la que desee eliminar los recursos:</p> 
    <ol> 
     <li value="1"> <p> Haga clic en <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Introduzca o asigne el ID de colección.</p> </li> 
     <li value="3"> <p>Haga clic en <strong>[!UICONTROL Agregar elemento]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ASSETS ID</td> 
   <td> <p>Para cada recurso que desee eliminar de una colección:</p> 
    <ol> 
     <li value="1"> <p> Haga clic en <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Introduzca o asigne el ID de recurso.</p> </li> 
     <li value="3"> <p>Haga clic en <strong>[!UICONTROL Agregar elemento]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de recursos con los que desea que trabaje el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar metadatos de recursos]

Este módulo de acción actualiza los campos de metadatos de un recurso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
  <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Widen] a [!DNL Workfront Fusion], vea <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Widen] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de recurso]</td> 
   <td> <p>Introduzca o asigne el ID del recurso donde desea actualizar los metadatos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de metadatos]</td> 
   <td> <p>Seleccione el tipo de metadatos para los metadatos que desea actualizar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadatos]</td> 
   <td>Seleccione los campos de metadatos que desea actualizar. Para cada campo, introduzca el nuevo valor para el campo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de recursos con los que desea que trabaje el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Descargar archivo]

Este módulo de acción descarga un recurso de su cuenta de [!DNL Widen].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
  <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Widen] a [!DNL Workfront Fusion], vea <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Widen] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de recurso]</td> 
   <td> <p>Introduzca o asigne el ID del recurso que desea descargar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cargar un archivo]

Este módulo de acción carga un archivo en su cuenta de [!DNL Widen].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
  <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Widen] a [!DNL Workfront Fusion], vea <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Widen] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cargar perfil]</td> 
   <td> <p>Seleccione el perfil de carga que desea que utilice el módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método de carga]</td> 
   <td> <p>Seleccione cómo desea cargar el archivo.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Desde Archivo]</strong> </p> <p>Seleccione o asigne el archivo de origen de un módulo anterior.</p> </li> 
     <li> <p><strong>[!UICONTROL Por dirección URL]</strong> </p> <p>Introduzca o asigne la dirección URL del archivo que desea cargar.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de archivo]</td> 
   <td>Introduzca o asigne un nombre para el archivo cargado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de metadatos]</td> 
   <td>Seleccione el tipo de metadatos del archivo que desea cargar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadatos]</td> 
   <td>Seleccione los campos de metadatos que desee incluir en la carga del archivo. Para cada campo, introduzca el [!UICONTROL valor] para el campo.</td> 
  </tr> 
 </tbody> 
</table>

### Buscar módulos

* [[!UICONTROL Leer recursos de colección]](#read-collection-assets)
* [[!UICONTROL Buscar recursos]](#search-assets)

#### [!UICONTROL Leer recursos de colección]

Este módulo de acción recupera una lista de recursos dentro de una colección.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
  <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Widen] a [!DNL Workfront Fusion], vea <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Widen] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de colección]</td> 
   <td> <p>Introduzca o asigne el ID de la colección que contiene los recursos que desea leer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Iniciar]</td> 
   <td>Escriba o asigne el número del primer elemento que desee enumerar. Esta es una forma de paginar los registros.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordenar por]</td> 
   <td> <p>Seleccione la propiedad según la cual desea ordenar los recursos. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pedido]</td> 
   <td>Seleccione si desea ordenar los recursos de forma ascendente o descendente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td>Seleccione los campos que desea incluir en la salida del módulo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Buscar recursos]

Este módulo de búsqueda recupera una lista de recursos que coinciden con los criterios de búsqueda específicos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
  <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Widen] a [!DNL Workfront Fusion], vea <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Widen] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Consulta de búsqueda]</td> 
   <td> <p>Introduzca los criterios según los cuales quiere buscar recursos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordenar por]</td> 
   <td> <p>Seleccione cómo desea ordenar los recursos. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pedido]</td> 
   <td>Seleccione si desea ordenar los recursos de forma ascendente o descendente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Incluir eliminado]</td> 
   <td>Active esta opción para incluir los recursos eliminados en la búsqueda.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Incluir archivado]</p> </td> 
   <td> <p>Active esta opción para incluir recursos archivados en la búsqueda.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Buscar texto de documento]</td> 
   <td>Active esta opción para incluir el texto del documento en la búsqueda o false para incluir solo los recursos cuyo título coincida con los criterios de búsqueda.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Desplazamiento]</td> 
   <td>Introduzca o asigne el número del primer elemento para el que desea recuperar detalles. Esta es una forma de paginar los registros.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Desplazamiento]</td> 
   <td>Active esta opción para permitir el desplazamiento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expandir]</td> 
   <td> <p>Seleccione las propiedades que desee incluir en la salida del módulo además de los campos de recurso.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td>Seleccione los campos que desea incluir en la salida del módulo.</td> 
  </tr> 
 </tbody> 
</table>
