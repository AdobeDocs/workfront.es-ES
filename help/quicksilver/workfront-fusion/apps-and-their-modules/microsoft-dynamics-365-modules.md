---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Microsoft Dynamics 365
description: En un [!DNL Adobe Workfront Fusion] En este escenario, se pueden automatizar los flujos de trabajo que utilizan Microsoft Dynamics 365 y conectarlos a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
source-git-commit: 46c282062ed737be860aeb4af96ac5f5efe9360d
workflow-type: tm+mt
source-wordcount: '1633'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 modules]

En un [!DNL Adobe Workfront Fusion] , puede automatizar los flujos de trabajo que utilizan [!DNL Microsoft Dynamics 365], así como conectarlo a múltiples aplicaciones y servicios de terceros.

>[!NOTE]
>
>El [!DNL Microsoft Dynamics 365] el conector no es compatible [!DNL Dynamics Finance and Operations].

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

Para usar [!DNL Microsoft Dynamics] 365, usted debe tener un [!DNL Microsoft Dynamics 365] cuenta.

## Conexión de Microsoft Dynamics 365 a Workfront Fusion

Puede crear una conexión con su [!DNL Microsoft Dynamics 365] cuenta directamente desde dentro de un [!DNL Microsoft Dynamics 365] módulo.

1. En cualquier [!DNL Microsoft Dynamics 365] , haga clic en **[!UICONTROL Añadir]** junto al [!UICONTROL Conexión] field.
1. Introduzca un nombre para la conexión.
1. En el **[!UICONTROL Recurso]** , introduzca la dirección de su [!DNL Dynamics 365] cuenta, sin `https://`.
1. Clic **[!UICONTROL Continuar]** para crear la conexión y volver al módulo.

>[!NOTE]
>
>Al registrarse [!DNL Workfront Fusion] en su [!DNL Microsoft Azure] , utilice el siguiente URI de redireccionamiento:
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`


## [!DNL Microsoft Dynamics 365] módulos y sus campos

Al configurar [!DNL Microsoft Dynamics 365] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, se añaden [!DNL Microsoft Dynamics 365] Los campos pueden mostrarse, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Ver registros (programados)]](#watch-records-scheduled)
* [[!UICONTROL Ver registros (tiempo real)]](#watch-records-real-time)
* [[!UICONTROL Crear registro]](#create-record)
* [[!UICONTROL Realizar una llamada de API]](#make-an-api-call)
* [[!UICONTROL Eliminar registro]](#delete-record)
* [[!UICONTROL Leer registros]](#read-records)
* [[!UICONTROL Actualizar registro]](#update-record)
* [[!UICONTROL Buscar registros]](#search-records)

### [!UICONTROL Ver registros (programados)]

Este módulo de déclencheur programado ejecuta un escenario cuando se crea o actualiza un registro del objeto especificado después de la última ejecución programada en [!DNL Dynamics 365].

La salida del módulo indica si el registro que ha encontrado es nuevo o actualizado (si se añadió y actualizó en el período de tiempo, se marca como nuevo). Puede asignar esta información en módulos subsiguientes en el escenario.

Esto sucede en un intervalo programado de forma regular que usted especifica.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
  <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Microsoft Dynamics 365] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] hasta [!DNL Workfront Fusion]</a> en este artículo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Incluir]</td> 
   <td>Seleccione si desea que el módulo vea <strong>[!UICONTROL Solo registros nuevos]</strong>, <strong>[!UICONTROL Sólo registros actualizados]</strong>, o <strong>[!UICONTROL Nuevos registros y todos los cambios]</strong>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidad]</td> 
   <td>Elija el tipo de registro de [!UICONTROL Microsoft Dynamics 365] que desea que vea el escenario.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione la información que desee incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Registros máximos]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Ver registros (tiempo real)]

Este módulo de déclencheur instantáneo ejecuta un escenario cuando se crea o actualiza un registro (objeto) especificado en [!DNL Dynamics 365].

Se requiere un webhook en este módulo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Seleccione el webhook que desee utilizar para este módulo. </p> <p>Para agregar un nuevo webhook:</p> 
    <ol> 
     <li value="1"> <p>Clic <strong>[!UICONTROL Agregar]</strong> a la derecha del campo Webhook</p> </li> 
     <li value="2"> <p>En el <strong>[!UICONTROL Webhook]</strong> campo nombre, escriba un nombre descriptivo para el webhook.</p> </li> 
     <li value="3"> <p>En el <strong>[!UICONTROL Conexión]</strong> , seleccione la Conexión que desea utilizar seleccionada</p> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Microsoft Dynamics 365] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] hasta [!DNL Workfront Fusion]</a> en este artículo. </p> </li> 
     <li value="4"> <p>Clic <strong>[!UICONTROL Guardar]</strong> para guardar su webhook y volver al módulo.</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Crear registro]

Este módulo de acción crea una entidad, como una cita o una tarea.

Especifique información sobre la entidad que desea crear.

El módulo devuelve el ID de la nueva entidad y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Microsoft Dynamics 365] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] hasta [!DNL Workfront Fusion]</a> en este artículo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidad]</td> 
   <td>Seleccione el tipo de entidad que desea que cree el módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar campos para asignar]</td> 
   <td>Seleccione los campos para los que desea incluir valores cuando se cree el registro. Los campos disponibles dependen del tipo de entidad.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Campos de propiedad]</td> 
   <td> Estos son los campos que ha seleccionado. Introduzca el valor que desea que tenga el registro para una propiedad determinada. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Realizar una llamada de API]

Este módulo de acción le permite realizar una llamada autenticada personalizada a [!DNL Microsoft Dynamics 365] API. De este modo, se puede crear una automatización del flujo de datos que el otro no puede realizar [!DNL Microsoft Dynamics 365] módulos.

El módulo devuelve información sobre el código de estado, los encabezados y el cuerpo. Puede asignar esta información en módulos subsiguientes en el escenario.

Para obtener más información, consulte la [!DNL Microsoft] documentación sobre el uso de [!DNL Dynamics 365 Customer Engagement Web API].

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
  <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Microsoft Dynamics 365] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] hasta [!DNL Workfront Fusion]</a> en este artículo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Introduzca una ruta relativa a <code>&lt;Instance URL>/api/data/v9.1/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> <p>Para obtener más información en</p> </td> 
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

### [!UICONTROL Eliminar registro]

Este módulo de acción elimina una entidad.

Especifique el ID de la entidad.

El módulo devuelve el ID de la entidad y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
  <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Microsoft Dynamics 365] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] hasta [!DNL Workfront Fusion]</a> en este artículo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidad]</td> 
   <td> <p>Seleccione el tipo de entidad que desea que elimine el módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Introduzca o asigne el único [!DNL Microsoft Dynamics 365] ID del registro que desea que elimine el módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Leer registros]

Este módulo de acción lee datos de una sola entidad en [!DNL Microsoft Dynamics 365].

Especifique el ID de la entidad.

El módulo devuelve el ID de la entidad y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
  <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Microsoft Dynamics 365] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] hasta [!DNL Workfront Fusion]</a> en este artículo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidad]</td> 
   <td>Seleccione el tipo de entidad que desea que lea el módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione la información que desee incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Introduzca o asigne el único [!DNL Microsoft Dynamics 365] ID del registro que desea que lea el módulo.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Actualizar registro]

Este módulo de acción actualiza una entidad.

Especifique el ID de la entidad.

El módulo devuelve el ID del registro actualizado y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
  <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Microsoft Dynamics 365] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] hasta [!DNL Workfront Fusion]</a> en este artículo. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Tipo de entidad]</td> 
   <td>Seleccione el tipo de entidad que desea que actualice el módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seleccionar campos para asignar]</td> 
   <td>Seleccione los campos para los que desea incluir valores cuando se cree el registro. Los campos disponibles dependen del tipo de entidad.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Campos de propiedad]</td> 
   <td>Estos son los campos que ha seleccionado. Introduzca el valor que desea que tenga el registro para una propiedad determinada.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Introduzca o asigne el único [!DNL Microsoft Dynamics] 365 ID del registro que desea que actualice el módulo.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Buscar registros]

Este módulo de búsqueda busca registros en un objeto de [!DNL Microsoft Dynamics 365] que coincidan con la consulta de búsqueda especificada. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
  <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Microsoft Dynamics 365] cuenta a [!DNL Workfront Fusion], consulte <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] hasta [!DNL Workfront Fusion]</a> en este artículo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidad]</td> 
   <td>Seleccione el tipo de entidad que desea que actualice el módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtros]</td> 
   <td> <p>Seleccione el filtro que desee utilizar para esta búsqueda.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Filtros estándar]</strong> </p> <p>Configure el filtro seleccionando un campo y un operador e introduciendo o asignando el valor que desea buscar. Puede utilizar las reglas AND u OR para aplicar el filtro.</p> </li> 
     <li> <p><strong>[!UICONTROL Funciones de consulta]</strong> </p> <p>Introduzca el [!DNL Dynamics 365] función de consulta de API web que desee utilizar para la búsqueda. </p> <p>Para obtener más información sobre las funciones de consulta, consulte <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">Referencia de función de consulta de API web</a> en el [!DNL Microsoft] documentación.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordenar]</td> 
   <td> <p>Especifique el orden en que se devuelven los elementos. Puede agregar varias ordenaciones.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Campo]</strong> </p> <p>Especifique el campo por el que desea ordenar los resultados.</p> </li> 
     <li> <p><strong>[!UICONTROL Dirección]</strong> </p> <p>Especifique la dirección de la ordenación (ascendente o descendente).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Registros máximos]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione la información que desee incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>
