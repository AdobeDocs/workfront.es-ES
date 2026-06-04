---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aplicar estados al trabajo asociado a un grupo
description: Si un proyecto está asociado a un grupo, puede aplicar tanto los estados de nivel de sistema como un estado personalizado asociado a ese grupo al proyecto, tarea o problemas de ese proyecto.
author: Alina
feature: Work Management
exl-id: 7564ab6a-8ddf-4e76-8e45-d59f9cf8d38b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/D6IbseeEu-prRZcdJNLvHvW-wSaclUAreufre9Fkyjo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 309
ht-degree: 90%

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

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p>
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos del proyecto</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:
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
   >![Se ha ampliado la lista desplegable de estado con los estados personalizados del proyecto](assets/status-drop-down-expanded-with-custom-statuses-for-project-nwe.png)
   >

1. Seleccione el estado del proyecto. Los estados personalizados que ha creado y aplicado a ese grupo se muestran en la lista.
