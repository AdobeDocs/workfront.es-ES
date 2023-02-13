---
title: Configure las variables [!DNL SharePoint] integración
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Puede integrar [!DNL Workfront] con [!DNL SharePoint] En línea, lo que permite a los usuarios navegar, vincular y agregar [!DNL SharePoint] documentos en Workfront. La funcionalidad proporcionada es similar a la de otros [!DNL Workfront] integraciones como Google Drive, Box y Dropbox.
author: Becky, Caroline
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: 5292069412a73f824dbcd967d47737cff5ef58fa
workflow-type: tm+mt
source-wordcount: '2515'
ht-degree: 0%

---

# Configurar el heredado [!DNL SharePoint] integración

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>El nuevo [!DNL SharePoint] con la versión 22.3 (julio de 2022). Aunque los usuarios aún pueden acceder a los documentos vinculados a través del archivo heredado [!DNL SharePoint] integraciones, deben utilizar el nuevo [!DNL SharePoint] para vincular documentos de SharePoint.
>
>* La nueva integración de SharePoint no requiere la configuración de ningún administrador y la pueden configurar usuarios individuales. Sin embargo, para garantizar una transición sin problemas a la nueva integración de SharePoint, un administrador de Workfront debe realizar algunos cambios pequeños en la configuración del área de configuración de Workfront.
   >
   >    Para obtener información e instrucciones, consulte [Configurar la integración heredada de SharePoint para el acceso continuo a los documentos](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents) en este artículo.
>    
>* Recomendamos que los usuarios vinculen documentos que estén actualmente vinculados a través del heredado [!DNL SharePoint] a través de la nueva integración.
   >    
   >    Para obtener instrucciones sobre cómo vincular documentos, consulte [Vincular documentos de aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).


Puede integrar [!DNL Workfront] con [!DNL SharePoint Online], lo que permite a los usuarios navegar, vincular y agregar [!DNL SharePoint] documentos en Workfront. La funcionalidad proporcionada es similar a la de otros [!DNL Workfront] integraciones como [!DNL Google Drive], [!DNL Box]y [!DNL Dropbox].

Esta integración solo es compatible con [!DNL SharePoint Online]. Instancias locales de [!DNL SharePoint] no son compatibles.

## Requisitos de acceso

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser [!DNL Workfront] administrador. Para obtener información sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Requisitos previos

Debe tener los accesos o permisos necesarios en [!DNL SharePoint] para modificar o configurar el [!DNL SharePoint].

## Vincular documentos a través de la nueva integración con SharePoint

Los usuarios individuales pueden vincular documentos a través del nuevo [!DNL SharePoint] integración. La integración no requiere configuración de administrador. En su lugar, el usuario inicia sesión en su [!DNL Microsoft] cuando se vincula un documento, lo que permite que la integración acceda a los documentos disponibles en el [!DNL SharePoint].

La primera vez que un usuario conecta la variable [!DNL Workfront] [!DNL SharePoint] integración a sus [!DNL SharePoint] , verán y aceptarán todos los permisos que [!DNL Workfront] cuando interactúa con sus [!UICONTROL SharePoint] cuenta. Permiso de permisos de lectura [!DNL Workfront] para ver y acceder a archivos en [!DNL SharePoint]y los permisos de escritura permiten al usuario cargar archivos en [!DNL SharePoint].

Para obtener instrucciones sobre cómo vincular documentos a través del nuevo [!DNL SharePoint] integración, consulte [Vincular un documento externo a [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* A [!DNL SharePoint] la integración puede conectarse a un [!DNL SharePoint] instancia. Por lo tanto, un usuario puede configurar una integración para uno [!DNL SharePoint], pero no puede configurar una integración en un segundo [!DNL SharePoint], incluso si tienen permisos y documentos en la segunda [!DNL SharePoint].
>
>* Un usuario tiene acceso a los mismos sitios, colecciones, carpetas, subcarpetas y archivos a través de la variable [!DNL Workfront] [!DNL SharePoint] integración tal como tienen en su [!DNL SharePoint] cuenta.


## Configurar la integración heredada de SharePoint para el acceso continuo a los documentos

Para garantizar que los usuarios tengan acceso continuado a los documentos vinculados a Workfront mediante la integración heredada de SharePoint, debe volver a configurar el acceso a la integración heredada de SharePoint y mantener el Secreto de cliente de SharePoint actualizado.

* [Volver a configurar el acceso al heredado [!DNL SharePoint] integración](#reconfigure-access-to-the-legacy-dnl-sharepoint-integration)
* [Configuración del secreto del cliente para continuar con el acceso al heredado [!DNL SharePoint] integración](#configure-the-client-secret-for-continued-access-to-the-legacy-dnl-sharepoint-integration)

### Volver a configurar el acceso al heredado [!DNL SharePoint] integración

Para asegurarse de que puede acceder a los documentos vinculados a través del archivo heredado [!DNL SharePoint] , a la vez que se garantiza que los usuarios no puedan vincular nuevos documentos a través de esa integración, complete el siguiente procedimiento.

>[!NOTE]
>
> * El legado [!DNL SharePoint] la integración está etiquetada como &quot;[!DNL SharePoint].&quot;
> * El nuevo [!DNL SharePoint] la integración está etiquetada como &quot;[!UICONTROL [!DNL SharePoint] (API de gráfico)].&quot;


1. Haga clic en el **[!UICONTROL Menú principal]** icono ![Menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **[!UICONTROL Configuración]** ![Configuración](../get-started-wf-administration/assets/gear-icon-settings.png).
1. Select **[!UICONTROL Documentos]** en el panel de navegación izquierdo, seleccione **[!UICONTROL Proveedores de nube]**.
1. Asegúrese de que la variable **[!DNL SharePoint]** y **[!UICONTROL [!DNL SharePoint](API de gráfico)]** están activadas.
1. Haga clic en **[!UICONTROL Guardar]**.
1. Select **[!UICONTROL Documentos]** en el panel de navegación izquierdo, seleccione **[!UICONTROL [!DNL SharePoint]Integración]**.
1. Seleccione la marca de verificación de la izquierda de la lista para todas las integraciones existentes y, a continuación, seleccione **[!UICONTROL Deshabilitar]**.


### Configuración del secreto del cliente para continuar con el acceso al heredado [!DNL SharePoint] integración

Su [!DNL SharePoint] El Secreto del cliente caduca una vez al año. Para garantizar un acceso continuado a los documentos de su legado [!DNL SharePoint] integración, debe mantener su [!DNL SharePoint] Secreto del cliente actualizado.

>[!IMPORTANT]
>
> Porque [!DNL SharePoint] Los secretos del cliente los gestiona [!DNL Microsoft], las características y los procedimientos del Secreto del cliente pueden cambiar según las actualizaciones a [!DNL SharePoint] hecho por [!DNL Microsoft]. Compruebe siempre la [!DNL Microsoft] documentación para obtener la información más reciente sobre procedimientos y características de [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. Genere un nuevo secreto de cliente como se describe en [Reemplazar un secreto de cliente caducado en un [!DNL SharePoint] Complemento](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret)
1. Copie este Secreto del cliente en una ubicación segura.
1. Iniciar sesión [!DNL Workfront] como administrador.
1. En Workfront, haga clic en el botón **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).
1. En el panel izquierdo, haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL [!DNL SharePoint]Integración]**.
1. Haga clic en el [!DNL SharePoint] integración que desea actualizar y, a continuación, haga clic en **[!UICONTROL Editar]**.
1. Introduzca el nuevo Secreto de cliente en la **[!UICONTROL Secreto del cliente]** campo .
1. Haga clic en **[!UICONTROL Guardar]**.



## Instrucciones para configurar la integración heredada de SharePoint

>[!IMPORTANT]
>
>Esta integración ha quedado obsoleta. Las instrucciones aquí son sólo para información y serán eliminadas en un futuro próximo.


Workfront se conecta a [!DNL SharePoint] En línea con OAuth 2.0, un estándar utilizado por la mayoría de las integraciones basadas en web para la autenticación y autorización de los usuarios.

Para configurar OAuth, debe crear un [!DNL SharePoint] sitio y aplicación de sitio dentro de [!DNL SharePoint]. Este proceso se describe en las secciones siguientes.

Para obtener más información sobre OAuth, consulte [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>Para facilitar la copia y pegado de información entre [!DNL Workfront] y [!DNL SharePoint] en estos pasos, se recomienda mantener ambas aplicaciones abiertas en pestañas independientes.

* [Cree y configure un [!DNL SharePoint] site](#create-and-configure-a-sharepoint-site)
* [Conceder permisos de escritura a la aplicación del sitio](#grant-write-permissions-to-the-site-app)
* [Cree un [!DNL Workfront] [!DNL SharePoint] instancia de integración](#create-a-workfront-sharepoint-integration-instance)
* [Completar la integración](#complete-your-integration)
* [Agregar documentos](#add-documents)

### Cree y configure un [!DNL SharePoint] site  {#create-and-configure-a-sharepoint-site}

Para [!DNL Workfront] para autenticarse con [!DNL SharePoint], [!DNL Workfront] puede utilizar un sitio maestro en el que los usuarios tengan la variable [!UICONTROL Control total] nivel de permiso o permisos específicos de administración. Esta ubicación maestra actúa como punto de entrada de autenticación para [!DNL Workfront].

Para crear y configurar un [!DNL SharePoint] Sitio:

1. (Opcional) Si no desea utilizar el sitio raíz de su organización, puede crear un sitio principal en [!DNL SharePoint].

   Para obtener instrucciones, visite [Crear un sitio](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) en el [!DNL Microsoft] Documentación.

   * Seleccione el **[!UICONTROL Sitio del equipo]** al crear el sitio.

1. (Condicional) Si creó un sitio en el paso 1, vaya al sitio que acaba de crear.

   O

   Si no creó un sitio en el paso 1, vaya al sitio raíz de su organización.

1. Agregar `/_layouts/15/appregnew.aspx` al final de la dirección URL en la barra de búsqueda de la parte superior de la ventana del explorador.
1. Configure los campos siguientes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client ID]</p> </td> 
      <td> <p>Haga clic en <strong>[!UICONTROL Generate]</strong> para generar un ID de cliente. Copie este ID en una ubicación segura. Lo utilizará más adelante al configurar la variable [!DNL SharePoint] integración en [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client Secret]</p> </td> 
      <td> <p>Haga clic en <strong>[!UICONTROL Generate]</strong> para generar un secreto de cliente. Copie este Secreto en una ubicación segura. Lo utilizará más adelante al configurar la variable [!DNL SharePoint] integración en [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Título</p> </td> 
      <td> <p>Introduzca un título, como [!DNL Workfront] Aplicación del sitio. Los usuarios ven este título al agregar documentos.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App Domain]</p> </td> 
      <td> <p><code>my.workfront.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL URI de redirección]</p> </td> 
      <td> <p><code>https://oauth.my.workfront.com/oauth2/redirect</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Crear]**
1. Continúe con [Conceder permisos de escritura a la aplicación del sitio](#grant-write-permissions-to-the-site-app).

### Conceder permisos de escritura a la aplicación del sitio  {#grant-write-permissions-to-the-site-app}

En este punto, ha creado correctamente una aplicación del sitio y la ha registrado en [!DNL Workfront]. Esta aplicación de sitio también se conoce como entidad de seguridad de aplicación en [!DNL SharePoint]. Se encuentra dentro del inquilino. Las nuevas aplicaciones de sitio no tienen acceso automático a las colecciones de sitios dentro del inquilino. Los permisos deben otorgarse explícitamente para cada colección de sitios. Los pasos siguientes le mostrarán cómo conceder permiso de escritura a la nueva aplicación del sitio en una colección de sitios. Repita estos pasos para cada una de las colecciones de sitios agregadas en [!UICONTROL Colecciones visibles del sitio] en los pasos anteriores.

Esta aplicación de sitio debe tener [!UICONTROL Escritura] permiso para cualquier colección de sitios a la que los usuarios tengan acceso mediante [!DNL Workfront].

1. Añada &#39;/_layouts/15/appinv.aspx&#39; a la dirección URL en [!DNL Sharepoint].

   **Ejemplo:**

   ```
   https://mycompany.sharepoint.com/sites/mysite/_layouts/15/appinv.aspx
   ```

1. Configure los campos siguientes

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL App ID]</td> 
      <td> <p>Añadir el ID de cliente que ha creado en <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Cree y configure un [!DNL SharePoint] site </a>y haga clic en <strong>[!UICONTROL Buscar]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client] / [!UICONTROL App Domain] / [!UICONTROL Redirect URL]</p> </td> 
      <td> <p>Se rellenan automáticamente al hacer clic en [!UICONTROL Buscar].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Solicitud de permiso XML]</td> 
      <td> <p>Copie el siguiente XML al campo [!UICONTROL Permission Request XML]. Asegúrese de que se añada exactamente como se muestra sin espacios adicionales, etc. para evitar errores.</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre></pre></div></div></td></tr></tbody></table>

1. Haga clic en **[!UICONTROL Crear]**.
1. En el cuadro de diálogo que aparece, haga clic en **[!UICONTROL Confiar en ella]**.
1. Compruebe que la aplicación del sitio tiene acceso a la colección de sitios haciendo clic en el botón **[!UICONTROL Permisos de la aplicación de recopilación de sitios]** vincular en [!UICONTROL Configuración del sitio].
1. Repita los pasos anteriores para las colecciones de sitios restantes y, a continuación, continúe con [Cree un [!DNL Workfront] [!DNL SharePoint] instancia de integración](#create-a-workfront-sharepoint-integration-instance).

### Cree un [!DNL Workfront] [!DNL SharePoint] instancia de integración {#create-a-workfront-sharepoint-integration-instance}

Cuando haya creado una aplicación de sitio en [!DNL SharePoint], ahora puede copiar información de la aplicación del sitio en [!DNL Workfront]. La aplicación del sitio es una entidad de seguridad de la aplicación y actúa como el conducto a través del cual se realizan las solicitudes de OAuth para acceder a los documentos dentro de las colecciones del sitio.

1. Iniciar sesión [!DNL Workfront] como administrador.
1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL [!DNL SharePoint]Integración]**.
1. Haga clic en **[!UICONTROL Agregar[!DNL SharePoint]]**.
1. Configure los campos siguientes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Name]</p> </td> 
      <td> <p>Escriba un nombre para la variable [!DNL SharePoint] integración. Los usuarios ven este nombre cuando hacen clic en [!UICONTROL Agregar] &gt; [!UICONTROL Desde] "nombre de integración". </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] Instancia de host]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] Dominio de acceso]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>Esto hace referencia al sitio maestro que los usuarios utilizarán para autenticarse. Es probable que el mismo dominio que el [!UICONTROL [!DNL SharePoint] Instancia de host].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>Importante</b> Las colecciones de sitios solo se utilizan en la [!DNL SharePoint] Integración.
       <ul> 
        <li> <p><b>Si utiliza el sitio raíz de su organización</b><b>:</b> </p> <p>Entrar <code>/</code></p> </li> 
        <li> <p><b>Si está utilizando una ubicación maestra y subsitios:</b> </p> <p><b>IMPORTANTE</b>: [!DNL Microsoft SharePoint] ya no recomienda el uso de subsitios.</p> <p>Introduzca el sistema de URL para la colección de sitios que ha creado en la sección anterior.</p> <p>Esta es la sección de la dirección URL después de .com.</p> <p>Ejemplo: para la dirección URL <code>https://mycompany.sharepoint.com/sites/mysite</code>, el tallo sería <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] ID del cliente]</td> 
      <td>Introduzca el ID de cliente que ha generado en <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Cree y configure un [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Secreto del cliente]</td> 
      <td>Introduzca el Secreto de cliente que ha generado en <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Cree y configure un [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Colecciones de sitios visibles]</td> 
      <td> <b>Importante</b> Las colecciones de sitios solo se utilizan en la [!DNL SharePoint] integración.
       <ul> 
        <li> <p><b> Si utiliza el sitio raíz de su organización</b><b>:</b> </p> <p>Entrar <code>/</code></p> </li> 
        <li> <p><b>Si está utilizando una ubicación maestra y subsitios:</b> </p> <p><b>IMPORTANTE</b>: [!DNL Microsoft SharePoint] ya no recomienda el uso de subsitios.</p> <p>Para cada subsitio que desee agregar a su [!DNL SharePoint] , introduzca la raíz del subsitio.</p> <p>Ejemplo: para la dirección URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, el tallo sería <code>/sites/mysite/mysubsite</code>.</p> <p><b>NOTA</b>:   <p>Si solo desea probar la configuración (sin subsitios), introduzca el tallo de la ubicación maestra. </p> <p>Ejemplo: para la dirección URL <code> https://mycompany.sharepoint.com/sites/mysite</code>, el tallo sería <code>/sites/mysite</code>.</p> <p>Cuando haya probado su configuración como se describe en <a href="#complete-your-integration" class="MCXref xref">Completar la integración</a>, debe quitar la ubicación maestra e introducir los subsitios.</p> 
          <ol> 
           <li value="1">Haga clic en el <strong>[!UICONTROL Menú Principal]</strong> icono <img src="assets/main-menu-icon.png"> en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en <strong>[!UICONTROL Setup]</strong> <img src="assets/gear-icon-settings.png">.<li><p>En el panel izquierdo, haga clic en <strong>[!UICONTROL Documents]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] Integración]</strong>.</p></li><li><p>Haga clic en el [!DNL SharePoint] integración que está configurando y, a continuación, haga clic en Editar.</p></li><li><p>Elimine la raíz de la ubicación maestra del campo [!UICONTROL Colecciones de sitio visibles].</p></li><li><p>Para cada subsitio que desee agregar a su [!DNL SharePoint] , introduzca la raíz del subsitio.</p></li><p>Ejemplo: para la dirección URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, el tallo sería <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Guardar]**
1. Continúe con [Completar la integración](#complete-your-integration).

### Completar la integración {#complete-your-integration}

La configuración básica está casi completa.

1. En Workfront, haga clic en el botón **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **[!UICONTROL Documentos]** ![](assets/document-icon.png).
1. Haga clic en **[!UICONTROL Agregar nuevo]**.
1. Haga clic en **[!UICONTROL De]`<title of your [!DNL SharePoint] site>`** en la lista desplegable .

   Aparece un cuadro de diálogo que le invita a confiar en este sitio.

   >[!NOTE]
   >
   >Si este cuadro de diálogo no aparece, su [!DNL SharePoint] la integración no está configurada correctamente.

1. Haga clic en **[!UICONTROL Confiar en ella]**.

### Agregar documentos {#add-documents}

Ahora puede agregar documentos desde su [!DNL SharePoint] sitio.

Para obtener instrucciones, consulte [Vincular un documento externo a [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) en [Vincular documentos de aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>Si el usuario que vinculó una carpeta ya no tiene acceso a la aplicación externa, [!DNL Workfront] ya no puede acceder al contenido de la carpeta. Esto puede suceder, por ejemplo, si el usuario que vinculó originalmente la carpeta abandona la empresa. Para garantizar un acceso continuado, un usuario con acceso a la carpeta debe volver a vincular la carpeta.

## Resolución de problemas

* [Problema: Los usuarios experimentan errores basados en la autenticación al usar la variable [!DNL SharePoint] integración.](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [Problema: Como [!DNL Workfront] usuario, no puedo aprovisionar un nuevo [!DNL SharePoint] instancia. Cuando intento hacerlo, veo un error.](#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error)
* [Problema: Cuando se intenta examinar [!DNL SharePoint] archivos en [!DNL Workfront], no veo ninguna o todas mis colecciones de sitios.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [Problema: No puedo acceder a carpetas y documentos previamente vinculados en [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### Problema: Los usuarios experimentan errores basados en la autenticación al usar la variable [!DNL SharePoint] integración. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

Soluciones:

Los usuarios deben ser miembros de un grupo que tenga los permisos adecuados para el [!DNL SharePoint] sitio.

Usuarios con [!UICONTROL Control total] tiene todos los permisos necesarios para su [!DNL SharePoint] integración. Si no desea conceder acceso de Control total a los usuarios, debe otorgar los siguientes permisos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Design]</p> </td> 
   <td> <p>Pueden ver, agregar, actualizar, eliminar, aprobar y personalizar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Editar]</p> </td> 
   <td> <p>Puede agregar, editar y eliminar listas; puede ver, agregar, actualizar y eliminar elementos y documentos de lista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contribute]</p> </td> 
   <td> <p>Puede ver, agregar, actualizar y eliminar elementos y documentos de lista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Ver solamente]</p> </td> 
   <td> <p>Pueden ver páginas, elementos de lista y documentos (los tipos de documentos con controladores de archivos del lado del servidor se pueden ver en el explorador, pero no descargar)</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener instrucciones sobre la creación y edición de niveles de permisos, consulte [Creación y edición de niveles de permisos](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels) en la documentación de Microsoft.

### Problema: Como [!DNL Workfront] usuario, no puedo aprovisionar un nuevo [!DNL SharePoint] instancia. Cuando intento hacerlo, veo un error. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Soluciones:

Esto puede deberse a una serie de cosas, originadas en [!DNL Workfront] o [!DNL SharePoint]la configuración de . Compruebe que:

* El ID del cliente, el Secreto del cliente, la URL de retorno y otros campos de configuración se asignan correctamente entre los campos [!DNL Workfront] [!DNL SharePoint] La instancia de integración y el [!DNL SharePoint] Aplicación del sitio.
* El usuario tiene [!UICONTROL Control total] permiso para acceder a la colección de sitios que se utiliza para la autenticación.
* La aplicación del sitio aparece en [!UICONTROL Permisos de la aplicación del sitio] para el [!UICONTROL Colección de sitios] se utiliza para la autenticación.

### Problema: Cuando se intenta examinar [!DNL SharePoint] archivos en [!DNL Workfront], no veo ninguna o todas mis colecciones de sitios. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

Soluciones:

Para ver una colección de sitios en [!DNL Workfront], deben cumplirse las siguientes condiciones:

* La colección de sitios debe estar registrada en el [!DNL Workfront] [!DNL SharePoint] Instancia de integración.

   Para verificarlo en [!DNL Workfront]:

   1. Vaya a [!UICONTROL Configuración] > [!UICONTROL Documentos] > [!UICONTROL [!DNL SharePoint] Integración].
   1. Edite el [!DNL SharePoint] Información de la instancia de integración.
   1. Compruebe que la colección de sitios está incluida en [!UICONTROL Colecciones visibles del sitio].

* El usuario debe tener acceso de vista a la colección de sitios de [!DNL SharePoint].
* Para verificarlo en [!DNL SharePoint], vaya a [!DNL SharePoint]y abra la colección de sitios > [!UICONTROL Configuración] > [!UICONTROL Permisos del sitio].
* La variable [!DNL SharePoint] La aplicación del sitio debe tener acceso a la colección de sitios.

   Para verificarlo en [!DNL SharePoint]:

   1. Vaya a la colección de sitios > [!UICONTROL Configuración] > [!UICONTROL Permisos de las aplicaciones del sitio].
   1. Asegúrese de que la variable [!UICONTROL Aplicación del sitio] usado por [!DNL Workfront] aparece aquí.
   1. (Condicional) Si la aplicación del sitio no aparece en la lista, agregue a la colección de sitios mediante _layouts/15/appinv.aspx.

      Para obtener información sobre cómo agregar la colección de sitios, consulte Concesión de permisos de escritura a la aplicación del sitio.

### Problema: No puedo acceder a carpetas y documentos previamente vinculados en [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

Solución:

Si el usuario que vinculó un [!DNL SharePoint] carpeta ya no puede autenticarse, [!DNL Workfront] ya no puede acceder al contenido de la carpeta. Esto puede suceder, por ejemplo, si el usuario que vinculó originalmente la carpeta abandona la empresa.

Para garantizar un acceso continuado, un usuario con acceso a la carpeta debe volver a vincular la carpeta.

Para obtener información sobre cómo vincular carpetas de proveedores externos, consulte [Vincular documentos de aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Problema: Veo un error &quot;404 no encontrado&quot; al intentar agregar un documento desde [!DNL Sharepoint]

#### Solución:

Este error puede producirse si uno de los sitios configurados en la variable [!UICONTROL Colecciones visibles del sitio] La lista se ha eliminado en Sharepoint. Marque la [!UICONTROL Colecciones visibles del sitio] y elimine los sitios que se hayan eliminado en Sharepoint.
