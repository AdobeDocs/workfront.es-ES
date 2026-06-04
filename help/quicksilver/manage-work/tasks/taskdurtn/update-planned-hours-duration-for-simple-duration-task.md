---
product-area: projects
navigation-topic: task-duration
title: Actualizar las horas planificadas y la duración de una tarea con un tipo de duración simple
description: De forma predeterminada, Adobe Workfront calcula la duración de una tarea con un tipo de duración simple en función de la cantidad de horas planificadas. Sin embargo, también puede editar manualmente la cantidad de horas planificadas y la duración de una tarea de duración simple en ciertas áreas de Workfront.
author: Alina
feature: Work Management
exl-id: 47a9b095-2b7d-4ed0-8cb6-e6bd5e37ce9c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/SLemiOnFj-dOnWtXjH6gNzHZdVaXfp47qB0xzVJkRck
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 450
ht-degree: 19%

---

# Actualización de las horas planificadas y la duración de una tarea con un tipo de duración simple

De forma predeterminada, Adobe Workfront calcula la duración de una tarea con un tipo de duración simple en función de la cantidad de horas planificadas. Sin embargo, también puede editar manualmente la cantidad de horas planificadas y la duración de una tarea de duración simple en ciertas áreas de Workfront.

Puede editar las horas planificadas y la duración de una tarea con un tipo de duración simple en línea o en el nivel de tarea en el área Asignaciones.

Para obtener más información sobre cómo editar información en línea, consulte [Editar elementos en línea en una lista en Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

En este artículo se describe cómo actualizar las horas y la duración planificadas de una tarea con un tipo de duración simple en el nivel de tarea, en el área Asignaciones.

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
   <td><p>Estándar o superior</p> 
   <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior a los proyectos</p> <p>Editar acceso a Tareas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar el acceso a la tarea </p></td> 
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
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Actualización de las horas planificadas y la duración de una tarea con un tipo de duración simple

>[!IMPORTANT]
>
>Después de actualizar manualmente la Duración de una tarea de Duración simple, Workfront deja de calcularla en función de las Horas planificadas.

Para editar las horas planificadas y la duración de una tarea con un tipo de duración simple en la ventana Asignaciones avanzadas:

1. En una lista de tareas, haga clic en el nombre de la tarea para la que desea cambiar el tipo de duración.
1. Realice una de las siguientes acciones:

   * Haga clic en el icono **Más** ![Más en un objeto](assets/qs-more-icon-on-an-object.png) junto al nombre de la tarea, haga clic en **Editar** y, a continuación, en **Asignaciones**.
   * Haga clic en **Asignado a** o en el nombre de las asignaciones en el área Asignaciones del encabezado de la tarea y, a continuación, haga clic en **Avanzado**.

1. Escriba un valor total de **Horas planificadas** para todas las asignaciones, por ejemplo, 10 horas. El número total de horas planificadas se distribuye equitativamente entre todos los recursos asignados a la tarea.
1. (Opcional) Ajuste manualmente las horas planificadas de cada recurso asignado a la tarea. El número total de horas planificadas para la tarea se actualiza para reflejar las nuevas horas asignadas individualmente a los recursos.
1. Escriba un valor para la tarea **Duration**, por ejemplo 2 días.

   ![Asignaciones avanzadas de duración simple con varios recursos](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. Haga clic en **Guardar**.
