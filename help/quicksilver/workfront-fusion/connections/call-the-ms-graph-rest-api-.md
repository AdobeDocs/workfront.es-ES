---
title: Llame a la API de REST de MS Graph a través de la función [!DNL Adobe Workfront Fusion] HTTP &gt; Crear un módulo de solicitud OAuth 2.0
description: Llame a la API de REST de MS Graph a través de la función [!DNL Adobe Workfront Fusion] HTTP &gt; Crear un módulo de solicitud OAuth 2.0
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 1%

---

# Llame a la función[!UICONTROL  API de REST de MS Graph] a través de la variable [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud de OAuth 2.0] módulo

Muchas [!DNL Microsoft] se puede acceder a los servicios web a través de la [!DNL Microsoft Graph API]. En este artículo se describe cómo crear una conexión con esa API mediante la [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL Realizar una solicitud de OAuth 2.0] módulo.

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

## Registro [!DNL Workfront Fusion] en el [!DNL Microsoft Application Registration Portal]

Para crear una conexión con el [!DNL Microsoft Graph REST API], primero debe registrarse [!DNL Adobe Workfront Fusion].

1. Comience a registrar una nueva aplicación, tal como se describe en [Registre su aplicación](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) en el [!DNL Microsoft] documentación.

   Como parte del registro, [!DNL Microsoft] requiere la siguiente información:

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Application name]</td>
        <td>Escriba un nombre para la aplicación, como "Mi [!DNL Workfront Fusion] aplicación".</td>
      </tr>
      <tr>
        <td>[!UICONTROL URL de redireccionamiento]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. Cuando haya completado el registro de la aplicación, tome nota de la [!UICONTROL ID de aplicación].

   >[!IMPORTANT]
   >
   >Necesitará el ID de aplicación para configurar la conexión en [!DNL Workfront Fusion].

1. Genere un [!UICONTROL Secreto de la aplicación]. Anote este secreto.

   Para obtener instrucciones, consulte [Registre su aplicación](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) en el [!DNL Microsoft] documentación.

   >[!IMPORTANT]
   >
   >Necesitará la variable [!UICONTROL Secreto de la aplicación] para configurar la conexión en [!DNL Workfront Fusion].

1. Configure los permisos para la aplicación.

   Para obtener información detallada sobre cómo localizar y configurar estos campos, consulte la sección &quot;Configurar permisos para Microsoft Graph&quot; en [Obtener acceso sin un usuario](https://docs.microsoft.com/en-us/graph/auth-v2-service) en el [!UICONTROL Microsoft] documentación.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL ¿Qué tipo de permisos requiere su aplicación?]</td> 
      <td>Seleccionar <code>[!UICONTROL Delegated permissions]</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Seleccionar permisos]</td> 
      <td> <p>Seleccione los siguientes permisos:</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>Todos los demás permisos requeridos por las integraciones (Ejemplo: <code>User.Read</code>)</p> </li> 
       </ul> <p>Importante: Necesitará los permisos seleccionados para configurar la conexión en [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Continúe con [Configure las [!DNL MS Graph API] conexión en [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## Configure las [!DNL MS Graph API] conexión en [!DNL Workfront Fusion]

Después de registrarse [!DNL Workfront Fusion] tal como se describe en [Registro [!DNL Workfront Fusion] en el [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal), puede configurar la conexión en el [!UICONTROL HTTP] >[!UICONTROL Hacer un Oauth 2.0] módulo de solicitud.

1. Agregue un [!UICONTROL HTTP] >[!UICONTROL Realizar una llamada a OAuth 2.0] al escenario.
1. Haga clic en **[!UICONTROL Agregar]** junto a la variable [!UICONTROL connection] campo .
1. Configure los campos de conexión de la siguiente manera:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name]</td> 
      <td>Introduzca un nombre para la conexión.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Tipo de flujo]</p> </td> 
      <td><code>[!UICONTROL Authorization Code]</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Autorizar URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/authorize</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ámbito]</td> 
      <td> <p>Introduzca los permisos seleccionados en el paso 4 de <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registro [!DNL Workfront Fusion] en el [!DNL Microsoft Application Registration Portal]</a>.</p> <p>Para cada ámbito, haga clic en <b>[!UICONTROL Agregar]</b> y escriba el permiso.</p> <p>Ejemplo: <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Separador de ámbito]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>Introduzca el [!UICONTROL Application ID] del paso 2 en <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registro [!DNL Workfront Fusion] en el [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>Introduzca el [!UICONTROL Application Secret] que ha generado en el paso 2 de <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registro [!DNL Workfront Fusion] en el [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Autorizar parámetros]</td> 
      <td> <p>Agregue los siguientes parámetros de Autorización:</p> 
       <ul> 
        <li> <p>[!UICONTROL Key]:<code> response_mode</code> [!UICONTROL Valor]: <code>query</code></p> </li> 
        <li> <p>[!UICONTROL Key]: <code>prompt </code>[!UICONTROL Valor]: <code>consent</code></p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parámetros del token de acceso]</td> 
      <td>No es necesario que introduzca nada en este campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Actualizar parámetros de token]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Haga clic en <b>[!UICONTROL Agregar]</b>.</p> </li> 
        <li value="2"> <p>En el <b>[!UICONTROL Key]</b> , introduzca <code>scope</code>.</p> </li> 
        <li value="3"> <p>En el <b>[!UICONTROL Valor]</b> , introduzca todos los [!UICONTROL scope]s que introdujo en el campo de ámbito, separados por espacios.</p> <p>Ejemplo: <code>offline_access openid User.Read</code></p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Encabezados personalizados]</td> 
      <td>No es necesario que introduzca nada en este campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Placement]</td> 
      <td><code>[!UICONTROL In the header]</code> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Continuar]**.
1. En la ventana que aparece, haga clic en **[!UICONTROL Accept]** para completar la conexión y volver al módulo.
