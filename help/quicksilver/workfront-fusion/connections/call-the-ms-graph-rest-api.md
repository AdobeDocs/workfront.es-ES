---
title: Llame a la API REST de MS Graph a través del módulo  [!DNL Adobe Workfront Fusion] HTTP > Realizar una solicitud OAuth 2.0
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 87%

---

# Llame a la [!UICONTROL API de REST de MS Graph] a través del módulo [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud OAuth 2.0]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Llamar a la API de REST de MS Graph](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/call-the-ms-graph-rest-api.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

<!-- Audited: 3/2024-->

Se puede acceder a muchos servicios web de [!DNL Microsoft] a través de [!DNL Microsoft Graph API]. Puede crear una conexión con [!DNL Microsoft Graph API], usando el módulo [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL Realizar una solicitud OAuth 2.0].

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

## Registrar [!DNL Workfront Fusion] en [!DNL Microsoft Application Registration Portal]

Para crear una conexión con [!DNL Microsoft Graph REST API], primero debe registrar [!DNL Adobe Workfront Fusion].

1. Empiece a registrar una aplicación nueva como se describe en [Registrar su aplicación](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) en la documentación de [!DNL Microsoft].

   Como parte del registro, [!DNL Microsoft] requiere la siguiente información:

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Application name]</td>
        <td>Escriba un nombre para la aplicación, como “Mi aplicación [!DNL Workfront Fusion]”.</td>
      </tr>
      <tr>
        <td>[!UICONTROL Redirect URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. Cuando haya completado el registro de la aplicación, anote el [!UICONTROL ID de la aplicación].

   >[!IMPORTANT]
   >
   >Necesitará el ID de aplicación para configurar la conexión en [!DNL Workfront Fusion].

1. Generar un [!UICONTROL Secreto de aplicación]. Anote este secreto.

   Para obtener instrucciones, consulte [Registrar su aplicación](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) en la documentación de [!DNL Microsoft].

   >[!IMPORTANT]
   >
   >Necesitará el [!UICONTROL Secreto de aplicación] para configurar su conexión en [!DNL Workfront Fusion].

1. Configure los permisos para su aplicación.

   Para obtener información específica sobre cómo localizar y configurar estos campos, consulte la sección “Configuración de permisos para Microsoft Graph” en [Obtener acceso sin un usuario](https://docs.microsoft.com/en-us/graph/auth-v2-service) en la documentación de [!UICONTROL Microsoft].

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL What type of permissions does your application require?]</td> 
      <td>Seleccione <code>[!UICONTROL Delegated permissions]</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Select permissions]</td> 
      <td> <p>Seleccione los siguientes permisos:</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>Cualquier otro permiso requerido por sus integraciones (Ejemplo: <code>User.Read</code>)</p> </li> 
       </ul> <p><b>Importante</b>: necesitará los permisos seleccionados para configurar su conexión en [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Continúe con [Configurar su conexión de  [!DNL MS Graph API]  en  [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## Configurar su conexión de [!DNL MS Graph API] en [!DNL Workfront Fusion]

Después de registrar [!DNL Workfront Fusion] tal como se describe en [Registrar  [!DNL Workfront Fusion]  en  [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal), puede configurar la conexión en el módulo [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud Oauth 2.0].

1. Añada un módulo [!UICONTROL HTTP] > [!UICONTROL Realizar una llamada OAuth 2.0] a su escenario.
1. Haga clic en **[!UICONTROL Añadir]** junto al campo [!UICONTROL conexión].
1. Configure los campos de conexión de la siguiente manera:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name]</td> 
      <td>Introduzca un nombre para la conexión. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Flow type]</p> </td> 
      <td><code>[!UICONTROL Authorization Code]</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authorize URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/authorize</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope]</td> 
      <td> <p>Escriba los permisos que seleccionó en el paso 4 de <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrar [!DNL Workfront Fusion] en [!DNL Microsoft Application Registration Portal]</a>.</p> <p>Para cada ámbito, haga clic en <b>[!UICONTROL Add]</b> y escriba el permiso.</p> <p>Ejemplo: <code>offline_access</code></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope separator]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>Escriba el [!UICONTROL Application ID] del paso 2 en <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrar [!DNL Workfront Fusion] en [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>Escriba el [!UICONTROL Application Secret] generado en el paso 3 en <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrar [!DNL Workfront Fusion] en [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authorize parameters]</td> 
      <td> <p>Añada los siguientes parámetros Authorize:</p> 
       <ul> 
        <li> <p>[!UICONTROL Key]:<code> response_mode</code> [!UICONTROL Value]: <code>query</code></p> </li> 
        <li> <p>[!UICONTROL Key]: <code>prompt </code>[!UICONTROL Value]: <code>consent</code></p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Access token parameters]</td> 
      <td>No es necesario que introduzca nada en este campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Refresh token parameters]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Haga clic en <b>[!UICONTROL Add]</b>.</p> </li> 
        <li value="2"> <p>En el campo <b>[!UICONTROL Key]</b>, escriba <code>scope</code>.</p> </li> 
        <li value="3"> <p>En el campo <b>[!UICONTROL Value]</b>, escriba todos los [!UICONTROL scope]s que haya especificado en el campo de ámbito, separados por espacios.</p> <p>Ejemplo: <code>offline_access openid User.Read</code></p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Custom Headers]</td> 
      <td>No es necesario que introduzca nada en este campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Placement]</td> 
      <td><code>[!UICONTROL In the header]</code> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Continuar]**.
1. En la ventana que aparece, haga clic en **[!UICONTROL Aceptar]** para completar la conexión y volver al módulo.
