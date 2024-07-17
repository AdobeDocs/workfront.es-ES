---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Microsoft Dynamics 365
description: En un  [!DNL Adobe Workfront Fusion] escenario, puede automatizar los flujos de trabajo que utilizan Microsoft Dynamics 365, así como conectarlos a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '1724'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 modules]

En un escenario de [!DNL Adobe Workfront Fusion], puede automatizar los flujos de trabajo que utilizan [!DNL Microsoft Dynamics 365], así como conectarlo a varias aplicaciones y servicios de terceros.

>[!NOTE]
>
>El conector [!DNL Microsoft Dynamics 365] no admite [!DNL Dynamics Finance and Operations].

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

Para usar [!DNL Microsoft Dynamics] 365, debe tener una cuenta de [!DNL Microsoft Dynamics 365].

## Conexión de Microsoft Dynamics 365 a Workfront Fusion

Puede crear una conexión con su cuenta de [!DNL Microsoft Dynamics 365] directamente desde un módulo de [!DNL Microsoft Dynamics 365].

>[!NOTE]
>
>Algunas aplicaciones de Microsoft utilizan la misma conexión, que está vinculada a permisos de usuario individuales. Por lo tanto, al crear una conexión, la pantalla de consentimiento de permisos muestra todos los permisos que se hayan concedido anteriormente a la conexión de este usuario, además de los nuevos permisos necesarios para la aplicación actual.
>
>Por ejemplo, si un usuario tiene permisos de &quot;Leer tabla&quot; concedidos a través del conector de Excel y, a continuación, crea una conexión en el conector de Outlook para leer correos electrónicos, la pantalla de consentimiento de permisos mostrará tanto el permiso de &quot;Leer tabla&quot; ya concedido como el permiso de &quot;Escribir correo electrónico&quot; recién requerido.

1. En cualquier módulo de [!DNL Microsoft Dynamics 365], haga clic en **[!UICONTROL Agregar]** junto al campo [!UICONTROL Conexión].
1. Introduzca un nombre para la conexión.
1. En el campo **[!UICONTROL Recurso]**, escriba la dirección de su cuenta de [!DNL Dynamics 365], sin `https://`.
1. Haga clic en **[!UICONTROL Continuar]** para crear la conexión y volver al módulo.

>[!NOTE]
>
>Al registrar [!DNL Workfront Fusion] en el portal [!DNL Microsoft Azure], use el siguiente URI de redirección:
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`


## [!DNL Microsoft Dynamics 365] módulos y sus campos

Al configurar [!DNL Microsoft Dynamics 365] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL Microsoft Dynamics 365] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Registros De Inspección (Programados)]](#watch-records-scheduled)
* [[!UICONTROL Registros De Inspección (Tiempo Real)]](#watch-records-real-time)
* [[!UICONTROL Crear registro]](#create-record)
* [[!UICONTROL Realizar una llamada API]](#make-an-api-call)
* [[!UICONTROL Eliminar registro]](#delete-record)
* [[!UICONTROL Leer registros]](#read-records)
* [[!UICONTROL Actualizar registro]](#update-record)
* [[!UICONTROL Registros de búsqueda]](#search-records)

### [!UICONTROL Registros De Inspección (Programados)]

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
  <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion], vea <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> en este artículo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Incluir]</td> 
   <td>Seleccione si desea que el módulo vea <strong>[!UICONTROL Solo registros nuevos]</strong>, <strong>[!UICONTROL Solo registros actualizados]</strong> o <strong>[!UICONTROL Registros nuevos y todos los cambios]</strong>.</td> 
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

### [!UICONTROL Registros De Inspección (Tiempo Real)]

Este módulo de déclencheur instantáneo ejecuta un escenario cuando un registro (objeto) especificado se crea o actualiza en [!DNL Dynamics 365].

Se requiere un webhook en este módulo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Seleccione el webhook que desee utilizar para este módulo. </p> <p>Para agregar un nuevo webhook:</p> 
    <ol> 
     <li value="1"> <p>Haga clic en <strong>[!UICONTROL Add]</strong> a la derecha del campo Webhook</p> </li> 
     <li value="2"> <p>En el campo de nombre <strong>[!UICONTROL Webhook]</strong>, escriba un nombre descriptivo para el webhook.</p> </li> 
     <li value="3"> <p>En el campo <strong>[!UICONTROL Connection]</strong>, seleccione la Conexión que desea utilizar seleccionada</p> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion], vea <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> en este artículo. </p> </li> 
     <li value="4"> <p>Haga clic en <strong>[!UICONTROL Guardar]</strong> para guardar el webhook y volver al módulo.</p> </li> 
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
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion], vea <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> en este artículo. </p> </td> 
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

### [!UICONTROL Realizar una llamada API]

Este módulo de acción le permite realizar una llamada autenticada personalizada a la API [!DNL Microsoft Dynamics 365]. De este modo, puede crear una automatización del flujo de datos que no puedan realizar los otros [!DNL Microsoft Dynamics 365] módulos.

El módulo devuelve información sobre el código de estado, los encabezados y el cuerpo. Puede asignar esta información en módulos subsiguientes en el escenario.

Para obtener más información, consulte la documentación de [!DNL Microsoft] acerca del uso de [!DNL Dynamics 365 Customer Engagement Web API].

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
  <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion], vea <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> en este artículo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Escriba una ruta relativa a <code>&lt;Instance URL>/api/data/v9.1/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> <p>Para obtener más información en</p> </td> 
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
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando utilice afirmaciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la afirmación condicional.</p> 
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
  <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion], vea <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> en este artículo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de entidad]</td> 
   <td> <p>Seleccione el tipo de entidad que desea que elimine el módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Escriba o asigne el identificador único [!DNL Microsoft Dynamics 365] del registro que desea que elimine el módulo.</p> </td> 
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
  <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion], vea <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> en este artículo. </p> </td> 
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
   <td>Escriba o asigne el identificador único [!DNL Microsoft Dynamics 365] del registro que desea que lea el módulo.</td> 
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
  <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion], vea <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> en este artículo. </p> </td> 
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
   <td>Escriba o asigne el identificador único [!DNL Microsoft Dynamics] 365 del registro que desea que actualice el módulo.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Registros de búsqueda]

Este módulo de búsqueda busca registros en un objeto de [!DNL Microsoft Dynamics 365] que coincidan con la consulta de búsqueda especificada. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
  <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion], vea <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Conectar [!DNL Microsoft Dynamics 365] a [!DNL Workfront Fusion]</a> en este artículo. </p> </td> 
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
     <li> <p><strong>[!UICONTROL Funciones de consulta]</strong> </p> <p>Escriba la función de consulta de API web [!DNL Dynamics 365] que desee usar para la búsqueda. </p> <p>Para obtener más información sobre las funciones de consulta, consulte <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">Referencia de función de consulta de API web</a> en la documentación de [!DNL Microsoft].</p> </li> 
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
