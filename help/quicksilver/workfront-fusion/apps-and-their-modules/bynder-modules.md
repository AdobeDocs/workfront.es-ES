---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos Bynder
description: En un  [!DNL Adobe Workfront Fusion] escenario, puede automatizar los flujos de trabajo que usan [!DNL Bynder], así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: e4dc9588-334a-41a3-85d1-996cb819c3fa
source-git-commit: 2e91e9a4c691430f3c98e3cbddb30706ea57f84a
workflow-type: tm+mt
source-wordcount: '1676'
ht-degree: 0%

---

# [!DNL Bynder] módulos

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!DNL Bynder], así como conectarlo a varias aplicaciones y servicios de terceros.

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

Para usar módulos de [!DNL Bynder], debe tener una cuenta de [!DNL Bynder].

## Información de API de Bynder

El conector Bynder utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Versión de API</td> 
   <td> v4 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 1.25.21</td> 
  </tr>
 </tbody> 
 </table>

## Conectar [!DNL Bynder] a Workfront Fusion  {#connect-bynder-to-workfront-fusion}

* [Crear una conexión con [!DNL Bynder] from [!DNL Workfront Fusion]](#create-a-connection-to-bynder-from-workfront-fusion)
* [Generar un [!UICONTROL ID de cliente] y [!UICONTROL Secreto de cliente] en [!DNL Bynder] (opcional)](#generate-a-client-id-and-client-secret-in-bynder-optional)

### Crear una conexión con [!DNL Bynder] desde [!DNL Workfront Fusion]

Puede crear una conexión desde [!DNL Workfront Fusion] a su cuenta de [!DNL Bynder] directamente desde un módulo de [!DNL Bynder].

1. En cualquier módulo de [!DNL Bynder], haga clic en **[!UICONTROL Agregar]** junto al campo [!UICONTROL Conexión].
1. Seleccione el dominio [!DNL Bynder] al que desea conectarse.
1. (Opcional) Haga clic en **[!UICONTROL Configuración avanzada]** y, a continuación, introduzca su [!UICONTROL ID de cliente] y [!UICONTROL Secreto de cliente].

   Para obtener instrucciones sobre cómo generar el ID de cliente y el Secreto de cliente, consulte [Generar un ID de cliente y un Secreto de cliente en [!DNL Bynder] (opcional)](#generate-a-client-id-and-client-secret-in-bynder-optional) en este artículo.

1. En la ventana [!UICONTROL login], ingrese su nombre de usuario (dirección de correo electrónico) y contraseña.
1. Haga clic en **[!UICONTROL Continuar]** para crear la conexión y volver al módulo.

### Generar un [!UICONTROL ID de cliente] y [!UICONTROL Secreto de cliente] en [!DNL Bynder] (opcional)

Si desea crear una conexión utilizando el ID de cliente y el Secreto de cliente, puede generarlos desde su cuenta de [!DNL Bynder]. El ID de cliente y el Secreto de cliente se generan al crear una aplicación en [!DNL Bynder].

Para obtener instrucciones para crear una aplicación en [!DNL Bynder], consulte [Aplicaciones de Oauth 2.0](https://developer-docs.bynder.com/api/authentication-oauth2-oauth-apps/) en la documentación de [!DNL Bynder].

>[!NOTE]
>
>Al crear la aplicación en [!DNL Bynder], escriba lo siguiente como `redirect uri`:
>
>`https://app.workfrontfusion.com/oauth/cb/workfront-bynder`

## [!DNL Bynder] módulos y sus campos

Al configurar [!DNL Bynder] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Bynder] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Acciones](#actions)
* [Búsquedas](#searches)
* [Déclencheur](#triggers)

### Acciones

* [[!UICONTROL Llamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Leer metadatos de recursos]](#read-asset-metadata)
* [[!UICONTROL Actualizar metadatos de recursos]](#update-asset-metadata)
* [[!UICONTROL Agregar recursos a una colección]](#add-assets-to-a-collection)
* [[!UICONTROL Quitar recursos de la colección]](#remove-assets-from-collection)
* [[!UICONTROL Agregar una etiqueta a los recursos]](#add-a-tag-to-assets)
* [[!UICONTROL Quitar una etiqueta] de los recursos](#remove-a-tag-from-assets)
* [[!UICONTROL Descargar recurso]](#download-asset)
* [[!UICONTROL Cargar recurso]](#upload-asset)

#### [!UICONTROL Llamada de API personalizada]

Este módulo de acción le permite realizar una llamada autenticada personalizada a la API [!DNL Bynder]. De este modo, puede crear una automatización del flujo de datos que no puedan realizar los otros [!DNL Bynder] módulos.

Al configurar este módulo, se muestran los campos siguientes.

El módulo devuelve un código de estado, junto con los encabezados y el cuerpo de la llamada de API.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Bynder] a [!DNL Workfront Fusion], vea <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Escriba una ruta relativa a <code>https://{your-bynder-domain}/api/{api-version}/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   td&gt; <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion añade los encabezados de autorización por usted.</p> </td> 
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

#### [!UICONTROL Leer metadatos de recursos]

Este módulo de acción lee los metadatos de un recurso.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Bynder] a [!DNL Workfront Fusion], vea <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de recurso]</td> 
   <td>Introduzca o asigne el ID del recurso para el que desea recuperar los metadatos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione la información que desee incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar metadatos de recursos]

Este módulo de acción actualiza los metadatos de un recurso existente.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Bynder] a [!DNL Workfront Fusion], vea <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de recurso]</td> 
   <td>Introduzca o asigne el ID del recurso para el que desea actualizar los metadatos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campos]</td> 
   <td> <p>Seleccione los campos para los que desea introducir información y, a continuación, introduzca o asigne la información con la que desea actualizar los metadatos en esos campos. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Metaproperties]</p> </td> 
   <td>Seleccione las opciones que desea actualizar y, a continuación, introduzca o asigne la información a esas propiedades. Las metapropiedades son información sobre el recurso que no representa campos específicos en el recurso.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Agregar recursos a una colección]

Este módulo de acción agrega uno o más recursos a una colección.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Bynder] a [!DNL Workfront Fusion], vea <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de colección]</td> 
   <td> <p>Introduzca o asigne el ID de la colección a la que desea agregar recursos.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de recursos]</td> 
   <td> <p>Para cada recurso que desee agregar a la colección, haga clic en <strong>[!UICONTROL Agregar elemento]</strong> y, a continuación, escriba o asigne el ID del recurso.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Quitar recursos de la colección]

Este módulo de acción elimina uno o varios recursos de una colección.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Bynder] a [!DNL Workfront Fusion], vea <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de colección]</td> 
   <td> <p>Introduzca o asigne el ID de la colección en la que desea eliminar los recursos.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de recursos]</td> 
   <td> <p>Para cada recurso que desee eliminar de la colección, haga clic en <strong>[!UICONTROL Agregar elemento]</strong> y, a continuación, escriba o asigne el ID del recurso.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Agregar una etiqueta a los recursos]

Añadir una etiqueta a uno o varios recursos

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Bynder] a [!DNL Workfront Fusion], vea <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de etiqueta]</td> 
   <td> <p>Introduzca o asigne el ID de la etiqueta que desea agregar a los recursos.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de recursos]</td> 
   <td> <p>Para cada recurso que desee etiquetar, haga clic en <strong>[!UICONTROL Agregar elemento]</strong> y, a continuación, escriba o asigne el ID del recurso.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Quitar una etiqueta de los recursos]

Eliminación de una etiqueta de uno o varios recursos

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Bynder] a [!DNL Workfront Fusion], vea <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de etiqueta]</td> 
   <td> <p>Introduzca o asigne el ID de la etiqueta que desea eliminar de los recursos.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de recursos]</td> 
   <td> <p>Para cada recurso del que desee quitar una etiqueta, haga clic en <strong>[!UICONTROL Agregar elemento]</strong> y, a continuación, escriba o asigne el ID del recurso.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Descargar recurso]

Este módulo de acción descarga un solo recurso.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Bynder] a [!DNL Workfront Fusion], vea <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID de recurso]</td> 
   <td>Introduzca o asigne el ID del recurso que desea descargar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset version]</td> 
   <td> <p>Introduzca o asigne la versión del recurso que desea descargar. Para descargar la última versión del recurso, deje vacío el campo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Cargar recurso]

Este módulo de acción carga un solo recurso.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Bynder] a [!DNL Workfront Fusion], vea <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Guardar como]</td> 
   <td> <p>Seleccione cómo desea guardar el archivo que está cargando.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nuevo recurso]</strong> </p> <p>Seleccione los campos y las metapropiedades para los que desea introducir información y, a continuación, introduzca la información en esos campos.</p> <p>Introduzca o asigne el ID de la marca que desea utilizar para el recurso cargado.</p> </li> 
     <li> <p><strong>[!UICONTROL Nueva versión del recurso]</strong> </p> <p>Introduzca el ID del recurso para el que está cargando una nueva versión.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL archivo Source]</td> 
   <td>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

* [[!UICONTROL Registro de lista]](#list-record)
* [[!UICONTROL Buscar recursos]](#search-for-assets)

#### [!UICONTROL Registro de lista]

Este módulo de búsqueda recupera todos los elementos de un tipo específico.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Bynder] a [!DNL Workfront Fusion], vea <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro que desea enumerar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Leer todas las colecciones]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Leer información sobre todas las etiquetas]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Leer todos los recursos de una colección]</strong> </p> <p>Introduzca o asigne el ID de la colección de la que desea enumerar los recursos.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione los campos que desea incluir en la salida del módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de recursos que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Buscar recursos]

Este módulo de búsqueda busca recursos en función de los criterios proporcionados.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Bynder] a [!DNL Workfront Fusion], vea <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Criterios]</td> 
   <td> <p>Introduzca los criterios de búsqueda. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Campo]</strong> </p> <p>Seleccione el campo que desee utilizar en la búsqueda</p> </li> 
     <li> <p><strong>[!UICONTROL Operador lógico]</strong> </p> <p>Seleccione el operador que desee utilizar en la búsqueda.</p> </li> 
     <li> <p><strong>[!UICONTROL Valor]</strong> </p> <p>Introduzca o asigne el valor que desea buscar en el campo seleccionado. El tipo de valor debe ser el mismo que el tipo de datos del campo seleccionado. </p> <p>Para obtener más información sobre los tipos de datos, vea <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Tipos de datos de elementos en [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conjunto de resultados]</td> 
   <td>Seleccione si desea devolver el primer recurso coincidente o todos los recursos coincidentes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordenar por]</td> 
   <td> <p>Seleccione el campo por el que desea ordenar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dirección de orden]</td> 
   <td> <p>Seleccione si desea ordenar de forma ascendente o descendente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione los campos que desea incluir en la salida del módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de recursos que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Déclencheur

#### [!UICONTROL Observar recursos]

Este módulo de déclencheur inicia un escenario cuando se crea o actualiza un recurso.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Bynder] a [!DNL Workfront Fusion], vea <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Bynder] a [!DNL Workfront Fusion] </a> en este artículo.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Event type</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select whether you want to start the scenario when a new asset is created or when an existing asset is updated.</td>
   --> 
  </tr> 
  <tr>
     <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Colecciones]</td>
   <td> <p>Seleccione la colección que desea inspeccionar para ver si hay nuevos recursos. Para ver todas las colecciones, deje este campo vacío.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Outputs</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the fields that you want to include in the output.</td>
   --> 
  </tr> 
  <tr> 
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Límite]</td>

<td> <p>Introduzca el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>
