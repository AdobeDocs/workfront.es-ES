---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Salesforce
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 3c8adcd9-fb5f-400d-9edd-6d9fc30cc728
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '2806'
ht-degree: 90%

---

# Módulos de [!DNL Salesforce]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Módulos Salesforce](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

En un escenario de Adobe Workfront Fusion, puede automatizar los flujos de trabajo que utilizan [!DNL Salesforce], así como conectarlo a varias aplicaciones y servicios de terceros.

Para ver un vídeo introductorio del conector de Salesforce, consulte:

* [Salesforce](https://video.tv.adobe.com/v/3427027/){target=_blank}

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!NOTE]
>
>* No todas las ediciones de [!DNL Salesforce] tienen acceso a la API. Para obtener más información, consulte la información sobre ediciones de [!DNL Salesforce] con acceso a la API en el sitio de la comunidad de [!DNL Salesforce].
>* Para obtener información sobre los errores específicos que devuelve la API de [!DNL Salesforce], consulte los documentos de la API de [!DNL Salesforce]. También puede comprobar el estado de la API de [!DNL Salesforce] en busca de posibles interrupciones del servicio.
>

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

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
   <td>
   <p>Requisito de licencia actual: no se requiere ninguna licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

Para usar módulos [!DNL Salesforce], debe tener una cuenta de [!DNL Salesforce].

## Información de API de Salesforce

El conector de Salesforce utiliza lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">URL básica</td> 
   <td> {{connection.instanceUrl}}</td>
  </tr> 
  <tr> 
   <td role="rowheader">Versión de API</td> 
   <td> v46.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Etiqueta de API</td> 
   <td>Versión 1.15.14</td> 
  </tr>
 </tbody> 
 </table>

## Acerca de la búsqueda de objetos de [!DNL Salesforce]

Al buscar objetos, puede introducir palabras de búsqueda individuales o crear una consulta más compleja utilizando comodines y operadores:

* Utilice el comodín de asterisco (\*) como sustituto de cero o más caracteres. Por ejemplo, una búsqueda de Ca\* encuentra elementos que empiezan por Ca
* Utilice un signo de interrogación comodín (?) como sustituto de un solo carácter. Por ejemplo, una búsqueda de Jo?n encuentra elementos con el término John o Joan pero no Jon
* Utilice el operador de comillas (&quot;&quot;) para encontrar una coincidencia de frase exacta. Por ejemplo: “reunión del lunes&quot;

Para obtener más información sobre las posibilidades de búsqueda, consulte la documentación para desarrolladores de [!DNL Salesforce] sobre SOQL y SOSL.

## Módulos de [!DNL Salesforce] y sus campos

* [Activadores](#triggers)
* [Acciones](#actions)
* [Búsquedas](#searches)

### Activadores

* [[!UICONTROL Ver registros]](#watch-for-records)
* [[!UICONTROL Ver mensajes salientes]](#watch-outbound-messages)
* [[!UICONTROL Ver un campo]](#watch-a-field)

#### [!UICONTROL Observar registros]

Este módulo activador ejecuta un escenario cuando se crea o actualiza un registro de un objeto. El módulo devuelve todos los campos estándar asociados con el registro o registros, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Salesforce] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type] </td> 
   <td> <p>Seleccione el tipo de registro de [!DNL Salesforce] que desea que observe el módulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Fields]</td> 
   <td>Seleccione los campos que desea que observe el módulo. Los campos disponibles dependen del tipo de registro.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximal count of records]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p>Determine si desea que el escenario observe solo los registros nuevos del tipo seleccionado, o los registros nuevos del tipo seleccionado y todos los demás cambios realizados en los registros de ese tipo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Observar mensajes salientes]

Este módulo activador ejecuta un escenario cuando alguien envía un mensaje. El módulo devuelve todos los campos estándar asociados con el registro o registros, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Este módulo requiere cierta configuración adicional:

1. Vaya a la página de configuración de [!DNL Salesforce].

   Para tener acceso a la página de instalación, busque y haga clic en el botón con la etiqueta &quot;[!UICONTROL Configuración]&quot; en la esquina superior derecha de la cuenta de [!DNL Salesforce]. En la página de configuración de [!DNL Salesforce], busque la barra &quot;[!UICONTROL Búsqueda rápida / Búsqueda]&quot; en el lado izquierdo. Busque &quot;[!UICONTROL Reglas de flujo de trabajo]&quot;.

1. Haga clic en **[!UICONTROL Reglas de flujo de trabajo]**.
1. En la página [!UICONTROL Reglas de flujo de trabajo] que aparece, haga clic en **[!UICONTROL Nueva regla]** y seleccione el tipo de objeto al que se aplicará la regla (como &quot;[!UICONTROL Oportunidad]&quot; si supervisa las actualizaciones de los registros de oportunidad).
1. Haga clic en **[!UICONTROL Siguiente]**.
1. Defina un nombre de regla, criterios de evaluación y criterios de regla, y luego haga clic en **[!UICONTROL Guardar]** y **[!UICONTROL Siguiente]**.

1. Haga clic en **[!UICONTROL Completado]**.
1. En la regla de flujo de trabajo recién creada, haga clic en **[!UICONTROL Editar]**.
1. En la lista desplegable **[!UICONTROL Añadir acción de flujo de trabajo]**, seleccione **[!UICONTROL Nuevo mensaje saliente]**.

1. Especifique el nombre, la descripción, la dirección URL de extremo y los campos que desee incluir en el nuevo mensaje saliente y, a continuación, haga clic en **[!UICONTROL Guardar]**.

   El campo **[!UICONTROL Dirección URL de extremo]** contiene la dirección URL proporcionada en el [!DNL Salesforce] [!UICONTROL Mensaje saliente] de [!DNL Workfront Fusion].

1. Configure un escenario que comience con el evento [!UICONTROL Mensaje saliente].

1. Haga clic en el icono **&lt;/>** en la parte inferior derecha y copie la dirección URL proporcionada.
1. Vuelva a la página **[!UICONTROL Reglas de flujo de trabajo]**, busque la regla recién creada y haga clic en **[!UICONTROL Activar]**.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td> <p>Seleccione el webhook que desee utilizar para observar los mensajes salientes. Para agregar un webhook, haga clic en <strong>[!UICONTROL Add]</strong> e introduzca el nombre y la conexión del webhook.</p> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Salesforce] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!UICONTROL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>Seleccione el tipo de registro de [!DNL Salesforce] que desea que observe el módulo en busca de mensajes salientes.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fields]</td> 
   <td> <p>Seleccione los campos que desea que el módulo observe para detectar mensajes salientes. Los campos disponibles dependen del tipo de registro.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### *[!UICONTROL Observar un campo]*

Este módulo activador inicia un escenario cuando se actualiza un campo en [!DNL Salesforce].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Salesforce] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>Seleccione el tipo de registro que contiene el campo que desea que el módulo vea. Debe elegir un tipo de registro que tenga [!UICONTROL Field History] activado en la configuración de [!DNL Salesforce]. Para obtener más información, consulte <a href="https://help.salesforce.com/articleView?id=tracking_field_history.htm&amp;type=5">Seguimiento del historial de campos</a> en la documentación de [!DNL Salesforce]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Field]</td> 
   <td> <p>Seleccione los campos en los que desea que el módulo vea los cambios.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Introduzca o asigne el número máximo de campos que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Crear un registro]](#create-a-record)
* [[!UICONTROL Leer un registro]](#read-a-record)
* [[!UICONTROL Eliminar un grupo]](#delete-a-record)
* [[!UICONTROL Llamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Cargar archivo adjunto/documento]](#upload-attachmentdocument)
* [[!UICONTROL Descargar archivo adjunto/documento]](#download-attachmentdocument)

#### [!UICONTROL Crear un registro]

Este módulo de acción crea un nuevo registro en un objeto.

El módulo le permite seleccionar qué campos del objeto están disponibles en el módulo. Esto reduce el número de campos por los que debe desplazarse al configurar el módulo.

El módulo devuelve el identificador del registro y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Salesforce] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Record Type] </p> </td> 
   <td> <p>Seleccione el tipo de registro de [!DNL Salesforce] que desea que cree el módulo. Los campos estarán disponibles en función del tipo de registro seleccionado en el campo [!UICONTROL Record Type]. Estos campos se basan en la API de [!DNL Salesforce].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Select fields to map]</td> 
   <td> <p>Seleccione los campos que desea que configure el módulo al crear el nuevo registro. Los campos obligatorios están en la parte superior de la lista. </p> <p>Los campos que seleccione se abren debajo de este campo. Ahora puede introducir valores en estos campos.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leer un registro]

Este módulo de acción lee datos de un solo objeto en [!DNL Salesforce].

Especifique el identificador del registro.

El módulo devuelve el ID del registro y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Salesforce] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Record Type]</td>
    <td>Seleccione el tipo de registro de [!DNL Salesforce] que desea que el módulo [action] lea.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Record Fields]</td>
    <td>Seleccione los campos que desea que lea el módulo. Debe seleccionar al menos un campo.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL ID]</td>
    <td> <p>Escriba o asigne el ID de [!DNL Salesforce] único del registro que desea que lea el módulo.</p> <p>Para obtener el identificador, abra el objeto [!DNL Salesforce] en el explorador y copie el texto al final de la dirección URL después de la última barra diagonal (/). Por ejemplo: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un registro]

Este módulo de acción elimina un registro existente en un objeto.

Especifique el identificador del registro.

El módulo devuelve el identificador del registro y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Salesforce] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>Seleccione el tipo de registro [!DNL Salesforce] que desea que elimine el módulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Escriba o asigne el identificador único [!DNL Salesforce] del registro que desea que elimine el módulo.</p> <p>Para obtener el identificador, abra el objeto [!DNL Salesforce] en el explorador y copie el texto al final de la dirección URL después de la última barra diagonal (/). Por ejemplo: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Llamada de API personalizada]

Este módulo de acción le permite realizar una llamada autenticada personalizada a la API [!DNL Salesforce]. De este modo, puede crear una automatización del flujo de datos que no puedan realizar los otros módulos de [!DNL Salesforce].

El módulo devuelve lo siguiente:

* **[!UICONTROL Código de estado]** (número): esto indica si la solicitud HTTP se realizó correctamente o no. Se trata de códigos estándar que puede buscar en internet.
* **[!UICONTROL Encabezados]** (objeto): contexto más detallado para el código de respuesta/estado que no está relacionado con el cuerpo de salida. No todos los encabezados que aparecen en un encabezado de respuesta son de respuesta, por lo que algunos podrían no resultarle útiles.

  Los encabezados de respuesta dependen de la petición HTTP elegida al configurar el módulo.

* **[!UICONTROL Cuerpo]** (objeto): según la petición HTTP elegida al configurar el módulo, es posible que reciba de vuelta algunos datos. Esos datos, como los datos de una solicitud [!UICONTROL GET], están contenidos en este objeto.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Salesforce] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Escriba una ruta relativa a <code> &lt;Instance URL&gt;/services/data/v46.0/</code>.</p> <p>Para obtener la lista de puntos finales disponibles, consulte la <a href="https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_what_is_rest_api.htm">Guía para desarrolladores de API de REST de Salesforce</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   td&gt; <p>Seleccione el método de petición HTTP que necesita para configurar la llamada de la API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de petición HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar. Por ejemplo, <code>{"Content-type":"application/json"}</code>. Workfront Fusion añade los encabezados de autorización para usted.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar. Por ejemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando utilice afirmaciones condicionales como <code>if</code> en su JSON, coloque las comillas fuera de la afirmación condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Ejemplo:** La siguiente llamada de API devuelve la lista de todos los usuarios de su cuenta de [!DNL Salesforce]:
>
>* **URL**: `query`
>
>* **Método**: [!UICONTROL GET]
>
>* **Cadena de consulta**:
>
>* **Clave**: `q`
>
>* **Valor**: `SELECT Id, Name, CreatedDate, LastModifiedDate FROM User LIMIT 10`
>
>Las coincidencias de la búsqueda se encuentran en la salida del módulo en **[!UICONTROL Paquete] > [!UICONTROL Cuerpo] > [!UICONTROL registros]**.
>
>En nuestro ejemplo, se encontraron 6 usuarios:
>
>![](assets/matches-of-the-search-350x573.png)


#### [!UICONTROL Cargar archivo adjunto/documento]

Este módulo de acción carga un archivo y lo adjunta al registro que especifique o carga un documento.

El módulo devuelve el ID del archivo adjunto o documento y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Salesforce] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type of Upload]</td> 
   <td>Seleccione si desea que el módulo cargue un archivo adjunto o un documento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Introduzca o asigne el ID del objeto en el que desea cargar un archivo adjunto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td>Seleccione la carpeta que contiene el archivo que desea que cargue el módulo. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source File]</td> 
   <td>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Descargar archivo adjunto/documento]

Este módulo de acción descarga un documento o archivo adjunto de un registro.

Especifique el ID del registro y el tipo de descarga que desee.

El módulo devuelve el ID del archivo adjunto o documento y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Salesforce] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Type of Download]</td>
    <td> <p>Especifique el tipo de archivo que desea descargar de Salesforce.</p> 
     <ul> 
      <li>[!UICONTROL Attachment]</li> 
      <li>[!UICONTROL Document]</li> 
      <li>[!UICONTROL ContentDocument] (Documento que se ha cargado en una biblioteca de [!DNL Saleforce CRM Content] o [!DNL Salesforce Files].)</li> 
     </ul> </td>
  </tr> 
  <tr>
    <td> <p>[!UICONTROL ID] / </p> <p>[!UICONTROL Attachment ID] / </p> <p>[!UICONTROL ContentDocument ID]</p> </td>
    <td> <p>Escriba o asigne el identificador único de [!DNL Salesforce] del registro que desea que descargue el módulo.</p> <p>Para obtener el identificador, abra el objeto de [!DNL Salesforce] en el explorador y copie el texto al final de la dirección URL después de la última barra diagonal (/). Por ejemplo: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Actualizar un registro]

Este módulo de acción edita un registro en un objeto.

El módulo le permite seleccionar qué campos del objeto están disponibles en el módulo. Esto reduce el número de campos por los que debe desplazarse al configurar el módulo.

El módulo devuelve el identificador del registro y cualquier campo asociado, junto con cualquier campo y valor personalizados a los que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Salesforce] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Introduzca o asigne el ID del registro que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Record Type] </p> </td> 
   <td> <p>Seleccione el tipo de registro de [!DNL Salesforce] que desea que actualice el módulo. Los campos están disponibles en función del tipo de registro seleccionado en el campo Tipo de registro. Estos campos se basan en la API de [!DNL Salesforce].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Select fields to map]</td> 
   <td> <p>Seleccione los campos que desea que configure el módulo al crear el nuevo registro. Los campos obligatorios están en la parte superior de la lista. </p> <p>Los campos que seleccione se abren debajo de este campo. Ahora puede introducir valores en estos campos.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

#### [!UICONTROL Buscar con una consulta]

Este módulo de búsqueda busca registros en un objeto de [!DNL Salesforce] que coincidan con la consulta de búsqueda especificada. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Salesforce] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion]: instrucciones básicas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search Type]</td> 
   <td> <p>Seleccione el tipo de búsqueda que desea que realice el módulo:</p> 
    <ul> 
     <li> <p>[!UICONTROL Simple]</p> </li> 
     <li> <p>[!UICONTROL Using SOSL (Salesforce Object Search Language)]</p> </li> 
     <li> <p>[!UICONTROL Using SOQL (Salesforce Object Query Language)]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Type] </p> </td> 
   <td> <p>Si seleccionó el tipo de búsqueda simple, elija el tipo de registro de [!DNL Salesforce] que desea que busque el módulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query] / [!UICONTROL SOSL Query] / [!UICONTROL SOQL Query]</td> 
   <td> <p>Introduzca la consulta con la que desea buscar.</p> <p>Para obtener más información sobre SOSL, consulte <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm">Lenguaje de búsqueda de objetos de Salesforce (SOSL)</a> en la documentación de [!DNL Salesforce].</p> <p>Para obtener más información sobre SOQL, consulte <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm">Lenguaje de consulta de objetos de Salesforce (SOQL)</a> en la documentación de [!DNL Salesforce].</p> <p>Nota: Tenga en cuenta que el valor del parámetro <code>RETURNING </code> influye en la salida del módulo. Si usa <code>LIMIT</code>, [!DNL Fusion] omitirá la configuración del campo [!UICONTROL Maximal count of records]. Si no define ningún límite, Fusion insertará el valor [!UICONTROL LIMIT = Maximal count of records].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximal count of records]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Búsqueda]

Este módulo de acción recupera todos los registros que cumplen un criterio determinado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL Salesforce] a [!DNL Workfront Fusion], vea <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a[!DNL  Adobe Workfront Fusion] - Instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td> <p>Seleccione el tipo de objeto que desea buscar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search criteria]</td> 
   <td>Seleccione el campo por el que desea buscar, el operador que desea utilizar en la consulta y el valor que está buscando en el campo. Puede conectar consultas mediante AND u OR.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Seleccione los campos que desea incluir en la salida del módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Result set]</td> 
   <td>Seleccione si desea que el módulo devuelva todos los registros coincidentes o solo el primero.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximal]</td> 
   <td>Introduzca o asigne el número máximo de registros que desea que el módulo recupere durante cada ciclo de ejecución de escenario.</td> 
  </tr> 
 </tbody> 
</table>
