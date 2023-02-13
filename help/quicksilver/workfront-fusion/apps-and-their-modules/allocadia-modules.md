---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos de Allocadia
description: En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan Allocadia, así como conectarlos a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: f1edefd1-9fe0-48fc-bea2-c3f9facf7363
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1354'
ht-degree: 0%

---

# [!DNL Allocadia] módulos

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Allocadia], así como conectarlo a varias aplicaciones y servicios de terceros.

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

Para usar [!DNL Allocadia] módulos, debe tener un [!DNL Allocadia] cuenta.

## Connect [!DNL Allocadia] a [!DNL Workfront Fusion]

Puede crear una conexión con su [!DNL Allocadia] cuenta directamente desde dentro de un [!DNL Allocadia] módulo.

1. En cualquier [!DNL Allocadia] módulo, haga clic en **[!UICONTROL Agregar]** junto a la variable [!UICONTROL Conexión] campo .
1. Seleccione si desea utilizar el servidor de Norteamérica o el de Europa.
1. Introduzca su nombre de usuario y contraseña.
1. Haga clic en **[!UICONTROL Continuar]** para crear la conexión y volver al módulo .

## [!DNL Allocadia] módulos y sus campos

Al configurar [!DNL Allocadia] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL Allocadia] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheur](#triggers)
* [Acciones](#actions)
* [Búsquedas](#searches)

### Déclencheur

#### [!UICONTROL Registro de Watch]

Este módulo de déclencheur ejecuta un escenario cuando se agregan, actualizan o ambas cosas objetos de un tipo específico. El módulo devuelve todos los campos estándar asociados con el registro o registros, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> <table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowhader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de Allocadia a [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Conectar Allocadia] a Workfront Fusion</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filtro</td> 
   <td> <p>Seleccione si desea que el escenario vea Solo registros nuevos, [!UICONTROL Registros actualizados solamente] o Registros nuevos y actualizados.</p> </td> 
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
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo vea durante cada ciclo de ejecución del escenario.</p> </td> 
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

Este módulo de acción le permite realizar una llamada autenticada personalizada al [!DNL Allocadia] API. De este modo, puede crear una automatización del flujo de datos que no se pueda lograr con la otra [!DNL Allocadia] módulos.

La acción se basa en el tipo de entidad (tipo de objeto Allocadia) que especifique.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Allocadia] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Especifique una ruta relativa a <code>https://api-na.allocadia.com/{version}</code> o <code>https://api-eu.allocadia.com/{version}</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   td&gt; <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada a la API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] añade los encabezados de autorización por usted.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p> </td> 
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

#### [!UICONTROL Leer registro]

Este módulo de acción lee datos de un registro único de [!DNL Allocadia].

Especifique el ID del registro.

El módulo devuelve todos los campos estándar asociados con el registro, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowhader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Allocadia] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidad]</td> 
   <td>Seleccione el tipo de [!DNL Allocadia] registro que desea que lea el módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione los campos que desea incluir en la salida del módulo. Los campos disponibles dependen del [!UICONTROL Entity Type] seleccionado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Introduzca o asigne la variable única [!DNL Allocadia] ID del registro que desea que lea el módulo.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear registro]

Este módulo de acción crea un registro.

El módulo devuelve el ID del registro y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowhader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Allocadia] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidad]</td> 
   <td>Seleccione si desea crear un nuevo registro basado en la opción de columna o elemento de línea.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Presupuestos]</td> 
   <td> <p>Seleccione el presupuesto en el que desea crear un registro.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Column choices]</td> 
   <td>Seleccione la columna que desee utilizar para crear un nuevo registro.</td> 
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

El módulo devuelve el ID del registro y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowhader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Allocadia] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidad]</td> 
   <td> <p>Seleccione el tipo de entidad que desea eliminar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Line item]</strong> </p> <p>Introduzca el ID de artículo de línea</p> </li> 
     <li> <p><strong>[!UICONTROL Opción de columna]</strong> </p> <p>Seleccione el presupuesto desde el que desea eliminar un registro e introduzca el ID de columna y el ID de opción.</p> </li> 
     <li> <p><strong>[!UICONTROL Etiquetas de previsión]</strong> </p> <p>Seleccione el presupuesto desde el que desea eliminar un registro e introduzca el ID de la etiqueta.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Actualizar registro]

Este módulo de acción actualiza un registro, como un elemento de línea, un usuario o una opción de columna.

Especifique el ID del registro.

El módulo devuelve el ID del registro y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [!UICONTROL Allocadia] a [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidad]</td> 
   <td>Seleccione el tipo de [!DNL Allocadia] registro que desea que el módulo se actualice. Aparecen otros campos en función del tipo de entidad seleccionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Presupuestos]</td> 
   <td> <p>Seleccione el presupuesto en el que desea actualizar un registro. </p> </td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

#### [!UICONTROL Registro de búsqueda]

Este módulo de búsqueda busca registros en un objeto de [!DNL Allocadia] que coinciden con la consulta de búsqueda especificada.

Puede asignar esta información en módulos posteriores en el escenario.

Especifique el tipo de registros que desea.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowhader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Allocadia] cuenta para [!DNL Workfront Fusion], consulte <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidad]</td> 
   <td>Seleccione el tipo de [!DNL Allocadia] registro que desea que busque el módulo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Presupuestos]</td> 
   <td> <p>Seleccione el presupuesto que desee buscar. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resultado establecido]</td> 
   <td>Seleccione si desea que el módulo devuelva Todos los registros coincidentes o solo el registro coincidente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recuento máximo de registros]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Criterios de búsqueda]</td> 
   <td>Seleccione el campo que desee buscar, seleccione la operación e introduzca o asigne el valor que desee buscar. Puede añadir [!DNL AND] o [!DNL OR] reglas para filtrar aún más la búsqueda.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione los campos que desea incluir en la salida del módulo. Los campos disponibles dependen del tipo de entidad seleccionado.</p> </td> 
  </tr> 
 </tbody> 
</table>
