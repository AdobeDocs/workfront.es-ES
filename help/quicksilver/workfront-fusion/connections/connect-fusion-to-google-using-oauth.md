---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Conectar [!DNL Adobe Workfront Fusion] a [!DNL Google Services] mediante un cliente OAuth personalizado
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 91%

---

# Conectar [!DNL Adobe Workfront Fusion] a [!DNL Google Services] mediante un cliente de OAuth personalizado

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Conecte Adobe Workfront Fusion a los servicios de Google mediante un cliente OAuth personalizado](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/connect-fusion-to-google-using-oauth.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td> <p>Nuevo: [!UICONTROL Standard]</p><p>O</p><p>Actual: [!UICONTROL Work] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Actual: no se requiere licencia para [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Heredado: cualquiera </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Nuevo:</p> <ul><li>Plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Workfront]: su organización debe comprar [!DNL Adobe Workfront Fusion].</li><li>Plan [!UICONTROL Ultimate] [!DNL Workfront]: [!DNL Workfront Fusion] está incluido.</li></ul>
   <p>O</p>
   <p>Actual: su organización debe comprar [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obtener información sobre las licencias de [!DNL Adobe Workfront Fusion], consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Necesita una cuenta existente de [!DNL Google] para realizar esta conexión.

## Conectar Fusion a Google Services mediante un cliente de OAuth personalizado

Para crear esta conexión, debe crear y configurar un proyecto en la plataforma Google Cloud y, a continuación, configurar una conexión en Fusion basada en ese proyecto.

* [Crear un proyecto en [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform)
* [Establecer la configuración de [!UICONTROL consentimiento de OAuth]](#configure-oauth-consent-settings)
* [Crear credenciales de OAuth](#create-oauth-credentials)
* [Conectarse a [!DNL Google] en [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion)

>[!NOTE]
>
>Este procedimiento está diseñado para:
>
>* Uso personal (usuarios de [!DNL `@gmail.com`] y [!DNL `@googlemail.com`])
>* Uso interno (usuarios de [!DNL Google Workspace] que prefieren utilizar un cliente OAuth personalizado)

### Crear un proyecto en [!DNL Google Cloud Platform]

Para crear un proyecto en la plataforma [!DNL Google Cloud]:

1. Inicie sesión en [[!DNL Google Cloud] Platform](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) con sus credenciales de [!DNL Google].
1. En el panel izquierdo, haga clic en **[!UICONTROL Panel de control]**.
1. Haga clic en **[!UICONTROL Crear proyecto]** en la esquina superior derecha de la pantalla.
1. Escriba el **[!UICONTROL Nombre del proyecto]** y haga clic en **[!UICONTROL Crear]**.

1. Haga clic en la pestaña **[!UICONTROL Habilitar API y servicios]** cerca de la parte superior de la pantalla.
1. En el campo **[!UICONTROL Buscar API y servicios]** de la parte superior de la pantalla, escriba el nombre del servicio que desea usar (como API de [!DNL Gmail] o API de [!DNL Google Drive]).
1. Cuando se muestre, haga clic en la API o el servicio que desea conectar a [!DNL Workfront Fusion].
1. Haga clic en **[!UICONTROL Habilitar]** para habilitar la API seleccionada.
1. Repita los pasos del 6 al 8 para cada API que desee habilitar.

   >[!NOTE]
   >
   >Debe habilitar la API de [!DNL Google Drive], así como la API de todas las aplicaciones de [!DNL Google] que desee usar (como la API de [!DNL Google Sheets]).

1. En la pantalla que aparece, haga clic en **[!UICONTROL Crear credenciales]** en la esquina superior derecha.
1. Continúe en la sección [Establecer la configuración de consentimiento de OAuth](#configure-oauth-consent-settings) de este artículo.

### Establecer configuración de [!UICONTROL consentimiento de OAuth]

1. En el panel izquierdo, haga clic en **[!UICONTROL Pantalla de consentimiento de OAuth]**.
1. Seleccione **[!UICONTROL Externa]** y haga clic en **[!UICONTROL Crear]**.

   >[!NOTE]
   >
   >No se le aplicará ningún cargo si selecciona esta opción. Para obtener más información, consulte la información de [!DNL Google] sobre las excepciones a los requisitos de verificación.

1. Rellene los campos obligatorios tal como se indica a continuación:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App name]</p> </td> 
      <td> <p>Introduzca el nombre de la aplicación que solicita consentimiento.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL User support email]</td> 
      <td>Introduzca una dirección de correo electrónico para que los usuarios se pongan en contacto con usted si tienen preguntas sobre su consentimiento al conectarse a esta aplicación.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Email addresses]</td> 
      <td>Escriba una o más direcciones de correo electrónico que Google puede utilizar para notificarle sobre cualquier cambio en su proyecto.</td> 
     </tr> 
    </tbody> 
   </table>

1. En [!UICONTROL Dominios autorizados], haga clic en **[!UICONTROL Añadir dominio]** e introduzca `workfrontfusion.com`.

1. Haga clic en **[!UICONTROL Guardar y continuar]**.
1. Haga clic en **[!UICONTROL Añadir o quitar ámbitos]**.
1. En el panel derecho, habilite los siguientes ámbitos:

<table style="table-layout:auto">
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Servicio/API</th> 
      <th>Ámbitos obligatorios</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p>[!DNL Gmail]</p> </td> 
      <td> <p>https://mail.google.com/</p> <p>https://www.googleapis.com/auth/gmail.labels</p> <p>https://www.googleapis.com/auth/gmail.send</p> <p>https://www.googleapis.com/auth/gmail.readonly</p> <p>https://www.googleapis.com/auth/gmail.compose</p> <p>https://www.googleapis.com/auth/gmail.insert</p> <p>https://www.googleapis.com/auth/gmail.modify</p> <p>https://www.googleapis.com/auth/gmail.metadata</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!DNL Google Drive]</p> </td> 
      <td> <p>https://www.googleapis.com/auth/drive</p> <p>https://www.googleapis.com/auth/drive.readonly</p> </td> 
     </tr> 
    </tbody> 
   </table>

Es posible que tenga que expandir la lista o ir a la siguiente página de la lista para verlos todos.

1. Haga clic en **[!UICONTROL Actualizar]**.
1. Haga clic en **[!UICONTROL Guardar y continuar]**.
1. (Opcional) Añada al proyecto cualquier usuario de prueba.
1. Haga clic en **[!UICONTROL Guardar y continuar]**.
1. Examine la información para comprobar su precisión y, a continuación, haga clic en **[!UICONTROL Volver al panel de control]**.

   >[!NOTE]
   >
   >No es necesario que envíe su pantalla de consentimiento y su solicitud para que lo verifique [!DNL Google].

1. Continúe hasta [Crear credenciales de OAuth](#create-oauth-credentials).

### Crear credenciales de OAuth

1. En el panel izquierdo, haga clic en **[!UICONTROL Credenciales]**.

   >[!NOTE]
   >
   >Si no es la primera API o servicio ([!DNL Gmail] o [!DNL Google Drive]) que ha habilitado, no es necesario que cree nuevas credenciales.

1. Haga clic en **[!UICONTROL Crear credenciales]** cerca de la parte superior de la pantalla y, a continuación, seleccione **[!UICONTROL ID de cliente de OAuth]** en el menú desplegable.

1. Rellene los campos obligatorios tal como se indica a continuación:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Application type]</td> 
      <td> <p> [!UICONTROL Web application]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. En [!UICONTROL URI de redireccionamiento autorizados], haga clic en **[!UICONTROL Añadir URI]** e introduzca **uno** de los siguientes elementos:

   * Para [!DNL Gmail] o [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * Para otras aplicaciones de [!DNL Google]: `https://app.workfrontfusion.com/oauth/cb/google`

1. Haga clic en **[!UICONTROL Crear]**.

   Se muestran [!UICONTROL ID de cliente] y [!UICONTROL Secreto de cliente].

1. Copie el [!UICONTROL Client ID] y el [!UICONTROL Client Secret] a una ubicación segura. Los usará para establecer una conexión en [!DNL Workfront Fusion].
1. Continúe a [Conectarse a [!DNL Google] en [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

### Conectar con [!DNL Google] en [!DNL Workfront Fusion]

El proceso de creación de una conexión con [!DNL Google] difiere dependiendo de si está usando un módulo de un servicio de [!DNL Google] (como [!DNL Google Sheets] o [!DNL Google Docs]), o si se está conectando a [!DNL Google] a través del módulo de solicitud [!UICONTROL HTTP] >[!UICONTROL Make an OAuth2.0].

* [Conectarse a  [!DNL Google] en un servicio de [!DNL Google] ](#connect-to-google-in-a-google-service)
* [Conectarse a [!DNL Google] en el módulo [!UICONTROL HTTP] > [!UICONTROL Make an OAuth2.0 request]](#connect-to-google-in-the-http--make-an-oauth20-request-module)

#### Conectarse a [!DNL Google] en un servicio de [!DNL Google]

1. En [!DNL Workfront Fusion], busque el módulo [!DNL Google] para el que necesita crear una conexión.
1. Haga clic en **[!UICONTROL Create a connection]** y luego haga clic en **[!UICONTROL Show advanced settings]**.

1. Escriba el [!UICONTROL Client ID] y el [!UICONTROL Client Secret] que recuperó en [[!UICONTROL Create OAuth Credentials]](#create-oauth-credentials) en los campos respectivos y luego haga clic en **[!UICONTROL Continue]**.

1. Inicie sesión con su cuenta de [!DNL Google].

   Se muestra la ventana **[!UICONTROL This app isn&#39;t verified]**. Tenga en cuenta que la &quot;aplicación&quot; mencionada en el título de la ventana es el cliente de OAuth que ha creado anteriormente.

1. Haga clic en **[!UICONTROL Avanced]** y, a continuación, haga clic en **[!UICONTROL Go to [!DNL Workfront Fusion] (no seguro)]** para permitir el acceso con su cliente OAuth personalizado.

1. Haga clic en **[!UICONTROL Allow]** para conceder el permiso a [!DNL Workfront Fusion].
1. En la ventana que aparece, vuelva a hacer clic en **[!UICONTROL Allow]** para confirmar sus opciones.

   Se ha establecido la conexión con el servicio [!DNL Google] deseado mediante un cliente OAuth personalizado.

#### Conectarse a [!DNL Google] en el módulo [!UICONTROL HTTP] > [!UICONTROL Make an OAuth2.0 request] {#connect-to-google-in-the-http--make-an-oauth20-request-module}

Para obtener instrucciones sobre cómo conectarse a [!DNL Google] en el módulo [!UICONTROL HTTP] > [!UICONTROL Make an OAuth2.0 request], consulte [Instrucciones para crear una conexión a [!DNL Google] en el módulo [!UICONTROL HTTP] > [!UICONTROL Make an OAuth2.0 request] ](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module) en [[!UICONTROL HTTP] > [!UICONTROL Make an OAuth2.0 request] ](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Posible mensaje de error:[!UICONTROL [403] Access Not Configured]

Si se muestra el mensaje de error [!UICONTROL `403 Access Not Configured`], debe habilitar la API correspondiente en Google Cloud Platform. Para habilitar la API, siga los pasos de la sección [Crear un proyecto en [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) de este artículo.
