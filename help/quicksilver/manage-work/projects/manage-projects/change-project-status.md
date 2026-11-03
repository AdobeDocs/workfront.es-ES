---
product-area: projects
navigation-topic: manage-projects
title: Cambiar el estado de un proyecto
description: Puede actualizar manualmente el estado de un proyecto a cualquier otro estado, si es necesario. Puede actualizar manualmente el estado de un proyecto a un estado que equivalga a Completo solo cuando el modo de finalización del proyecto esté establecido en Manual.
author: Alina
feature: Work Management
exl-id: 80098514-fd44-436d-836b-bd9c1b52b3a9
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/PRLph0Euqn69SUFkRMT1N7BmJinnao-xfzMWWEE407Q
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 00706e8c7ed590cf112f4817da9740a970a4a4b3
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 85%
---
# Cambiar el estado de un proyecto

<!--Audited: 02/2024-->

Puede actualizar manualmente el estado de un proyecto a cualquier otro estado, si es necesario.

Puede actualizar manualmente el estado de un proyecto a un estado que equivalga a Completo solo cuando el modo de finalización del proyecto esté establecido en Manual.

De lo contrario, Adobe Workfront marca automáticamente el proyecto como Completo cuando todas las tareas y problemas del proyecto se completan y aprueban.

Para obtener más información acerca del modo de finalización del proyecto, vea [Editar proyectos](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

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
   <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos en el proyecto</p> </td> 
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
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard </p> 
   Or
   <p>Current: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Consideraciones sobre la actualización a estados específicos

* **Al actualizar un proyecto a Completo:** Asegúrese de que todas las tareas y problemas se hayan completado en el proyecto. No puede seleccionar el estado Completado de un proyecto ni ningún otro estado que equivalga a Completado cuando hay tareas o problemas que no se han completado en el proyecto. Esto incluye la aprobación de cualquier tarea o problema que esté en un estado de Aprobación completa-pendiente.
* **Al actualizar un proyecto de Completo a Actual:** Si se han completado todas las tareas y problemas del proyecto, asegúrese de que el modo de finalización del proyecto esté establecido en Manual. Si el modo de finalización del proyecto es automático, el estado del proyecto permanece completo.

<!--
* If a project status is deleted or becomes unavailable, the Status of the project displays as Not applicable.  As a user with Manage permissions to the project, you can update the status to a different one, or ask a Workfront administrator to recreate the status or add a new one. 
-->

<!--
IN THE ABOVE NOTE: ensure this is the status, because I asked for a change to "Not available"
ALSO: see in the steps below for more commented out text. 
-->

## Cambio del estado del proyecto

1. Vaya al proyecto cuyo estado desee actualizar.
1. En el encabezado del proyecto, haga clic en el nombre del estado en el campo **Estado** y, a continuación, seleccione un nuevo estado.

   ![Cambiar estado del proyecto](assets/change-project-status-in-header-drop-down-nwe-350x371.png)

   O

   Haga clic en el menú **Más** ![Menú más](assets/qs-more-menu.png) junto al nombre del proyecto, haga clic en **Editar**, seleccione un nuevo estado en el campo **Estado** y, a continuación, haga clic en **Guardar**.

   El estado del proyecto se actualiza al estado seleccionado.

<!--
1. (Conditional) When the status of the project is **Not applicable**, click the warning sign for the **Status** field, select a new status from the list, then click **Save**. (*****************VERIFY UI - I ASKED FOR "Not available)

  If you don't see an acceptable status, ask your administrator to create one.
-->
