---
title: Concesión de acceso administrativo a una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Como administrador de Adobe Workfront, puede otorgar acceso administrativo a una plantilla de diseño a los administradores de grupo de un grupo en particular para que puedan editar la plantilla. Esto no asigna la plantilla a los usuarios del grupo.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 066a55ef-1904-4678-8866-c59428f78bc1
source-git-commit: 76e32fa6b87583d2b8c296045da731afdb6d1f9a
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 99%

---

# Concesión de acceso administrativo a una plantilla de diseño

Como administrador de Adobe Workfront, puede otorgar acceso administrativo a una plantilla de diseño a los administradores de grupo de un grupo en particular para que puedan editar la plantilla. Esto no asigna la plantilla a los usuarios del grupo.

Para obtener información acerca de cómo asignar usuarios a una plantilla de diseño, vea [Asignar usuarios a una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

Para obtener más información acerca de las plantillas de diseño, vea [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Para obtener información sobre las plantillas de diseño para grupos, consulte [Crear y modificar las plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Para realizar estos pasos en el sistema, necesita el nivel de acceso de administrador del sistema.</p>
        <p>Para realizarlos para un grupo, debe ser administrador de ese grupo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

1. Puede hacer clic en **Guardar** en cualquier momento para guardar el progreso y luego seguir modificando la plantilla más adelante.
