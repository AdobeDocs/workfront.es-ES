---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aplicar estados a trabajos asociados a un grupo
description: Si un proyecto está asociado con un grupo, puede aplicar tanto estados de nivel de sistema como un estado personalizado asociado con ese grupo al proyecto, tarea o problemas en ese proyecto.
author: Alina
feature: Work Management
exl-id: 7564ab6a-8ddf-4e76-8e45-d59f9cf8d38b
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---

# Aplicar estados a trabajos asociados a un grupo

<!--
Alina, I moved this out of an admin article about statuses (Create and customize statuses)
-->

Si un proyecto está asociado con un grupo, puede aplicar al proyecto estados de nivel de sistema, así como un estado personalizado asociado con ese grupo, o tareas y problemas en ese proyecto. Para obtener información sobre los estados de grupo en Adobe Workfront, consulte [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

>[!TIP]
>
>Solo puede asociar proyectos con grupos. Los problemas y las tareas heredan el grupo del proyecto al que pertenecen.

## Requisitos de acceso

<!--drafted for P&P:

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para el proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Actualizar el grupo y estado del proyecto

Al actualizar el Grupo para un proyecto, las opciones disponibles para Estado de las tareas, los problemas o el proyecto cambian para que coincidan con el grupo.

1. Vaya a un proyecto o cree un nuevo proyecto, tal como se describe en [Crear un proyecto](../../../manage-work/projects/create-projects/create-project.md).
1. Haga clic en el **Más** icono ![](assets/more-icon.png)y haga clic en **Editar**.

1. En el **Editar proyecto** que se muestra, cerca de la parte inferior del **Información general** , seleccione el grupo en la sección **Grupo** menú desplegable.

1. En el **Estado** menú desplegable, seleccione el estado personalizado.

   >[!NOTE]
   >
   >Si selecciona un grupo diferente en la variable **Grupo** menú desplegable, los estados personalizados en la **Estado** cambia automáticamente para correlacionar con el nuevo grupo.
   >
   >
   >![](assets/status-drop-down-expanded-with-custom-statuses-for-project-nwe.png)   >

1. Seleccione el estado del proyecto. Los estados personalizados que ha creado y aplicado a ese grupo se muestran en la lista.
