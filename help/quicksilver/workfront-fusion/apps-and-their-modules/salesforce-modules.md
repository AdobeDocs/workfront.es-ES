---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos de Salesforce
description: En un escenario de Adobe Workfront Fusion, puede automatizar los flujos de trabajo que utilizan Salesforce, así como conectarlos a varias aplicaciones y servicios de terceros.
author: Becky
feature: Workfront Fusion
exl-id: 3c8adcd9-fb5f-400d-9edd-6d9fc30cc728
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2720'
ht-degree: 0%

---

# [!DNL Salesforce] módulos

En un escenario de Adobe Workfront Fusion, puede automatizar los flujos de trabajo que utilizan [!DNL Salesforce], así como conectarlo a varias aplicaciones y servicios de terceros.

Si necesita instrucciones para crear un escenario, consulte [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Para obtener información sobre los módulos, consulte [Módulos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!NOTE]
>
>* No todas las ediciones de [!DNL Salesforce] tienen acceso a la API. Para obtener más información, consulte la información sobre [!DNL Salesforce] ediciones con acceso a API en [!DNL Salesforce] Sitio de la comunidad.
>* Para obtener información sobre errores específicos devueltos por la variable [!DNL Salesforce] API, consulte la [!DNL Salesforce] Documentos de API. También puede comprobar el estado de la variable [!DNL Salesforce] API para cualquier posible interrupción del servicio.
>


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

Para usar [!DNL Salesforce] módulos, debe tener un [!DNL Salesforce] cuenta.

## Acerca de la búsqueda [!DNL Salesforce] objetos

Al buscar objetos, puede introducir palabras de búsqueda individuales o crear una consulta más compleja utilizando comodines y operadores:

* Utilice el carácter comodín del asterisco (\*) como sustituto de cero o más caracteres. Por ejemplo, una búsqueda de Ca\* encuentra elementos que comienzan con Ca
* Usar un signo de interrogación comodín (?) como sustituto de un solo carácter. Por ejemplo, una búsqueda de Jo?n encuentra elementos con el término John o Joan pero no Jon
* Utilice el operador de comillas (&quot;&quot;) para encontrar una coincidencia exacta de frases. Por ejemplo: &quot;Reunión del lunes&quot;

Para obtener más información sobre las posibilidades de búsqueda, consulte la [!DNL Salesforce] documentación para desarrolladores sobre SOQL y SOSL.

## [!DNL Salesforce] módulos y sus campos

* [Déclencheur](#triggers)
* [Acciones](#actions)
* [Búsquedas](#searches)

### Déclencheur

* [[!UICONTROL Ver registros]](#watch-for-records)
* [[!UICONTROL Ver mensajes salientes]](#watch-outbound-messages)
* [[!UICONTROL Ver un campo]](#watch-a-field)

#### [!UICONTROL Ver registros]

Este módulo de déclencheur ejecuta un escenario cuando se crea o actualiza un registro de un objeto. El módulo devuelve todos los campos estándar asociados con el registro o registros, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Salesforce] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type] </td> 
   <td> <p>Seleccione el tipo de [!DNL Salesforce] registre que desea que el módulo vea.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campos de registro]</td> 
   <td>Seleccione los campos que desea que el módulo mire. Los campos disponibles dependen del tipo de registro.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recuento máximo de registros]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p>Determine si desea que el escenario vea solo registros nuevos del tipo seleccionado, o registros nuevos del tipo seleccionado y todos los demás cambios a registros de ese tipo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ver mensajes salientes]

Este módulo de déclencheur ejecuta un escenario cuando alguien envía un mensaje. El módulo devuelve todos los campos estándar asociados con el registro o registros, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Este módulo requiere una configuración adicional:

1. Vaya a la [!DNL Salesforce] configuración .

   Para acceder a la página de configuración, busque y haga clic en el botón denominado &quot;[!UICONTROL Configuración]&quot; en la esquina superior derecha de la [!DNL Salesforce] cuenta. En el [!DNL Salesforce] configuración, busque la[!UICONTROL Búsqueda rápida / Búsqueda]&quot; en el lado izquierdo. Buscar &quot;[!UICONTROL Reglas de flujo de trabajo].&quot;

1. Haga clic en **[!UICONTROL Reglas de flujo de trabajo]**.
1. En el [!UICONTROL Reglas de flujo de trabajo] página que aparecerá, haga clic en **[!UICONTROL Nueva regla]** y seleccione el tipo de objeto al que se aplicará la regla (como &quot;[!UICONTROL Oportunidad]&quot; si está monitorizando las actualizaciones de los registros de oportunidad).
1. Haga clic en **[!UICONTROL Siguiente]**.
1. Establezca un nombre de regla, criterios de evaluación y criterios de regla, y luego haga clic en **[!UICONTROL Guardar]** y **[!UICONTROL Siguiente]**.

1. Haga clic en **[!UICONTROL Listo]**.
1. En la regla de flujo de trabajo recién creada, haga clic en **[!UICONTROL Editar]**...
1. En el **[!UICONTROL Añadir acción de flujo de trabajo]** lista desplegable, seleccione **[!UICONTROL Nuevo mensaje de salida]**.

1. Especifique el nombre, la descripción, la dirección URL del extremo y los campos que desea incluir en el nuevo mensaje saliente y, a continuación, haga clic en **[!UICONTROL Guardar]**.

   La variable **[!UICONTROL Dirección URL del extremo]** contiene la dirección URL proporcionada en la variable [!DNL Salesforce] [!UICONTROL Mensaje saliente] en [!DNL Workfront Fusion].

1. Configure un escenario empezando por el [!UICONTROL Mensaje saliente] evento.

1. Haga clic en el **&lt;/>** en la parte inferior derecha y copie la dirección URL proporcionada.
1. Vuelva a la **[!UICONTROL Reglas de flujo de trabajo]** , busque la regla recién creada y haga clic en **[!UICONTROL Activar]**.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Weblock]</td> 
   <td> <p>Seleccione el vínculo web que desea utilizar para ver los mensajes salientes. Para añadir un vínculo web, haga clic en <strong>[!UICONTROL Agregar]</strong> e introduzca el nombre y la conexión del vínculo web.</p> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Salesforce] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!UICONTROL Adobe Workfront Fusion]: Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro] </td> 
   <td> <p>Seleccione el tipo de [!DNL Salesforce] registre que desea que el módulo observe los mensajes salientes.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fields]</td> 
   <td> <p>Seleccione los campos que desea que el módulo observe para los mensajes salientes. Los campos disponibles dependen del tipo de registro.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### *[!UICONTROL Ver un campo]*

Este módulo de déclencheur inicia un escenario cuando se actualiza un campo en [!DNL Salesforce].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Salesforce] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro] </td> 
   <td> <p>Seleccione el tipo de registro que contiene el campo que desea que vea el módulo. Debe elegir un tipo de registro que tenga activado [!UICONTROL Field History] [!DNL Salesforce] configuración. Para obtener más información, consulte <a href="https://help.salesforce.com/articleView?id=tracking_field_history.htm&amp;type=5">Seguimiento del historial de campos</a> en el [!DNL Salesforce] documentación. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Field]</td> 
   <td> <p>Seleccione los campos que desea que el módulo observe si hay cambios.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Límite]</td> 
   <td> <p>Introduzca o asigne el número máximo de campos que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Crear un registro]](#create-a-record)
* [[!UICONTROL Leer un registro]](#read-a-record)
* [[!UICONTROL Eliminar un registro]](#delete-a-record)
* [[!UICONTROL Llamada de API personalizada]](#custom-api-call)
* [[!UICONTROL Cargar archivo adjunto/documento]](#upload-attachmentdocument)
* [[!UICONTROL Descargar archivo adjunto/documento]](#download-attachmentdocument)

#### [!UICONTROL Crear un registro]

Este módulo de acción crea un nuevo registro en un objeto.

El módulo le permite seleccionar qué campos del objeto están disponibles en el módulo. Esto reduce el número de campos que debe desplazarse al configurar el módulo.

El módulo devuelve el ID del registro y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Salesforce] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Tipo de registro] </p> </td> 
   <td> <p>Seleccione el tipo de [!DNL Salesforce] registro que desea que cree el módulo. Los campos estarán disponibles en función del tipo de registro seleccionado en el campo [!UICONTROL Record Type]. Estos campos se basan en la variable [!DNL Salesforce] API.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Seleccionar campos para asignar]</td> 
   <td> <p>Seleccione los campos que desea que configure el módulo al crear el nuevo registro. Los campos obligatorios están en la parte superior de la lista. </p> <p>Los campos que seleccione se abren debajo de este campo. Ahora puede introducir valores en estos campos.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leer un registro]

Este módulo de acción lee datos de un único objeto de [!DNL Salesforce].

Especifique el ID del registro.

El módulo devuelve el ID del registro y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Salesforce] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Tipo de registro]</td>
    <td>Seleccione el tipo de [!DNL Salesforce] registro que desea que el módulo sea [action].read.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Campos de registro]</td>
    <td>Seleccione los campos que desea que lea el módulo. Debe seleccionar al menos un campo.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL ID]</td>
    <td> <p>Introduzca o asigne la variable única [!DNL Salesforce] ID del registro que desea que lea el módulo.</p> <p>Para obtener el ID, abra el [!DNL Salesforce] en el explorador y copie el texto al final de la dirección URL después de la última barra diagonal (/). Por ejemplo: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un registro]

Este módulo de acción elimina un registro existente en un objeto.

Especifique el ID del registro.

El módulo devuelve el ID del registro y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Salesforce] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de registro] </td> 
   <td> <p>Seleccione el tipo de [!DNL Salesforce] registro que desea que el módulo elimine.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Introduzca o asigne la variable única [!DNL Salesforce] ID del registro que desea que elimine el módulo.</p> <p>Para obtener el ID, abra el [!DNL Salesforce] en el explorador y copie el texto al final de la dirección URL después de la última barra diagonal (/). Por ejemplo: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Llamada de API personalizada]

Este módulo de acción le permite realizar una llamada autenticada personalizada al [!DNL Salesforce] API. De este modo, puede crear una automatización del flujo de datos que no se pueda lograr con la otra [!DNL Salesforce] módulos.

El módulo devuelve lo siguiente:

* **[!UICONTROL Código de estado]** (número): Esto indica el éxito o el error de la solicitud HTTP. Estos son códigos estándar que se pueden consultar en Internet.
* **[!UICONTROL Encabezados]** (objeto): Un contexto más detallado para el código de respuesta/estado que no está relacionado con el cuerpo de salida. No todos los encabezados que aparecen en un encabezado de respuesta son encabezados de respuesta, por lo que es posible que algunos no sean útiles para usted.

   Los encabezados de respuesta dependen de la solicitud HTTP que haya elegido al configurar el módulo.

* **[!UICONTROL Cuerpo]** (objeto): Según la solicitud HTTP que haya elegido al configurar el módulo, puede recibir algunos datos de vuelta. Esos datos, como los datos de un [!UICONTROL GET] , está contenido en este objeto.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Salesforce] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Especifique una ruta relativa a<code> &lt;Instance URL&gt;/services/data/v46.0/</code>.</p> <p>Para obtener la lista de extremos disponibles, consulte la <a href="https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_what_is_rest_api.htm">Guía para desarrolladores de API de Salesforce REST</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   td&gt; <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada a la API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de un objeto JSON estándar. Por ejemplo, <code>{"Content-type":"application/json"}</code>. Workfront Fusion añade los encabezados de autorización por usted.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar. Por ejemplo: <code>{"name":"something-urgent"}</code></p> </td> 
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

>[!INFO]
>
>**Ejemplo:** La siguiente llamada de API devuelve la lista de todos los usuarios de su [!DNL Salesforce] cuenta:
>
>* **URL**: `query`
>
>* **Método**: [!UICONTROL GET]
>
>* **Cadena de consulta**:
>
>* **Clave**: `q`
>
>* **Valor**: `SELECT Id, Name, CreatedDate, LastModifiedDate FROM User LIMIT 10`
>
>Las coincidencias de la búsqueda se pueden encontrar en la salida del módulo en **[!UICONTROL Paquete] > [!UICONTROL Cuerpo] > [!UICONTROL records]**.
>
>En nuestro ejemplo, se devolvieron 6 usuarios:
>
>![](assets/matches-of-the-search-350x573.png)


#### [!UICONTROL Cargar archivo adjunto/documento]

Este módulo de acción carga un archivo y lo adjunta a un registro que especifique o carga un documento.

El módulo devuelve el ID del archivo adjunto o documento y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Salesforce] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de carga]</td> 
   <td>Seleccione si desea que el módulo cargue un archivo adjunto o un documento.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Introduzca o asigne el ID del objeto al que desea cargar un archivo adjunto.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td>Seleccione la carpeta que contiene el archivo que desea que cargue el módulo. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archivo de origen]</td> 
   <td>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Descargar archivo adjunto/documento]

Este módulo de acción descarga un documento o archivo adjunto de un registro.

Especifique el ID del registro y el tipo de descarga que desee.

El módulo devuelve el ID del archivo adjunto o documento y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Connection]</td>
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Salesforce] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Tipo de descarga]</td>
    <td> <p>Especifique el tipo de archivo que desea descargar de Salesforce.</p> 
     <ul> 
      <li>[!UICONTROL Attachment]</li> 
      <li>[!UICONTROL Document]</li> 
      <li>[!UICONTROL ContentDocument] (es un documento que se ha cargado en una biblioteca de [!DNL Saleforce CRM Content] o [!DNL Salesforce Files].)</li> 
     </ul> </td>
  </tr> 
  <tr>
    <td> <p>[!UICONTROL ID] / </p> <p>[!UICONTROL ID de archivo adjunto] / </p> <p>[!UICONTROL ContentDocument ID]</p> </td>
    <td> <p>Introduzca o asigne la variable única [!DNL Salesforce] ID del registro que desea que descargue el módulo.</p> <p>Para obtener el ID, abra el [!DNL Salesforce] en el explorador y copie el texto al final de la dirección URL después de la última barra diagonal (/). Por ejemplo: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Actualizar un registro]

Este módulo de acción edita un registro en un objeto.

El módulo le permite seleccionar qué campos del objeto están disponibles en el módulo. Esto reduce el número de campos que debe desplazarse al configurar el módulo.

El módulo devuelve el ID del registro y los campos asociados, junto con los campos y valores personalizados a los que accede la conexión. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Salesforce] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Introduzca o asigne el ID del registro que desea actualizar.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Tipo de registro] </p> </td> 
   <td> <p>Seleccione el tipo de [!DNL Salesforce] registro que desea que el módulo se actualice. Los campos estarán disponibles en función del tipo de registro seleccionado en el campo Tipo de registro . Estos campos se basan en la variable [!DNL Salesforce] API.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Seleccionar campos para asignar]</td> 
   <td> <p>Seleccione los campos que desea que configure el módulo al crear el nuevo registro. Los campos obligatorios están en la parte superior de la lista. </p> <p>Los campos que seleccione se abren debajo de este campo. Ahora puede introducir valores en estos campos.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Búsquedas

#### [!UICONTROL Buscar con consulta]

Este módulo de búsqueda busca registros en un objeto de [!DNL Salesforce] que coinciden con la consulta de búsqueda especificada. Puede asignar esta información en módulos posteriores en el escenario.

Al configurar este módulo, se muestran los campos siguientes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su [!DNL Salesforce] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con [!DNL Adobe Workfront Fusion] - Instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo de búsqueda]</td> 
   <td> <p>Seleccione el tipo de búsqueda que desea que realice el módulo:</p> 
    <ul> 
     <li> <p>[!UICONTROL Simple]</p> </li> 
     <li> <p>[!UICONTROL Usando SOSL (Lenguaje De Búsqueda De Objetos De Salesforce)]</p> </li> 
     <li> <p>[!UICONTROL Uso de SOQL (Lenguaje de consulta de objeto de Salesforce)]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Type] </p> </td> 
   <td> <p>Si ha seleccionado el tipo de búsqueda Simple , elija el tipo de [!DNL Salesforce] registro que desea que busque el módulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query] / [!UICONTROL SOSL Query] / [!UICONTROL SOQL Query]</td> 
   <td> <p>Introduzca la consulta por la que desea buscar.</p> <p>Para obtener más información sobre SOSL, consulte <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm">Lenguaje de búsqueda de objetos de Salesforce (SOSL)</a> en el [!DNL Salesforce] documentación.</p> <p>Para obtener más información sobre SOQL, consulte <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm">Lenguaje de consulta de objeto de Salesforce (SOQL)</a> en el [!DNL Salesforce] documentación.</p> <p>Nota: Tenga en cuenta que el valor del parámetro <code>RETURNING </code>influye en la salida del módulo. Si usa <code>LIMIT</code>, [!DNL Fusion] ignorará la configuración del campo [!UICONTROL Recuento máximo de registros]. Si no establece ningún límite, Fusion insertará el valor [!UICONTROL LIMIT = Recuento máximo de registros].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recuento máximo de registros]</td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que el módulo devuelva durante cada ciclo de ejecución del escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Buscar]

Este módulo de acción recupera todos los registros que cumplen un criterio determinado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Para obtener instrucciones sobre cómo conectar su [!DNL Salesforce] cuenta para [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión con[!DNL  Adobe Workfront Fusion] - Instrucciones básicas</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td> <p>Seleccione el tipo de objeto que desea buscar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Criterios de búsqueda]</td> 
   <td>Seleccione el campo por el que desea buscar, el operador que desea utilizar en la consulta y el valor que está buscando en el campo . Puede conectar consultas utilizando AND u OR.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Salidas]</td> 
   <td>Seleccione los campos que desea incluir en la salida del módulo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resultado establecido]</td> 
   <td>Seleccione si desea que el módulo devuelva Todos los registros coincidentes o solo el registro coincidente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Máximo]</td> 
   <td>Introduzca o asigne el número máximo de registros que desea que el módulo recupere durante cada ciclo de ejecución del escenario.</td> 
  </tr> 
 </tbody> 
</table>
