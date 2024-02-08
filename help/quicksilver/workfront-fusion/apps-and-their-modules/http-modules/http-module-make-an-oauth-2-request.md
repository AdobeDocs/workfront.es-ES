---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: http-modules
title: HTTP &gt; Crear un módulo de solicitud OAuth 2.0
description: Con el fin de hacer una [!DNL Adobe Workfront Fusion] Solicitud HTTP(S) a servidores que requieren una autorización OAuth 2.0; primero debe crear una conexión OAuth. [!DNL Adobe Workfront Fusion] garantiza que todas las llamadas realizadas con esta conexión tengan los encabezados de autorización adecuados y actualicen automáticamente los tokens asociados cuando sea necesario.
author: Becky
feature: Workfront Fusion
exl-id: 6c68c9b9-9f74-44a7-94ed-3785081b8331
source-git-commit: 45540ccc3b9fca98f8aaae86ac4d6574a067a6e4
workflow-type: tm+mt
source-wordcount: '2236'
ht-degree: 0%

---

# [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud de OAuth 2.0] módulo

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requiere un [!DNL Adobe Workfront Fusion] además de una licencia de [!DNL Adobe Workfront] licencia.

Con el fin de hacer una [!DNL Adobe Workfront Fusion] Solicitud HTTP(S) a servidores que requieren una autorización OAuth 2.0; primero debe crear una conexión OAuth. [!DNL Adobe Workfront Fusion] garantiza que todas las llamadas realizadas con esta conexión tengan los encabezados de autorización adecuados y actualicen automáticamente los tokens asociados cuando sea necesario.

[!DNL Workfront Fusion] admite los siguientes flujos de autenticación OAuth 2.0:

* Flujo de código de autorización
* Flujo implícito

Otros flujos, como el flujo de credenciales de contraseña de propietario de recursos y el flujo de credenciales de cliente, no se admiten automáticamente a través de este módulo.

Para obtener más información sobre la autenticación OAuth 2.0, consulte [El marco de autorización de OAuth 2.0](https://tools.ietf.org/html/rfc6749).

>[!NOTE]
>
>Si se está conectando a un producto de Adobe que actualmente no tiene un conector dedicado, le recomendamos que utilice el módulo de Adobe Authenticator.
>
>Para obtener más información, consulte [módulo de Adobe Authenticator](/help/quicksilver/workfront-fusion/apps-and-their-modules/adobe-authenticator-modules.md).

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

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Creación de una conexión para una [!DNL OAuth] solicitud

* [Instrucciones generales para crear una conexión en el módulo de solicitud HTTP > Crear una OAuth 2.0](#general-instructions-for-creating-a-connection-in-the-http--make-an-oauth-20-request-module)
* [Instrucciones para crear una conexión con Google en la página HTTP >[!UICONTROL Marca] un módulo de solicitud OAuth 2.0](#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module)
* [Instrucciones para conectarse a la API de Microsoft Graph mediante el módulo de solicitud HTTP > Crear una OAuth 2.0](#instructions-for-connecting-to-microsoft-graph-api-via-the-http--make-an-oauth-20-request-module)

### Instrucciones generales para crear una conexión en [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud de OAuth 2.0] módulo

1. Cree un cliente de OAuth en [!DNL target] servicio con el que desea [!DNL Adobe Workfront Fusion] para comunicarse. Es muy probable que esta opción se encuentre en el [!UICONTROL Desarrollador] del servicio dado.

   1. Al crear un cliente, introduzca la dirección URL adecuada en la `[!UICONTROL Redirect URL]` o `[!UICONTROL Callback URL]` campo:

      | América/APAC | https://app.workfrontfusion.com/oauth/cb/oauth2 |
      |---|---|
      | EMEA | https://app-eu.workfrontfusion.com/oauth/cb/oauth2 |

   1. Después de crear el cliente, el servicio dado muestra 2 claves: `[!UICONTROL Client ID]` y `[!UICONTROL Client Secret]`. Algunos servicios llaman a esto `[!UICONTROL App Key]` y `[!UICONTROL App Secret]` . Guarde la clave y el secreto en una ubicación segura, de modo que pueda proporcionarlos al crear la conexión en Workfront Fusion.

1. Busque el `[!UICONTROL Authorize URI]` y `[!UICONTROL Token URI]` en la documentación de API del servicio determinado. Son direcciones URL a través de las cuales [!DNL Workfront Fusion] se comunica con [!DNL target] servicio. Las direcciones sirven para la autorización de OAuth.

   >[!NOTE]
   >
   >Si el servicio utiliza un flujo implícito, solo necesitará el `[!UICONTROL Authorize URI]`.

   >[!INFO]
   >
   >**Ejemplo:** Direcciones de Yahoo:
   >
   >* URI autorizado:
   >
   >`https://api.login.yahoo.com/oauth2/request_auth`
   >
   >* URI de token:
   >
   >`https://api.login.yahoo.com/oauth2/get_token`

1. (Condicional) Si el servicio de destino utiliza ámbitos (derechos de acceso), compruebe cómo el servicio separa los ámbitos individuales y asegúrese de establecer el separador en la configuración avanzada en consecuencia. Si el separador no está configurado correctamente, [!DNL Workfront Fusion] no se puede crear la conexión y recibe un error de ámbito no válido.
1. Después de completar los pasos anteriores, puede empezar a crear la conexión OAuth en [!DNL Workfront Fusion]. Añada el módulo de procesamiento de respuestas y solicitudes HTTP(S) de OAuth 2.0 a su escenario.
1. En el campo Connection del módulo, haga clic en **[!UICONTROL Añadir]**.

1. Rellene los campos siguientes para crear una conexión:

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre de conexión] </td> 
      <td> <p>Introduzca el nombre de la conexión.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Tipo de flujo]</p> </td> 
      <td> <p>Seleccione el flujo para obtener tokens.</p> 
       <ul> 
        <li><strong>[!UICONTROL Código de autorización]</strong>: introduzca el <code>[!UICONTROL Authorize URI]</code> y <code>[!UICONTROL Token URI]</code> de la documentación de API del servicio.</li> 
        <li><strong>[!UICONTROL Implícito]</strong>: introduzca el <code>[!UICONTROL Authorize URI]</code> de la documentación de API del servicio.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ámbito] </td> 
      <td> <p>Agregar ámbitos individuales. Puede encontrar esta información en la documentación para desarrolladores (API) de un servicio determinado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Separador de ámbitos] </td> 
      <td> <p>Seleccione por qué se deben separar los ámbitos especificados anteriormente. Puede encontrar esta información en la documentación para desarrolladores (API) de un servicio determinado.</p> <p>Advertencia: Si el separador no está configurado correctamente, [!DNL Workfront Fusion] no se puede crear la conexión y recibe un error de ámbito no válido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID de cliente] </td> 
      <td> <p>Introduzca el ID de cliente. Obtuvo el ID de cliente al crear un cliente de OAuth en el servicio al que desea conectarse.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Secreto de cliente]</td> 
      <td> <p> Introduzca el Secreto del cliente. Obtuvo el Secreto del cliente al crear un cliente de OAuth en el servicio que desea conectar.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Autorizar parámetros]</p> </td> 
      <td> <p>Agregue los parámetros que desee incluir en la llamada de autorización. Los siguientes parámetros estándar siempre se incluyen automáticamente y no es necesario añadirlos.</p> <p>Parámetros estándar:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL response_type]</strong> </p> <p> <code>code </code>para el flujo de código de autorización de [!UICONTROL] y <code>token </code>para [!UICONTROL Implicit flow]</p> </li> 
        <li> <p><strong>[!UICONTROL_redirect_uri]</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">América/APAC</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">EMEA </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong> </p> <p> El ID de cliente que recibió al crear la cuenta</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Parámetros de token de acceso]</p> </td> 
      <td> <p>Añada cualquier parámetro que desee incluir en la llamada de token. Los siguientes parámetros estándar siempre se incluyen automáticamente y no es necesario añadirlos.</p> <p>Parámetros estándar:</p> 
       <ul> 
        <li><strong>[!UICONTROL grant_type]</strong>: <code>authorization_code</code></li> 
        <li> <p><strong>[!UICONTROL_redirect_uri]:</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">América/APAC</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">EMEA </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li><strong>[!UICONTROL client_id]</strong>: el ID de cliente que recibió al crear la cuenta se incluye automáticamente en el cuerpo de la solicitud</li> 
        <li><strong>client_secret</strong>: el Secreto de cliente que recibió al crear la cuenta se incluye automáticamente en el cuerpo de la solicitud</li> 
        <li><strong>código</strong>: el código devuelto por la solicitud de autorización</li> 
       </ul> <p>Nota:  <p>El estándar OAuth 2.0 admite al menos 2 métodos de autenticación de cliente durante este paso (<code>[!UICONTROL client_secret_basic]</code> y <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] envía automáticamente el ID de cliente y el secreto especificados a través de <code>[!UICONTROL client_secret_post]</code> método. Por lo tanto, estos parámetros se incluyen automáticamente como parte del cuerpo de solicitud de token. </p> <p>Para obtener más información sobre la autenticación OAuth 2.0, consulte <a href="https://tools.ietf.org/html/rfc6749">El marco de autorización de OAuth 2.0</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Actualizar parámetros de token]</p> </td> 
      <td> <p>Añada cualquier parámetro que desee incluir en la llamada de token. Los siguientes parámetros estándar siempre se incluyen automáticamente y no es necesario añadirlos.</p> <p>Parámetros estándar:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL grant_type]</strong>: <code>refresh_token</code></p> </li> 
        <li> <p><strong>[!UICONTROL refresh_token]</strong>: el token de actualización más reciente obtenido por el servicio al que se está conectando</p> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong>: el ID de cliente que recibió al crear la cuenta se incluye automáticamente en el cuerpo de la solicitud</p> </li> 
        <li> <p><strong>[!UICONTROL client_secret]</strong>: el Secreto de cliente que recibió al crear la cuenta se incluye automáticamente en el cuerpo de la solicitud</p> </li> 
       </ul> <p>Nota:  <p>El estándar OAuth 2.0 admite al menos 2 métodos de autenticación de cliente durante este paso (<code>[!UICONTROL client_secret_basic]</code> y <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] envía automáticamente el ID de cliente y el secreto especificados a través de <code>[!UICONTROL client_secret_post]</code> método. Por lo tanto, estos parámetros se incluyen automáticamente como parte del cuerpo de solicitud de token. </p> <p>Para obtener más información sobre la autenticación OAuth 2.0, consulte <a href="https://tools.ietf.org/html/rfc6749">El marco de autorización de OAuth 2.0</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Encabezados personalizados]</p> </td> 
      <td> <p>Especifique las claves y los valores adicionales que se incluirán en el encabezado de los pasos de [!UICONTROL Token] y R[!UICONTROL Token de actualización].</p> <p>Nota:  <p>El estándar OAuth 2.0 admite al menos 2 métodos de autenticación de cliente durante este paso (<code>[!UICONTROL client_secret_basic]</code> y <code>[!UICONTROL client_secret_post]</code>). [!DNL Workfront Fusion] no admite automáticamente el <code>[!UICONTROL client_secret_basic]</code> método. Si el servicio al que se está conectando espera que el ID de cliente y el Secreto del cliente se combinen en una sola cadena y luego se codifique base64 en el encabezado Autorización, debe agregar ese encabezado y valor clave aquí.</p> <p> Para obtener más información sobre la autenticación OAuth 2.0, consulte <a href="https://tools.ietf.org/html/rfc6749">El marco de autorización de OAuth 2.0</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Colocación del token]</p> </td> 
      <td> <p>Seleccione si desea enviar el token en [!UICONTROL encabezado], [!UICONTROL cadena de consulta] o en ambos al conectarse a la dirección URL especificada.</p> <p>Normalmente, los tokens se envían en el encabezado de la solicitud.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre de token de encabezado] </td> 
      <td> <p>Introduzca el nombre del token de autorización en el encabezado. Predeterminado: <code>[!UICONTROL Bearer]</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Query string parameter name] </td> 
      <td> <p>Introduzca el nombre del token de autorización en la cadena de consulta. Predeterminado: <code>[!UICONTROL access_token]</code>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **[!UICONTROL Continuar]** para guardar la configuración de conexión.
1. Continuar a [Configuración del módulo de solicitud OAuth 2.0](#oauth-20-request-module-setup).

### Instrucciones para crear una conexión con [!DNL Google] en el [!UICONTROL HTTP] >[!UICONTROL Crear un módulo de solicitud OAuth 2.0]

El siguiente ejemplo muestra cómo utilizar el [!UICONTROL HTTP] > [!UICONTROL Crear un OAuth 2.0] solicitar al módulo que se conecte [!DNL Google].

1. Asegúrese de haber creado un proyecto, configurado la configuración de OAuth y generado sus credenciales tal como se describe en [Connect [!DNL Adobe Workfront Fusion] hasta [!DNL Google Services] uso de un cliente de OAuth personalizado](../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).
1. Abra el [!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud de OAuth 2.0] módulo.
1. Clic **[!UICONTROL Añadir]** situado junto al cuadro de conexión.
1. Introduzca los siguientes valores:

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre de conexión] </td> 
      <td> <p>Introduzca el nombre de la conexión.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Tipo de flujo]</p> </td> 
      <td> <p>[!UICONTROL Código de autorización]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Autorizar URI]</td> 
      <td><code>https://accounts.google.com/o/oauth2/v2/auth</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token URI]</td> 
      <td><code>https://www.googleapis.com/oauth2/v4/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ámbito] </td> 
      <td> <p>Agregar ámbitos individuales. Para obtener más información sobre los ámbitos, consulte <a href="https://developers.google.com/identity/protocols/oauth2/scopes">Ámbitos de OAuth 2.O para [!DNL Google] API</a> en el [!DNL Google] documentación.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Separador de ámbitos] </td> 
      <td> <p>[!UICONTROL ESPACIO]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID de cliente] </td> 
      <td> <p>Introduzca su [!DNL Google] ID de cliente. </p> <p>Para crear un ID de cliente, consulte <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">Crear credenciales de OAuth</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] hasta [!DNL Google Services] uso de un cliente de OAuth personalizado</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Secreto de cliente]</td> 
      <td> <p>Introduzca su [!DNL Google] Secreto del cliente. </p> <p>Para crear un secreto de cliente, consulte <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">Crear credenciales de OAuth</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] hasta [!DNL Google] Servicios que utilizan un cliente de OAuth personalizado</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Autorizar parámetros]</p> </td> 
      <td> <p>Añadir <code>[!UICONTROL access_type]</code> - <code>[!UICONTROL offline] </code>par clave-valor.</p> <p> <img src="assets/google-authentication-http.png"> </p> <p>Nota: Si tiene problemas de autenticación, por ejemplo, con la actualización de tokens, intente agregar la variable <code>[!UICONTROL prompt] </code>- <code>[!UICONTROL consent] </code>par clave-valor.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **[!UICONTROL Continuar]** para guardar la configuración de conexión.
1. Continuar a [Configuración del módulo de solicitud OAuth 2.0](#oauth-20-request-module-setup).

### Instrucciones para conectarse a [!DNL Microsoft Graph API] a través de [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud de OAuth 2.0] módulo

Para obtener instrucciones sobre [!DNL Microsoft Graph API], consulte [Llame a [!DNL MS Graph REST API] a través de [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud de OAuth 2.0] módulo](../../../workfront-fusion/connections/call-the-ms-graph-rest-api-.md).

## Configuración del módulo de solicitud OAuth 2.0

Cuando haya establecido un [!DNL Oauth 2]Conexión .0 tal como se describe en [Creación de una conexión para una [!DNL OAuth] solicitud](#creating-a-connection-for-an-oauth-request), continúe configurando el módulo como desee. Todos los tokens de autorización se incluyen automáticamente en esta solicitud y en cualquier otra solicitud que utilice la misma conexión.

Al configurar la variable [!UICONTROL HTTP] >[!UICONTROL Realizar una solicitud de OAuth 2.0] módulo, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, consulte [Asignación de información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<!--
<img src="assets/map-toggle-350x74.png" style="width: 350;height: 74;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener información sobre la configuración de una conexión, consulte <a href="#creating-a-connection-for-an-oauth-request" class="MCXref xref">Creación de una conexión para una solicitud de OAuth</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Evaluar todos los estados como errores (excepto 2xx y 3xx]) </td> 
   <td> <p>Utilice esta opción para configurar la gestión de errores.</p> <p>Para obtener más información, consulte <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Tratamiento de errores en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Introduzca la dirección URL a la que desea enviar una solicitud, como un punto final de API, un sitio web, etc.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Método]</p> </td> 
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, consulte <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados] </td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar. Por ejemplo, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p> Introduzca los pares de clave-valor de consulta deseados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de cuerpo]</p> </td> 
   <td> <p>El cuerpo HTTP son los bytes de datos transmitidos en un mensaje de transacción HTTP inmediatamente después de los encabezados si hay alguno que utilizar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>El tipo de cuerpo sin procesar suele ser adecuado para la mayoría de las solicitudes de cuerpo HTTP incluso en situaciones en las que la documentación para desarrolladores no especifica datos para enviar.</p> <p>Especifique una forma de analizar los datos en el campo [!UICONTROL Content type].</p> <p>A pesar del tipo de contenido seleccionado, los datos se introducen en cualquier formato estipulado o requerido por la documentación del desarrollador.</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>Este tipo de cuerpo es para almacenar en POST los datos mediante <code>[!UICONTROL application/x-www-form-urlencoded]</code>.</p> <p>Para <code>[!UICONTROL application/x-www-form-urlencoded]</code>, el cuerpo del mensaje HTTP enviado al servidor es esencialmente una cadena de consulta. Las claves y los valores se codifican en pares clave-valor separados por <code>&amp;</code> y con un <code>=</code> entre la clave y el valor. </p> <p>Para datos binarios, <code>use [!UICONTROL multipart/form-data]</code> en su lugar.</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>Ejemplo: </b></span></span> 
       <p>Ejemplo del formato de solicitud HTTP resultante:</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>[!UICONTROL Multipart/form-data] es una solicitud HTTP multipart que se utiliza para enviar archivos y datos. Normalmente se utiliza para cargar archivos en el servidor.</p> <p>Añada campos para enviarlos en la solicitud. Cada campo debe contener un par clave-valor.</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Texto]</strong> </p> <p>Introduzca la clave y el valor que se enviarán dentro del cuerpo de la solicitud.</p> </li> 
       <li> <p><strong>[!UICONTROL Archivo]</strong> </p> <p>Introduzca la clave y especifique el archivo de origen que desea enviar en el cuerpo de la solicitud.</p> <p>Asigne el archivo que desea cargar desde el módulo anterior (como [!UICONTROL HTTP] &gt;[!UICONTROL Obtener un archivo] o [!UICONTROL Google Drive] &gt;[!UICONTROL Descargar un archivo)], o bien introduzca el nombre de archivo y los datos de archivo manualmente.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Respuesta de análisis]</p> </td> 
   <td> <p>Active esta opción para analizar automáticamente las respuestas y convertir las respuestas JSON y XML, de modo que no necesite utilizar los módulos [!UICONTROL JSON] &gt; [!UICONTROL Parse JSON] o [!UICONTROL XML] &gt; [!UICONTROL Parse XML].</p> <p>Antes de poder utilizar contenido JSON o XML analizado, ejecute el módulo una vez manualmente para que el módulo pueda reconocer el contenido de la respuesta y le permita asignarlo en módulos posteriores.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tiempo de espera] </td> 
   <td> <p>Introduzca el tiempo de espera de la solicitud en segundos (1-300). El valor predeterminado es 40 segundos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Compartir cookies con otros módulos HTTP]</td> 
   <td> <p> Active esta opción para compartir cookies del servidor con todos los módulos HTTP de su escenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Certificado autofirmado]</td> 
   <td> <p> Cargue el certificado si desea utilizar TLS con el certificado autofirmado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rechazar conexiones que utilizan certificados no verificados (autofirmados)] </td> 
   <td> <p>Active esta opción para rechazar conexiones que utilicen certificados TLS no verificados.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seguir redirección]</td> 
   <td> <p> Active esta opción para seguir las redirecciones de URL con respuestas 3xx.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seguir todas las redirecciones] </td> 
   <td> <p>Active esta opción para seguir las redirecciones URL con todos los códigos de respuesta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Deshabilitar la serialización de varias claves de cadena de consulta iguales que matrices]</p> </td> 
   <td> <p>De forma predeterminada, [!DNL Workfront Fusion] administra varios valores para la misma clave de parámetro de cadena de consulta de URL que las matrices. Por ejemplo, <code>www.test.com?foo=bar&amp;foo=baz</code> se convertirá en <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. Active esta opción para deshabilitar esta función. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Solicitar contenido comprimido]</td> 
   <td> <p> Active esta opción para solicitar una versión comprimida del sitio web.</p> <p>Esto añade un <code>[!UICONTROL Accept-Encoding]</code> encabezado para solicitar contenido comprimido.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Utilizar TLS mutuo]</td> 
   <td> <p>Active esta opción para utilizar TLS mutuo en la solicitud HTTP.</p> <p>Para obtener más información sobre TLS mutuo, consulte <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">Usar TLS mutuo en módulos HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
