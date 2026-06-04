---
product-area: projects
navigation-topic: use-predecessors
title: Crear relaciones de predecesoras encadenando tareas
description: Puede crear relaciones de predecesoras de varias formas en Adobe Workfront. Un método consiste en encadenar tareas.
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/iHJkCABzPdAjLYSlUTtXyBvQzU7eney-daOuvhXLbPQ
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
source-wordcount: 288
ht-degree: 96%

---

# Crear relaciones de predecesoras mediante el encadenamiento de tareas

Puede crear relaciones de predecesoras de varias formas en Adobe Workfront. Un método consiste en encadenar tareas.

Para obtener información acerca de las tareas predecesoras, consulte [Información general sobre las tareas predecesoras](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Al encadenar tareas, puede permitir que el sistema cree automáticamente las relaciones de predecesoras en las tareas seleccionadas, en lugar de crear manualmente una relación en cada tarea. Se pueden seguir utilizando distintos tipos de relación de predecesoras entre las tareas.

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
   <td><p>Estándar</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Tareas y Proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para las tareas y el proyecto</p></td> 
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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Standard </p>
    <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Encadenar tareas para crear relaciones de predecesoras

1. Vaya al proyecto que contiene las tareas que desea encadenar.
1. Haga clic en **Tareas** en el panel izquierdo.
1. (Condicional) Seleccione **Guardar automáticamente** en la esquina superior derecha de la lista de tareas y, a continuación, seleccione las tareas que desee encadenar.

   ![Icono de autoguardar en resaltado](assets/nwe-autosave-icon-on-highlighted-350x295.png)

   >[!IMPORTANT]
   >
   >No es posible encadenar tareas en una lista de tareas cuando se guardan manualmente los cambios realizados en las tareas o cuando se utiliza el modo Planificación de cronología para guardar tareas.

1. Haga clic con el botón derecho en las tareas seleccionadas y, a continuación, haga clic en **Encadenar**.
1. Seleccione entre los siguientes tipos de dependencia:

   * **Finalizar-Iniciar**
   * **Finalizar-Finalizar**
   * **Iniciar-Iniciar**
   * **Iniciar-Finalizar**

   Para obtener más información acerca de los tipos de dependencia de predecesoras, consulte [Información general sobre los tipos de dependencia entre tareas](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. (Opcional) Haga clic en **Desencadenar** si algunas de las tareas se han encadenado anteriormente.

   >[!CAUTION]
   >
   >Solo se quitan las predecesoras secuenciales mediante la opción de desencadenar al editar tareas de forma masiva.

   Las tareas seleccionadas ahora están vinculadas por relaciones de predecesoras.
