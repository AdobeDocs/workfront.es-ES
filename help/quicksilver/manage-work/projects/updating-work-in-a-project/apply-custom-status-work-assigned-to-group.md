---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aplicar estados al trabajo asociado a un grupo
description: Si un proyecto está asociado a un grupo, puede aplicar tanto los estados de nivel de sistema como un estado personalizado asociado a ese grupo al proyecto, tarea o problemas de ese proyecto.
author: Alina
feature: Work Management
exl-id: 7564ab6a-8ddf-4e76-8e45-d59f9cf8d38b
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 97%

---

# Aplicar estados al trabajo asociado a un grupo

<!--
Alina, I moved this out of an admin article about statuses (Create and customize statuses)
-->

Si un proyecto está asociado a un grupo, puede aplicar tanto los estados de nivel de sistema como un estado personalizado asociado a ese grupo al proyecto o a las tareas y problemas de ese proyecto. Para obtener información acerca de los estados de grupo en Adobe Workfront, consulte [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

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
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a proyectos</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos del proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Actualizar grupo y estado del proyecto

Al actualizar el grupo de un proyecto, las opciones disponibles para el estado de las tareas, problemas o el proyecto cambian para coincidir con el grupo.

1. Vaya a un proyecto o cree uno nuevo, tal como se describe en [Crear un proyecto](../../../manage-work/projects/create-projects/create-project.md).
1. Haga clic en el icono **Más** ![Más iconos](assets/more-icon.png) y, a continuación, haga clic en **Editar**.

1. En el cuadro **Editar proyecto** que aparece, cerca de la parte inferior de la sección **Información general**, seleccione el grupo en el menú desplegable **Grupo**.

1. En el menú desplegable **Estado**, seleccione el estado personalizado.

   >[!NOTE]
   >
   >Si selecciona un grupo diferente en el menú desplegable **Grupo**, los estados personalizados en el menú **Estado** cambian automáticamente para correlacionarse con el nuevo grupo.
   >
   >
   >![](assets/status-drop-down-expanded-with-custom-statuses-for-project-nwe.png)   >
   >

1. Seleccione el estado del proyecto. Los estados personalizados que ha creado y aplicado a ese grupo se muestran en la lista.
