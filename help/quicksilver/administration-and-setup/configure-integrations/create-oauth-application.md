---
title: Crear aplicaciones OAuth2 para  [!DNL Workfront] integraciones
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Como administrador de  [!DNL Adobe Workfront] , puede crear aplicaciones OAuth2 para su instancia de [!DNL Workfront], que permiten que otras aplicaciones accedan a Workfront. A continuación, los usuarios pueden dar permiso a esas otras aplicaciones para acceder a sus datos de Workfront. De este modo, puede integrar Workfront con las aplicaciones de su elección, incluidas sus propias aplicaciones internas.
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: e13c7dda-8945-47ad-b6d3-4d6a62b368f5
source-git-commit: 711812d9fd4bf48bb7612c0339cee2cdbe08ef10
workflow-type: tm+mt
source-wordcount: '1960'
ht-degree: 98%

---

# Crear aplicaciones OAuth2 para integraciones de [!DNL Workfront]

Como administrador de [!DNL Adobe Workfront], puede crear aplicaciones OAuth2 para la instancia de [!DNL Workfront], que permiten que otras aplicaciones tengan acceso a [!DNL Workfront]. Los usuarios pueden dar permiso a esas otras aplicaciones para acceder a sus datos de [!DNL Workfront]. De este modo, puede integrar con aplicaciones de su elección, incluidas las propias aplicaciones internas.

Cuando crea una aplicación [!UICONTROL OAuth2], genera un ID de cliente y un secreto de cliente. A continuación, los usuarios pueden utilizar el ID de cliente en las llamadas de API para integrarse con la aplicación que ha creado.

>[!NOTE]
>
>En el contexto de OAuth2, “crear una aplicación” hace referencia al proceso de creación de este tipo de vínculo de acceso entre una aplicación y un servidor como [!DNL Workfront].

* Para obtener instrucciones sobre cómo configurar y utilizar la aplicación OAuth2 con credenciales de usuario (flujo de código de autorización), consulte [Configure y utilice las aplicaciones OAuth 2 personalizadas de su organización mediante el flujo del código de autorización](../../wf-api/api/oauth-app-code-token-flow.md).
* Para obtener instrucciones sobre cómo configurar y utilizar la aplicación OAuth2 con la autenticación de servidor (flujo JWT), consulte [Configurar y utilizar las aplicaciones personalizadas OAuth 2 de su organización mediante el flujo JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Para instrucciones sobre cómo configurar y usar la aplicación OAuth2 utilizando PKCE, consulta [Configure y utilice las aplicaciones OAuth 2 personalizadas de su organización mediante el flujo PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de Workfront. </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Información general sobre OAuth2

Imagine que una aplicación debe extraer información específica de [!DNL Workfront]. La aplicación que solicita información se denomina cliente. Para este ejemplo, el nombre de cliente es ClientApp. ClientApp necesita acceder a la información de un usuario en particular y, por lo tanto, debe acceder a [!DNL Workfront] como ese usuario. Si el usuario proporciona a ClientApp su nombre de usuario y contraseña, ClientApp podría acceder a todos los datos a los que el usuario puede acceder. Esto supone un riesgo para la seguridad, ya que ClientApp únicamente necesita un pequeño conjunto específico de información.

Cuando crea una aplicación OAuth2 para ClientApp, básicamente le está diciendo a [!DNL Workfront] que ClientApp tiene permiso para acceder a [!DNL Workfront], pero únicamente si el usuario a cuya cuenta está accediendo ClientApp da permiso para el acceso.

## Creación de una aplicación OAuth2

Al crear una aplicación OAuth2, elija el tipo de aplicación que mejor se adapte a las necesidades de su integración.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Tipo de aplicación</th> 
   <th>Ideal para</th> 
   <th>Método de autenticación</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Aplicación equipo a equipo (MtM)</p> </td> 
   <td> <p>Es ideal para CLI, daemons o scripts que se ejecutan en su servidor</p> <p>Ejemplos:</p> 
    <ul> 
     <li> <p>[!DNL Shell] </p> </li> 
     <li> <p>[!DNL Python]</p> </li> 
    </ul> </td> 
   <td> <p>Autenticación mediante token web JSON con cifrado de par clave público/privado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Aplicación web de una sola página</p> </td> 
   <td> <p>Ideal para aplicaciones móviles o de una sola página</p> <p>Ejemplos:</p> 
    <ul> 
     <li> <p>[!DNL Javascript]</p> </li> 
     <li> <p>[!DNL Angular]</p> </li> 
     <li> <p>[!DNL React]</p> </li> 
     <li> <p>[!DNL Vue]</p> </li> 
    </ul> </td> 
   <td> <p>Flujo de autenticación a través del código de autorización de OAuth 2.0 con clave de prueba para intercambio de código (PKCE)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Aplicación web</p> </td> 
   <td> <p>Ideal para aplicaciones del lado del servidor que administran credenciales y tókenes en el servidor</p> <p>Ejemplos:</p> 
    <ul> 
     <li> <p>[!DNL Go]</p> </li> 
     <li> <p>[!DNL Java]</p> </li> 
     <li> <p>[!DNL ASP.Net]</p> </li> 
     <li> <p>[!DNL Node.js]</p> </li> 
     <li> <p>[!DNL PHP]</p> </li> 
    </ul> </td> 
   <td> <p>Flujo de autenticación a través del código de autorización de OAuth 2.0.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Puede tener hasta un total de diez aplicaciones OAuth2 a la vez.

* [Creación de una aplicación OAuth2 con autenticación de servidor (flujo JWT)](#create-an-oauth2-application-using-server-authentication-jwt-flow)
* [Creación de una aplicación OAuth2 con credenciales de usuario (flujo de código de autorización)](#create-an-oauth2-application-using-user-credentials-authorization-code-flow)
* [Creación de una aplicación web de una sola página de OAuth2 con PKCE](#create-an-oauth2-single-page-web-application-using-pkce)

### Creación de una aplicación OAuth2 con autenticación de servidor (flujo JWT) {#create-an-oauth2-application-using-server-authentication-jwt-flow}

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]** y seleccione **[!UICONTROL Aplicaciones OAuth2]**.
1. Haga clic en **[!UICONTROL Crear integración de aplicaciones]**.
Se muestra el cuadro **Nueva aplicación OAuth2**.
1. En el cuadro **Nueva aplicación OAuth2**, seleccione **[!UICONTROL Aplicación de equipo a equipo]**.
1. Escriba un nombre para la nueva aplicación, como “[!DNL Workfront] para ClientApp”.
1. Haga clic en **[!UICONTROL Crear]**.
1. Rellene los campos de la nueva aplicación.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td> <p>Este campo se genera automáticamente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client secret]</td> 
      <td> <p>Este campo se genera automáticamente</p> <p><b>IMPORTANTE</b>:  <p>Copie el contenido de este campo en otro archivo seguro antes de cerrar esta página. No podrá volver a ver esta clave secreta.</p> <p>Si pierde esta clave, elimínela y cree un Secreto de cliente.</p> 
        <ol> 
         <li value="1"> <p>Haga clic en el icono <b>[!UICONTROL Delete]</b> <img src="assets/delete.png"> para eliminar el Secreto de cliente actual.</p> </li> 
         <li value="2"> <p>Haga clic en <b>[!UICONTROL Add client secret]</b> para generar un nuevo Secreto de cliente.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Public Keys]</td> 
      <td> <p>Las aplicaciones de servidor a servidor utilizan claves públicas y privadas para la autenticación. Realice una de las siguientes acciones:</p> 
       <ul> 
        <li> <p>Haga clic en <b>[!UICONTROL Add a public key]</b> e introduzca la clave pública desde la otra aplicación.</p> </li> 
        <li> <p>Haga clic en <b>[!UICONTROL Generate a public/private keypair]</b> y comparta la clave pública con la otra aplicación.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Este es el mismo nombre que le dio a la aplicación. Esta celda no puede estar vacía.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Introduzca una descripción para la integración.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Guardar]**.

Para obtener instrucciones sobre cómo configurar y utilizar la aplicación OAuth2 con credenciales de usuario (flujo de código de autorización), consulte [Configurar y utilizar las aplicaciones personalizadas OAuth 2 de la organización mediante el flujo JWT](../../wf-api/api/oauth-app-jwt-flow.md).

### Creación de una aplicación OAuth2 con credenciales de usuario (flujo de código de autorización) {#create-an-oauth2-application-using-user-credentials-authorization-code-flow}

>[!NOTE]
>
>Si está creando una aplicación para conectarse a Workfront Fusion, utilice una de las siguientes URL de redireccionamiento:
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-workfront`
>* `https://app-eu.workfrontfusion.com/oauth/cb/workfront-workfront` (centro de datos de la UE)
>* `https://app-az.workfrontfusion.com/oauth/cb/workfront-workfront` (Centro de datos de Azure)

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]** y seleccione **[!UICONTROL Aplicaciones OAuth2]**.
1. Haga clic en **[!UICONTROL Crear integración de aplicaciones]**.

   Se muestra la **Nueva aplicación OAuth2**.
1. En el cuadro **Nueva aplicación OAuth2**, seleccione **[!UICONTROL Aplicación web]**.
1. Escriba un nombre para la nueva aplicación OAuth2, como “[!DNL Workfront] para ClientApp”.
1. Haga clic en **[!UICONTROL Crear]**.
1. Rellene los campos de la nueva aplicación.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td> <p>Este campo se genera automáticamente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client secret]</td> 
      <td> <p>Este campo se genera automáticamente</p> <p><b>IMPORTANTE</b>:  <p>Copie el contenido de este campo en otro archivo seguro antes de cerrar esta página. No podrá volver a ver esta clave secreta.</p> <p>Si pierde esta clave, elimínela y cree un Secreto de cliente.</p> 
        <ol> 
         <li value="1"> <p>Haga clic en el icono <b>[!UICONTROL Delete]</b> <img src="assets/delete.png"> para eliminar el Secreto de cliente actual.</p> </li> 
         <li value="2"> <p>Haga clic en <b>[!UICONTROL Add client secret]</b> para generar un nuevo Secreto de cliente.</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Redirect URLs]</td> 
      <td>Se redirigirá a los usuarios a esta ruta después de que se hayan autenticado con [!DNL Workfront].</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Refresh token rotation]</td> 
      <td>Habilite esta opción para emitir un nuevo token de actualización cada vez que se use el token. Su aplicación debe almacenar el nuevo token de actualización después de cada actualización.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Absolute refresh token expiration]</td> 
      <td> <p>Seleccione la cantidad de tiempo que desea que tenga un token de actualización antes de que venza. Cuando vence, los usuarios deben volver a iniciar sesión en la integración. Seleccione “[!UICONTROL No expiration]” si desea que el token de actualización no venza.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Caducidad del token de actualización por inactividad</td> 
      <td> <p>Seleccione la cantidad de tiempo después de la cual, si el usuario no ha estado activo en el sistema, su token de actualización vence. </p> <p>Por ejemplo, si la caducidad del token de actualización por inactividad es de seis meses y el usuario no inicia sesión durante este periodo, el token de actualización caduca, aunque la caducidad del token de actualización absoluta se pueda establecer para más tiempo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Logo]</td> 
      <td>Puede añadir un logotipo para que sea más sencillo identificar esta aplicación. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Este es el mismo nombre que le dio a la aplicación. Esta celda no puede estar vacía.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Introduzca una descripción para la integración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL App Description URL]</td> 
      <td>Puede ser un vínculo a una página “Acerca de nosotros” o una con más información sobre la integración.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Guardar]**.

Para obtener instrucciones sobre cómo configurar y utilizar la aplicación OAuth2 con credenciales de usuario (flujo de código de autorización), consulte [Configurar y utilizar las aplicaciones personalizadas OAuth 2 de su organización mediante el flujo de código de autorización](../../wf-api/api/oauth-app-code-token-flow.md).

### Creación de una aplicación web de una sola página de OAuth2 con PKCE {#create-an-oauth2-single-page-web-application-using-pkce}

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **[!UICONTROL Sistema]** y seleccione **[!UICONTROL Aplicaciones OAuth2]**.
1. Haga clic en **[!UICONTROL Crear integración de aplicaciones]**.

   Se muestra el cuadro **Nueva aplicación OAuth2**.
1. En el cuadro **Nueva aplicación OAuth2**, seleccione **[!UICONTROL Aplicación web de una sola página]**.
1. Escriba un nombre para la nueva aplicación [!UICONTROL OAuth2], como “[!DNL Workfront] para ClientApp”.
1. Haga clic en **[!UICONTROL Crear]**.
1. Rellene los campos de la nueva aplicación.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td> <p>Este campo se genera automáticamente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Redirect URLs]</td> 
      <td>Se redirigirá a los usuarios a esta ruta después de autenticarse en Workfront.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Rotate refresh token every time it is used]</td> 
      <td>Habilite esta opción para emitir un nuevo token de actualización cada vez que se use el token. Su aplicación debe almacenar el nuevo token de actualización después de cada actualización.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Absolute expiration]</td> 
      <td> <p>Seleccione la cantidad de tiempo que desea que tenga un token de actualización antes de que venza. Cuando vence, los usuarios deben volver a iniciar sesión en la integración. Seleccione “[!UICONTROL No expiration]” si desea que el token de actualización no venza.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Inactivity expiration]</td> 
      <td> <p>Seleccione la cantidad de tiempo después de la cual, si el usuario no ha estado activo en el sistema, su token de actualización vence. </p> <p>Por ejemplo, si la caducidad del token de actualización por inactividad es de seis meses y el usuario no inicia sesión durante este periodo, el token de actualización caduca, aunque la caducidad del token de actualización absoluta se pueda establecer para más tiempo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Logo]</td> 
      <td>Puede añadir un logotipo para que sea más sencillo identificar esta aplicación. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Este es el mismo nombre que le dio a la aplicación. Esta celda no puede estar vacía.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Introduzca una descripción para la integración.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Developer name]</td> 
      <td>Este es el nombre del desarrollador que configura la aplicación OAuth2.</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[!UICONTROL Developer email address]</td> 
      <td>Esta es la dirección de correo electrónico del desarrollador que configura la aplicación OAuth2.</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[!UICONTROL Privacy policy URL]</td> 
      <td>Este es el vínculo a donde su organización almacena la política de privacidad.</td> 
     </tr>


   </tbody> 
   </table>

   <!-- removed this from the table, and added "Developer name" and following rows:
   [!UICONTROL App Description URL]</td> 
      <td>This can be a link to an "About us" page or a page with more information about the integration.> -->

1. Haga clic en **[!UICONTROL Guardar]**.

## Configuración y uso de la aplicación OAuth2 creada

La configuración y el uso posteriores de la aplicación OAuth2 creada requieren algunos conocimientos técnicos, incluidas las llamadas de API.

* Para obtener instrucciones sobre cómo configurar y utilizar la aplicación OAuth2 con credenciales de usuario (flujo de código de autorización), consulte [Configurar y utilizar las aplicaciones personalizadas OAuth 2 de su organización mediante el flujo de código de autorización](../../wf-api/api/oauth-app-code-token-flow.md).
* Para obtener instrucciones sobre cómo configurar y utilizar la aplicación OAuth2 con la autenticación de servidor (flujo JWT), consulte [Configurar y utilizar las aplicaciones personalizadas OAuth 2 de su organización mediante el flujo JWT](../../wf-api/api/oauth-app-jwt-flow.md).
* Para obtener instrucciones sobre cómo configurar y utilizar la aplicación OAuth2 con PKCE, consulte [Configurar y utilizar las aplicaciones personalizadas OAuth 2 de su organización mediante el flujo PKCE](../../wf-api/api/oauth-app-pkce-flow.md).

## Procesos de OAuth2 para el flujo del código de autorización

>[!NOTE]
>
>Los usuarios tienen acceso a la aplicación [!UICONTROL OAuth2] a través de la API. Esta sección describe la funcionalidad en términos generales y se proporciona solo a título informativo.
>
>Para obtener instrucciones específicas sobre el uso de la aplicación OAuth2, incluidas las llamadas de API específicas, consulte [Configurar y utilizar las aplicaciones personalizadas OAuth 2 de su organización mediante el flujo del código de autorización](../../wf-api/api/oauth-app-code-token-flow.md).

### Autorización con un código de autorización y un token de acceso {#authorizing-with-an-authorization-code-and-access-token}

1. ClientApp necesita información de [!DNL Workfront], por lo que envía una solicitud al punto final [!DNL Workfront]de la API`/authorize`. La solicitud incluye [!UICONTROL response_type] `code`, que indica que la solicitud debe devolver un código de autorización.
1. Esto activa a [!DNL Workfront] para enviar un mensaje de autenticación al usuario. El usuario puede escribir sus credenciales en el mensaje, que da permiso a [!DNL Workfront] para comunicarse con ClientApp. Si el usuario ya ha iniciado sesión en [!DNL Workfront], se puede omitir este paso.
1. La API de [!DNL Workfront] envía un código de autorización a ClientApp.
1. ClientApp envía la siguiente información en una solicitud al punto final de la API de [!DNL Workfront] `/token`:

   * Código de autorización enviado a ClientApp en el paso 3. Esto identifica la instancia específica del permiso de usuario.
   * Secreto de cliente que se generó al configurar la aplicación OAuth2 de ClientApp en [!DNL Workfront]. Esto permite que [!DNL Workfront] sepa que la solicitud proviene de ClientApp.

1. Si el código de autorización y el secreto de cliente son correctos, [!DNL Workfront] enviará un token de acceso a ClientApp. Este token de acceso se envía directamente desde [!DNL Workfront] a ClientApp y ningún otro usuario o aplicación cliente puede verlo, copiarlo o utilizarlo.
1. ClientApp envía el token de acceso a [!DNL Workfront] junto con la solicitud de información específica.
1. Dado que el token de acceso es correcto, [!DNL Workfront] envía la información a ClientApp.

#### Actualización de tókenes de acceso

Por motivos de seguridad, los tókenes de acceso vencen después de un corto período de tiempo. Para obtener nuevos tókenes de acceso sin tener que escribir credenciales cada vez, [!DNL OAuth2] utiliza tókenes de actualización. El cliente almacena los tókenes de actualización.

El proceso para adquirir un token de actualización es el mismo que el procedimiento descrito en la sección [Autorización con un código de autorización y un token de acceso](#authorizing-with-an-authorization-code-and-access-token). La solicitud del código de autorización incluye el ámbito `offline_access`, que indica que la solicitud debe devolver un token de solicitud junto con el código de autorización.
