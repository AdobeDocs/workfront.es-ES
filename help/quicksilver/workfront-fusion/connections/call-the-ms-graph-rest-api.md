---
title: Llame a la API de REST de MS Graph a través de  [!DNL Adobe Workfront Fusion] HTTP &gt; Crear un módulo de solicitud de OAuth 2.0
description: Llame a la API de REST de MS Graph a través de  [!DNL Adobe Workfront Fusion] HTTP &gt; Crear un módulo de solicitud de OAuth 2.0
author: Becky
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 1%

---

# Llamar a la API [!UICONTROL  de REST de MS Graph] a través del módulo [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Realizar una solicitud OAuth 2.0]

<!-- Audited: 3/2024-->

Se tiene acceso a muchos servicios web de [!DNL Microsoft] a través de [!DNL Microsoft Graph API]. Puede crear una conexión con [!DNL Microsoft Graph API], usando el módulo [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL Realizar una solicitud OAuth 2.0].

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

## Registrar [!DNL Workfront Fusion] en [!DNL Microsoft Application Registration Portal]

Para crear una conexión con [!DNL Microsoft Graph REST API], primero debe registrar [!DNL Adobe Workfront Fusion].

1. Empiece a registrar una aplicación nueva como se describe en [Registre su aplicación](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) en la documentación de [!DNL Microsoft].

   Como parte del registro, [!DNL Microsoft] requiere la siguiente información:

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Nombre de aplicación]</td>
        <td>Escriba un nombre para la aplicación, como "Mi aplicación [!DNL Workfront Fusion]".</td>
      </tr>
      <tr>
        <td>[!UICONTROL URL de redireccionamiento]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. Cuando haya completado el registro de la aplicación, anote [!UICONTROL ID de la aplicación].

   >[!IMPORTANT]
   >
   >Necesitará el identificador de aplicación para configurar la conexión en [!DNL Workfront Fusion].

1. Generar un [!UICONTROL Secreto de aplicación]. Tome nota de este secreto.

   Para obtener instrucciones, consulta [Registrar tu aplicación](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) en la documentación de [!DNL Microsoft].

   >[!IMPORTANT]
   >
   >Necesitará el [!UICONTROL Secreto de aplicación] para configurar su conexión en [!DNL Workfront Fusion].

1. Configure los permisos para su aplicación.

   Para obtener información específica sobre cómo localizar y configurar estos campos, consulte la sección &quot;Configuración de permisos para Microsoft Graph&quot; en [Obtener acceso sin un usuario](https://docs.microsoft.com/en-us/graph/auth-v2-service) en la documentación de [!UICONTROL Microsoft].

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL ¿Qué tipo de permisos requiere su aplicación?]</td> 
      <td>Seleccione <code>[!UICONTROL Delegated permissions]</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Seleccionar permisos]</td> 
      <td> <p>Seleccione los siguientes permisos:</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>Cualquier otro permiso requerido por sus integraciones (Ejemplo: <code>User.Read</code>)</p> </li> 
       </ul> <p><b>Importante</b>: Necesitará los permisos seleccionados para configurar su conexión en [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Continúe con [Configurar su [!DNL MS Graph API] conexión en [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## Configurar su conexión de [!DNL MS Graph API] en [!DNL Workfront Fusion]

Después de registrar [!DNL Workfront Fusion] como se describe en [Registrar [!DNL Workfront Fusion] en [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal), puede configurar la conexión en el módulo de solicitud [!UICONTROL HTTP] > [!UICONTROL Crear un módulo de solicitud Oauth 2.0].

1. Agregue un módulo [!UICONTROL HTTP] > [!UICONTROL Realice una llamada OAuth 2.0] a su escenario.
1. Haga clic en **[!UICONTROL Agregar]** junto al campo [!UICONTROL conexión].
1. Configure los campos de conexión de la siguiente manera:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre de conexión]</td> 
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
      <td> <p>Escriba los permisos que seleccionó en el paso 4 de <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrar [!DNL Workfront Fusion] en [!DNL Microsoft Application Registration Portal]</a>.</p> <p>Para cada ámbito, haga clic en <b>[!UICONTROL Add]</b> y escriba el permiso.</p> <p>Ejemplo: <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Separador de ámbitos]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID de cliente]</td> 
      <td>Escriba el [!UICONTROL Application ID] del paso 2 en <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registrar [!DNL Workfront Fusion] en [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Secreto de cliente]</td> 
      <td>Escriba el [!UICONTROL Application Secret] generado en el paso 3 del <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">Registro [!DNL Workfront Fusion] en [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Autorizar parámetros]</td> 
      <td> <p>Añada los siguientes parámetros Authorize:</p> 
       <ul> 
        <li> <p>[!UICONTROL Clave]:<code> response_mode</code> [!UICONTROL Valor]: <code>query</code></p> </li> 
        <li> <p>[!UICONTROL Clave]: <code>prompt </code>[!UICONTROL Valor]: <code>consent</code></p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parámetros de token de acceso]</td> 
      <td>No es necesario que introduzca nada en este campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Actualizar parámetros de token]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Haga clic en <b>[!UICONTROL Add]</b>.</p> </li> 
        <li value="2"> <p>En el campo <b>[!UICONTROL Key]</b>, escriba <code>scope</code>.</p> </li> 
        <li value="3"> <p>En el campo <b>[!UICONTROL Value]</b>, escriba todos los [!UICONTROL scope] que ha especificado en el campo de ámbito, separados por espacios.</p> <p>Ejemplo: <code>offline_access openid User.Read</code></p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Encabezados personalizados]</td> 
      <td>No es necesario que introduzca nada en este campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Colocación de token]</td> 
      <td><code>[!UICONTROL In the header]</code> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Continuar]**.
1. En la ventana que aparece, haga clic en **[!UICONTROL Aceptar]** para completar la conexión y volver al módulo.
