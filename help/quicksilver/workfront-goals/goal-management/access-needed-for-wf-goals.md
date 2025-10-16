---
content-type: reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Requisitos para utilizar las metas de Workfront
description: El administrador de Adobe Workfront debe asegurarse de que se cumplen determinadas condiciones para que pueda acceder a los objetivos de Adobe Workfront. En este artículo, aprenderá sobre los requisitos de acceso, permisos y diseño para acceder a las metas de Workfront.
author: Alina
feature: Workfront Goals
exl-id: 3c7c832b-3e00-4ced-8829-8b1c23fa3871
source-git-commit: dacfd8ef7475b197ac6ce5dd598c99df97037479
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 71%

---

# Requisitos para utilizar Workfront Goals

<!--Audited P&P only: 04/2025-->

El administrador de Adobe Workfront debe asegurarse de que se cumplan todas las condiciones siguientes antes de que pueda acceder a Adobe Workfront Goals:

* Su organización ha comprado un paquete de Objetivos de Adobe Workfront en el pasado. Adobe Workfront Goals ya no se puede adquirir.

  Para obtener más información, consulte la sección [Obtener acceso a la organización de Workfront Goals](#obtain-workfront-goals-organization-access) en este artículo.

* Asigne el tipo correcto de licencia de Workfront. Para obtener información acerca de la asignación de tipos de licencia y niveles de acceso, consulte la sección [Actualizar tipos de licencia y configuración de nivel de acceso](#update-license-types-and-access-level-settings) en este artículo.

  >[!NOTE]
  >
  >Los usuarios con un tipo de licencia externa no pueden acceder a Workfront Goals.

* Proporcionarle acceso a Goals en su nivel de acceso. Para obtener más información, consulte [Conceder acceso a Adobe Workfront Goals](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

  >[!NOTE]
  >
  >De forma predeterminada, los usuarios no tienen acceso a los objetivos de su nivel de acceso.


* Asigne la plantilla de diseño que incluya el área Metas en el menú principal.

  >[!NOTE]
  >
  >A todos los usuarios, incluidos los administradores del sistema, se les debe asignar una plantilla de diseño que incluya el área Objetivos en el menú principal.

  Para obtener información, consulte la sección [Añadir Workfront Goals a una plantilla de diseño](#add-workfront-goals-to-a-layout-template) en este artículo.

* Si debe modificar las metas que no creó usted mismo, el creador de las metas debe compartirlas con usted y concederle permisos de administración sobre ellas.

  Para obtener más información, consulte la sección [Compartir metas individuales con otros usuarios](#share-individual-goals-with-other-users) en este artículo.

## Obtener acceso a la organización de Workfront Goals {#obtain-workfront-goals-organization-access}

El último paquete de Adobe Workfront que incluyó los objetivos de Workfront fue Adobe Workfront Ultimate.
Los objetivos de Workfront ya no se pueden adquirir en paquetes más recientes.
Hable con el representante de su cuenta para consultar sobre los objetivos de Workfront.

<!--Old: >
Depending on which Workfront plan your company is currently on, the following scenarios exist: 

* **A new Workfront plan**: You must have an Ultimate Workfront plan. Workfront Goals are included only in this plan. 

* **A current Workfront plan**: Your organization must purchase an additional license, in addition to the Workfront license.

  After your organization purchases the additional license, Workfront enables Workfront Goals for your account. For information about purchasing a license for Workfront Goals contact your Workfront account manager.

For information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Actualizar tipos de licencia y configuración de nivel de acceso  {#update-license-types-and-access-level-settings}

Si su empresa tiene acceso a las metas de Workfront de una compra anterior, su administrador de Workfront debe concederle lo siguiente para acceder a las metas de Workfront:

1. Una de las siguientes licencias:

   * Colaborador o superior
   * Solicitud o superior

<!--Old: 
* **The new access level model**: Your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals: 

  * Contributor
  * Light
  * Standard

* **The current access level model**: Your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals:

  * Plan
  * Work 
  * Review
  * Request
-->

1. El siguiente nivel de acceso:

   * Vea o aumente el acceso a los Objetivos en su nivel de acceso.

   Para obtener información sobre el acceso a las metas, consulte [Conceder acceso a Adobe Workfront Goals](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

Como administrador de Workfront, puede revisar el número de licencias de Workfront Goals que hay en su sistema y saber cuántas están habilitadas actualmente. Para obtener más información, consulte [Administrar las licencias disponibles en el sistema](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

>[!NOTE]
>
>Workfront le permite asignar más licencias de Workfront Goals que haya adquirido. Sin embargo, cuando asigne más licencias de las que permite su contrato de Workfront Goals, un administrador de cuentas de Workfront se pondrá en contacto con usted para informarle de que ha superado su número contractual.

## Añadir Workfront Goals a una plantilla de diseño {#add-workfront-goals-to-a-layout-template}

El administrador de Workfront o de grupo debe asignarle una plantilla de diseño que incluya el área Metas en el menú principal para que pueda acceder a Workfront Goals.

![Plantilla de diseño](assets/layout-template-align-highlighted-350x220.png)

El administrador de Workfront o del grupo también puede añadir lo siguiente a la plantilla de diseño para que pueda acceder fácilmente a Workfront Goals:

* Una pestaña anclada
* Convierta el área Metas en su página de destino

Para obtener información sobre la actualización de la plantilla de diseño, consulte los siguientes artículos:

* [Crear y administrar plantillas de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)
* [Personalizar el menú principal con una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
* [Personalizar las páginas ancladas con una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
* [Personalizar la página de destino mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
* [Asignar usuarios a una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

## Compartir metas individuales con otros usuarios {#share-individual-goals-with-other-users}

De forma predeterminada, todos los usuarios que tengan al menos acceso de visualización a las metas en su nivel de acceso pueden ver todas las metas en Workfront.

Cualquier usuario con acceso de edición a las metas puede crear metas y obtener automáticamente acceso de administración a las metas que cree. Si tienen que editar las metas de otros usuarios, alguien con permisos de administración sobre esas metas debe compartir con ellos las metas que no crearon.

Para obtener información sobre el uso compartido de metas con los usuarios y concederles permisos de administración, consulte [Compartir una meta en Workfront Goals](../../workfront-goals/workfront-goals-settings/share-a-goal.md).
