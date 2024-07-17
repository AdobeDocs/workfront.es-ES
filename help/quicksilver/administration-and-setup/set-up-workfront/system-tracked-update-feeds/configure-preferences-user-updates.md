---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurar preferencias para actualizaciones de usuarios
description: Puede configurar las preferencias que permiten acceder a determinadas funciones cuando los usuarios agregan comentarios en el área [!UICONTROL Actualizaciones] de un objeto.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: fd876089c964d57224452023b4656cd6df40b5a3
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 1%

---

# Configurar preferencias para actualizaciones de usuarios

Puede configurar las preferencias que conceden a los usuarios acceso a determinadas características cuando agregan comentarios en el área [!UICONTROL Actualizaciones] de un objeto.

## Requisitos de acceso

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
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Para realizar estos pasos en el sistema, necesita el nivel de acceso de [!UICONTROL System Administrator].</p><p>Para realizarlos para un grupo, debe ser administrador de ese grupo.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Permitir que los usuarios agreguen imágenes en las actualizaciones

De forma predeterminada, los usuarios no pueden agregar imágenes en las actualizaciones. Al habilitar esta preferencia, los usuarios podrán adjuntar imágenes en las actualizaciones. La preferencia se aplica a todas las actualizaciones en todas las áreas de la instancia de [!DNL Workfront].

>[!NOTE]
>
>* Las imágenes guardadas en las actualizaciones se contabilizan en el límite de almacenamiento de documentos. Para obtener más información, consulte [Comprobar límites de almacenamiento de documentos](../../../documents/managing-documents/check-document-storage.md).
>* Se puede acceder a las imágenes a través de la ficha [!UICONTROL Actualizaciones] de un objeto y también están disponibles en el área de [!UICONTROL Documentos] en el [!UICONTROL Menú principal].
>

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront] y, a continuación, haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).
1. En el panel izquierdo, seleccione **[!UICONTROL Interfaz]** > **[!UICONTROL Actualizar fuentes]**.
1. Seleccione la ficha **[!UICONTROL Preferencias]**.

   ![Preferencias de usuario para actualizar fuentes](assets/updatefeeds-preferences-350x137.png)

1. Active la casilla de verificación **[!UICONTROL Permitir que los usuarios agreguen imágenes en actualizaciones]**.
1. Seleccione **[!UICONTROL Guardar]**.

   Cuando esta preferencia está habilitada, puede deshabilitarla en cualquier momento. Las imágenes que ya se hayan publicado en las actualizaciones permanecerán en el área de [!UICONTROL Actualizaciones] del objeto.
