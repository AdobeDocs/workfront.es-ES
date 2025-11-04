---
product-area: templates
navigation-topic: templates-navigation-topic
title: Eliminar plantillas de proyecto
description: Se recomienda desactivar las plantillas que ya no utilice, en lugar de eliminarlas, para poder conservar la información histórica sobre sus proyectos a lo largo del tiempo.
author: Alina
feature: Work Management
exl-id: 41e0979c-f8ef-4a07-8848-e4ee8cc212c5
source-git-commit: 87bf2a4485d3b0c29fcfe8e00dcca57874cdec04
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 9%

---

# Eliminar plantillas de proyecto

Se recomienda desactivar las plantillas que ya no utilice, en lugar de eliminarlas, para poder conservar la información histórica sobre sus proyectos a lo largo del tiempo. Para obtener información sobre cómo desactivar una plantilla, consulte [Editar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

>[!IMPORTANT]
>
>Al eliminar una plantilla, los proyectos que la utilizan no se modifican en modo alguno. Sin embargo, ya no puede ver el nombre de la plantilla original en el campo Plantilla del proyecto. Además, ya no puede ver los nombres de las tareas de plantilla para las tareas del proyecto en una vista de tareas. El campo Plantilla del proyecto y el campo Tarea de plantilla de las tareas permanecen en blanco después de que se elimine la plantilla asociada originalmente al proyecto.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a las plantillas que incluye el acceso a Eliminar</p> <td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para la plantilla que incluye permisos para eliminarla</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Templates that includes access to Delete</p> <p> <img src="assets/template-access-level-with-advanced-settings-350x113.png" style="width: 350;height: 113;"> </p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the template that includes permissions to Delete it</p> <p> <img src="assets/template-manage-permissions-with-advanced-settings-350x352.png" style="width: 350;height: 352;"> </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Consideraciones para eliminar plantillas

* Las tareas que se agregaron a los proyectos cuando se adjuntó la plantilla permanecen en los proyectos. Sin embargo, se elimina la información de la tarea de plantilla asociada con las tareas.
* El nombre de la plantilla ya no aparece en el campo **Plantilla** de la subpestaña **Información general** del proyecto.

* Puede recuperar una plantilla eliminada recientemente de la papelera de reciclaje. Para obtener información acerca de cómo recuperar elementos de la papelera de reciclaje, vea [Restaurar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Eliminación de una plantilla

{{step1-to-templates}}

Se abrirá una lista de plantillas

1. Seleccione la plantilla que desea eliminar haciendo clic en la casilla de verificación situada a la izquierda del nombre de la plantilla y, a continuación, haga clic en **Eliminar > Sí, eliminarla** para confirmar la eliminación.

   O

   Haga clic en el nombre de una plantilla para acceder a ella y, a continuación, haga clic en el menú **Más** ![Icono de más](assets/more-icon.png), luego en **Eliminar plantilla > Sí, eliminarla**.

   La plantilla ya no está disponible para asociarse a un proyecto.
