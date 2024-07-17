---
title: Deshabilitar integraciones de documentos
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Como administrador de  [!DNL anAdobe] [!DNL Workfront], puede deshabilitar la conexión entre Workfront y cualquiera de los proveedores de documentos de terceros.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Deshabilitar integraciones de documentos

Como administrador de [!DNL Adobe] [!DNL Workfront], puede deshabilitar la conexión entre [!DNL Workfront] y cualquiera de los proveedores de documentos de terceros.

Cuando deshabilita la conexión entre [!DNL Workfront] y un proveedor de documentos, los vínculos a los documentos desaparecen de [!DNL Workfront]. Los usuarios ya no pueden ver los documentos vinculados, no pueden realizar cambios en los documentos a través de los vínculos [!DNL Workfront] y no pueden agregar más documentos a ese proveedor.

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
   <td> <p>Debe ser administrador de [!DNL Workfront]. Para obtener información sobre los administradores de [!DNL Workfront], consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Deshabilitar integraciones de proveedores en la nube

Para deshabilitar las integraciones de documentos para [!UICONTROL Workfront DAM], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM]:

1. Inicie sesión en [!DNL Workfront] como administrador de [!DNL Workfront].
1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront] y, a continuación, haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL Proveedores de nube]**.

1. Anule la selección de cualquiera de los proveedores en la nube de los que quiera desconectarse [!DNL Workfront].
1. Haga clic en **[!UICONTROL Guardar]**.

   Los usuarios no pueden conectarse al proveedor de nube específico que deshabilitó y ya no pueden vincular documentos de ese proveedor de nube a Workfront.

## Deshabilitar la integración de [!DNL SharePoint]

1. Inicie sesión en [!DNL Workfront] como administrador de [!DNL Workfront].
1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront] y, a continuación, haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Expanda **[!UICONTROL Documentos]** y, a continuación, haga clic en **[!UICONTROL [!DNL SharePoint]Integración]**.
1. Seleccione la integración [!DNL SharePoint] que desee deshabilitar.
1. Haga clic en **[!UICONTROL Deshabilitar]**.\
   Los usuarios no pueden conectarse al sitio [!DNL SharePoint] que deshabilitó y ya no pueden vincular documentos de [!DNL SharePoint] a [!DNL Workfront].

## Deshabilitar integraciones personalizadas

1. Inicie sesión en [!DNL Workfront] como administrador.
1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront] y, a continuación, haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL Integración personalizada]**.
1. Seleccione la integración personalizada que desee desactivar.
1. Haga clic en **[!UICONTROL Deshabilitar]**.

   Los usuarios no pueden conectarse al proveedor de documentos de terceros que deshabilitó y ya no pueden vincular documentos de ese proveedor de la nube a [!DNL Workfront].
