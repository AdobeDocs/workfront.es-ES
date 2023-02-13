---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos de Adobe Workfront
description: Puede utilizar el conector Adobe Workfront de Adobe Workfront Fusion para automatizar sus procesos en Workfront. Si tiene una licencia de Workfront Fusion para automatización de trabajo e integración, también puede utilizarla para conectarse a aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: b84d2d41-a983-4ea3-b331-0302bfcf8a2b
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '5276'
ht-degree: 3%

---

# [!DNL Adobe Workfront] módulos

Puede usar la variable [!DNL Adobe Workfront Fusion] [!DNL Adobe Workfront] conector para automatizar los procesos en [!DNL Workfront]. Si tiene una [!UICONTROL [!DNL Workfront Fusion] para la automatización e integración del trabajo] licencia, también puede utilizarla para conectarse a aplicaciones y servicios de terceros.

La variable [!DNL Workfront] El conector no cuenta con el número de aplicaciones activas disponibles para su organización. Todos los escenarios, incluso si solo utilizan la variable [!DNL Workfront] aplicación, haga un recuento con el recuento total de escenarios de su organización.

Para obtener más información sobre las aplicaciones y los escenarios disponibles de su organización, consulte [Organizaciones](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2) en [[!DNL Adobe Workfront Fusion] organizaciones y equipos](../../workfront-fusion/organizations/organizations-and-teams.md).

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>


Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connect [!DNL Workfront] a [!DNL Workfront Fusion]

La variable [!DNL Workfront] El conector utiliza OAuth 2.0 para conectarse a [!DNL Workfront].

Puede crear una conexión con su [!DNL Workfront] cuenta directamente desde dentro de un [!DNL Workfront Fusion] módulo.

1. En cualquier [!DNL Workfront] módulo de aplicación, haga clic en **[!UICONTROL Agregar]** junto a la variable [!UICONTROL Conexión] en la ventana
1. Introduzca el nombre de la instancia en la dirección URL. Ejemplo: `https://<your instance>.my.workfront.com`.
1. Haga clic en **[!UICONTROL Siguiente]**.
1. Haga clic en **[!UICONTROL Inicio de sesión en SAML]** para crear la conexión y volver al módulo .

   O

   Introduzca su nombre de usuario y contraseña y, a continuación, haga clic en **[!UICONTROL Iniciar sesión]** para crear la conexión y volver al módulo .

   >[!NOTE]
   >
   >* Si no ve un botón de inicio de sesión SAML, su organización no ha habilitado el inicio de sesión único (SSO). Puede iniciar sesión con su nombre de usuario y contraseña.
      >   
      >   Para obtener más información sobre SSO, consulte [Información general sobre el inicio de sesión único [!DNL Adobe Workfront]](../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)
   >   
   >* Conexiones de OAuth 2.0 con la variable [!DNL Workfront] La API ya no depende de claves de API.


## [!DNL Workfront] módulos y sus campos

Al configurar [!DNL Workfront] módulos, [!DNL Workfront Fusion] muestra los campos que se enumeran a continuación. Además de estos, se incluyen [!DNL Workfront] pueden mostrarse los campos, en función de factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón de asignación encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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

+++ **[!UICONTROL Eventos de Watch]**

Este módulo de déclencheur ejecuta un escenario en tiempo real cuando se agregan, actualizan o eliminan objetos de un tipo específico en Workfront

El módulo devuelve todos los campos estándar asociados con el registro, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

1. Haga clic en **[!UICONTROL Agregar]** a la derecha del **Weblock** en la ventana

1. Configure el vínculo web en la variable **[!UICONTROL Añadir un gancho]** que se muestra.

   Al configurar este módulo, se muestran los campos siguientes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Nombre de Weblock]</td> 
      <td>(Opcional) Escriba un nuevo nombre para el vínculo web</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Connection]</td> 
      <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Tipo de registro]</td> 
      <td>Seleccione el tipo de [!DNL Workfront] registre que desea que el módulo vea.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL State]</td> 
      <td>Seleccione si desea ver el estado antiguo o el nuevo.<ul><li><p><b>[!UICONTROL Nuevo estado]</b></p><p>Déclencheur de un escenario cuando cambie el registro <b>a</b> un valor determinado.</p><p>Por ejemplo, si el estado se establece en [!UICONTROL Nuevo estado] y el filtro se establece en [!UICONTROL estado] [!UICONTROL igual a] [!UICONTROL en curso], el vínculo web déclencheur un escenario cuando el [!UICONTROL estado] cambia a [!UICONTROL en curso], independientemente del estado anterior. </p></li><li><p><b>[!UICONTROL Estado antiguo]</b></p><p>Déclencheur de un escenario cuando cambie el registro <b>from</b> un valor determinado.</p><p>Por ejemplo, si el estado se establece en [!UICONTROL Old State] y el filtro se establece en [!UICONTROL Status] [!UICONTROL Equals] [!UICONTROL In Progress], el enlace web déclencheur un escenario cuando un [!UICONTROL Status] que actualmente es [!UICONTROL In Progress] cambia a otro estado. </p></li></ul></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Filtros de eventos]</p> </td> 
      <td> <p>Puede definir filtros para que solo vean los registros que cumplan los criterios seleccionados.</p> <p>Para cada filtro, introduzca el campo que desea que evalúe el filtro, el operador y el valor que desea que permita el filtro. Puede utilizar más de un filtro añadiendo reglas AND.</p> <p>Nota: No se pueden editar filtros en [!DNL Workfront] webhooks. Para configurar diferentes filtros para [!DNL Workfront] suscripciones a eventos, elimine el weblink actual y cree uno nuevo.</p> <p>Para obtener más información sobre los filtros de evento, consulte <a href="#event-subscription-filters-in-the-workfront-watch-events-modules" class="MCXref xref">Filtros de suscripción de eventos en la [!DNL Workfront] &gt; Módulos de [!UICONTROL Watch Events]</a> en este artículo.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Excluir eventos realizados por esta conexión</td> 
      <td>Active esta opción para excluir los eventos creados o actualizados con el mismo conector que utiliza este módulo de déclencheur. Esto puede evitar situaciones en las que un escenario se pueda déclencheur a sí mismo, lo que hace que se repita en un bucle sin fin.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Record Origin]</td> 
      <td> <p>Elija si desea que el escenario vea <strong>[!UICONTROL Sólo Registros Nuevos]</strong>, <strong>[!UICONTROL Registros actualizados solamente]</strong>, <strong>[!UICONTROL Registros nuevos y actualizados]</strong>o <strong>[!DNL Deleted Records Only]</strong>.</p> <p>Nota: Si elige <strong>[!UICONTROL Registros nuevos y actualizados]</strong>, la creación de weblock crea 2 suscripciones de evento (para la misma dirección de weblock).</p> </td> 
     </tr> 
    </tbody> 
   </table>

Una vez creado el vínculo web, puede ver la dirección del extremo al que se envían los eventos.

Para obtener más información, consulte la sección [Ejemplos de cargas de eventos](../../wf-api/general/event-subs-api.md#examples-of-event-payloads) en el [!DNL Workfront] Artículo de ayuda [API de suscripción de evento](../../wf-api/general/event-subs-api.md).

Consulte una lista de [!DNL Workfront] tipos de objetos para los que se puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Campo de inspección]**

Este módulo de déclencheur ejecuta un escenario cuando se actualiza un campo especificado. El módulo devuelve el valor antiguo y el nuevo del campo especificado. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de [!DNL Workfront] registre que desea que el módulo vea.</p> <p>Por ejemplo, seleccione [!UICONTROL Task] si desea comenzar a ejecutar el escenario cada vez que se actualice un campo de registro en una tarea.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Field]</td> 
   <td>Seleccione el campo que desea que el módulo vea para las actualizaciones. Estos campos reflejan los campos que [!DNL Workfront] administrador se ha configurado para el seguimiento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Salidas]</td> 
   <td>Seleccione la información que desee incluir en el paquete de salida para este módulo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de [!DNL Workfront] tipos de objetos para los que se puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Registro de Watch]**

Este módulo de déclencheur ejecuta un escenario cuando se agregan, actualizan o ambas cosas objetos de un tipo específico. El módulo devuelve todos los campos estándar asociados con el registro o registros, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario. En la salida, el módulo indica si cada registro es nuevo o actualizado.

Los registros que se agregaron y actualizaron en el período de tiempo dado se devuelven como registros nuevos.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro]</td> 
   <td> <p>Elija si desea que el escenario vea <strong>[!UICONTROL Sólo Registros Nuevos]</strong>, <strong>[!UICONTROL Registros actualizados solamente]</strong>o <strong>[!UICONTROL Registros nuevos y actualizados]</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de registro]</td> 
   <td> <p>(Se muestra después de elegir una <strong>Filtro</strong>.) Seleccione el tipo de [!DNL Workfront] registre que desea que el módulo vea.</p> <p>Por ejemplo, si desea iniciar el escenario cada vez que se cree un nuevo proyecto, seleccione [!UICONTROL Proyecto]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione la información que desee incluir en el paquete de salida para este módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtro opcional]</td> 
   <td> <p>(Avanzado) Escriba una cadena de código de API para definir cualquier parámetro o código adicional que vaya a refinar los criterios. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de [!DNL Workfront] tipos de objetos para los que se puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

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

* Convertir un problema a un proyecto
* Convertir problema a tarea
* Convertir tarea a proyecto

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tipo de objeto]</td> 
   <td> <p>Seleccione el tipo de objeto que desea convertir. Es el tipo que tiene el objeto antes de la conversión.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Convertir en]</td> 
   <td>Seleccione el objeto al que desea convertirlo. Es el tipo que tiene el objeto después de la conversión.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL &lt;object&gt; ID]</td> 
   <td> <p>Introduzca el ID del objeto. </p> <p>Nota: Al introducir el ID de un objeto, puede empezar a escribir el nombre del objeto y, a continuación, seleccionarlo en la lista. A continuación, el módulo introduce la ID adecuada en el campo .</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Template ID]</td> 
   <td> <p>Si va a realizar la conversión a un proyecto, seleccione el ID de plantilla que desee utilizar para el proyecto.</p> <p>Nota: Al introducir el ID de un objeto, puede empezar a escribir el nombre del objeto y, a continuación, seleccionarlo en la lista. A continuación, el módulo introduce la ID adecuada en el campo .</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Formularios personalizados]</td> 
   <td>Seleccione los formularios personalizados que desee agregar al objeto recién convertido y, a continuación, introduzca valores para los campos del formulario personalizado.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Opciones]</td> 
   <td> <p>Active las opciones que desee al convertir el objeto. Las opciones están disponibles en función del objeto desde el que realice la conversión.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Crear un registro (adjuntar formularios personalizados)]**

Este módulo de acción crea un objeto, como un proyecto, una tarea o un problema en [!DNL Workfront]y le permite agregar un formulario personalizado al nuevo objeto. El módulo le permite seleccionar qué campos del objeto están disponibles en el módulo.

Especifique el ID del registro.

El módulo devuelve el ID del registro y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Puede utilizar este módulo, por ejemplo, para crear una tarea en [!DNL Workfront] cuando un cliente agrega una fila nueva en una [!DNL Google Sheets] lista de tareas que deben realizarse.

Al configurar este módulo, se muestran los campos siguientes:

Asegúrese de proporcionar el número mínimo de campos de entrada. Por ejemplo, si desea crear un problema, debe proporcionar un ID de proyecto principal válido en el campo ID del proyecto para indicar dónde debe plantearse el problema en Workfront. Puede utilizar el panel de asignación para asignar esta información de otro módulo de su escenario o puede introducirla manualmente escribiendo el nombre y seleccionándolo a continuación en la lista.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de [!DNL Workfront] registro que desea que cree el módulo.</p> <p>Por ejemplo, si desea crear un proyecto, seleccione [!UICONTROL Project] en la lista desplegable y, a continuación, asegúrese de que tiene acceso a los datos (de módulos anteriores en el escenario) que rellenarán el proyecto.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Seleccionar campos para asignar]</td> 
   <td> <p>Seleccione los campos que desea que estén disponibles para la entrada de datos. Esto le permite utilizar estos campos sin tener que desplazarse por los que no necesita.</p> <p>Para los campos de los formularios personalizados, utilice la variable <b>[!UICONTROL Adjuntar formulario personalizado]</b> campo .</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Adjuntar formulario personalizado]</td> 
   <td>Seleccione los formularios personalizados que desee agregar al nuevo objeto y, a continuación, introduzca valores para esos campos.</td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de [!DNL Workfront] tipos de objetos para los que se puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Al introducir el ID de un objeto, puede empezar a escribir el nombre del objeto y, a continuación, seleccionarlo en la lista. A continuación, el módulo introduce la ID adecuada en el campo .
>* Al introducir el texto de un campo personalizado o de un [!UICONTROL Nota] (Comentario o respuesta), puede utilizar etiquetas HTML en la variable [!UICONTROL Texto de la nota] para crear texto enriquecido, como texto en negrita o cursiva.
>
>  Para obtener más información sobre el texto enriquecido en las actualizaciones, consulte [Agregar una actualización a un elemento de trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) en [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

+++

+++ **[!UICONTROL Crear registro]**

Este módulo de acción crea un objeto, como un proyecto, una tarea o un problema en Workfront. El módulo le permite seleccionar qué campos del objeto están disponibles en el módulo.

Especifique el ID del registro.

El módulo devuelve el ID del registro y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Puede utilizar este módulo, por ejemplo, para crear una tarea en [!DNL Workfront] cuando un cliente agrega una fila nueva en una lista de hojas de Google de tareas que deben realizarse.

Al configurar este módulo, se muestran los campos siguientes:

Asegúrese de proporcionar el número mínimo de campos de entrada. Por ejemplo, si desea crear un problema, debe proporcionar un ID de proyecto principal válido en el campo ID del proyecto para indicar dónde debe plantearse el problema en Workfront. Puede utilizar el panel de asignación para asignar esta información de otro módulo de su escenario o puede introducirla manualmente escribiendo el nombre y seleccionándolo a continuación en la lista.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de [!DNL Workfront] registro que desea que cree el módulo.</p> <p>Por ejemplo, si desea crear un proyecto, seleccione [!UICONTROL Project] en la lista desplegable y, a continuación, asegúrese de que tiene acceso a los datos (de módulos anteriores en el escenario) que rellenarán el proyecto.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Seleccionar campos para asignar]</td> 
   <td>Seleccione los campos que desea que estén disponibles para la entrada de datos. Esto le permite utilizar estos campos sin tener que desplazarse por los que no necesita.</td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de [!DNL Workfront] tipos de objetos para los que se puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Al introducir el ID de un objeto, puede empezar a escribir el nombre del objeto y, a continuación, seleccionarlo en la lista. A continuación, el módulo introduce la ID adecuada en el campo .
>* Al introducir el texto de un campo personalizado o de un [!UICONTROL Nota] (Comentario o respuesta), puede utilizar etiquetas HTML en la variable [!UICONTROL Texto de la nota] para crear texto enriquecido, como texto en negrita o cursiva.
>
>  Para obtener más información sobre el texto enriquecido en las actualizaciones, consulte [Agregar una actualización a un elemento de trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) en [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

+++

+++ **[!UICONTROL Llamada de API personalizada]**

Este módulo de acción le permite realizar una llamada autenticada personalizada al [!DNL Workfront] API. De este modo, puede crear una automatización del flujo de datos que no se pueda lograr con la otra [!DNL Workfront] módulos.

El módulo devuelve la siguiente información:

* **[!UICONTROL Código de estado]** (número): Esto indica el éxito o el error de la solicitud HTTP. Estos son códigos estándar que se pueden consultar en Internet.
* **[!UICONTROL Encabezados]** (objeto): Un contexto más detallado para el código de respuesta/estado que no está relacionado con el cuerpo de salida. No todos los encabezados que aparecen en un encabezado de respuesta son encabezados de respuesta, por lo que es posible que algunos no sean útiles para usted.

   Los encabezados de respuesta dependen de la solicitud HTTP que haya elegido al configurar el módulo.

* **[!UICONTROL Cuerpo]** (objeto): Según la solicitud HTTP que haya elegido al configurar el módulo, puede recibir algunos datos de vuelta. Esos datos, como los datos de una solicitud de GET, están contenidos en este objeto.

Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Dirección URL</td> 
   <td> <p>Especifique una ruta relativa a<code> https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API Version]</td> 
   <td>Seleccione la versión del [!DNL Workfront] que desea que utilice el módulo de .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   td&gt; <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada a la API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar. Esto determina el tipo de contenido de la solicitud.</p> <p>Por ejemplo,<code> {"Content-type":"application/json"}</code></p> <p>Nota: Si está obteniendo errores y es difícil determinar su origen, considere la posibilidad de modificar los encabezados en función del [!DNL Workfront] documentación. Si su llamada de API personalizada devuelve un error de solicitud HTTP 422, intente utilizar un <code>"Content-Type":"text/plain"</code> encabezado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p> <p>Sugerencia: Le recomendamos que envíe información a través del cuerpo de JSON en lugar de como parámetros de consulta.</p> </td> 
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

Consulte una lista de [!DNL Workfront] tipos de objetos para los que se puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Eliminar registro]**

Este módulo de acción elimina un objeto, como un proyecto, una tarea o un problema de Workfront.

Especifique el ID del registro.

El módulo devuelve el ID del registro y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Force delete]</td> 
   <td>Active esta opción para asegurarse de que se elimina el registro, incluso si la variable [!DNL Workfront] La interfaz de usuario solicitaría la confirmación de la eliminación.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Identificador</td> 
   <td> <p>Escriba la variable única [!DNL Workfront] ID del registro que desea que elimine el módulo.</p> <p>Para obtener el ID, abra el [!DNL Workfront] en el explorador y copie el texto al final de la dirección URL después de "ID=." Por ejemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td>Seleccione el tipo de [!DNL Workfront] registro que desea que el módulo elimine.</td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de [!DNL Workfront] tipos de objetos para los que se puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Descargar documento]**

Este módulo de acción descarga un documento de Workfront.

Especifique el ID del registro.

El módulo devuelve el contenido, el nombre de archivo, la extensión de archivo y el tamaño de archivo del documento. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document ID]</td> 
   <td> <p>Asignar o introducir manualmente la variable única [!DNL Workfront] ID del documento que desea que descargue el módulo.</p> <p>Para obtener el ID, abra el [!DNL Workfront] en el explorador y copie el texto al final de la dirección URL después de "ID=." Por ejemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de [!DNL Workfront] tipos de objetos para los que se puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Acción Misc]**

Este módulo de acción permite realizar acciones con la API.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de [!DNL Workfront] registro con el que desea que el módulo interactúe.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Action]</td> 
   <td> <p>Seleccione la acción que desea que realice el módulo.</p> <p>Es posible que necesite rellenar campos adicionales, según el [!UICONTROL Record Type] y la [!UICONTROL Action] que elija. Algunas combinaciones de estas dos configuraciones pueden requerir únicamente un ID de registro, mientras que otras (como Project para el <strong>[!UICONTROL Tipo de registro]</strong> y [!UICONTROL Adjuntar plantilla] para <strong>[!UICONTROL Action]</strong>) requieren información adicional (como un ID de objeto y un ID de plantilla).</p> <p>Para obtener más información sobre campos individuales, consulte la <a href="http://developer.workfront.com/">Documentación para desarrolladores de Workfront</a>. </p> 
    <ol> 
     <li value="1"> <p>Seleccione el tipo de registro en la navegación izquierda del [!DNL Workfront] página de documentación para desarrolladores. Los siguientes tipos tienen sus propias páginas:</p> 
      <ul> 
       <li> <p>[!UICONTROL Proyectos]</p> </li> 
       <li> <p>[!UICONTROL Tasks]</p> </li> 
       <li> <p>[!UICONTROL Problemas]</p> </li> 
       <li> <p>[!UICONTROL Usuarios]</p> </li> 
       <li> <p>[!UICONTROL Documents]</p> </li> 
      </ul> <p>Para todos los demás tipos de registros, seleccione <b>[!UICONTROL Otros objetos y extremos]</b>y busque el tipo de registro en las páginas ordenadas alfabéticamente.</p> </li> 
     <li value="2"> <p>En la página del tipo de registro correspondiente, busque la acción (Ctrl-F o Cmd-F).</p> </li> 
     <li value="3"> <p>Vea las descripciones de los campos disponibles en la acción seleccionada.</p> </li> 
    </ol> <p>Nota:  <p>Al crear una prueba a través del [!DNL Workfront] módulo de [!UICONTROL Misc Action], se recomienda crear una prueba sin ninguna opción avanzada y, a continuación, actualizar la prueba utilizando la variable [!DNL Workfront Proof] API SOAP.</p> <p>Para obtener más información sobre la creación de una prueba con la variable [!DNL Workfront] API (que utiliza este módulo), consulte <a href="../../wf-api/tips-tricks-and-troubleshooting/api-create-proof-options-json.md" class="MCXref xref">Añada opciones de prueba avanzadas al crear una prueba mediante el [!DNL Adobe Workfront] API</a></p> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td>Introduzca o asigne la variable única [!DNL Workfront] ID del registro con el que desea que interactúe el módulo.<p>Para obtener el ID, abra el [!DNL Workfront] en el explorador y copie el texto al final de la dirección URL después de "ID=." Por ejemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de [!DNL Workfront] tipos de objetos para los que se puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Leer un registro]**

Este módulo de acción recupera datos de un solo registro.

Especifique el ID del registro. También puede especificar qué registros relacionados desea que lea el módulo.

Por ejemplo, si el registro que está leyendo el módulo es un proyecto, puede especificar que desea que se lean las tareas del proyecto.

El módulo devuelve una matriz de datos de los campos estándar para la salida especificada.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>

<td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
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
    <td>[!UICONTROL Referencias]</td>
   <td>Seleccione los campos de referencia que desee incluir en la salida.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Colecciones]</td>
   <td>Seleccione los campos de referencia que desee incluir en la salida.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL ID]</td>
   <td> <p>Escriba la variable única [!DNL Workfront] ID del registro que desea que lea el módulo.</p> <p>Para obtener el ID, abra el [!DNL Workfront] en el explorador y copie el texto al final de la dirección URL después de "ID=." Por ejemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de [!DNL Workfront] tipos de objetos para los que se puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Actualizar registro]**

Este módulo de acción actualiza un objeto, como un proyecto, una tarea o un problema. El módulo le permite seleccionar qué campos del objeto están disponibles en el módulo.

Especifique el ID del registro.

El módulo devuelve el ID del objeto y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Escriba la variable única [!DNL Workfront] ID del registro que desea que actualice el módulo.</p> <p>Para obtener el ID, abra el [!DNL Workfront] en el explorador y copie el texto al final de la dirección URL después de "ID=." Por ejemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Record Type]</td> 
   <td> <p>Seleccione el tipo de [!DNL Workfront] registro que desea que el módulo se actualice.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!DNL Select fields to map]</td> 
   <td>Seleccione los campos que desea que estén disponibles para la entrada de datos. Esto le permite utilizar estos campos sin tener que desplazarse por los que no necesita.</td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de [!DNL Workfront] tipos de objetos para los que se puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Al introducir el ID de un objeto, puede empezar a escribir el nombre del objeto y, a continuación, seleccionarlo en la lista. A continuación, el módulo introduce la ID adecuada en el campo .
>* Al introducir el texto de un campo personalizado o de un [!UICONTROL Nota] (Comentario o respuesta), puede utilizar etiquetas HTML en la variable [!UICONTROL Texto de la nota] para crear texto enriquecido, como texto en negrita o cursiva.
>
>  Para obtener más información sobre el texto enriquecido en las actualizaciones, consulte [Agregar una actualización a un elemento de trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) en [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

+++

+++ **[!UICONTROL Cargar documento]**

Este módulo de acción carga un documento en un [!DNL Workfront] como un proyecto, una tarea o un problema.

Especifique la ubicación del documento, el archivo que desea cargar y un nombre nuevo opcional para el archivo.

El módulo devuelve el ID del documento y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID de registro relacionado]</td> 
   <td>Escriba la variable única [!DNL Workfront] ID del registro en el que desea cargar el documento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro relacionado]</td> 
   <td>Seleccione el tipo de [!DNL Workfront] registro en el que desea que el módulo cargue el documento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archivo de origen]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de [!DNL Workfront] tipos de objetos para los que se puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

### Búsquedas

<!--
* [Read Related Records](#read-related-records) 
* [Search](#search)
-->

+++ **[!UICONTROL Leer registros relacionados]**

Este módulo de búsqueda lee registros que coinciden con la consulta de búsqueda especificada, en un objeto principal concreto.

Puede especificar qué campos desea incluir en la salida. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo del registro principal (objeto Workfront) cuyos registros asociados desee leer.</p> <p>Consulte una lista de [!DNL Workfront] tipos de objetos para los que se puede utilizar este módulo en <a href="#object-types-available-for-each-workfront-search-module" class="MCXref xref">[!DNL Workfront] tipos de objetos disponibles para cada [!DNL Workfront] módulo</a> en este artículo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Parent Record ID]</td> 
   <td> <p>Introduzca o asigne el ID del registro principal cuyos registros asociados desee leer.</p> <p>Para obtener el ID, abra el [!DNL Workfront] en el explorador y copie el texto al final de la dirección URL después de "ID=." Por ejemplo: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
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

+++ **[!UICONTROL Buscar]**

Este módulo de búsqueda busca registros en un objeto de [!DNL Workfront] que coinciden con la consulta de búsqueda especificada.

Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Workfront] aplicación a [!DNL Workfront Fusion], consulte <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro]</td> 
   <td> <p>Seleccione el tipo de [!DNL Workfront] registro que desea que busque el módulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Conjunto de resultados]</td> 
   <td>Seleccione una opción para especificar si desea que el módulo obtenga el primer resultado que coincida con sus criterios de búsqueda o con todos los resultados que coincidan con él.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Máximo]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Criterios de búsqueda]</td> 
   <td> <p>Introduzca el campo por el que desea buscar, el operador que desea utilizar en la consulta y el valor que está buscando en el campo .</p> <p>Nota: No use <code>username </code>en los criterios de búsqueda. Inclusión <code>username </code>en una consulta de API a [!DNL Workfront] inicia sesión en Workfront y la búsqueda no se realizará correctamente.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Salidas]</td> 
   <td> <p>Seleccione los campos que desea incluir en la salida de este módulo.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Referencias]</td> 
   <td>Seleccione los campos de referencia que desee incluir en la búsqueda.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Colecciones]</td> 
   <td>Seleccione las colecciones que desee agregar a la búsqueda.</td> 
  </tr> 
 </tbody> 
</table>

Consulte una lista de [!DNL Workfront] tipos de objetos para los que se puede utilizar este módulo en [[!DNL Workfront] object types available for each [!DNL Workfront] módulo](#workfront-object-types-available-for-each-workfront-module).

+++

## [!DNL Workfront] tipos de objetos disponibles para cada [!DNL Workfront] módulo

<!-- [Object types available for each Workfront trigger module](#object-types-available-for-each-workfront-trigger-module) 
* [Object types available for each Workfront action module](#object-types-available-for-each-workfront-action-module) 
* [Object types available for each Workfront search module](#object-types-available-for-each-workfront-search-module)-->

+++**Tipos de objetos disponibles para cada [!DNL Workfront] módulo déclencheur**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Watch Record]</th> 
   <th>[!UICONTROL Campo de inspección]</th> 
   <th>[!UICONTROL Watch Events]</th> 
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
   <td>Versión de documento</td> 
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
   <td>Aprobador de pasos</td> 
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

+++**Tipos de objetos disponibles para cada [!DNL Workfront] módulo de acción**

>[!NOTE]
>
>La variable [!UICONTROL Descargar documento] no se incluye en esta tabla porque [!DNL Workfront] los tipos de objetos no forman parte de su configuración.

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
   <th>[!UICONTROL Llamada de API personalizada]</th> 
   <th>[!UICONTROL Acción Misc]</th> 
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
   <td>Versión de documento</td> 
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
   <td>Aprobador de pasos</td> 
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

+++**Tipos de objetos disponibles para cada [!DNL Workfront] módulo de búsqueda**

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
   <td>Versión de documento</td> 
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
   <td>Aprobador de pasos</td> 
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

Le recomendamos que verifique dos veces para asegurarse de que esto funciona del modo esperado.

+++

## Filtros de suscripción de eventos en la [!DNL Workfront] > [!UICONTROL Eventos de Watch] módulos

>[!NOTE]
>
>Recomendamos encarecidamente usar filtros de suscripción de eventos en su [!UICONTROL Eventos de Watch] módulos.

La variable [!DNL Workfront] [!UICONTROL Eventos de Watch] déclencheur de módulos basados en un enlace web que crea una suscripción de evento en el [!DNL Workfront] API. La suscripción de evento es un conjunto de datos que determina qué eventos se envían al vínculo web. Por ejemplo, si configura un [!UICONTROL Eventos de Watch] que está viendo problemas, la suscripción de eventos envía solo eventos relacionados con problemas.

Mediante filtros de suscripción de eventos, los usuarios de Fusion pueden crear suscripciones de eventos que se adapten mejor a sus casos de uso. Por ejemplo, puede configurar una suscripción de evento en la [!DNL Workfront] API para enviar solo los problemas que están en un proyecto específico al vínculo web, asegurándose de que la variable [!UICONTROL Eventos de Watch] solo realizará el déclencheur para problemas en ese proyecto. La capacidad de crear déclencheur más estrechos mejora el diseño del escenario al reducir el número de déclencheur irrelevantes.

Esto es diferente a configurar un filtro en la variable [!DNL Workfront Fusion] escenario. Sin un filtro de suscripción de evento, el vínculo web recibe todos los eventos relacionados con el tipo de objeto seleccionado. La mayoría de estos eventos serían irrelevantes para el escenario y deben filtrarse para que el escenario pueda continuar.

>[!NOTE]
>
>No se pueden editar filtros en [!DNL Workfront] webhooks. Para configurar diferentes filtros para [!DNL Workfront] suscripciones a eventos, elimine el weblink actual y cree uno nuevo.

>[!INFO]
>
>**Ejemplo:** Considere un escenario que procese nuevos problemas asignados a un usuario específico, Ana.
>
>### Filtrado de eventos mediante un filtro de suscripción de eventos (recomendado)
>
>Con el filtro de eventos, puede configurar el enlace web para almacenar en déclencheur el escenario cuando se asigne un problema a Ana cuando se cree el problema. Ana tiene el userID b378489d8f7cd3cee0539260720a84b7.
>
>![](assets/event-filter-watch-events-350x277.png)
>
>Si se crean 100 problemas en un día, pero sólo dos de ellos están asignados a Ana, el escenario se ejecutaría dos veces.
>
>### Filtre eventos dentro del escenario (no recomendado)
>
>Para filtrar eventos de modo que solo se procesen los problemas asignados a Ana, puede crear un filtro después de [!UICONTROL Eventos de Watch] módulo.
>
>![](assets/watch-events-non-event-filter-350x206.png)
>
>Si se crean 100 problemas en un día, pero sólo dos de ellos están asignados a Ana, el escenario se ejecutaría 100 veces. 98 de las ejecuciones se detendrían en el filtro, pero el módulo de déclencheur sigue consumiendo datos y realizando operaciones en todas las ejecuciones.

Para obtener más información sobre las suscripciones a eventos, consulte [Preguntas más frecuentes: Suscripciones a eventos](../../wf-api/general/event-subs-faq.md).

Para obtener más información sobre los enlaces web, consulte [Déclencheur instantáneos (enlaces web) en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)

Para obtener más información sobre filtros en escenarios, consulte [Añadir un filtro a un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).
