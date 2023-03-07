---
title: Configure las variables [!DNL SharePoint] integración
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Se puede integrar [!DNL Workfront] con [!DNL SharePoint] En línea, lo que permite a los usuarios navegar, vincular y agregar elementos [!DNL SharePoint] documentos en Workfront. La funcionalidad proporcionada es similar a la de otros [!DNL Workfront] integraciones, como Google Drive, Box y Dropbox.
author: Becky, Caroline
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: 15aa025c9a35e30867f942047ec1989fdd6834e5
workflow-type: tm+mt
source-wordcount: '2517'
ht-degree: 0%

---

# Configuración del heredado [!DNL SharePoint] integración

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>El nuevo [!DNL SharePoint] La integración de se lanzó al entorno de producción con la versión 22.3 de (julio de 2022). Aunque los usuarios aún pueden acceder a los documentos vinculados a través del heredado [!DNL SharePoint] integración, deben utilizar el nuevo [!DNL SharePoint] integración para vincular documentos desde SharePoint.
>
>* La nueva integración de SharePoint no requiere configuración por parte de un administrador y puede ser configurada por usuarios individuales. Sin embargo, para garantizar una transición sin problemas a la nueva integración de SharePoint, un administrador de Workfront debe realizar algunos pequeños cambios en la configuración del área Configuración de Workfront.
   >
   >    Para obtener información e instrucciones, consulte [Configuración de la integración heredada de SharePoint para el acceso continuo a documentos](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents) en este artículo.
>    
>* Se recomienda que los usuarios vinculen los documentos que actualmente están vinculados a través del heredado [!DNL SharePoint] mediante la nueva integración.
   >    
   >    Para obtener instrucciones sobre cómo vincular documentos, consulte [Vinculación de documentos desde aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).


Se puede integrar [!DNL Workfront] con [!DNL SharePoint Online], que permite a los usuarios navegar, vincular y agregar elementos [!DNL SharePoint] documentos en Workfront. La funcionalidad proporcionada es similar a la de otros [!DNL Workfront] integraciones, como [!DNL Google Drive], [!DNL Box], y [!DNL Dropbox].

Esta integración solo es compatible con [!DNL SharePoint Online]. Instancias on-premise de [!DNL SharePoint] no son compatibles.

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
   <td> <p>Debe ser un [!DNL Workfront] administrador. Para obtener información sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Requisitos previos

Debe tener los accesos o permisos necesarios en [!DNL SharePoint] para modificar o configurar el [!DNL SharePoint].

## Vinculación de documentos con la nueva integración de SharePoint

Los usuarios individuales pueden vincular documentos a través del nuevo [!DNL SharePoint] integración. La integración no requiere la configuración del administrador. En su lugar, el usuario inicia sesión en su [!DNL Microsoft] al vincular un documento, lo que permite a la integración acceder a los documentos disponibles en el [!DNL SharePoint].

La primera vez que un usuario conecta el [!DNL Workfront] [!DNL SharePoint] integración a sus [!DNL SharePoint] cuenta de, verán y aceptarán todos los permisos que [!DNL Workfront] utiliza al interactuar con su [!UICONTROL SharePoint] cuenta. Permisos de lectura permitidos [!DNL Workfront] para ver y acceder a archivos en [!DNL SharePoint], y los permisos de escritura permiten al usuario cargar archivos en [!DNL SharePoint].

![Permisos de Sharepoint](assets/sharepoint-permissions.png)

Para obtener instrucciones sobre cómo vincular documentos a través del nuevo [!DNL SharePoint] integración, consulte [Vincular un documento externo a [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* A [!DNL SharePoint] La integración de puede conectarse a un único [!DNL SharePoint] ejemplo. Por lo tanto, un usuario puede configurar una integración para uno [!DNL SharePoint], pero no puede configurar una integración en un segundo [!DNL SharePoint], incluso si tienen permisos de y documentos en el segundo [!DNL SharePoint].
>
>* Un usuario tiene acceso a los mismos sitios, colecciones, carpetas, subcarpetas y archivos a través del [!DNL Workfront] [!DNL SharePoint] integración, tal como lo hacen en su [!DNL SharePoint] cuenta.


## Configuración de la integración heredada de SharePoint para el acceso continuo a documentos

Para garantizar que los usuarios tengan acceso continuo a los documentos vinculados a Workfront a través de la integración heredada de SharePoint, debe volver a configurar el acceso a la integración heredada de SharePoint y mantener actualizado el Secreto del cliente de SharePoint.

* [Volver a configurar el acceso al heredado [!DNL SharePoint] integración](#reconfigure-access-to-the-legacy-dnl-sharepoint-integration)
* [Configure el Secreto del cliente para acceder de forma continua al heredado [!DNL SharePoint] integración](#configure-the-client-secret-for-continued-access-to-the-legacy-dnl-sharepoint-integration)

### Volver a configurar el acceso al heredado [!DNL SharePoint] integración

Para asegurarse de que puede acceder a los documentos vinculados a través del heredado [!DNL SharePoint] integración, asegurándose de que los usuarios no puedan vincular nuevos documentos a través de esa integración, complete el siguiente procedimiento.

>[!NOTE]
>
> * El legado [!DNL SharePoint] La integración de se denomina &quot;[!DNL SharePoint].&quot;
> * El nuevo [!DNL SharePoint] La integración de se denomina &quot;[!UICONTROL [!DNL SharePoint] (API de gráficos)].&quot;


1. Haga clic en **[!UICONTROL Menú principal]** icono ![Menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **[!UICONTROL Configurar]** ![Configurar](../get-started-wf-administration/assets/gear-icon-settings.png).
1. Seleccionar **[!UICONTROL Documentos]** en el panel de navegación izquierdo, seleccione **[!UICONTROL Proveedores de nube]**.
1. Asegúrese de que la variable **[!DNL SharePoint]** opción y **[!UICONTROL [!DNL SharePoint](API de gráficos)]** están habilitadas.
1. Haga clic en **[!UICONTROL Guardar]**.
1. Seleccionar **[!UICONTROL Documentos]** en el panel de navegación izquierdo, seleccione **[!UICONTROL [!DNL SharePoint]Integración]**.
1. Seleccione la marca de la izquierda de la lista para todas las integraciones existentes y, a continuación, seleccione **[!UICONTROL Deshabilitar]**.


### Configure el Secreto del cliente para acceder de forma continua al heredado [!DNL SharePoint] integración

Su [!DNL SharePoint] El secreto del cliente caduca una vez al año. Para garantizar el acceso continuo a los documentos de su heredado [!DNL SharePoint] integración, debe mantener su [!DNL SharePoint] Secreto del cliente actualizado.

>[!IMPORTANT]
>
> Porque [!DNL SharePoint] Los secretos del cliente los gestiona [!DNL Microsoft], las funciones y procedimientos de Secreto del cliente pueden cambiar según las actualizaciones de [!DNL SharePoint] realizado por [!DNL Microsoft]. Compruebe siempre la [!DNL Microsoft] para obtener la información más reciente acerca de los procedimientos y las funciones de [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. Genere un nuevo secreto de cliente como se describe en [Reemplazar un secreto de cliente expirado en una [!DNL SharePoint] Complemento de](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret)
1. Copie este Secreto del cliente a una ubicación segura.
1. Iniciar sesión en [!DNL Workfront] como administrador.
1. En Workfront, haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).
1. En el panel izquierdo, haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL [!DNL SharePoint]Integración]**.
1. Haga clic en [!DNL SharePoint] integración que desea actualizar y haga clic en **[!UICONTROL Editar]**.
1. Introduzca el nuevo Secreto de cliente en la **[!UICONTROL Secreto del cliente]** field.
1. Haga clic en **[!UICONTROL Guardar]**.



## Instrucciones para configurar la integración heredada de SharePoint

>[!IMPORTANT]
>
>Esta integración ha quedado obsoleta. Las instrucciones aquí son solo para información y se eliminarán en un futuro próximo.


Workfront se conecta a [!DNL SharePoint] En línea, se utiliza OAuth 2.0, un estándar utilizado por la mayoría de las integraciones basadas en la web para la autenticación y autorización de usuarios.

Para configurar OAuth, debe crear un [!DNL SharePoint] y una aplicación de sitio dentro de [!DNL SharePoint]. Este proceso se describe en las secciones siguientes.

Para obtener más información sobre OAuth, consulte [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>Para que sea más fácil copiar y pegar información entre [!DNL Workfront] y [!DNL SharePoint] en estos pasos, se recomienda mantener ambas aplicaciones abiertas en pestañas independientes.

* [Creación y configuración de un [!DNL SharePoint] sitio](#create-and-configure-a-sharepoint-site)
* [Conceder permisos de escritura a la aplicación del sitio](#grant-write-permissions-to-the-site-app)
* [Crear un [!DNL Workfront] [!DNL SharePoint] instancia de integración](#create-a-workfront-sharepoint-integration-instance)
* [Finalización de la integración](#complete-your-integration)
* [Agregar documentos](#add-documents)

### Creación y configuración de un [!DNL SharePoint] sitio  {#create-and-configure-a-sharepoint-site}

Para que [!DNL Workfront] para autenticarse con [!DNL SharePoint], [!DNL Workfront] puede utilizar una ubicación maestra en la que los usuarios tengan [!UICONTROL Control total] nivel de permiso o permisos específicos de Administrar. Esta ubicación maestra actúa como punto de entrada de autenticación para [!DNL Workfront].

Para crear y configurar un [!DNL SharePoint] Sitio:

1. (Opcional) Si no desea utilizar la ubicación raíz de su organización, puede crear una ubicación maestra en [!DNL SharePoint].

   Para obtener instrucciones, visite [Crear un sitio](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) en el [!DNL Microsoft] Documentación.

   * Seleccione el **[!UICONTROL Sitio de equipo]** al crear el sitio.

1. (Condicional) Si creó un sitio en el paso 1, vaya al sitio que acaba de crear.

   O

   Si no creó ningún sitio en el paso 1, vaya al sitio raíz de su organización.

1. Añadir `/_layouts/15/appregnew.aspx` al final de la dirección URL en la barra de búsqueda de la parte superior de la ventana del explorador.
1. Configure los campos siguientes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL ID de cliente]</p> </td> 
      <td> <p>Clic <strong>[!UICONTROL Generar]</strong> para generar un ID de cliente. Copie este ID en una ubicación segura. La utilizará más adelante cuando configure el [!DNL SharePoint] integración en [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Secreto de cliente]</p> </td> 
      <td> <p>Clic <strong>[!UICONTROL Generar]</strong> para generar un Secreto de cliente. Copie este Secreto en una ubicación segura. La utilizará más adelante cuando configure el [!DNL SharePoint] integración en [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Título</p> </td> 
      <td> <p>Escriba un título, como [!DNL Workfront] Aplicación del sitio. Los usuarios ven este título al agregar documentos.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App Domain]</p> </td> 
      <td> <p><code>my.workfront.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL URI de redireccionamiento]</p> </td> 
      <td> <p><code>https://oauth.my.workfront.com/oauth2/redirect</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clic **[!UICONTROL Crear]**
1. Continuar a [Conceder permisos de escritura a la aplicación del sitio](#grant-write-permissions-to-the-site-app).

### Conceder permisos de escritura a la aplicación del sitio  {#grant-write-permissions-to-the-site-app}

En este punto, ha creado correctamente una aplicación de sitio y la ha registrado en [!DNL Workfront]. Esta aplicación de sitio también se conoce como entidad de seguridad de aplicación en [!DNL SharePoint]. Reside dentro de su inquilino. Las nuevas aplicaciones de sitio no tienen acceso automáticamente a las colecciones de sitios dentro del inquilino. Los permisos deben concederse explícitamente para cada colección de sitios. Los pasos siguientes le mostrarán cómo conceder permiso de escritura a la nueva aplicación del sitio para una colección de sitios. Repita estos pasos para cada una de las colecciones de sitios agregadas en [!UICONTROL Colecciones de sitios visibles] en los pasos anteriores.

Esta aplicación del sitio debe tener [!UICONTROL Escritura] permiso para acceder a cualquier colección de sitios a través de los cuales los usuarios deban acceder [!DNL Workfront].

1. Añada &quot;/_layouts/15/appinv.aspx&quot; a la dirección URL en [!DNL Sharepoint].

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
      <td role="rowheader">[!UICONTROL ID de aplicación]</td> 
      <td> <p>Añada el ID de cliente que creó en <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Creación y configuración de un [!DNL SharePoint] sitio </a>y haga clic en <strong>[!UICONTROL Búsqueda]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client] / [!UICONTROL App Domain] / [!UICONTROL Redirect URL]</p> </td> 
      <td> <p>Se rellenan automáticamente al hacer clic en [!UICONTROL Consulta].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL XML de solicitud de permiso]</td> 
      <td> <p>Copie el siguiente XML en el campo [!UICONTROL Permiso Solicitar XML]. Asegúrese de que se agrega exactamente como se muestra sin espacios adicionales, etc. para evitar errores.</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre></pre></div></div></td></tr></tbody></table>

1. Haga clic en **[!UICONTROL Crear]**.
1. En el cuadro de diálogo que aparece, haga clic en **[!UICONTROL Confíe en él]**.
1. Compruebe que la aplicación del sitio tiene acceso a la colección de sitios haciendo clic en **[!UICONTROL Permisos de aplicación de colección de sitios]** vincular en [!UICONTROL Configuración del sitio].
1. Repita los pasos anteriores para las colecciones de sitios restantes y continúe con [Crear un [!DNL Workfront] [!DNL SharePoint] instancia de integración](#create-a-workfront-sharepoint-integration-instance).

### Crear un [!DNL Workfront] [!DNL SharePoint] instancia de integración {#create-a-workfront-sharepoint-integration-instance}

Cuando haya creado una aplicación del sitio en [!DNL SharePoint], ahora puede copiar información de la aplicación del sitio en [!DNL Workfront]. La aplicación del sitio es una entidad de seguridad de la aplicación y actúa como el conducto a través del cual se realizan las solicitudes de OAuth para acceder a los documentos dentro de las colecciones de sitios.

1. Iniciar sesión en [!DNL Workfront] como administrador.
1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL [!DNL SharePoint]Integración]**.
1. Clic **[!UICONTROL Añadir[!DNL SharePoint]]**.
1. Configure los campos siguientes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Nombre]</p> </td> 
      <td> <p>Introduzca un nombre para el [!DNL SharePoint] integración. Los usuarios verán este nombre cuando hagan clic en [!UICONTROL Agregar] &gt; [!UICONTROL Desde] 'nombre de la integración'. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] Instancia de host]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] Acceder al dominio]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>Hace referencia a la ubicación maestra que utilizarán los usuarios para autenticarse. Probablemente sea el mismo dominio que [!UICONTROL [!DNL SharePoint] Instancia de host].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>Importante</b> Las colecciones de sitios solo se utilizan en el heredado [!DNL SharePoint] Integración.
       <ul> 
        <li> <p><b>Si utiliza el sitio raíz de su organización</b><b>:</b> </p> <p>Entrar <code>/</code></p> </li> 
        <li> <p><b>Si utiliza una ubicación maestra y sububicaciones:</b> </p> <p><b>IMPORTANTE</b>: [!DNL Microsoft SharePoint] ya no recomienda el uso de subsitios.</p> <p>Escriba el sistema de direcciones URL para la colección de sitios que creó en la sección anterior.</p> <p>Esta es la sección de la dirección URL después de .com.</p> <p>Ejemplo: para la dirección URL <code>https://mycompany.sharepoint.com/sites/mysite</code>, el tallo sería <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] ID de cliente]</td> 
      <td>Introduzca el ID de cliente que generó en <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Creación y configuración de un [!DNL SharePoint] sitio </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Secreto del cliente]</td> 
      <td>Introduzca el Secreto de cliente que ha generado en <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Creación y configuración de un [!DNL SharePoint] sitio </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Colecciones de sitios visibles]</td> 
      <td> <b>Importante</b> Las colecciones de sitios solo se utilizan en el heredado [!DNL SharePoint] integración.
       <ul> 
        <li> <p><b> Si utiliza el sitio raíz de su organización</b><b>:</b> </p> <p>Entrar <code>/</code></p> </li> 
        <li> <p><b>Si utiliza una ubicación maestra y sububicaciones:</b> </p> <p><b>IMPORTANTE</b>: [!DNL Microsoft SharePoint] ya no recomienda el uso de subsitios.</p> <p>Para cada subsitio que desee agregar a su [!DNL SharePoint] integración, introduzca la raíz del subsitio.</p> <p>Ejemplo: para la dirección URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, el tallo sería <code>/sites/mysite/mysubsite</code>.</p> <p><b>NOTA</b>:   <p>Si sólo desea probar la configuración (sin sububicaciones), introduzca la ubicación de la ubicación maestra. </p> <p>Ejemplo: para la dirección URL <code> https://mycompany.sharepoint.com/sites/mysite</code>, el tallo sería <code>/sites/mysite</code>.</p> <p>Cuando haya probado la configuración como se describe en <a href="#complete-your-integration" class="MCXref xref">Finalización de la integración</a>, debe eliminar la ubicación maestra e introducir los subsitios.</p> 
          <ol> 
           <li value="1">Haga clic en <strong>[!UICONTROL Menú principal]</strong> icono <img src="assets/main-menu-icon.png"> en la esquina superior derecha de [!DNL Adobe Workfront], luego haga clic en <strong>[!UICONTROL Configuración]</strong> <img src="assets/gear-icon-settings.png">.<li><p>En el panel izquierdo, haga clic en <strong>[!UICONTROL Documentos]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] Integración]</strong>.</p></li><li><p>Haga clic en [!DNL SharePoint] integración que está configurando y haga clic en Editar.</p></li><li><p>Elimine la raíz de la ubicación maestra del campo [!UICONTROL Colecciones de sitios visibles].</p></li><li><p>Para cada subsitio que desee agregar a su [!DNL SharePoint] integración, introduzca la raíz del subsitio.</p></li><p>Ejemplo: para la dirección URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, el tallo sería <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Guardar]**
1. Continuar a [Finalización de la integración](#complete-your-integration).

### Finalización de la integración {#complete-your-integration}

La configuración básica está casi completa.

1. En Workfront, haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **[!UICONTROL Documentos]** ![](assets/document-icon.png).
1. Clic **[!UICONTROL Añadir nuevo]**.
1. Clic **[!UICONTROL Desde]`<title of your [!DNL SharePoint] site>`** en el menú desplegable.

   Aparecerá un cuadro de diálogo que le invita a Confiar en este sitio.

   >[!NOTE]
   >
   >Si no aparece este cuadro de diálogo, [!DNL SharePoint] La integración de no está configurada correctamente.

1. Clic **[!UICONTROL Confíe en él]**.

### Agregar documentos {#add-documents}

Ahora puede agregar documentos desde su [!DNL SharePoint] sitio.

Para obtener instrucciones, consulte [Vincular un documento externo a [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in [Vinculación de documentos desde aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>Si el usuario que ha vinculado una carpeta ya no tiene acceso a la aplicación externa, [!DNL Workfront] ya no puede acceder al contenido de la carpeta. Esto puede suceder, por ejemplo, si el usuario que vinculó originalmente la carpeta abandona la compañía. Para garantizar el acceso continuo, un usuario con acceso a la carpeta debe volver a vincular la carpeta.

## Solución de problemas

* [Problema: Los usuarios experimentan errores basados en la autenticación al utilizar el [!DNL SharePoint] integración.](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [Problema: Como [!DNL Workfront] usuario, no puedo aprovisionar un nuevo [!DNL SharePoint] ejemplo. Cuando intento hacerlo, veo un error.](#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error)
* [Problema: Al intentar examinar [!DNL SharePoint] archivos en [!DNL Workfront], no veo ninguna o todas las colecciones de sitios.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [Problema: No puedo acceder a carpetas y documentos enlazados anteriormente en [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### Problema: Los usuarios experimentan errores basados en la autenticación al utilizar el [!DNL SharePoint] integración. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

Soluciones:

Los usuarios deben ser miembros de un grupo que tenga los permisos adecuados para [!DNL SharePoint] sitio.

Usuarios con [!UICONTROL Control total] tiene todos los permisos necesarios para su [!DNL SharePoint] integración. Si no desea conceder acceso de Control total a los usuarios, debe conceder los siguientes permisos:

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

Para obtener instrucciones sobre cómo crear y editar niveles de permisos, consulte [Crear y editar niveles de permisos](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels) en la documentación de Microsoft.

### Problema: Como [!DNL Workfront] usuario, no puedo aprovisionar un nuevo [!DNL SharePoint] ejemplo. Cuando intento hacerlo, veo un error. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Soluciones:

Esto puede deberse a varias causas, que se originan en [!DNL Workfront] o [!DNL SharePoint]La configuración de. Compruebe que:

* El ID del cliente, el Secreto del cliente, la URL de retorno y otros campos de configuración se asignan correctamente entre los campos [!DNL Workfront] [!DNL SharePoint] Instancia de integración y [!DNL SharePoint] Aplicación del sitio.
* El usuario tiene [!UICONTROL Control total] permiso para acceder a la colección de sitios utilizada para la autenticación.
* La aplicación del sitio se enumera en [!UICONTROL Permisos de aplicación del sitio] para el [!UICONTROL Colección del sitio] se utiliza para la autenticación.

### Problema: Al intentar examinar [!DNL SharePoint] archivos en [!DNL Workfront], no veo ninguna o todas las colecciones de sitios. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

Soluciones:

Para ver una colección de sitios en [!DNL Workfront], deben cumplirse las siguientes condiciones:

* La colección de sitios debe estar registrada en [!DNL Workfront] [!DNL SharePoint] Instancia de integración.

   Para verificarlo en [!DNL Workfront]:

   1. Ir a [!UICONTROL Configurar] > [!UICONTROL Documentos] > [!UICONTROL [!DNL SharePoint] Integración].
   1. Edite el [!DNL SharePoint] Información de instancia de integración.
   1. Compruebe que la colección de sitios aparece en [!UICONTROL Colecciones de sitios visibles].

* El usuario debe tener acceso de visualización a la colección de sitios en [!DNL SharePoint].
* Para verificarlo en [!DNL SharePoint], vaya a [!DNL SharePoint]y abra la colección de sitios > [!UICONTROL Configuración] > [!UICONTROL Permisos del sitio].
* El [!DNL SharePoint] La aplicación del sitio debe tener acceso a la colección de sitios.

   Para verificarlo en [!DNL SharePoint]:

   1. Vaya a la colección de sitios > [!UICONTROL Configuración] > [!UICONTROL Permisos de aplicación del sitio].
   1. Asegúrese de que la variable [!UICONTROL Aplicación del sitio] utilizado por [!DNL Workfront] aparece aquí.
   1. (Condicional) Si la aplicación del sitio no aparece en la lista, agregue a la colección de sitios mediante _layouts/15/appinv.aspx.

      Para obtener información sobre cómo agregar la colección de sitios, vea Conceder permisos de escritura a la aplicación del sitio.

### Problema: No puedo acceder a carpetas y documentos enlazados anteriormente en [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

Solución:

Si el usuario que vinculó un [!DNL SharePoint] ya no se puede autenticar, [!DNL Workfront] ya no puede acceder al contenido de la carpeta. Esto puede suceder, por ejemplo, si el usuario que vinculó originalmente la carpeta abandona la compañía.

Para garantizar el acceso continuo, un usuario con acceso a la carpeta debe volver a vincular la carpeta.

Para obtener información sobre la vinculación de carpetas desde proveedores externos, consulte [Vinculación de documentos desde aplicaciones externas](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Problema: Veo un error &quot;404 not found&quot; al intentar añadir un documento desde [!DNL Sharepoint]

#### Solución:

Este error puede producirse si uno de los sitios configurados en la variable [!UICONTROL Colecciones de sitios visibles] se ha eliminado en Sharepoint. Compruebe la [!UICONTROL Colecciones de sitios visibles] y quite los sitios que se hayan eliminado en Sharepoint.
