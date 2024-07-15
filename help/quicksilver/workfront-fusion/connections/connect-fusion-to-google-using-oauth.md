---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Conectar [!DNL Adobe Workfront Fusion] a [!DNL Google Services] mediante un cliente OAuth personalizado
description: Puede usar [!DNL Adobe Workfront Fusion] para conectarse a [!DNL Google Services] mediante un cliente OAuth personalizado. Este procedimiento requiere una cuenta  [!DNL Google] existente.
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# Conectar [!DNL Adobe Workfront Fusion] a [!DNL Google Services] mediante un cliente de OAuth personalizado

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

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
   <td role="rowheader">Product</td> 
   <td>
   <p>Nuevo:</p> <ul><li>Plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Workfront]: su organización debe adquirir [!DNL Adobe Workfront Fusion].</li><li>Se incluye el plan [!UICONTROL Ultimate] [!DNL Workfront]: [!DNL Workfront Fusion].</li></ul>
   <p>O</p>
   <p>Actual: su organización debe comprar [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Necesita una cuenta existente de [!DNL Google] para realizar esta conexión.

## Conexión de Fusion a los servicios de Google mediante un cliente de OAuth personalizado

Para crear esta conexión, debe crear y configurar un proyecto en Google Cloud Platform y, a continuación, configurar la conexión en Fusion basada en ese proyecto.

* [Crear un proyecto en  [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform)
* [Configurar el [!UICONTROL consentimiento de OAuth] configuración](#configure-oauth-consent-settings)
* [Crear credenciales de OAuth](#create-oauth-credentials)
* [Conectarse a [!DNL Google] en [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion)

>[!NOTE]
>
>Este procedimiento está diseñado para:
>
>* Uso personal ([!DNL `@gmail.com`] y [!DNL `@googlemail.com`] usuarios)
>* Uso interno ([!DNL Google Workspace] usuarios que prefieren utilizar un cliente OAuth personalizado)

### Crear un proyecto en [!DNL Google Cloud Platform]

Para crear un proyecto en la plataforma [!DNL Google Cloud]:

1. Inicie sesión en [[!DNL Google Cloud] Platform](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) con sus credenciales de [!DNL Google].
1. En el panel izquierdo, haga clic en **[!UICONTROL Panel]**.
1. Haga clic en **[!UICONTROL Crear proyecto]** en la esquina superior derecha de la pantalla.
1. Escriba el **[!UICONTROL nombre del proyecto]** y haga clic en **[!UICONTROL Crear]**.

1. Haga clic en la ficha **[!UICONTROL Habilitar API y servicios]** cerca de la parte superior de la pantalla.
1. En el campo **[!UICONTROL Buscar API y servicios]** de la parte superior de la pantalla, escriba el nombre del servicio que desea usar (como la API [!DNL Gmail] o la API [!DNL Google Drive]).
1. Cuando se muestre, haga clic en la API o el servicio al que desee conectarse [!DNL Workfront Fusion].
1. Haga clic en **[!UICONTROL Habilitar]** para habilitar la API seleccionada.
1. Repita los pasos del 6 al 8 para cada API que desee habilitar.

   >[!NOTE]
   >
   >Debe habilitar la API [!DNL Google Drive], así como la API de todas las aplicaciones de [!DNL Google] que desee usar (como la API [!DNL Google Sheets]).

1. En la pantalla que aparece, haga clic en **[!UICONTROL Crear credenciales]** en la esquina superior derecha.
1. Continúe en la sección [Configurar opciones de consentimiento de OAuth](#configure-oauth-consent-settings) de este artículo.

### Configurar [!UICONTROL consentimiento de OAuth]

1. En el panel izquierdo, haga clic en **[!UICONTROL Pantalla de consentimiento de OAuth]**.
1. Seleccione **[!UICONTROL External]** y haga clic en **[!UICONTROL Crear]**.

   >[!NOTE]
   >
   >No se le cobrará al seleccionar esta opción. Para obtener más información, consulte la información de [!DNL Google] sobre las excepciones a los requisitos de verificación.

1. Rellene los campos obligatorios como se indica a continuación:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nombre de aplicación]</p> </td> 
      <td> <p>Introduzca el nombre de la aplicación que solicita consentimiento.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Correo electrónico de asistencia al usuario]</td> 
      <td>Introduzca una dirección de correo electrónico para que los usuarios se pongan en contacto con usted si tienen preguntas sobre su consentimiento al conectarse a esta aplicación.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Direcciones de correo electrónico]</td> 
      <td>Escriba una o más direcciones de correo electrónico que Google pueda usar para notificarle sobre cualquier cambio en su proyecto.</td> 
     </tr> 
    </tbody> 
   </table>

1. En [!UICONTROL Dominios autorizados], haga clic en **[!UICONTROL Agregar dominio]** e introduzca `workfrontfusion.com`.

1. Haz clic en **[!UICONTROL Guardar y continuar]**.
1. Haga clic en **[!UICONTROL Agregar o quitar ámbitos]**.
1. En el panel derecho, habilite los siguientes ámbitos:

<table style="table-layout:auto">
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Servicio/API</th> 
      <th>Ámbitos requeridos</th> 
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
1. Haz clic en **[!UICONTROL Guardar y continuar]**.
1. (Opcional) Añada al proyecto cualquier usuario de prueba.
1. Haz clic en **[!UICONTROL Guardar y continuar]**.
1. Examine la información para comprobar su precisión y, a continuación, haga clic en **[!UICONTROL Volver al tablero]**.

   >[!NOTE]
   >
   >No es necesario que envíe su pantalla de consentimiento y su solicitud para verificación por [!DNL Google].

1. Continuar a [Crear credenciales de OAuth](#create-oauth-credentials).

### Crear credenciales de OAuth

1. En el panel izquierdo, haga clic en **[!UICONTROL Credenciales]**.

   >[!NOTE]
   >
   >Si no es la primera API o servicio ([!DNL Gmail] o [!DNL Google Drive]) que habilitó, no es necesario que cree nuevas credenciales.

1. Haga clic en **[!UICONTROL Crear credenciales]** cerca de la parte superior de la pantalla y, a continuación, seleccione **[!UICONTROL ID de cliente de OAuth]** en el menú desplegable.

1. Rellene los campos obligatorios como se indica a continuación:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo de aplicación]</td> 
      <td> <p> [!UICONTROL Aplicación web]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. En [!UICONTROL URI de redireccionamiento autorizados], haga clic en **[!UICONTROL Agregar URI]** e introduzca **uno** de los siguientes elementos:

   * Para [!DNL Gmail] o [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * Para otras [!DNL Google] aplicaciones: `https://app.workfrontfusion.com/oauth/cb/google`

1. Haga clic en **[!UICONTROL Crear]**.

   Se muestran [!UICONTROL ID de cliente] y [!UICONTROL Secreto de cliente].

1. Copie el [!UICONTROL ID de cliente] y el [!UICONTROL Secreto de cliente] a una ubicación segura. Los usará para establecer una conexión en [!DNL Workfront Fusion].
1. Continuar a [Conectarse a [!DNL Google] en [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

### Conectar con [!DNL Google] en [!DNL Workfront Fusion]

El proceso de creación de una conexión con [!DNL Google] difiere dependiendo de si está usando un módulo de un servicio de [!DNL Google] (como [!DNL Google Sheets] o [!DNL Google Docs]), o si se está conectando a [!DNL Google] a través del módulo de solicitud [!UICONTROL HTTP] >[!UICONTROL Make an OAuth2.0].

* [Conectarse a  [!DNL Google] en un servicio [!DNL Google] de](#connect-to-google-in-a-google-service)
* [Conéctese a [!DNL Google] en el módulo [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud OAuth2.0]](#connect-to-google-in-the-http--make-an-oauth20-request-module)

#### Conectarse a [!DNL Google] en un servicio de [!DNL Google]

1. En [!DNL Workfront Fusion], busque el módulo [!DNL Google] para el que necesita crear una conexión.
1. Haz clic en **[!UICONTROL Crear una conexión]** y luego haz clic en **[!UICONTROL Mostrar configuración avanzada]**.

1. Escriba el [!UICONTROL ID de cliente] y el [!UICONTROL Secreto de cliente] que recuperó en [[!UICONTROL Crear credenciales de OAuth]](#create-oauth-credentials) en los campos respectivos y luego haga clic en **[!UICONTROL Continuar]**.

1. Inicie sesión con su cuenta de [!DNL Google].

   Se muestra la ventana **[!UICONTROL Esta aplicación no está verificada]**. Tenga en cuenta que la &quot;aplicación&quot; mencionada en el título de la ventana es el cliente de OAuth que ha creado anteriormente.

1. Haga clic en **[!UICONTROL Avanzado]** y, a continuación, haga clic en **[!UICONTROL Ir a [!DNL Workfront Fusion] (no seguro)]** para permitir el acceso con su cliente OAuth personalizado.

1. Haga clic en **[!UICONTROL Permitir]** para conceder el permiso a [!DNL Workfront Fusion].
1. En la ventana que aparece, vuelve a hacer clic en **[!UICONTROL Permitir]** para confirmar tus opciones.

   Se ha establecido la conexión con el servicio [!DNL Google] deseado mediante un cliente OAuth personalizado.

#### Conéctese a [!DNL Google] en el módulo [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud OAuth2.0] {#connect-to-google-in-the-http--make-an-oauth20-request-module}

Para obtener instrucciones sobre cómo conectarse a [!DNL Google] en el módulo [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud OAuth2.0], consulte [Instrucciones para crear una conexión a [!DNL Google] en el módulo [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud OAuth 2.0]](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module) en [[!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud OAuth 2.0]](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## Posible mensaje de error:[!UICONTROL [403] Acceso no configurado]

Si se muestra el mensaje de error [!UICONTROL `403 Access Not Configured`], debe habilitar la API correspondiente en Google Cloud Platform. Para habilitar la API, siga los pasos de la sección [Crear un proyecto el [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) de este artículo.
