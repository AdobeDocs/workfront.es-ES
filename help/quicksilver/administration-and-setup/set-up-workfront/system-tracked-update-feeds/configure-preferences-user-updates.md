---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurar preferencias para actualizaciones de usuarios
description: Puede configurar las preferencias que permiten acceder a determinadas funciones cuando los usuarios añaden comentarios en el área [!UICONTROL Actualizaciones] de un objeto.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 80%

---

# Configurar preferencias para actualizaciones de usuarios

<!--Audited: 08/2025-->

Puede configurar las preferencias que conceden a los usuarios acceso a determinadas funciones cuando añaden comentarios en el área [!UICONTROL Actualizaciones] de un objeto.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] paquete</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td><p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td><p>Administrador del sistema, para realizar estos pasos en el sistema. </p>
   <p>Planificador, para realizar estos pasos para un grupo, además de ser el administrador de ese grupo.</p></td>
  </tr> 
 </tbody> 
</table>

*Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: [!UICONTROL Standard]</p>
   Or
   <p>Current: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td><p>To perform these steps at the system level, you need the [!UICONTROL System Administrator] access level.</p><p>To perform them for a group, you must be a manager of that group.</p></td>
  </tr> 
 </tbody> 
</table>-->

## Permitir que los usuarios añadan imágenes en las actualizaciones

De forma predeterminada, los usuarios no pueden añadir imágenes en las actualizaciones. Al habilitar esta preferencia, los usuarios podrán adjuntar imágenes en las actualizaciones. La preferencia se aplica a todas las actualizaciones en todas las áreas de la instancia de [!DNL Workfront].

>[!NOTE]
>
>* Las imágenes guardadas en las actualizaciones se contabilizan en el límite de almacenamiento de documentos. Para obtener más información, consulte [Comprobar límites de almacenamiento de documentos](../../../documents/managing-documents/check-document-storage.md).
>* Se puede acceder a las imágenes a través de la pestaña [!UICONTROL Actualizaciones] de un objeto y también están disponibles en el área de [!UICONTROL Documentos] en el [!UICONTROL Menú principal].
>

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront] y, a continuación, haga clic en **[!UICONTROL Configurar]** ![Icono de configuración de engranajes](assets/gear-icon-settings.png).
1. En el panel izquierdo, seleccione **[!UICONTROL Interfaz]** > **[!UICONTROL Actualizar fuentes]**.
1. Seleccione la pestaña **[!UICONTROL Preferencias]**.

   ![Preferencias de usuario para actualizar fuentes](assets/updatefeeds-preferences-350x137.png)

1. Active la casilla de verificación **[!UICONTROL Permitir que los usuarios añadan imágenes en actualizaciones]**.
1. Seleccione **[!UICONTROL Guardar]**.

   Cuando esta preferencia está habilitada, puede deshabilitarla en cualquier momento. Las imágenes que ya se hayan publicado en las actualizaciones permanecerán en el área de [!UICONTROL Actualizaciones] del objeto.
