---
title: Configurar asignación de metadatos
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Los metadatos son información descriptiva asociada a un documento. Puede configurar [!DNL Adobe Workfront] para que incluya metadatos con los documentos enviados a aplicaciones de  [!DNL Workfront] .
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7cf4787d-7cff-489e-bd5b-69db3ff09f6e
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 98%

---

# Configuración de la asignación de metadatos

Los metadatos son información descriptiva asociada a un documento. Puede configurar [!DNL Adobe Workfront] para que incluya metadatos con los documentos enviados a las aplicaciones de [!DNL Workfront].

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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

## Acerca de metadatos de [!DNL Workfront]

Los metadatos de los documentos de [!DNL Workfront] pueden incluir información como el nombre del proyecto relacionado, la descripción de la tarea o la fecha planificada de finalización. Como administrador de [!DNL Workfront], puede configurar [!DNL Workfront] para que incluya metadatos con los documentos enviados desde [!DNL Workfront] a las aplicaciones de [!DNL Workfront] siguientes:

* [!DNL Workfront DAM]

Para poder enviar metadatos con documentos, primero debe especificar o asignar los metadatos que desea incluir. Puede asignar cualquier campo utilizado en [!DNL Workfront]. Una vez configurada la asignación de metadatos, todos los documentos cargados en una aplicación de [!DNL Workfront] incluirán los metadatos asignados.

Cuando un usuario envía un documento de [!DNL Workfront] a una aplicación de [!DNL Workfront], los metadatos asignados se transfieren a lo largo del documento. Aunque la versión del documento en la aplicación de [!DNL Workfront] está vinculada a [!DNL Workfront], los cambios realizados en los metadatos del documento en [!DNL Workfront] no se reflejan en los metadatos del documento en la aplicación de [!DNL Workfront]. Si se cambia un campo asignado en [!DNL Workfront], debe enviar una nueva versión del documento con los metadatos actualizados a la aplicación de [!DNL Workfront].

>[!NOTE]
>
>Solo puede asignar metadatos en una dirección: de [!DNL Workfront] a [!DNL Workfront DAM]. Los metadatos de los documentos vinculados a [!DNL Workfront] desde [!DNL Workfront DAM] no se pueden transferir a Workfront.

Puede asignar el mismo campo [!DNL Workfront] a varios campos de metadatos en [!DNL Workfront DAM], pero no puede utilizar un campo de metadatos en ninguna de esas aplicaciones para varios campos de metadatos de [!DNL Workfront].

Para configurar varios campos de [!DNL Workfront] para exportarlos a un campo de metadatos en una aplicación de [!DNL Workfront], cree primero un campo personalizado calculado en [!DNL Workfront] para mostrar todos los campos personalizados individuales de un objeto. A continuación, asigne el campo [!DNL Workfront] calculado a un campo de metadatos en la aplicación de [!DNL Workfront]. Para obtener más información sobre los campos personalizados calculados, consulte [Añadir campos calculados a un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Para poder asignar campos para el proceso de asignación de metadatos, debe habilitar la aplicación en [!DNL Workfront]. Para obtener más información, consulte [Configurar integraciones de documentos](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Configurar [!DNL Workfront] para enviar metadatos

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **[!UICONTROL Documentos]** > **[!UICONTROL Asignación de metadatos]**.

   ![Asignación de metadatos](assets/metadata-mapping.png)

1. En el cuadro **[!UICONTROL Select Source Field for Mapping]**, empiece a escribir el nombre del campo de Workfront que desea asignar a [!DNL Workfront DAM] y, a continuación, selecciónelo cuando lo vea en la lista.
1. En el cuadro **[!UICONTROL Select Target Field for Mapping]**, seleccione el campo que desee rellenar con la información del campo [!DNL Workfront] seleccionado.

1. Haga clic en **[!UICONTROL Add Mapping]**.

   El campo asignado se muestra en los campos asignados enumerados en la parte inferior de la página.

1. Repita los pasos 5 y 6 hasta que añada todos los campos [!DNL Workfront] deseados y sus correspondientes campos de [!DNL Workfront DAM].

## Eliminar campos asignados

1. Inicie sesión en [!DNL Workfront] como administrador.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **[!UICONTROL Documents]** > **[!UICONTROL Metadata Mapping]**.

1. En la lista de campos asignados, seleccione los campos que desea eliminar de la asignación de metadatos.
1. Haga clic **[!UICONTROL eliminar]**.

   Los campos designados ya no están asignados. Ahora, cuando un usuario envía un documento de [!DNL Workfront] a [!DNL Workfront DAM], los metadatos contenidos en los campos eliminados no se transfieren con el documento.

   Un documento enviado antes de eliminar los campos asignados conserva los metadatos originales enviados con él, incluidos los metadatos de los campos eliminados.
