---
title: Configurar la integración de  [!DNL SharePoint]
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Puedes integrar [!DNL Workfront] con [!DNL SharePoint] Online, lo que permite a los usuarios navegar, vincular y agregar [!DNL SharePoint] documentos dentro de Workfront. La funcionalidad proporcionada es similar a la de otras  [!DNL Workfront] integraciones de documentos.
author: Becky
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: 3c87c88245e79581c2a880c13038bcedb24caf4b
workflow-type: tm+mt
source-wordcount: '1729'
ht-degree: 0%

---

# Configurar la integración de [!DNL SharePoint]

<!--Audited: 12/2023-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>La nueva integración de [!DNL SharePoint] se lanzó a la producción con la versión 22.3 (julio de 2022).
>
>* Aunque los usuarios aún pueden tener acceso a los documentos vinculados a través de la integración heredada de [!DNL SharePoint], no pueden vincular documentos a través de ella. deben usar la nueva integración de [!DNL SharePoint] para vincular documentos desde SharePoint.
>
>* Si no tiene configurada una integración de SharePoint heredada, no puede agregarla. Debe utilizar la nueva integración de SharePoint para vincular documentos a SharePoint.
>
>* Es posible que la nueva integración de SharePoint no requiera la configuración de un administrador y que la configuren usuarios individuales. Sin embargo, para garantizar una transición sin problemas a la nueva integración de SharePoint, un administrador de Workfront debe realizar algunos pequeños cambios en la configuración del área Configuración de Workfront.
>
>    Para obtener información e instrucciones, consulte [Configuración de la integración heredada de SharePoint para obtener acceso continuo a los documentos](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents) en este artículo.
>    
>* Se recomienda que los usuarios vinculen los documentos que actualmente están vinculados a través de la integración heredada de [!DNL SharePoint] a través de la nueva integración.
>    
>    Para obtener instrucciones sobre cómo vincular documentos, consulte [Vincular documentos desde aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Puede integrar [!DNL Workfront] con [!DNL SharePoint Online], lo que permite a los usuarios navegar, vincular y agregar documentos de [!DNL SharePoint] en Workfront. La funcionalidad proporcionada es similar a la de otras integraciones de [!DNL Workfront], como [!DNL Google Drive], [!DNL Box] y [!DNL Dropbox].

Esta integración solamente es compatible con [!DNL SharePoint Online]. No se admiten instancias locales de [!DNL SharePoint].

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>Nuevo: estándar <p>O</p><p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td>Debe ser administrador de [!DNL Workfront]. </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Debe tener el acceso o los permisos necesarios en [!DNL SharePoint] para modificar o configurar la integración de [!DNL SharePoint].

## Vinculación de documentos con la nueva integración de SharePoint

Los usuarios individuales pueden vincular documentos mediante la nueva integración de [!DNL SharePoint]. La integración no requiere la configuración del administrador. En su lugar, el usuario inicia sesión en su cuenta de [!DNL Microsoft] al vincular un documento, lo que permite que la integración acceda a los documentos disponibles en [!DNL SharePoint] del usuario.

La primera vez que un usuario conecte la integración de [!DNL Workfront] [!DNL SharePoint] con su cuenta de [!DNL SharePoint], verá y aceptará todos los permisos que [!DNL Workfront] usa al interactuar con su cuenta de [!UICONTROL SharePoint], o bien podrá solicitar permisos a su administrador de Microsoft. Los permisos de lectura permiten que [!DNL Workfront] vea y tenga acceso a los archivos de [!DNL SharePoint], y los permisos de escritura permiten al usuario cargar archivos en [!DNL SharePoint].

![Permisos de Sharepoint](assets/sharepoint-permissions.png)

Para obtener instrucciones sobre cómo vincular documentos a través de la nueva integración de [!DNL SharePoint], consulte [Vincular un documento externo a [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* Según la configuración de Microsoft de la organización, los usuarios pueden ver una página &quot;Se requiere aprobación&quot; en lugar de &quot;Permisos solicitados&quot;. En este caso, los usuarios pueden utilizar esta página para solicitar al administrador de Microsoft de la organización que conceda permisos para la integración con Sharepoint.
>
>* Una integración de [!DNL SharePoint] puede conectarse a una sola instancia de [!DNL SharePoint]. Por lo tanto, un usuario puede configurar una integración para un(a) [!DNL SharePoint], pero no puede configurar una integración para un segundo(a) [!DNL SharePoint], aunque tenga permisos para y documentos en el segundo(a) [!DNL SharePoint].
>
>* Un usuario tiene acceso a los mismos sitios, colecciones, carpetas, subcarpetas y archivos mediante la integración de [!DNL Workfront] [!DNL SharePoint] que tiene en su cuenta de [!DNL SharePoint].

### Vincular documentos de SharePoint

Para obtener instrucciones sobre cómo vincular documentos desde SharePoint a través de la nueva integración de [!DNL SharePoint], consulte [Vincular un documento externo a [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront).

### Envío de documentos a SharePoint

Para enviar un documento a SharePoint:

1. Haga clic en el icono **Enviar a** ![Enviar a](assets/send-to-icon.png) y seleccione SharePoint (API de gráficos).
1. (Opcional) Busque en la barra de búsqueda el sitio o la carpeta a los que desea enviar el documento.
1. Seleccione el sitio o la carpeta en la lista.

   * Los sitios están marcados con ![icono del sitio](assets/site-icon.png).

   * Las carpetas están marcadas con ![icono de carpeta](assets/folder-icon.png).

   * Los archivos no están marcados con un icono.

1. Haga clic en **Guardar**.


## Información de seguridad, acceso y autorización para la integración de [!DNL SharePoint]

### Autenticación y autorización

[!DNL Workfront] usa OAuth2 para recuperar un token de acceso y un token de actualización. Este token de acceso se usa para la autorización en las áreas [!DNL SharePoint].

### Acceso y permisos

La primera vez que un usuario agrega un documento a [!DNL Workfront] desde [!DNL SharePoint], se le dirige a la página Permisos solicitados, donde puede conceder permisos para su integración con SharePoint.

>[!NOTE]
>
>Según la configuración de Microsoft de la organización, los usuarios pueden ver una página &quot;Se requiere aprobación&quot; en lugar de &quot;Permisos solicitados&quot;. En este caso, los usuarios pueden utilizar esta página para solicitar al administrador de Microsoft de la organización que conceda permisos para la integración con Sharepoint.

Se solicitan los siguientes permisos:

| Acceso | Motivo |
|---|---|
| Tener acceso completo a sus archivos | Permite que [!DNL Workfront] acceda a los archivos de un usuario para vincular recursos. Cuando los documentos se envían de [!DNL Workfront] a [!DNL SharePoint], [!DNL Workfront] requiere acceso para crear el recurso. |
| Leer elementos en todas las colecciones de sitios | Permite que [!DNL Workfront] lea recursos para habilitar la navegación del usuario. |
| Editar o eliminar elementos en todas las colecciones de sitios | Permite que [!DNL Workfront] cree recursos en sitios y colecciones de sitios. Eliminar solo se utiliza cuando se limpia después de intentos de vínculo fallidos. |
| Mantener el acceso a los datos a los que le ha dado acceso | Permite que [!DNL Workfront] genere un token de actualización. |
| Iniciar sesión y leer el perfil de usuario | Permite que [!DNL Workfront] use el token de acceso para actuar en nombre del usuario a través del flujo de inicio de sesión de OAuth2. |

* El usuario concede este acceso la primera vez que utiliza la integración y se puede revocar en cualquier momento.
* Los permisos solicitados para esta integración son **permisos delegados**.
* [!DNL Workfront] solicita el acceso mínimo requerido para realizar operaciones en la integración.
* El acceso para ver, editar o eliminar un documento [!DNL Adobe Workfront] vinculado a [!DNL SharePoint] se basa en el acceso del usuario en [!DNL Workfront]. Sin embargo, la navegación, descarga o edición de un archivo o carpeta de [!DNL SharePoint] requiere acceso a [!DNL SharePoint], y el acceso a estas acciones está controlado por [!DNL SharePoint].
* Los usuarios pueden ver miniaturas y previsualizar imágenes de [!DNL SharePoint], así como ver nombres de archivos y carpetas en [!DNL SharePoint], sin iniciar sesión en [!DNL SharePoint].
* El token de acceso de un usuario solo se usa cuando el usuario está sin conexión y otro usuario ve el contenido de una carpeta vinculada a [!DNL Workfront]. El token de acceso se utiliza para detectar si se han agregado, eliminado o editado documentos en la carpeta.

### Seguridad

Toda la comunicación entre [!DNL Workfront] y [!DNL SharePoint] se realiza a través de HTTPS, que cifra la información.

[!DNL Workfront] no almacena, copia o duplica datos de [!DNL SharePoint]. La única excepción es que [!DNL Workfront] almacena miniaturas de [!DNL SharePoint] para mostrarlas en la vista de lista y en la vista previa.

Si un recurso se cargó primero en [!DNL Workfront] y después se envió a [!DNL SharePoint], [!DNL Workfront] retiene los datos del primer archivo porque los usuarios pueden descargar una versión anterior de un documento [!DNL Workfront]. Si se creó un documento en [!DNL SharePoint], [!DNL Workfront] no almacena esos datos de archivo.

## Configurar la integración heredada de [!DNL SharePoint] para el acceso continuo a los documentos

Para garantizar que los usuarios tengan acceso continuo a los documentos vinculados a Workfront a través de la integración heredada de [!DNL SharePoint], debe volver a configurar el acceso a la integración heredada de [!DNL SharePoint] y mantener actualizado el Secreto de cliente de SharePoint.

* [Volver a configurar el acceso a la integración  [!DNL SharePoint] legacy](#reconfigure-access-to-the-legacy-sharepoint-integration)
* [Configure el Secreto del cliente para el acceso continuo a la integración  [!DNL SharePoint] heredada](#configure-the-client-secret-for-continued-access-to-the-legacy-sharepoint-integration)

### Volver a configurar el acceso a la integración heredada de [!DNL SharePoint]

La reconfiguración de la integración heredada de [!DNL SharePoint] permite a los usuarios acceder a los documentos vinculados a través de la integración heredada de [!DNL SharePoint], al tiempo que se asegura de que los usuarios no puedan vincular nuevos documentos a través de esa integración.

>[!NOTE]
>
> * La integración heredada [!DNL SharePoint] está etiquetada como &quot;[!DNL SharePoint]&quot;.
> * La nueva integración de [!DNL SharePoint] está etiquetada como &quot;[!UICONTROL [!DNL SharePoint] (API de gráficos)]&quot;.

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Configurar]** ![Icono de configuración](/help/_includes/assets/gear-icon-setup.png).
1. Seleccione **[!UICONTROL Documentos]** en el panel de navegación izquierdo y luego seleccione **[!UICONTROL Proveedores de nube]**.
1. Asegúrese de que la opción **[!DNL SharePoint]** y la opción **[!UICONTROL [!DNL SharePoint](API de gráficos)]** estén habilitadas.
1. Haga clic en **[!UICONTROL Guardar]**.
1. Seleccione **[!UICONTROL Documentos]** en el panel de navegación izquierdo, luego seleccione **[!UICONTROL [!DNL SharePoint]Integración]**.
1. Seleccione la marca de verificación de la izquierda de la lista para todas las integraciones existentes y luego seleccione **[!UICONTROL Deshabilitar]**.
   ![](assets/disable-old-sharepoint.png)


### Configure el Secreto de cliente para el acceso continuo a la integración heredada de [!DNL SharePoint]

El secreto de cliente de [!DNL SharePoint] caduca una vez al año. Para garantizar el acceso continuo a los documentos de su integración heredada de [!DNL SharePoint], debe mantener actualizado el secreto de cliente de [!DNL SharePoint].

>[!IMPORTANT]
>
> Dado que [!DNL Microsoft] administra los secretos de cliente de [!DNL SharePoint], las características y los procedimientos de los secretos de cliente pueden cambiar según las actualizaciones de [!DNL SharePoint] realizadas por [!DNL Microsoft]. Consulte siempre la documentación de [!DNL Microsoft] para obtener la información más reciente acerca de los procedimientos y características de [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. Genere un nuevo secreto de cliente como se describe en [Reemplace un secreto de cliente que caduque en un [!DNL SharePoint] complemento](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret).
1. Copie este Secreto del cliente a una ubicación segura.
1. Inicie sesión en [!DNL Workfront] como administrador.
1. En Workfront, haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Configurar]** ![Icono de configuración](/help/_includes/assets/gear-icon-setup.png).
1. En el panel izquierdo, haga clic en **[!UICONTROL Documentos]** > Integración de **[!UICONTROL [!DNL SharePoint]]**.
1. Haga clic en la integración de [!DNL SharePoint] que desee actualizar y luego haga clic en **[!UICONTROL Editar]**.
1. Busque la sección **Información de conexión** en la ventana de edición y, a continuación, escriba el nuevo Secreto de cliente en el campo **[!UICONTROL Secreto de cliente de SharePoint]**.
1. Haga clic en **[!UICONTROL Guardar]**.

<!--

## Instructions for setting up the legacy SharePoint integration

>[!IMPORTANT]
>
>This integration has been deprecated. The instructions here are for information only and will be removed in the near future.


Workfront connects to [!DNL SharePoint] Online using OAuth 2.0, a standard used by most web-based integrations for the authentication and authorization of users.

To configure OAuth, you need to create a [!DNL SharePoint] site and a Site App within [!DNL SharePoint]. This process is described in the following sections.

For more information about OAuth, see [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>To make it easy to copy and paste information between [!DNL Workfront] and [!DNL SharePoint] in these steps, we recommend keeping both applications open in separate tabs.

* [Create and configure a [!DNL SharePoint] site](#create-and-configure-a-sharepoint-site) 
* [Grant write permissions to the site app](#grant-write-permissions-to-the-site-app) 
* [Create a [!DNL Workfront] [!DNL SharePoint] integration instance](#create-a-workfront-sharepoint-integration-instance) 
* [Complete your integration](#complete-your-integration) 
* [Add documents](#add-documents)

### Create and configure a [!DNL SharePoint] site  {#create-and-configure-a-sharepoint-site}

In order for [!DNL Workfront] to authenticate with [!DNL SharePoint], [!DNL Workfront] ca use a master site where users have the [!UICONTROL Full Control] permission level or specific Manage permissions. This master site acts as an Authentication Entry Point for [!DNL Workfront].

To create and configure a [!DNL SharePoint] Site:

1. (Optional) If you do not want to use your organization's root site, you can create a master site in [!DNL SharePoint].

   For instructions, visit [Create a site](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) in the [!DNL Microsoft] Documentation.

   * Select the **[!UICONTROL Team Site]** option when creating the site.

1. (Conditional) If you created a site in step 1, go to the site you just created.

   Or

   If you did not create a site in step 1, go to your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client ID]</p> </td> 
      <td> <p>Click <strong>[!UICONTROL Generate]</strong> to generate a Client ID. Copy this ID to a secure location. You will use it later when you set up the [!DNL SharePoint] integration in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client Secret]</p> </td> 
      <td> <p>Click <strong>[!UICONTROL Generate]</strong> to generate a Client Secret. Copy this Secret to a secure location. You will use it later when you set up the [!DNL SharePoint] integration in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Title</p> </td> 
      <td> <p>Enter a title, such as [!DNL Workfront] Site App. Users see this title when adding documents..</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App Domain]</p> </td> 
      <td> <p><code>my.workfront.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Redirect URI]</p> </td> 
      <td> <p><code>https://oauth.my.workfront.com/oauth2/redirect</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**
1. Continue to [Grant write permissions to the site app](#grant-write-permissions-to-the-site-app).

### Grant write permissions to the site app  {#grant-write-permissions-to-the-site-app}

At this point, you have successfully created a Site App and registered it within [!DNL Workfront]. This site app is also known as an app principal in [!DNL SharePoint]. It resides within your tenant. New site apps do not automatically have access to site collections within the tenant. Permissions must be granted explicitly, for each site collection. The steps below will show you how to grant Write permission to the new Site App a site collection. Repeat these steps for each of the site collections you added under [!UICONTROL Visible Site Collections] in the steps above.

This site app must have [!UICONTROL Write] permission to any site collections that users need to access through [!DNL Workfront].

1. Add '/_layouts/15/appinv.aspx' to the URL in [!DNL Sharepoint].

   **Example:**

   ```
   https://mycompany.sharepoint.com/sites/mysite/_layouts/15/appinv.aspx
   ```

1. Configure the following fields

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL App ID]</td> 
      <td> <p>Add the Client ID that you created in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>and click <strong>[!UICONTROL Lookup]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client] / [!UICONTROL App Domain] / [!UICONTROL Redirect URL]</p> </td> 
      <td> <p>These automatically fill when you click [!UICONTROL Lookup].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Permission Request XML]</td> 
      <td> <p>Copy the following XML to the [!UICONTROL Permission Request XML] field. Make sure that it is added exactly as shown without additional spaces etc. in order to avoid errors.</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre><code><span style="color: #63a35c; ">&lt;AppPermissionRequests&gt;</span><br><span style="color: #63a35c; ">&lt;AppPermissionRequest <span style="color: #795da3; ">Scope</span><span style="color: #df5000; ">="http://sharepoint/content/sitecollection/web"</span> <span style="color: #795da3; ">Right</span><span style="color: #df5000; ">="Write"</span>/&gt;</span><br><span style="color: #63a35c; ">&lt;/AppPermissionRequests&gt;</span></code></pre> 
      </div> 
      </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**. 
1. In the dialog that appears, click **[!UICONTROL Trust it]**.
1. Verify that the site app has access to the site collection by clicking the **[!UICONTROL Site collection app permissions]** link in [!UICONTROL Site Settings].
1. Repeat the steps above for the remaining site collections, then continue with [Create a [!DNL Workfront] [!DNL SharePoint] integration instance](#create-a-workfront-sharepoint-integration-instance).

### Create a [!DNL Workfront] [!DNL SharePoint] integration instance {#create-a-workfront-sharepoint-integration-instance}

When you have created a site app in [!DNL SharePoint], you can now copy information from the site app into [!DNL Workfront]. The site app is an app principal and acts as the conduit through which OAuth requests are made to access documents within site collections.

1. Log into [!DNL Workfront] as an administrator.
1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. In the left panel, click **[!UICONTROL Documents]** > **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Click **[!UICONTROL Add [!DNL SharePoint]]**.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Name]</p> </td> 
      <td> <p>Enter a name for the [!DNL SharePoint] integration. Users see this name when they click [!UICONTROL Add] &gt; [!UICONTROL From] 'name of integration'. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] Host Instance]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] Access Domain]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>This refers to the Master Site that users will use to authenticate through. It is likely the same domain as the [!UICONTROL [!DNL SharePoint] Host Instance].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>Important</b> Site collections are used only in the Legacy [!DNL SharePoint] Integration.
       <ul> 
        <li> <p><b>If you are using your organization's root site</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>If you are using a master site and subsites:</b> </p> <p><b>IMPORTANT</b>: [!DNL Microsoft SharePoint] no longer recommends the use of subsites.</p> <p>Enter the URL stem for the site collection that you created in the section above.</p> <p>This is the section of the URL after .com.</p> <p>Example: for the URL <code>https://mycompany.sharepoint.com/sites/mysite</code>, the stem would be <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client ID]</td> 
      <td>Enter the Client ID that you generated in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client Secret]</td> 
      <td>Enter the Client Secret that you generated in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Visible Site Collections]</td> 
      <td> <b>Important</b> Site collections are used only in the Legacy [!DNL SharePoint] integration.
       <ul> 
        <li> <p><b> If you are using your organization's root site</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>If you are using a master site and subsites:</b> </p> <p><b>IMPORTANT</b>: [!DNL Microsoft SharePoint] no longer recommends the use of subsites.</p> <p>For each subsite you want to add to your [!DNL SharePoint] integration, enter the stem of the subsite.</p> <p>Example: for the URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, the stem would be <code>/sites/mysite/mysubsite</code>.</p> <p><b>NOTE</b>:   <p>If you want to test your configuration only (no subsites), enter the stem of the master site. </p> <p>Example: for the URL <code> https://mycompany.sharepoint.com/sites/mysite</code>, the stem would be <code>/sites/mysite</code>.</p> <p>When you have tested your configuration as described in <a href="#complete-your-integration" class="MCXref xref">Complete your integration</a>, you must remove the master site and enter the subsites.</p> 
          <ol> 
           <li value="1">Click the <strong>[!UICONTROL Main Menu]</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of [!DNL Adobe Workfront], then click <strong>[!UICONTROL Setup]</strong> <img src="assets/gear-icon-settings.png">.<li><p>In the left panel, click <strong>[!UICONTROL Documents]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] Integration]</strong>.</p></li><li><p>Click the [!DNL SharePoint] integration you are setting up, then click Edit.</p></li><li><p>Delete the stem for the master site from the [!UICONTROL Visible Site Collections] field.</p></li><li><p>For each subsite you want to add to your [!DNL SharePoint] integration, enter the stem of the subsite.</p></li><p>Example: for the URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, the stem would be <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Save]**
1. Continue to [Complete your integration](#complete-your-integration).

### Complete your integration {#complete-your-integration}

The basic configuration is almost complete.

1. In Workfront, Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Documents]** ![](assets/document-icon.png).
1. Click **[!UICONTROL Add new]**.
1. Click **[!UICONTROL From] `<title of your [!DNL SharePoint] site>`** in the dropdown.

   A dialog that invites you to Trust this site appears.

   >[!NOTE]
   >
   >If this dialog does not appear, your [!DNL SharePoint] integration is not configured correctly.

1. Click **[!UICONTROL Trust it]**.

### Add documents {#add-documents}

You can now add documents from your [!DNL SharePoint] site.

For instructions, see [Link an external document to [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in [Link documents from external applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>If the user who linked a folder no longer has access to the external application, [!DNL Workfront] can no longer access the contents of the folder. This may happen, for example, if the user who originally linked the folder leaves the company. To ensure continued access, a user with access to the folder must re-link the folder.
> 

-->

## Resolución de problemas

* [Problema: los usuarios experimentan errores basados en autenticación al usar la integración de  [!DNL SharePoint] xdm.](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [Problema: al intentar examinar [!DNL SharePoint] archivos en [!DNL Workfront], no veo ninguna o todas las colecciones de sitios.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [Problema: no puedo obtener acceso a carpetas y documentos vinculados anteriormente en  [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### Problema: Los usuarios experimentan errores basados en la autenticación al utilizar la integración de [!DNL SharePoint]. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

Soluciones:

Los usuarios deben tener los permisos adecuados para el sitio [!DNL SharePoint].

Los usuarios con acceso de [!UICONTROL Control total] tienen todos los permisos necesarios para la integración de [!DNL SharePoint]. Si no desea conceder acceso de Control total a los usuarios, debe conceder los siguientes permisos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Diseño]</p> </td> 
   <td> <p>Pueden ver, agregar, actualizar, eliminar, aprobar y personalizar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Editar]</p> </td> 
   <td> <p>Puede agregar, editar y eliminar listas; puede ver, agregar, actualizar y eliminar elementos y documentos de la lista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contribute]</p> </td> 
   <td> <p>Puede ver, agregar, actualizar y eliminar elementos y documentos de la lista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Solo vista]</p> </td> 
   <td> <p>Puede ver páginas, elementos de lista y documentos (los tipos de documento con controladores de archivos del lado del servidor se pueden ver en el explorador, pero no descargar)</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener instrucciones sobre cómo crear y editar niveles de permisos, consulte [Cómo crear y editar niveles de permisos](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels) en la documentación de Microsoft.

<!--

### Problem: As a [!DNL Workfront] user, I am unable to provision a new [!DNL SharePoint] instance. When I attempt to do I see an error. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Solutions:

This can be caused by a number of things, originating in either [!DNL Workfront] or [!DNL SharePoint]'s configuration. Verify that:

* The Client ID, Client Secret, return URL and other configuration fields are correctly mapped between the [!DNL Workfront] [!DNL SharePoint] Integration instance and the [!DNL SharePoint] Site App.
* The user has [!UICONTROL Full Control] permission to the Site Collection used for authentication.
* The Site App is listed under [!UICONTROL Site App Permissions] for the [!UICONTROL Site Collection] used for authentication.

-->

### Problema: Al intentar examinar [!DNL SharePoint] archivos en [!DNL Workfront], no veo ninguna o todas las colecciones de sitios. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

Soluciones:

Para ver una colección de sitios en [!DNL Workfront], se deben cumplir las siguientes condiciones:

<!--

* The site collection must be registered in the [!DNL Workfront] [!DNL SharePoint] Integration instance.

  To verify this in [!DNL Workfront]:

   1. Go to [!UICONTROL Setup] > [!UICONTROL Documents] > [!UICONTROL [!DNL SharePoint] Integration].
   1. Edit the [!DNL SharePoint] Integration instance information.
   1. Verify that the site collection is listed under [!UICONTROL Visible Site Collections].
   -->

* El usuario debe tener acceso de visualización a la colección de sitios en [!DNL SharePoint].

  Para comprobar esto en [!DNL SharePoint], compruebe los permisos de la colección de sitios en SharePoint.

<!--* The [!DNL SharePoint] Site App must have access to the site collection.

  To verify this in [!DNL SharePoint]:

   1. Go to the site collection > [!UICONTROL Settings] > [!UICONTROL Site app permissions].
   1. Ensure that the [!UICONTROL Site App] used by [!DNL Workfront] is listed here.
   1. (Conditional) If the Site App is not listed, add to the site collection using _layouts/15/appinv.aspx.

      For information about adding the site collection, see Granting Write Permissions To The Site App.
      
-->

### Problema: No puedo obtener acceso a carpetas y documentos enlazados anteriormente en [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

Solución:

Si el usuario que vinculó una carpeta [!DNL SharePoint] ya no puede autenticarse, [!DNL Workfront] ya no puede obtener acceso al contenido de la carpeta. Esto puede suceder, por ejemplo, si el usuario que vinculó originalmente la carpeta abandona la compañía.

Para garantizar el acceso continuo, un usuario con acceso a la carpeta debe volver a vincular la carpeta.

Para obtener información sobre cómo vincular carpetas desde proveedores externos, consulte [Vincular documentos desde aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<!--

### Problem: I see a "404 not found" error when attempting to add a document from [!DNL Sharepoint]

#### Solution:

This error might occur if one of the sites configured in the [!UICONTROL Visible Site Collections] list has been deleted in Sharepoint. Check the [!UICONTROL Visible Site Collections] list, and remove any sites that have been deleted in Sharepoint.-->