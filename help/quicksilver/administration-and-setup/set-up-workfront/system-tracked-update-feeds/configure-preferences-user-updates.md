---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configuración de preferencias para actualizaciones de usuarios
description: Puede configurar las preferencias que permiten acceder a determinadas funciones cuando los usuarios agregan comentarios en el informe [!UICONTROL Actualizaciones] .
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Configuración de preferencias para actualizaciones de usuarios

Puede configurar las preferencias que otorgan a los usuarios acceso a determinadas funciones cuando agregan comentarios en el informe [!UICONTROL Actualizaciones] .

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
   <td> <p>Para realizar estos pasos a nivel de sistema, necesita el nivel de acceso de [!UICONTROL System Administrator].</p><p>Para realizarlos para un grupo, debe ser administrador de dicho grupo.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Permitir que los usuarios agreguen imágenes en actualizaciones

De forma predeterminada, los usuarios no pueden agregar imágenes en las actualizaciones. Al habilitar esta preferencia, los usuarios podrán adjuntar imágenes en actualizaciones. La preferencia se aplica a todas las actualizaciones en todas las áreas del [!DNL Workfront] instancia.

>[!NOTE]
>
>* Las imágenes guardadas en actualizaciones se contabilizan en el límite de almacenamiento del documento. Para obtener más información, consulte [Comprobar límites de almacenamiento de documentos](../../../documents/managing-documents/check-document-storage.md).
>* Solo se puede acceder a las imágenes a través del [!UICONTROL Actualizaciones] en un objeto y no están disponibles en la [!UICONTROL Documentos] pestaña .
>




1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).
1. En el panel izquierdo, seleccione **[!UICONTROL Interfaz]** > **[!UICONTROL Actualizar fuentes]**.
1. Seleccione el **[!UICONTROL Preferencias]** pestaña .

   ![Preferencias de usuario para actualizar fuentes](assets/updatefeeds-preferences-350x137.png)

1. Seleccione el **[!UICONTROL Permitir que los usuarios agreguen imágenes en actualizaciones]** en el Navegador.
1. Select **[!UICONTROL Guardar]**.

   Cuando esta preferencia está habilitada, puede deshabilitarla en cualquier momento. Las imágenes que ya se hayan publicado en las actualizaciones permanecerán en la variable [!UICONTROL Actualizaciones] del objeto.
