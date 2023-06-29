---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Adobe Workfront
description: Puede utilizar el conector Adobe Workfront de Adobe Workfront Fusion para automatizar los procesos en Workfront. Si dispone de una licencia de integración y automatización del trabajo de Workfront Fusion, también puede utilizarla para conectarse a aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: b84d2d41-a983-4ea3-b331-0302bfcf8a2b
source-git-commit: 3604e67309b76c4e0e8c3af1341b80a607b95d6f
workflow-type: tm+mt
source-wordcount: '5428'
ht-degree: 3%

---

# [!DNL Adobe Workfront] módulos

Puede usar el complemento [!DNL Adobe Workfront Fusion] [!DNL Adobe Workfront] para automatizar los procesos dentro de [!DNL Workfront]. Si tiene un [!UICONTROL [!DNL Workfront Fusion] para la automatización e integración del trabajo] Con esta licencia, también puede utilizarla para conectarse a aplicaciones y servicios de terceros.

El [!DNL Workfront] connector no se cuenta con el número de aplicaciones activas disponibles para su organización. Todos los escenarios, incluso si solo utilizan la variable [!DNL Workfront] , no se contabilice con el recuento total de escenarios de su organización.

Para obtener más información sobre las aplicaciones y los escenarios disponibles de su organización, consulte [Organizaciones](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2) in [[!DNL Adobe Workfront Fusion] organizaciones y equipos](../../workfront-fusion/organizations/organizations-and-teams.md).

Si necesita instrucciones sobre cómo crear un escenario, consulte [Creación de un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo], [!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]</p>
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

## Connect [!DNL Workfront] hasta [!DNL Workfront Fusion]

El [!DNL Workfront] El conector de utiliza OAuth 2.0 para conectarse a [!DNL Workfront].

Puede crear una conexión con su [!DNL Workfront] cuenta directamente desde dentro de un [!DNL Workfront Fusion] módulo.

1. En cualquier [!DNL Workfront] módulo de la aplicación, haga clic en **[!UICONTROL Añadir]** junto al [!UICONTROL Conexión] cuadro.
1. Introduzca el nombre de la instancia en la dirección URL. Ejemplo: `https://<your instance>.my.workfront.com`.
1. Clic **[!UICONTROL Siguiente]**.
1. Clic **[!UICONTROL Inicio de sesión de SAML]** para crear la conexión y volver al módulo.

   O

   Introduzca su nombre de usuario y contraseña y haga clic en **[!UICONTROL Iniciar sesión]** para crear la conexión y volver al módulo.

   >[!NOTE]
   >
   >* Si no ve un botón de inicio de sesión de SAML, significa que su organización no ha habilitado el inicio de sesión único (SSO). Puede iniciar sesión con su nombre de usuario y contraseña.
   >   
   >   Para obtener más información sobre SSO, consulte [Información general sobre el inicio de sesión único en [!DNL Adobe Workfront]](../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)
   >   
   >* Conexiones OAuth 2.0 a [!DNL Workfront] Las API ya no dependen de las claves API.

## [!DNL Workfront] módulos y sus campos

Al configurar [!DNL Workfront] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, se añaden [!DNL Workfront] Los campos pueden mostrarse, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Déclencheur](#triggers)
* [Acciones](#actions)
* [Búsquedas](#searches)

### Déclencheur

<!--
* [Watch Events](#watch-events) 
* [Watch Record](#watch-record) 
* [Watch Field](#watch-field)
-->

+++ **[!UICONTROL Ver eventos]**

Este módulo de déclencheur ejecuta un escenario en tiempo real cuando se añaden, actualizan o eliminan objetos de un tipo específico en Workfront

El módulo devuelve cualquier campo estándar asociado con el registro, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

1. Clic **[!UICONTROL Añadir]** a la derecha del **Webhook** cuadro.

1. Configure el webhook en **[!UICONTROL Añadir un gancho]** que se muestra.

   Al configurar este módulo, se muestran los campos siguientes.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Nombre de webhook de [!UICONTROL]</td> 
      <td>(Opcional) Escriba un nuevo nombre para el webhook</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Conexión]</td> 
      <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Tipo de registro]</td> 
      <td>Seleccione el tipo de [!DNL Workfront] registre que desea que el módulo vea.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Estado]</td> 
      <td>Seleccione si desea ver el estado antiguo o el nuevo.<ul><li><p><b>[!UICONTROL Nuevo estado]</b></p><p>Déclencheur de un escenario cuando cambia el registro <b>hasta</b> un valor determinado.</p><p>Por ejemplo, si el estado se establece en [!UICONTROL Nuevo estado] y el filtro se establece en [!UICONTROL estado] [!UICONTROL igual a] [!UICONTROL en curso], el webhook crea un déclencheur cuando el [!UICONTROL estado] cambia a [!UICONTROL en curso], independientemente del estado anterior. </p></li><li><p><b>[!UICONTROL Estado anterior]</b></p><p>Déclencheur de un escenario cuando cambia el registro <b>de</b> un valor determinado.</p><p>Por ejemplo, si el estado se establece en [!UICONTROL Estado anterior] y el filtro se establece en [!UICONTROL Estado] [!UICONTROL Es igual a] [!UICONTROL En curso], el webhook genera un déclencheur cuando un [!UICONTROL Estado] que está actualmente [!UICONTROL En curso] cambia a otro estado. </p></li></ul></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Filtros de eventos]</p> </td> 
      <td> <p>Puede establecer filtros para inspeccionar sólo los registros que cumplan los criterios seleccionados.</p> <p>Para cada filtro, introduzca el campo que desea que evalúe el filtro, el operador y el valor que desea que permita el filtro. Puede utilizar más de un filtro añadiendo reglas AND.</p> <p>Nota: No puede editar filtros en filtros existentes [!DNL Workfront] webhooks. Para configurar diferentes filtros para [!DNL Workfront] Suscripciones de eventos, elimine el webhook actual y cree uno nuevo.</p> <p>Para obtener más información sobre los filtros de eventos, consulte <a href="#event-subscription-filters-in-the-workfront-watch-events-modules" class="MCXref xref">Filtros de suscripción de evento en la [!DNL Workfront] &gt; Módulos de [!UICONTROL Watch Events]</a> en este artículo.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Excluir eventos realizados por esta conexión</td> 
      <td>Active esta opción para excluir los eventos creados o actualizados con el mismo conector que utiliza este módulo de déclencheur. Esto puede evitar situaciones en las que un escenario podría entrar en déclencheur y provocar que se repita en un bucle interminable.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Origen de registro]</td> 
      <td> <p>Elija si desea que el escenario se vea <strong>[!UICONTROL Solo registros nuevos]</strong>, <strong>[!UICONTROL Solo registros actualizados]</strong>, <strong>[!UICONTROL Registros nuevos y actualizados]</strong>, o <strong>[!DNL Deleted Records Only]</strong>.</p> <p>Nota: Si elige <strong>[!UICONTROL Registros nuevos y actualizados]</strong>, la creación del gancho web crea 2 suscripciones de evento (para la misma dirección de gancho web).</p> </td> 
     </tr> 
    </tbody> 
   </table>

Una vez creado el gancho web, puede ver la dirección del extremo al que se envían los eventos.

Para obtener más información, consulte la sección [Ejemplos de cargas útiles de eventos](../../wf-api/general/event-subs-api.md#examples-of-event-payloads) en el [!DNL Workfront] Artículo de ayuda [API de suscripción de evento](../../wf-api/general/event-subs-api.md).

Consulte una lista de los [!DNL Workfront] tipos de objeto para los que puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Campo de observación]**

Este módulo de déclencheur ejecuta un escenario cuando se actualiza un campo que usted especifica. El módulo devuelve el valor antiguo y el nuevo del campo especificado. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de [!DNL Workfront] registre que desea que el módulo vea.</p> <p>Por ejemplo, seleccione [!UICONTROL Tarea] si desea comenzar a ejecutar el escenario cada vez que se actualice un campo de registro en una tarea.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campo]</td> 
   <td>Seleccione el campo en el que desea que el módulo inspeccione las actualizaciones. Estos campos reflejan los campos que su [!DNL Workfront] el administrador ha configurado para el seguimiento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Salidas]</td> 
   <td>Seleccione la información que desee incluir en el paquete de salida para este módulo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de los [!DNL Workfront] tipos de objeto para los que puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Ver registro]**

Este módulo de déclencheur ejecuta un escenario cuando se añaden, actualizan o ambos objetos de un tipo específico. El módulo devuelve todos los campos estándar asociados con el registro o registros, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario. En la salida, el módulo indica si cada registro es nuevo o se ha actualizado.

Los registros que se agregaron y actualizaron en el período de tiempo determinado se devuelven como registros nuevos.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Elija si desea que el escenario se vea <strong>[!UICONTROL Solo registros nuevos]</strong>, <strong>[!UICONTROL Solo registros actualizados]</strong>, o <strong>[!UICONTROL Registros nuevos y actualizados]</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>(Se muestra después de elegir una <strong>Filtrar</strong>.) Seleccione el tipo de [!DNL Workfront] registre que desea que el módulo vea.</p> <p>Por ejemplo, si desea iniciar el escenario cada vez que se cree un nuevo proyecto, seleccione [!UICONTROL Proyecto]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione la información que desee incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro opcional]</td> 
   <td> <p>(Avanzado) Escriba una cadena de código de API para definir cualquier parámetro o código adicional que restrinja sus criterios. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de los [!DNL Workfront] tipos de objeto para los que puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++


### Acciones

<!--
* [Convert object](#convert-object) 
* [Create a record (attaching custom forms)](#create-a-record-attaching-custom-forms) 
* [Create a record](#create-a-record) 
* [Custom API Call](#custom-api-call) 
* [Delete Record](#delete-record) 
* [Download Document](#download-document) 
* [Misc Action](#misc-action) 
* [Read a Record](#read-a-record) 
* [Update Record](#update-record) 
* [Upload Document](#upload-document)
-->

+++ **[!UICONTROL Convertir objeto]**

Este módulo de acción realiza una de las siguientes conversiones:

* Convertir problema a proyecto
* Convertir problema a tarea
* Convertir tarea al proyecto

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tipo de objeto]</td> 
   <td> <p>Seleccione el tipo de objeto que desea convertir. Es el tipo que tiene el objeto antes de la conversión.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Convertir a]</td> 
   <td>Seleccione el objeto al que desea convertirlo. Es el tipo que tiene el objeto después de la conversión.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL &lt;object&gt; [ID]</td> 
   <td> <p>Introduzca la ID del objeto. </p> <p>Nota: Al introducir el ID de un objeto, puede empezar a escribir su nombre y, a continuación, seleccionarlo en la lista. A continuación, el módulo introduce el ID adecuado en el campo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Id. de plantilla]</td> 
   <td> <p>Si está convirtiendo a un proyecto, seleccione el ID de plantilla que desee utilizar para el proyecto.</p> <p>Nota: Al introducir el ID de un objeto, puede empezar a escribir su nombre y, a continuación, seleccionarlo en la lista. A continuación, el módulo introduce el ID adecuado en el campo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Formularios personalizados]</td> 
   <td>Seleccione los formularios personalizados que desee agregar al objeto recién convertido y, a continuación, introduzca los valores de los campos del formulario personalizado.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Opciones]</td> 
   <td> <p>Active las opciones que desee al convertir el objeto. Las opciones están disponibles en función del objeto al que se convierta o desde el que se convierta.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Crear un registro (adjuntar formularios personalizados)]**

Este módulo de acción crea un objeto, como un proyecto, una tarea o un problema, en [!DNL Workfront]y le permite agregar un formulario personalizado al nuevo objeto. El módulo le permite seleccionar qué campos del objeto están disponibles en el módulo.

Especifique el ID del registro.

El módulo devuelve el ID del registro y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Puede utilizar este módulo, por ejemplo, para crear una tarea en [!DNL Workfront] cuando un cliente agrega una fila nueva en un [!DNL Google Sheets] lista de tareas que deben realizarse.

Al configurar este módulo, se muestran los campos siguientes.

Asegúrese de proporcionar el número mínimo de campos de entrada. Por ejemplo, si desea crear un problema, debe proporcionar un ID de proyecto principal válido en el campo ID de proyecto para indicar dónde debe residir el problema en Workfront. Puede utilizar el panel de asignación para asignar esta información desde otro módulo del escenario o puede introducirla manualmente escribiendo el nombre y seleccionándola a continuación en la lista.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de [!DNL Workfront] que desea que el módulo cree.</p> <p>Por ejemplo, si desea crear un proyecto, seleccione [!UICONTROL Proyecto] en la lista desplegable y, a continuación, asegúrese de que tiene acceso a los datos (de módulos anteriores en el escenario) que rellenarán el proyecto.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Seleccionar campos para asignar]</td> 
   <td> <p>Seleccione los campos que desea que estén disponibles para la entrada de datos. Esto le permite utilizar estos campos sin tener que desplazarse por los que no necesita.</p> <p>Para los campos de los formularios personalizados, utilice la variable <b>[!UICONTROL Adjuntar formulario personalizado]</b> field.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Adjuntar formulario personalizado]</td> 
   <td>Seleccione los formularios personalizados que desee agregar al nuevo objeto y, a continuación, introduzca los valores de esos campos.</td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de los [!DNL Workfront] tipos de objeto para los que puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Al introducir el ID de un objeto, puede empezar a escribir su nombre y, a continuación, seleccionarlo en la lista. A continuación, el módulo introduce el ID adecuado en el campo.
>* Al introducir el texto de un campo personalizado o una [!UICONTROL Nota] objeto (Comentario o respuesta), puede utilizar etiquetas de HTML en la variable [!UICONTROL Texto de nota] para crear texto enriquecido, como negrita o cursiva.
>
>  Para obtener más información sobre el texto enriquecido en las actualizaciones, consulte [Agregar una actualización a un elemento de trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Crear registro]**

Este módulo de acción crea un objeto, como un proyecto, una tarea o un problema, en Workfront. El módulo le permite seleccionar qué campos del objeto están disponibles en el módulo.

Especifique el ID del registro.

El módulo devuelve el ID del registro y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Puede utilizar este módulo, por ejemplo, para crear una tarea en [!DNL Workfront] cuando un cliente agrega una nueva fila en una lista de hojas de Google de tareas que deben realizarse.

Al configurar este módulo, se muestran los campos siguientes.

Asegúrese de proporcionar el número mínimo de campos de entrada. Por ejemplo, si desea crear un problema, debe proporcionar un ID de proyecto principal válido en el campo ID de proyecto para indicar dónde debe residir el problema en Workfront. Puede utilizar el panel de asignación para asignar esta información desde otro módulo del escenario o puede introducirla manualmente escribiendo el nombre y seleccionándola a continuación en la lista.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de [!DNL Workfront] que desea que el módulo cree.</p> <p>Por ejemplo, si desea crear un proyecto, seleccione [!UICONTROL Proyecto] en la lista desplegable y, a continuación, asegúrese de que tiene acceso a los datos (de módulos anteriores en el escenario) que rellenarán el proyecto.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Seleccionar campos para asignar]</td> 
   <td>Seleccione los campos que desea que estén disponibles para la entrada de datos. Esto le permite utilizar estos campos sin tener que desplazarse por los que no necesita.</td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de los [!DNL Workfront] tipos de objeto para los que puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Al introducir el ID de un objeto, puede empezar a escribir su nombre y, a continuación, seleccionarlo en la lista. A continuación, el módulo introduce el ID adecuado en el campo.
>* Al introducir el texto de un campo personalizado o una [!UICONTROL Nota] objeto (Comentario o respuesta), puede utilizar etiquetas de HTML en la variable [!UICONTROL Texto de nota] para crear texto enriquecido, como negrita o cursiva.
>
>  Para obtener más información sobre el texto enriquecido en las actualizaciones, consulte [Agregar una actualización a un elemento de trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Llamada de API personalizada]**

Este módulo de acción le permite realizar una llamada autenticada personalizada a [!DNL Workfront] API. De este modo, se puede crear una automatización del flujo de datos que el otro no puede realizar [!DNL Workfront] módulos.

El módulo devuelve la siguiente información:

* **[!UICONTROL Código de estado]** (número): Esto indica el éxito o el error de la solicitud HTTP. Estos son códigos estándar que puede buscar en Internet.
* **[!UICONTROL Encabezados]** (objeto): contexto más detallado para el código de respuesta/estado que no está relacionado con el cuerpo de salida. No todos los encabezados que aparecen en un encabezado de respuesta son encabezados de respuesta, por lo que algunos podrían no ser útiles para usted.

  Los encabezados de respuesta dependen de la solicitud HTTP elegida al configurar el módulo.

* **[!UICONTROL Cuerpo]** (objeto): Según la solicitud HTTP elegida al configurar el módulo, es posible que reciba algunos datos de nuevo. Esos datos, como los datos de una solicitud de GET, están contenidos en este objeto.

Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Introduzca una ruta relativa a<code> https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API Version]</td> 
   <td>Seleccione la versión de [!DNL Workfront] API que desea que utilice el módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   td&gt; <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar. Determina el tipo de contenido de la solicitud.</p> <p>Por ejemplo,<code> {"Content-type":"application/json"}</code></p> <p>Nota: Si se producen errores y es difícil determinar su origen, considere la posibilidad de modificar los encabezados según el [!DNL Workfront] documentación. Si la llamada de API personalizada devuelve un error de solicitud HTTP 422, intente utilizar una <code>"Content-Type":"text/plain"</code> encabezado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p> <p>Sugerencia: Le recomendamos que envíe información a través del cuerpo de JSON en lugar de como parámetros de consulta.</p> </td> 
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

Consulte una lista de los [!DNL Workfront] tipos de objeto para los que puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Eliminar registro]**

Este módulo de acción elimina un objeto, como un proyecto, una tarea o un problema en Workfront.

Especifique el ID del registro.

El módulo devuelve el ID del registro y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Forzar eliminación]</td> 
   <td>Active esta opción para asegurarse de que se elimina el registro, incluso si la variable [!DNL Workfront] La interfaz de usuario solicitaría la confirmación de la eliminación.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Identificador</td> 
   <td> <p>Introduzca el único [!DNL Workfront] ID del registro que desea que elimine el módulo.</p> <p>Para obtener el ID, abra el [!DNL Workfront] en el explorador y copie el texto al final de la dirección URL después de "ID=". Por ejemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td>Seleccione el tipo de [!DNL Workfront] que desea que el módulo elimine.</td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de los [!DNL Workfront] tipos de objeto para los que puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Descargar documento]**

Este módulo de acción descarga un documento de Workfront.

Especifique el ID del registro.

El módulo devuelve el contenido, el nombre de archivo, la extensión y el tamaño de archivo del documento. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID de documento]</td> 
   <td> <p>Asigne o introduzca manualmente la variable única [!DNL Workfront] ID del documento que desea que descargue el módulo.</p> <p>Para obtener el ID, abra el [!DNL Workfront] en el explorador y copie el texto al final de la dirección URL después de "ID=". Por ejemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de los [!DNL Workfront] tipos de objeto para los que puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Misc Action]**

Este módulo de acción le permite realizar acciones en la API.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de [!DNL Workfront] con el que desea que interactúe el módulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Acción]</td> 
   <td> <p>Seleccione la acción que desea que realice el módulo.</p> <p>Es posible que tenga que rellenar campos adicionales, según el [!UICONTROL Tipo de registro] y la [!UICONTROL Acción] que elija. Algunas combinaciones de estas dos configuraciones pueden requerir solo un ID de registro, mientras que otras (como Proyecto para el <strong>[!UICONTROL Tipo de registro]</strong> y [!UICONTROL Adjuntar plantilla] para <strong>[!UICONTROL Acción]</strong>) requieren información adicional (como un ID de objeto y un ID de plantilla).</p> <p>Para obtener más información sobre los campos individuales, consulte la <a href="http://developer.workfront.com/">Documentación para desarrolladores de Workfront</a>. </p> 
    <ol> 
     <li value="1"> <p>Seleccione el tipo de registro en el panel de navegación izquierdo de [!DNL Workfront] página de documentación para desarrolladores. Los siguientes tipos tienen sus propias páginas:</p> 
      <ul> 
       <li> <p>[!UICONTROL Proyectos]</p> </li> 
       <li> <p>[!UICONTROL Tareas]</p> </li> 
       <li> <p>[!UICONTROL Problemas]</p> </li> 
       <li> <p>[!UICONTROL Usuarios]</p> </li> 
       <li> <p>[!UICONTROL Documentos]</p> </li> 
      </ul> <p>Para el resto de tipos de registros, seleccione <b>[!UICONTROL Otros objetos y extremos]</b>y busque el tipo de registro en las páginas ordenadas alfabéticamente.</p> </li> 
     <li value="2"> <p>En la página del tipo de registro adecuado, busque la acción (Ctrl-F o Cmd-F).</p> </li> 
     <li value="3"> <p>Ver las descripciones de los campos disponibles en la acción seleccionada.</p> </li> 
    </ol> <p>Nota:  <p>Al crear una prueba a través de [!DNL Workfront] Módulo de [!UICONTROL Misc Action], la práctica recomendada es crear una prueba sin ninguna opción avanzada y, a continuación, actualizar la prueba mediante el [!DNL Workfront Proof] API DE SOAP.</p> <p>Para obtener más información sobre la creación de una prueba con [!DNL Workfront] API (que utiliza este módulo), consulte <a href="../../wf-api/tips-tricks-and-troubleshooting/api-create-proof-options-json.md" class="MCXref xref">Añada opciones de revisión avanzadas al crear una prueba a través de la [!DNL Adobe Workfront] API</a></p> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td>Introduzca o asigne el único [!DNL Workfront] ID del registro con el que desea que interactúe el módulo.<p>Para obtener el ID, abra el [!DNL Workfront] en el explorador y copie el texto al final de la dirección URL después de "ID=". Por ejemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de los [!DNL Workfront] tipos de objeto para los que puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Leer un registro]**

Este módulo de acción recupera datos de un único registro.

Especifique el ID del registro. También puede especificar qué registros relacionados desea que lea el módulo.

Por ejemplo, si el registro que está leyendo el módulo es un proyecto, puede especificar que desea que se lean las tareas del proyecto.

El módulo devuelve una matriz de datos de los campos estándar para la salida especificada.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Conexión]</td>

<td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Tipo de registro]</td>

<td>Elija la [!DNL Workfront] tipo de objeto que desea que lea el módulo.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Salidas]</td>

<td> <p>Seleccione la información que desee incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr> 
    <td>Referencias de [!UICONTROL]</td>
   <td>Seleccione cualquier campo de referencia que desee incluir en la salida.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Colecciones]</td>
   <td>Seleccione cualquier campo de referencia que desee incluir en la salida.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL ID]</td>
   <td> <p>Introduzca el único [!DNL Workfront] ID del registro que desea que lea el módulo.</p> <p>Para obtener el ID, abra el [!DNL Workfront] en el explorador y copie el texto al final de la dirección URL después de "ID=". Por ejemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de los [!DNL Workfront] tipos de objeto para los que puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Actualizar registro]**

Este módulo de acción actualiza un objeto, como un proyecto, una tarea o un problema. El módulo le permite seleccionar qué campos del objeto están disponibles en el módulo.

Especifique el ID del registro.

El módulo devuelve el ID del objeto y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Introduzca el único [!DNL Workfront] ID del registro que desea que actualice el módulo.</p> <p>Para obtener el ID, abra el [!DNL Workfront] en el explorador y copie el texto al final de la dirección URL después de "ID=". Por ejemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Record Type]</td> 
   <td> <p>Seleccione el tipo de [!DNL Workfront] que desea que el módulo actualice.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!DNL Select fields to map]</td> 
   <td>Seleccione los campos que desea que estén disponibles para la entrada de datos. Esto le permite utilizar estos campos sin tener que desplazarse por los que no necesita.</td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de los [!DNL Workfront] tipos de objeto para los que puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Al introducir el ID de un objeto, puede empezar a escribir su nombre y, a continuación, seleccionarlo en la lista. A continuación, el módulo introduce el ID adecuado en el campo.
>* Al introducir el texto de un campo personalizado o una [!UICONTROL Nota] objeto (Comentario o respuesta), puede utilizar etiquetas de HTML en la variable [!UICONTROL Texto de nota] para crear texto enriquecido, como negrita o cursiva.
>
>  Para obtener más información sobre el texto enriquecido en las actualizaciones, consulte [Agregar una actualización a un elemento de trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Cargar documento]**

Este módulo de acción carga un documento en una [!DNL Workfront] objeto, como un proyecto, una tarea o un problema.

Especifique la ubicación del documento, el archivo que desea cargar y, opcionalmente, un nuevo nombre para el archivo.

El módulo devuelve el ID del documento y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Identificador de registro relacionado]</td> 
   <td>Introduzca el único [!DNL Workfront] ID del registro en el que desea cargar el documento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro relacionado]</td> 
   <td>Seleccione el tipo de [!DNL Workfront] registre dónde desea que el módulo cargue el documento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de los [!DNL Workfront] tipos de objeto para los que puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

### Búsquedas

<!--
* [Read Related Records](#read-related-records) 
* [Search](#search)
-->

+++ **[!UICONTROL Leer registros relacionados]**

Este módulo de búsqueda lee registros que coinciden con la consulta de búsqueda especificada, en un objeto principal concreto.

Especifique qué campos desea incluir en la salida. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de registro principal (objeto Workfront) cuyos registros asociados desea leer.</p> <p>Consulte una lista de los [!DNL Workfront] tipos de objeto para los que puede utilizar este módulo en <a href="#object-types-available-for-each-workfront-search-module" class="MCXref xref">[!DNL Workfront] tipos de objeto disponibles para cada [!DNL Workfront] módulo</a> en este artículo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Id. de registro principal]</td> 
   <td> <p>Introduzca o asigne el ID del registro principal cuyos registros asociados desea leer.</p> <p>Para obtener el ID, abra el [!DNL Workfront] en el explorador y copie el texto al final de la dirección URL después de "ID=". Por ejemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Colecciones]</td> 
   <td>Seleccione o asigne el tipo de registro secundario que desea que lea el módulo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione la información que desee incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Búsqueda]**

Este módulo de búsqueda busca registros en un objeto de [!DNL Workfront] que coincidan con la consulta de búsqueda especificada.

Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] hasta [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de [!DNL Workfront] que desea que el módulo busque.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Conjunto de resultados]</td> 
   <td>Seleccione una opción para especificar si desea que el módulo obtenga el primer resultado que coincida con los criterios de búsqueda o todos los resultados que coincidan con él.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Máximo]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Criterios de búsqueda]</td> 
   <td> <p>Introduzca el campo por el que desea buscar, el operador que desea utilizar en la consulta y el valor que está buscando en el campo.</p> <p>Nota: No utilice <code>username </code>en los criterios de búsqueda. Incluyendo <code>username </code>en una consulta API a [!DNL Workfront] inicia sesión del usuario en Workfront y la búsqueda no se realizará correctamente.</p> <p>Nota: <code>In</code> y <code>NotIn</code>trabajar con matrices. Las entradas deben estar en formato de matriz.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione los campos que desea incluir en la salida para este módulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Referencias de [!UICONTROL]</td> 
   <td>Seleccione cualquier campo de referencia que desee incluir en la búsqueda.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Colecciones]</td> 
   <td>Seleccione las colecciones que desee añadir a la búsqueda.</td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de los [!DNL Workfront] tipos de objeto para los que puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

## [!DNL Workfront] tipos de objeto disponibles para cada [!DNL Workfront] módulo

<!-- [Object types available for each Workfront trigger module](#object-types-available-for-each-workfront-trigger-module) 
* [Object types available for each Workfront action module](#object-types-available-for-each-workfront-action-module) 
* [Object types available for each Workfront search module](#object-types-available-for-each-workfront-search-module)-->

+++**Tipos de objeto disponibles para cada [!DNL Workfront] módulo de déclencheur**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Registro del reloj]</th> 
   <th>[!UICONTROL Campo de observación]</th> 
   <th>[!UICONTROL Ver eventos]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Proceso de aprobación</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Asignación</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Línea base</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> Registro de facturación </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tarifa de facturación</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Compañía</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Panel</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Documento</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Carpeta de documentos</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Solicitud de documento</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Versión del documento</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gasto</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Tipo de gasto</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Grupo</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Hora</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Tipo de hora</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Iteración</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Función</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Entrada de cuaderno</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Hito</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ruta de hitos</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Nota</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Etiqueta de nota</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portafolio</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Programar</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Proyecto</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Usuario de proyecto</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aprobación de revisión</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Tiempo reservado* </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Informe</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Riesgo</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de riesgo</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aprobador de etapa</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tarea</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Equipo</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Plantilla</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Tarea de plantilla</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Hoja de horas</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Usuario</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Actualizar</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Tipos de objeto disponibles para cada [!DNL Workfront] módulo de acción**

>[!NOTE]
>
>El [!UICONTROL Descargar documento] Este módulo no se incluye en esta tabla porque [!DNL Workfront] los tipos de objeto no forman parte de su configuración.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Crear un registro]</th> 
   <th>[!UICONTROL Actualizar un registro]</th> 
   <th>[!UICONTROL Eliminar un registro]</th> 
   <th>[!UICONTROL Cargar documento]</th> 
   <th>[!UICONTROL Leer un registro]</th> 
   <th>Llamada de API personalizada de [!UICONTROL]</th> 
   <th>[!UICONTROL Misc Action]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Proceso de aprobación</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Asignación</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Registro de facturación</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tarifa de facturación</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Compañía</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Documento</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Carpeta de documentos</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Versión del documento</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Gasto</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Tipo de gasto</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Grupo</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Hora</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de hora</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Iteración</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Función</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Entrada de cuaderno</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Hito</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ruta de hitos</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Nota</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Etiqueta de nota</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portafolio</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Programar</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Proyecto</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Usuario de proyecto</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tiempo reservado* </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Riesgo</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de riesgo</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aprobador de etapa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tarea</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Equipo</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Plantilla</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tarea de plantilla</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Hoja de horas</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Usuario</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Actualizar</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Tipos de objeto disponibles para cada [!DNL Workfront] módulo de búsqueda**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Buscar]</th> 
   <th>[!UICONTROL Leer registros relacionados]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Proceso de aprobación</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Asignación</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Registro de facturación</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tarifa de facturación</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Compañía</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Documento</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Carpeta de documentos</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Versión del documento</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gasto</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de gasto</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Grupo</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Hora</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de hora</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problema</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Iteración</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Función</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Entrada de cuaderno</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Hito</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ruta de hitos</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Nota</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Etiqueta de nota</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portafolio</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Programar</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Proyecto</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Usuario de proyecto</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tiempo reservado* </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Riesgo</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tipo de riesgo</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aprobador de etapa</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tarea</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Equipo</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Plantilla</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tarea de plantilla</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Hoja de horas</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Usuario</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Delegación de usuario</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

Le recomendamos que verifique dos veces para asegurarse de que esto funciona de la manera que esperaba.

+++

## Filtros de suscripción de evento en la [!DNL Workfront] > [!UICONTROL Ver eventos] módulos

>[!NOTE]
>
>Recomendamos encarecidamente el uso de filtros de suscripción de evento en su [!UICONTROL Ver eventos] módulos.

El [!DNL Workfront] [!UICONTROL Ver eventos] módulo déclencheur escenarios basados en un webhook que crea una suscripción de evento en el [!DNL Workfront] API. La suscripción de evento es un conjunto de datos que determina qué eventos se envían al gancho web. Por ejemplo, si configura un [!UICONTROL Ver eventos] que está viendo problemas, la suscripción de evento solo envía eventos relacionados con los problemas.

Mediante filtros de suscripción de evento, los usuarios de Fusion pueden crear suscripciones de evento que se adapten mejor a sus casos de uso. Por ejemplo, puede configurar una suscripción de evento en la variable [!DNL Workfront] API para enviar solo los problemas que se encuentran en un proyecto específico al webhook, asegurándose de que la variable [!UICONTROL Ver eventos] El módulo solo entrará en déclencheur para los problemas de ese proyecto. La capacidad de crear déclencheur más estrechos mejora el diseño de escenarios al reducir el número de déclencheur irrelevantes.

Esto es diferente a configurar un filtro en la [!DNL Workfront Fusion] escenario. Sin un filtro de suscripción de eventos, el webhook recibe todos los eventos relacionados con el tipo de objeto seleccionado. La mayoría de estos eventos serían irrelevantes para el escenario y deben filtrarse para que el escenario pueda continuar.

Los siguientes operadores están disponibles en el filtro Workfront > Ver eventos:

* Es igual a
* No es igual a
* Bueno que
* Menor que
* Bueno que o igual a
* Menor o igual que
* Contiene
* Existe
   * Este operador no requiere un valor y el campo de valor está ausente.
* No existe
   * Este operador no requiere un valor y el campo de valor está ausente.
* Cambiado
   * Este operador no requiere un valor y el campo de valor está ausente.
   * Este operador ignora el campo State.
   * Al utilizar `Changed`, seleccione **Solo eventos actualizados** en el **Origen de registro** field.

>[!IMPORTANT]
>
>No puede editar filtros en filtros existentes [!DNL Workfront] webhooks. Para configurar diferentes filtros para [!DNL Workfront] Suscripciones de eventos, elimine el webhook actual y cree uno nuevo.

>[!INFO]
>
>**Ejemplo:** Considere un escenario que procese nuevos problemas asignados a un usuario específico, Ana.
>
>### Filtrado de eventos mediante un filtro de suscripción de eventos (recomendado)
>
>Mediante el filtro de eventos, puede configurar el webhook para que almacene en déclencheur el escenario cuando se asigne un problema a Ana cuando se cree el problema. Ana tiene el userID b378489d8f7cd3cee0539260720a84b7.
>
>![](assets/event-filter-watch-events-350x277.png)
>
>Si se crean 100 problemas en un día, pero solo dos de ellos se asignan a Ana, el escenario se ejecutaría dos veces.
>
>### Filtrar eventos dentro del escenario (no recomendado)
>
>Para filtrar eventos de modo que solo se procesen los problemas asignados a Ana, puede crear un filtro después de [!UICONTROL Ver eventos] módulo.
>
>![](assets/watch-events-non-event-filter-350x206.png)
>
>Si se crean 100 problemas en un día, pero solo dos de ellos se asignan a Ana, el escenario se ejecutaría 100 veces. 98 de las ejecuciones se detendrían en el filtro, pero el módulo de déclencheur sigue consumiendo datos y realizando operaciones en todas las ejecuciones.

Para obtener más información sobre las suscripciones a eventos, consulte [Preguntas frecuentes - Suscripciones de eventos](../../wf-api/general/event-subs-faq.md).

Para obtener más información sobre los webhooks, consulte [Déclencheur instantáneos (webhooks) en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)

Para obtener más información sobre los filtros en escenarios, consulte [Adición de un filtro a un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

