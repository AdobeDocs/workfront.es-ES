---
content-type: reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Requisitos para utilizar los objetivos de Workfront
description: El administrador de Adobe Workfront debe asegurarse de que se cumplan ciertas condiciones antes de poder acceder a los objetivos de Adobe Workfront.
author: Alina
feature: Workfront Goals
exl-id: 3c7c832b-3e00-4ced-8829-8b1c23fa3871
source-git-commit: 4298659c6eaf7c0370d8d88454e54aeba70f48cf
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 0%

---

# Requisitos para utilizar los objetivos de Workfront

El administrador de Adobe Workfront debe asegurarse de que se cumplan todas las condiciones siguientes para poder acceder a los objetivos de Adobe Workfront:

<!--drafted for P&P - replace the first bullet with this one when licensing changes: 
* Your company must purchase the correct Adobe Worfront plan or Adobe Workfront Goal license. For information, see the section [Obtain Workfront Goals organization access](#obtain-workfront-goals-organization-access)in this article.-->

* Su organización debe adquirir la licencia correcta para los objetivos de Workfront. Para obtener más información, consulte la sección [Obtener acceso a la organización de objetivos de Workfront](#obtain-workfront-goals-organization-access)en este artículo.

* Asigne el tipo correcto de licencia de Workfront. Para obtener información sobre la asignación de tipos de licencia y niveles de acceso, consulte la sección [Actualizar tipos de licencia y configuración del nivel de acceso](#update-license-types-and-access-level-settings) en este artículo.

>[!NOTE]
>
>Los usuarios con un tipo de licencia externa no pueden acceder a los objetivos de Workfront.

* Proporciónele acceso a Objetivos en su nivel de acceso. Para obtener más información, consulte [Conceder acceso a los objetivos de Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

* Asigne una plantilla de diseño que incluya el área Objetivos del menú principal.

   Para obtener más información, consulte la sección [Agregar objetivos de Workfront a una plantilla de diseño](#add-workfront-goals-to-a-layout-template) en este artículo.

* Si debe modificar los objetivos que no ha creado usted mismo, el creador de objetivos debe compartir los objetivos con usted y otorgarle permisos de administración.

   Para obtener más información, consulte la sección [Compartir objetivos individuales con otros usuarios](#share-individual-goals-with-other-users) en este artículo.

## Obtener acceso a la organización de objetivos de Workfront {#obtain-workfront-goals-organization-access}

<!--drafted for P&P release: 

If your company has a current Workfront plan, you must have one of the following:

* An Ultimate Workfront plan. Workfront Goals are included in this plan. 
* A Select or higher Workfront plan and a separate Workfront Goals license. -->

<!-- drafted for P&P - add this to the sentence below at release: 

If your company has a legacy Workfront plan, -->

Su organización debe adquirir una licencia adicional, además de la licencia de Workfront, para que los usuarios puedan acceder a los objetivos de Workfront. Una vez que su organización compra la licencia adicional, Workfront habilita los objetivos de Workfront para su cuenta. Para obtener más información sobre la compra de una licencia para los objetivos de Workfront, póngase en contacto con su administrador de cuentas de Workfront.

## Actualizar tipos de licencia y configuración del nivel de acceso  {#update-license-types-and-access-level-settings}

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

Una vez que el administrador de Workfront le conceda uno de estos tipos de licencia, también debe darle acceso a Objetivos en su nivel de acceso. Para obtener información sobre el acceso a los objetivos, consulte [Conceder acceso a los objetivos de Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

Como administrador de Workfront, puede revisar la cantidad de licencias de Workfront en su sistema y comprender cuántas están habilitadas actualmente. Para obtener más información, consulte [Administre las licencias disponibles en su sistema](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

>[!NOTE]
>
>Workfront le permite asignar más licencias de objetivos de Workfront que haya adquirido. Sin embargo, cuando asigne más licencias de las que permite el contrato de objetivos de Workfront, un administrador de cuentas de Workfront se pondrá en contacto con usted para informarle de que ha superado su número contractual.

## Agregar objetivos de Workfront a una plantilla de diseño {#add-workfront-goals-to-a-layout-template}

El administrador de Workfront o de grupo debe asignarle una plantilla de diseño que incluya el área Objetivos en el menú Principal para poder acceder a los Objetivos de Workfront.

![](assets/layout-template-align-highlighted-350x220.png)

El administrador de Workfront o el administrador de grupos también pueden agregar lo siguiente a la plantilla de diseño para que pueda acceder fácilmente a los objetivos de Workfront:

* Una ficha fija
* Hacer que el área Objetivos sea su página de aterrizaje

Para obtener información sobre la actualización de la plantilla de diseño, consulte los siguientes artículos:

* [Creación y administración de plantillas de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)
* [Personalización del menú principal mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
* [Personalización de páginas ancladas mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
* [Personalización de la página de aterrizaje mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
* [Asignar usuarios a una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

## Compartir objetivos individuales con otros usuarios {#share-individual-goals-with-other-users}

De forma predeterminada, todos los usuarios que tengan al menos Ver acceso a Objetivos en su nivel de acceso pueden ver todos los objetivos en Workfront.

Cualquier usuario con acceso de edición a objetivos puede crear objetivos y automáticamente obtiene acceso de administración a los objetivos que crea. Si deben editar los objetivos de otros usuarios, alguien con permisos de administración para dichos objetivos debe compartir con ellos los objetivos que no han creado.

Para obtener información sobre cómo compartir objetivos con usuarios y darles permisos de administración, consulte [Compartir un objetivo en los objetivos de Workfront](../../workfront-goals/workfront-goals-settings/share-a-goal.md).
