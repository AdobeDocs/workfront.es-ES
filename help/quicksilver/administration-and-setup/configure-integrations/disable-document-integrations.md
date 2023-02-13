---
title: Desactivar integraciones de documentos
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Como [!DNL anAdobe] [!DNL Workfront] administrador, puede desactivar la conexión entre Workfront y cualquiera de los proveedores de documentos de terceros.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Desactivar integraciones de documentos

Como [!DNL Adobe] [!DNL Workfront] administrador, puede desactivar la conexión entre [!DNL Workfront] y cualquiera de los proveedores de documentos de terceros.

Al desactivar la conexión entre [!DNL Workfront] y un proveedor de documentos, los vínculos a los documentos desaparecen de [!DNL Workfront]. Los usuarios ya no pueden ver los documentos vinculados, no pueden realizar ningún cambio en los documentos a través del [!DNL Workfront] y no pueden agregar más documentos a ese proveedor.

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

## Deshabilitar integraciones de proveedores de nube

Para desactivar las integraciones de documentos para [!UICONTROL DAM de Workfront], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM]:

1. Iniciar sesión en [!DNL Workfront] como [!DNL Workfront] administrador.
1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL Proveedores de nube]**.

1. Anule la selección de cualquiera de los proveedores de la nube que desee desconectar [!DNL Workfront].
1. Haga clic en **[!UICONTROL Guardar]**.

   Los usuarios no pueden conectarse al proveedor de nube específico que ha deshabilitado y ya no pueden vincular documentos de ese proveedor de nube a Workfront.

## Desactive el [!DNL SharePoint] integración

1. Iniciar sesión en [!DNL Workfront] como [!DNL Workfront] administrador.
1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. Expandir **[!UICONTROL Documentos]** y haga clic en **[!UICONTROL [!DNL SharePoint]Integración]**.
1. Seleccione el [!DNL SharePoint] integración que desea deshabilitar.
1. Haga clic en **[!UICONTROL Deshabilitar]**.\
   Los usuarios no pueden conectarse al [!DNL SharePoint] sitio que ha deshabilitado y que ya no pueden vincular documentos desde [!DNL SharePoint] a [!DNL Workfront].

## Desactivar integraciones personalizadas

1. Iniciar sesión en [!DNL Workfront] como administrador.
1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL Integración personalizada]**.
1. Seleccione la integración personalizada que desee deshabilitar.
1. Haga clic en **[!UICONTROL Deshabilitar]**.

   Los usuarios no pueden conectarse al proveedor de documentos de terceros que ha deshabilitado y ya no pueden vincular documentos de ese proveedor de nube a [!DNL Workfront].
