---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Configuración del acceso de revisión de un usuario
description: Como administrador de Adobe Workfront o de Workfront Proof, puede configurar el acceso de un usuario para crear y ver pruebas en Workfront y Workfront Proof.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
TQID: 'https://experienceleague.adobe.com/L-AMDvQYgtXJwxmtwekimbEA9OQQN72QHIcoQ2iKzGU'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4ea8bc003ce17978be5e5a6fd838012dfcfeae78
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 98%
---
# Configuración del acceso de revisión de un usuario

Como administrador de Adobe Workfront o de Workfront Proof, puede configurar el acceso de un usuario para crear y ver pruebas en Workfront y Workfront Proof.

Para obtener información acerca de la funcionalidad de revisión disponible para la revisión básica e integrada, consulte [Acceso a la funcionalidad de revisión en Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser administrador de Workfront o de Workfront Proof. Para obtener información sobre los administradores de Workfront, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo total a un usuario</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

+++

<!--

## Configure a user's proof permission profile

The permission profile you select is granted to the users for each proof that exists within your organization.

{{step-1-to-users}}
 
1. Select one or more users, then click **Edit**.  

1. In the **Access** section, click one of the following Workfront Proof permission options in the **Proof Permission Profile** drop-down menu:

   >[!NOTE]
   >
   >If you are on a legacy Workfront plan, make sure the **User can generate proofs** option is enabled, as explained above in the section [Enable and disable proofing for a user (legacy plans only)](#enable-and-disable-proofing-for-a-user-legacy-plans-only). 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Supervisor</strong> </td> 
      <td>Users can manage and view all proofs created on your organization's account. They can also edit reviewers added to these proofs. Users with this permission profile can't manage users or edit Workfront Proof settings.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Manager</strong> </td> 
      <td> <p> Users can manage and view proofs created or owned on your organization's account. They can view other users' proofs only when added as a reviewer. This is a default setting. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrator</strong> </td> 
      <td> Users are given Administrator permissions in Workfront Proof and can edit account settings. Users can manage and view all proofs created on your organization's account. This includes adding and removing reviewers, proofs, and comments.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Custom</strong> </td> 
      <td> <p>Available only if you have configured a custom permission profile within Workfront Proof.</p> <p><b>NOTE</b>:  <p>Ensure that the permission profile you grant here does not provide higher access than the user's Access Level setting in Workfront (see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>). If it does provide higher access, the user can access proofs within Workfront Proof that he or she cannot access within Workfront.</p> <p>This is especially important if you plan to allow all Workfront users to access Workfront Proof directly from the Workfront as described in <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Access Workfront Proof from Adobe Workfront</a>.</p> <p>By default, only Workfront administrators have access to a direct link to the Workfront Proof site from the Workfront Global Navigation Bar.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   The permission profile you select is granted to the users for each proof that exists within your organization.

1. Click **Save Changes** to complete the update to the user settings.

   >[!NOTE]
   >
   >When you create or update a user in Workfront and the user's Workfront email address matches that of a licensed Workfront Proof user, the system enables proofing for the user within Workfront. For more information, see [User synchronization between Adobe Workfront and Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Considerations

Consider the following information when setting permissions:

* If you change a user's permission profile to a profile with fewer permissions, the user might lose visibility to existing proofs within Workfront. This can occur when someone shares a task with a user within Workfront, but doesn't share the proof attached to the task (see [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* You can set Workfront Proof permissions from Workfront only if your Workfront environment is integrated with a Workfront Proof Premium account. If you cannot use proofing as discussed in this section, contact your Workfront administrator.
* At least one user in your Workfront environment must have Administrator permissions for proofing. An error message appears if you try to attempt to remove Administrator permissions for proofing from all users.
* When you change a user's Workfront Access level to any level other than System Administrator, the user's Workfront Proof permission profile defaults to Manager.   

* When you change the Workfront Access level to System Administrator, the Proof Permission profile changes to Administrator.

-->

## Configuración del acceso a Workfront Proof a través del menú principal de Workfront para todos los usuarios {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

De manera predeterminada, solo los usuarios con derechos administrativos en Workfront pueden acceder a Workfront Proof como se describe en [Acceder a Workfront Proof desde Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

Puede otorgar a todos los usuarios acceso al botón Workfront Proof dentro del menú principal de Workfront poniéndose en contacto con el servicio de asistencia técnica de Workfront y enviando una solicitud.

>[!IMPORTANT]
>
> Si planea permitir que todos los usuarios de Workfront accedan a Workfront Proof directamente desde la barra de navegación global de Workfront, asegúrese de que el perfil de permiso de cada usuario no proporcione más acceso que el nivel de acceso del usuario dentro de Workfront. Esto evita que los usuarios accedan a pruebas dentro de Workfront Proof a las que no pueden acceder dentro de Workfront. Para obtener más información, consulte [Habilitar y deshabilitar la revisión para un usuario (solo planes heredados)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

## Configuración del acceso de los usuarios al Visor de corrección de escritorio

Si los usuarios de su organización prefieren utilizar el Visor de corrección de escritorio en lugar del Visor de corrección web para revisar el contenido interactivo, puede configurar el Visor de corrección de escritorio para que se inicie automáticamente cuando los usuarios abran revisiones de contenido interactivo. Para obtener información acerca del Visor de corrección de escritorio y en qué se diferencia del Visor de corrección web, consulte [Comprender el Visor de corrección de escritorio](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) e [Información general sobre las diferencias entre el Visor de corrección web y el Visor de corrección de escritorio](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. En Workfront, haga clic en el icono Workfront Proof de la barra de navegación global para acceder a Workfront Proof.

   ![Icono de revisión](assets/proof-access-proofhq-350x39.png)

1. Haga clic en **Configuración de la cuenta** cerca de la esquina superior derecha de Workfront Proof y, a continuación, haga clic en la ficha **Configuración**.

1. En **Valores predeterminados de la prueba**, al final de la fila **Visor de corrección de escritorio para revisión interactiva**, haga clic en **Configuración**.

1. Modifique la configuración del Visor de corrección de escritorio, tal como se describe en [Visor de corrección de escritorio](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer) en el artículo [Configurar las opciones de revisiones para su organización](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

1. Haga clic en **Guardar**.

## Configuración de dispositivos personalizados para pruebas interactivas

Puede añadir cualquier dispositivo personalizado al sistema, lo que permite a los usuarios revisar el contenido interactivo y simular cómo aparece el contenido en un dispositivo específico cuando utilizan el Visor de corrección de escritorio. (Esta funcionalidad no está disponible en el Visor de corrección web, donde los usuarios pueden revisar el contenido interactivo, pero solo tal y como aparece en varias resoluciones, no en varios dispositivos).

Para obtener más información, consulte [Cambiar la resolución de prueba interactiva en el visor de revisión](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. Desde Workfront, acceda a la interfaz de Workfront Proof como se describe en [Acceder a Workfront Proof desde Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).
1. Modifique la configuración del Visor de corrección de escritorio, tal como se describe en [Configurar dispositivos personalizados para revisiones](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) en el artículo [Configurar las opciones de revisiones para su organización](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).
