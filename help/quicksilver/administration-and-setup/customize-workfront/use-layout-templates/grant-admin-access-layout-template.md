---
title: Concesión de acceso administrativo a una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Como administrador de Adobe Workfront, puede otorgar acceso administrativo a una plantilla de diseño a los administradores de grupo de un grupo en particular para que puedan editar la plantilla. Esto no asigna la plantilla a los usuarios del grupo.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 066a55ef-1904-4678-8866-c59428f78bc1
source-git-commit: a8214d9e10363881afbc2bd71f78f46cb6a25880
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# Concesión de acceso administrativo a una plantilla de diseño

Como administrador de Adobe Workfront, puede otorgar acceso administrativo a una plantilla de diseño a los administradores de grupo de un grupo en particular para que puedan editar la plantilla. Esto no asigna la plantilla a los usuarios del grupo.

Para obtener información acerca de cómo asignar usuarios a una plantilla de diseño, vea [Asignar usuarios a una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

Para obtener más información acerca de las plantillas de diseño, vea [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Para obtener información acerca de las plantillas de diseño para grupos, vea [Crear y modificar plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td><p>El nivel de acceso del administrador del sistema</p><p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Concesión de acceso administrativo a una plantilla de diseño

1. Empiece a trabajar en una plantilla de diseño, tal como se describe en [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Haga clic en **Conceder acceso a** en la sección superior de la página.
1. En el cuadro que aparece, haga clic en **Agregar un grupo**, empiece a escribir el nombre del grupo, haga clic en el nombre cuando aparezca y, a continuación, haga clic en **Listo**.

   Cualquier usuario designado como administrador del grupo que especifique podrá administrar la plantilla de diseño. Sin embargo, la plantilla no se asigna al miembro del grupo para su uso. Para obtener información acerca de cómo asignar una plantilla de diseño a un grupo, vea [Asignar una plantilla de diseño a los usuarios](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md#assign) en este artículo.

   >[!NOTE]
   >
   >* Cuando un administrador de grupo crea una plantilla de diseño, la asignación del acceso administrativo es obligatoria. La plantilla de diseño está designada y visible solo para el grupo especificado. Para obtener más información, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). Para obtener información sobre los administradores de grupos, consulte [Administradores de grupos](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).
   >   
   >* Si no concede acceso administrativo a los administradores del grupo en un grupo determinado, todos los usuarios que puedan editar cuentas de usuario tendrán acceso administrativo a la plantilla de diseño. Algunos administradores de Workfront eligen deliberadamente no conceder acceso administrativo a una plantilla de diseño para convertirla en una plantilla de diseño de nivel del sistema.

1. Puede hacer clic en Guardar en cualquier momento para guardar el progreso y seguir modificando la plantilla más adelante.
