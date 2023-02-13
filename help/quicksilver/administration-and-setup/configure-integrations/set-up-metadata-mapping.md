---
title: Configuración de la asignación de metadatos
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Los metadatos son información descriptiva asociada a un documento. Puede configurar [!DNL Adobe Workfront] incluir metadatos con documentos enviados a [!DNL Workfront] aplicaciones.
author: Caroline
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7cf4787d-7cff-489e-bd5b-69db3ff09f6e
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---

# Configuración de la asignación de metadatos

Los metadatos son información descriptiva asociada a un documento. Puede configurar [!DNL Adobe Workfront] incluir metadatos con documentos enviados a [!DNL Workfront] aplicaciones.

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
   <td> <p>Debe ser [!DNL Workfront] administrador. Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Acerca de [!DNL Workfront] metadata

Metadatos de los documentos de [!DNL Workfront] puede incluir información como el nombre del proyecto relacionado, la descripción de la tarea o la fecha de finalización prevista. Como [!DNL Workfront] administrador, puede configurar [!DNL Workfront] incluir metadatos con documentos enviados desde [!DNL Workfront] a lo siguiente [!DNL Workfront] aplicaciones:

* [!DNL Workfront DAM]

Antes de poder enviar los metadatos con los documentos, primero debe especificar o asignar los metadatos que desea incluir. Puede asignar cualquier campo utilizado en [!DNL Workfront]. Una vez configurada la asignación de metadatos, todos los documentos cargados en un [!DNL Workfront] la aplicación incluirá los metadatos asignados.

Cuando un usuario envía un documento desde [!DNL Workfront] a [!DNL Workfront] aplicación, los metadatos asignados se transfieren a lo largo del documento. Mientras que la versión del documento en la variable [!DNL Workfront] la aplicación está vinculada a [!DNL Workfront], cambios realizados en los metadatos del documento en [!DNL Workfront] no se reflejan en los metadatos del documento en la [!DNL Workfront] aplicación. Si un campo asignado [!DNL Workfront] se cambia, debe enviar una nueva versión del documento con los metadatos actualizados a la variable [!DNL Workfront] aplicación.

>[!NOTE]
>
>Los metadatos solo se pueden asignar en una dirección: from [!DNL Workfront] a [!DNL Workfront DAM]. Metadatos de los documentos vinculados a [!DNL Workfront] from [!DNL Workfront DAM] no se puede transferir a Workfront.

Puede asignar lo mismo [!DNL Workfront] campo a varios campos de metadatos [!DNL Workfront DAM], pero no puede utilizar un campo de metadatos en ninguna de estas aplicaciones para varias [!DNL Workfront] campos de metadatos.

Para configurar varias [!DNL Workfront] campos para exportar a un campo de metadatos de un [!DNL Workfront] , cree primero un campo personalizado calculado en [!DNL Workfront] para mostrar todos los campos personalizados individuales de un objeto. A continuación, asigne el valor calculado [!DNL Workfront] a un campo de metadatos en la variable [!DNL Workfront] aplicación. Para obtener más información sobre los campos personalizados calculados, consulte [Agregar datos calculados a un formulario personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Para poder asignar campos para el proceso de asignación de metadatos, debe activar la aplicación en [!DNL Workfront]. Para obtener más información, consulte [Configurar integraciones de documentos](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Configurar [!DNL Workfront] para enviar metadatos

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL Asignación de metadatos]**.

   ![](assets/metadata-mapping.png)

1. En el **[!UICONTROL Seleccionar campo de origen para asignación]** , empiece a escribir el nombre del campo de Workfront al que desea asignar [!DNL Workfront DAM]y, a continuación, selecciónela cuando la vea en la lista.
1. En el **[!UICONTROL Seleccionar campo de destino para asignación]** , seleccione el campo que desea rellenar con la información del [!DNL Workfront] campo .

1. Haga clic en **[!UICONTROL Agregar asignación]**.

   El campo asignado se muestra en los campos asignados que aparecen en la parte inferior de la página.

1. Repita los pasos 5 y 6 hasta que añada todos los [!DNL Workfront] campos y sus correspondientes [!DNL Workfront DAM] campos.

## Eliminar campos asignados

1. Iniciar sesión en [!DNL Workfront] como administrador.
1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL Asignación de metadatos]**.

1. En la lista de campos asignados, seleccione los campos que desea eliminar de la asignación de metadatos.
1. Haga clic en **[!UICONTROL Eliminar]**.

   Los campos designados ya no están asignados. Ahora, cuando un usuario envía un documento desde [!DNL Workfront] a [!DNL Workfront DAM], los metadatos contenidos en los campos eliminados no se transfieren con el documento.

   Un documento enviado antes de eliminar los campos asignados conserva los metadatos originales enviados con él, incluidos los metadatos de los campos eliminados.
