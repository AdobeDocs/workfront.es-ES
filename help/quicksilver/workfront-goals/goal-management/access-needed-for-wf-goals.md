---
content-type: reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Requisitos para utilizar Workfront Goals
description: El administrador de Adobe Workfront debe asegurarse de que se cumplen determinadas condiciones para que pueda acceder a los objetivos de Adobe Workfront.
author: Alina
feature: Workfront Goals
exl-id: 3c7c832b-3e00-4ced-8829-8b1c23fa3871
source-git-commit: 86f9a88518c8a03643061b3328719d2da4016f2b
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Requisitos para utilizar Workfront Goals

El administrador de Adobe Workfront debe asegurarse de que se cumplen todas las condiciones siguientes para que pueda acceder a los objetivos de Adobe Workfront:

<!--drafted for P&P - replace the first bullet with this one when licensing changes: 
* Your company must purchase the correct Adobe Worfront plan or Adobe Workfront Goal license. For information, see the section [Obtain Workfront Goals organization access](#obtain-workfront-goals-organization-access)in this article.-->

* Su organización debe adquirir la licencia correcta para los objetivos de Workfront. Para obtener más información, consulte la sección [Obtener acceso a la organización de Workfront Goals](#obtain-workfront-goals-organization-access)en este artículo.

* Asigne el tipo correcto de licencia de Workfront. Para obtener información sobre la asignación de tipos de licencia y niveles de acceso, consulte la sección [Actualizar tipos de licencia y configuración de nivel de acceso](#update-license-types-and-access-level-settings) en este artículo.

>[!NOTE]
>
>Los usuarios con un tipo de licencia externa no pueden acceder a los objetivos de Workfront.

* Proporcionarle acceso a los objetivos en su nivel de acceso. Para obtener más información, consulte [Concesión de acceso a Adobe Workfront Goals](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

* Asigne la plantilla de diseño que incluya el área Objetivos en el menú principal.

  >[!NOTE]
  >
  >A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área Objetivos en el menú principal.

  Para obtener más información, consulte la sección [Añadir Workfront Goals a una plantilla de diseño](#add-workfront-goals-to-a-layout-template) en este artículo.

* Si debe modificar las metas que no creó usted mismo, el creador de las metas debe compartirlas con usted y darle permisos de administración para ellas.

  Para obtener más información, consulte la sección [Compartir objetivos individuales con otros usuarios](#share-individual-goals-with-other-users) en este artículo.

## Obtener acceso a la organización de Workfront Goals {#obtain-workfront-goals-organization-access}

<!--drafted for P&P release: 

If your company has a current Workfront plan, you must have one of the following:

* An Ultimate Workfront plan. Workfront Goals are included in this plan. 
* A Select or higher Workfront plan and a separate Workfront Goals license. -->

<!-- drafted for P&P - add this to the sentence below at release: 

If your company has a legacy Workfront plan, -->

Su organización debe adquirir una licencia adicional, además de la licencia de Workfront, para que los usuarios puedan acceder a los objetivos de Workfront. Una vez que su organización ha adquirido la licencia adicional, Workfront habilita los objetivos de Workfront en su cuenta. Para obtener información sobre cómo adquirir una licencia para los objetivos de Workfront, póngase en contacto con el administrador de cuentas de Workfront.

## Actualizar tipos de licencia y configuración de nivel de acceso  {#update-license-types-and-access-level-settings}

<!--drafted for P&P release: 
If your company has the current access level model, your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals: 

* Contributor
* Light
* Standard-->

<!--drafted for P&P release: add this to the first sentence: 
If your company has the legacy access level model, -->

El administrador de Workfront debe otorgarle uno de los siguientes tipos de licencia de Workfront para acceder a los objetivos de Workfront:

* Plan
* Trabajo
* Revisar
* Solicitud

Una vez que el administrador de Workfront le concede uno de estos tipos de licencia, también debe darle acceso a los Objetivos en su nivel de acceso. Para obtener información sobre el acceso a las Metas, consulte [Concesión de acceso a Adobe Workfront Goals](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

Como administrador de Workfront, puede revisar el número de licencias de Workfront Goals que hay en su sistema y saber cuántas hay habilitadas actualmente. Para obtener más información, consulte [Administrar las licencias disponibles en el sistema](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

>[!NOTE]
>
>Workfront le permite asignar más licencias de Workfront Goals que haya adquirido. Sin embargo, cuando asigne más licencias de las que permite su contrato de Workfront Goals, un administrador de cuentas de Workfront se pondrá en contacto con usted para informarle de que ha superado su número contractual.

## Añadir Workfront Goals a una plantilla de diseño {#add-workfront-goals-to-a-layout-template}

El administrador de Workfront o de grupo debe asignarle una plantilla de diseño que incluya el área Objetivos en el menú principal para que pueda acceder a los Objetivos de Workfront.

![](assets/layout-template-align-highlighted-350x220.png)

El administrador de Workfront o del grupo también puede añadir lo siguiente a la plantilla de diseño para que pueda acceder fácilmente a los objetivos de Workfront:

* Una pestaña anclada
* Convierta el área Objetivos en su página de aterrizaje

Para obtener información sobre la actualización de la plantilla de diseño, consulte los siguientes artículos:

* [Creación y administración de plantillas de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)
* [Personalización del menú principal mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
* [Personalización de páginas ancladas con una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
* [Personalización de la página de aterrizaje mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
* [Asignar usuarios a una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

## Compartir objetivos individuales con otros usuarios {#share-individual-goals-with-other-users}

De forma predeterminada, todos los usuarios que tengan al menos acceso de Visualización de metas en su nivel de acceso pueden ver todas las metas en Workfront.

Cualquier usuario con acceso de Edición en las Metas puede crear metas y obtener automáticamente acceso de Administración en las metas que cree. Si debe editar las metas de otros usuarios, alguien con permisos de Administración de esas metas debe compartir con ellos las metas que no creó.

Para obtener información sobre cómo compartir objetivos con los usuarios y concederles permisos de administración, consulte [Compartir una meta en Workfront Goals](../../workfront-goals/workfront-goals-settings/share-a-goal.md).
