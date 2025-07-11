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
source-git-commit: 594f224e11b0e7708ed555410b7c331741113791
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 91%

---

# Configurar preferencias para actualizaciones de usuarios

<!--Audited: 06/2025-->

Puede configurar las preferencias que conceden a los usuarios acceso a determinadas funciones cuando añaden comentarios en el área [!UICONTROL Actualizaciones] de un objeto.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td><p>Nuevo: [!UICONTROL Standard]</p>
   O
   <p>Actual: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td><p>Para realizar estos pasos en el sistema, necesita el nivel de acceso de [!UICONTROL System Administrator].</p><p>Para realizarlos para un grupo, debe ser administrador de ese grupo.</p></td>
  </tr> 
 </tbody> 
</table>

*Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
