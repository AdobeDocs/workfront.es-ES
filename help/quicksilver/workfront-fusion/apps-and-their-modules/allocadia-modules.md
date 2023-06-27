---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Allocadia
description: En un [!DNL Adobe Workfront Fusion] En este escenario, puede automatizar los flujos de trabajo que utilizan Allocadia, así como conectarlo a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: f1edefd1-9fe0-48fc-bea2-c3f9facf7363
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1401'
ht-degree: 0%

---

# [!DNL Allocadia] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Allocadia], así como conectarlo a múltiples aplicaciones y servicios de terceros.

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

Para usar [!DNL Allocadia] módulos, debe tener un [!DNL Allocadia] cuenta.

## Connect [!DNL Allocadia] hasta [!DNL Workfront Fusion]

Puede crear una conexión con su [!DNL Allocadia] cuenta directamente desde dentro de un [!DNL Allocadia] módulo.

1. En cualquier [!DNL Allocadia] , haga clic en **[!UICONTROL Añadir]** junto al [!UICONTROL Conexión] field.
1. Seleccione si desea utilizar el servidor de Norteamérica o el de Europa.
1. Introduzca su nombre de usuario y contraseña.
1. Clic **[!UICONTROL Continuar]** para crear la conexión y volver al módulo.

## [!DNL Allocadia] módulos y sus campos

Al configurar [!DNL Allocadia] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, se añaden [!DNL Allocadia] Los campos pueden mostrarse, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheur](#triggers)
* [Acciones](#actions)
* [Búsquedas](#searches)

### Déclencheur

#### [!UICONTROL Ver registro]

Este módulo de déclencheur ejecuta un escenario cuando se añaden, actualizan o ambos objetos de un tipo específico. El módulo devuelve todos los campos estándar asociados con el registro o registros, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> <table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de Allocadia a [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Conectar Allocadia] a Workfront Fusion</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filtro</td> 
   <td> <p>Seleccione si desea que el escenario vea Sólo registros nuevos, [!UICONTROL Sólo registros actualizados] o Registros nuevos y actualizados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo de entidad</td> 
   <td>Seleccione el tipo de registro de Allocadia que desea que vea el módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Salidas</td> 
   <td> <p>Seleccione los campos que desea incluir en la salida del módulo. Los campos disponibles dependen del tipo de entidad seleccionado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Límite</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo vea durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [Llamada de API personalizada](#custom-api-call)
* [Leer registro](#read-record)
* [Crear registro](#create-record)
* [Eliminar registro](#delete-record)
* [Actualizar registro](#update-record)

#### [!UICONTROL Llamada de API personalizada]

Este módulo de acción le permite realizar una llamada autenticada personalizada a [!DNL Allocadia] API. De este modo, se puede crear una automatización del flujo de datos que el otro no puede realizar [!DNL Allocadia] módulos.

La acción se basa en el tipo de entidad (tipo de objeto Allocadia) especificado.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Allocadia] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Introduzca una ruta relativa a <code>https://api-na.allocadia.com/{version}</code> o <code>https://api-eu.allocadia.com/{version}</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] agrega los encabezados de autorización automáticamente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuerpo]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando se utilizan afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera del enunciado condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leer registro]

Este módulo de acción lee datos de un único registro en [!DNL Allocadia].

Especifique el ID del registro.

El módulo devuelve cualquier campo estándar asociado con el registro, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Allocadia] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidad]</td> 
   <td>Seleccione el tipo de [!DNL Allocadia] que desea que el módulo lea.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione los campos que desea incluir en la salida del módulo. Los campos disponibles dependen del [!UICONTROL Entity Type] seleccionado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Introduzca o asigne el único [!DNL Allocadia] ID del registro que desea que lea el módulo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear registro]

Este módulo de acción crea un registro.

El módulo devuelve el ID del registro y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Allocadia] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidad]</td> 
   <td>Seleccione si desea crear un nuevo registro basado en el elemento de línea o en la opción de columna.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Presupuestos]</td> 
   <td> <p>Seleccione el presupuesto donde desea crear un registro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Column choices]</td> 
   <td>Seleccione la columna que desea utilizar para crear un nuevo registro.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Label]</td> 
   <td>Introduzca o asigne una etiqueta para el nuevo registro</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar registro]

Este módulo de acción elimina un registro en particular.

Especifique el ID del registro.

El módulo devuelve el ID del registro y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Allocadia] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidad]</td> 
   <td> <p>Seleccione el tipo de entidad que desea eliminar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Elemento de línea]</strong> </p> <p>Introduzca el ID de artículo de línea</p> </li> 
     <li> <p><strong>[!UICONTROL Opción de columna]</strong> </p> <p>Seleccione el presupuesto desde el que desea eliminar un registro y, a continuación, introduzca el Id. de columna y el Id. de opción.</p> </li> 
     <li> <p><strong>[!UICONTROL Etiquetas de pronóstico]</strong> </p> <p>Seleccione el presupuesto desde el que desea eliminar un registro y, a continuación, introduzca el ID de etiqueta.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar registro]

Este módulo de acción actualiza un registro, como un elemento de línea, un usuario o una opción de columna,.

Especifique el ID del registro.

El módulo devuelve el ID del registro y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!UICONTROL Allocadia] a [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidad]</td> 
   <td>Seleccione el tipo de [!DNL Allocadia] que desea que el módulo actualice. Aparecerán otros campos en función del tipo de entidad seleccionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Presupuestos]</td> 
   <td> <p>Seleccione el presupuesto en el que desea actualizar un registro. </p> </td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

#### [!UICONTROL Buscar registro]

Este módulo de búsqueda busca registros en un objeto de [!DNL Allocadia] que coincidan con la consulta de búsqueda especificada.

Puede asignar esta información en módulos subsiguientes en el escenario.

Usted especifica el tipo de registros que desea.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Conexión]</p> </td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Allocadia] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidad]</td> 
   <td>Seleccione el tipo de [!DNL Allocadia] que desea que el módulo busque. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Presupuestos]</td> 
   <td> <p>Seleccione el presupuesto que desea buscar. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conjunto de resultados]</td> 
   <td>Seleccione si desea que el módulo devuelva todos los registros coincidentes o solo el primer registro coincidente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recuento máximo de registros]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Criterios de búsqueda]</td> 
   <td>Seleccione el campo que desea buscar, seleccione la operación e introduzca o asigne el valor que desea buscar. Puede añadir [!DNL AND] o [!DNL OR] reglas para filtrar aún más la búsqueda.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione los campos que desea incluir en la salida del módulo. Los campos disponibles dependen del tipo de entidad seleccionado.</p> </td> 
  </tr> 
 </tbody> 
</table>
