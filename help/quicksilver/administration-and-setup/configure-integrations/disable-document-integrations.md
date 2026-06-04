---
title: Deshabilitar integraciones de documentos
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Como administrador de  [!DNL anAdobe] [!DNL Workfront], puede deshabilitar la conexión entre Workfront y cualquiera de los proveedores de documentos de terceros.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
author: Courtney, Becky
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
TQID: https://experienceleague.adobe.com/3tfxxth82eJEjEmdVD3AJFxl6B1m3EVKMQP9Gy4LC24
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 279
ht-degree: 97%

---

# Deshabilitar integraciones de documentos

Como administrador de [!DNL Adobe] [!DNL Workfront], puede deshabilitar la conexión entre [!DNL Workfront] y cualquiera de los proveedores de documentos de terceros.

Al deshabilitar la conexión entre [!DNL Workfront] y un proveedor de documentos, los vínculos a los documentos desaparecerán de [!DNL Workfront]. Los usuarios ya no podrán ver los documentos vinculados, realizar cambios en los documentos a través de los vínculos a [!DNL Workfront] ni añadir más documentos a ese proveedor.

## Requisitos de acceso

+++Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table>
  <tr>
   <td>Paquete de Adobe Workfront
   </td>
   <td> <p>PRIME o ULTIMATE</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Licencias de Adobe Workfront
   </td>
   <td><p>Estándar</p>
   <p>Plan</p>
   </td>
  </tr>
   <tr>
   <td>Configuraciones de nivel de acceso
   </td>
   <td>Debe ser administrador de [!DNL Workfront].
   </td>
  </tr>
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Deshabilitar integraciones de proveedores de servicios en la nube

Para deshabilitar las integraciones de documentos para [!UICONTROL Workfront DAM], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive] y [!DNL WebDAM]:

1. Inicie sesión en [!DNL Workfront] como administrador de [!DNL Workfront].

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL Proveedores de servicios en la nube]**.

1. Anule la selección de cualquiera de los proveedores de servicios en la nube que desee desconectar de [!DNL Workfront].
1. Haga clic en **[!UICONTROL Guardar]**.

   Los usuarios no podrán conectarse al proveedor de servicios en la nube específico que ha deshabilitado y ya no podrán vincular documentos de ese proveedor de servicios en la nube a Workfront.

## Deshabilitar la integración de [!DNL SharePoint]

1. Inicie sesión en [!DNL Workfront] como administrador de [!DNL Workfront].

{{step-1-to-setup}}

1. Expanda **[!UICONTROL Documentos]** y, a continuación, haga clic en **[!UICONTROL [!DNL SharePoint]Integración]**.
1. Seleccione la integración de [!DNL SharePoint] que desee deshabilitar.
1. Haga clic en **[!UICONTROL Deshabilitar]**.\
   Los usuarios no podrán conectarse al sitio de [!DNL SharePoint] que ha deshabilitado y ya no podrán vincular documentos de [!DNL SharePoint] a [!DNL Workfront].

## Deshabilitar integraciones personalizadas

1. Inicie sesión en [!DNL Workfront] como administrador.

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL Integración personalizada]**.
1. Seleccione la integración personalizada que desee deshabilitar.
1. Haga clic en **[!UICONTROL Deshabilitar]**.

   Los usuarios no podrán conectarse al proveedor de documentos de terceros que ha deshabilitado y ya no podrán vincular documentos de ese proveedor de servicios en la nube a [!DNL Workfront].
