---
product-area: projects
navigation-topic: manage-projects
title: Cambiar el estado de un proyecto
description: Puede actualizar manualmente el estado de un proyecto a cualquier otro estado, si es necesario. Puede actualizar manualmente el estado de un proyecto a un estado que equivalga a Completo solo cuando el modo de finalización del proyecto esté establecido en Manual.
author: Alina
feature: Work Management
exl-id: 80098514-fd44-436d-836b-bd9c1b52b3a9
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 91%

---

# Cambiar el estado de un proyecto

<!--Audited: 02/2024-->

Puede actualizar manualmente el estado de un proyecto a cualquier otro estado, si es necesario.

Puede actualizar manualmente el estado de un proyecto a un estado que equivalga a Completo solo cuando el modo de finalización del proyecto esté establecido en Manual.

De lo contrario, Adobe Workfront marca automáticamente el proyecto como Completo cuando todas las tareas y problemas del proyecto se completan y aprueban.

Para obtener más información acerca del modo de finalización del proyecto, vea [Editar proyectos](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nuevo: estándar </p> 
   O
   <p>Actual: plan </p>
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

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront. Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Consideraciones sobre la actualización a estados específicos

* **Al actualizar un proyecto a Completo:** Asegúrese de que todas las tareas y problemas se hayan completado en el proyecto. No puede seleccionar el estado Completado de un proyecto ni ningún otro estado que equivalga a Completado cuando hay tareas o problemas que no se han completado en el proyecto. Esto incluye la aprobación de cualquier tarea o problema que esté en un estado de Aprobación completa-pendiente.
* **Al actualizar un proyecto de Completo a Actual:** Si se han completado todas las tareas y problemas del proyecto, asegúrese de que el modo de finalización del proyecto esté establecido en Manual. Si el modo de finalización del proyecto es automático, el estado del proyecto permanece como Completado.

## Cambio del estado del proyecto

1. Vaya al proyecto cuyo estado desee actualizar.
1. En el encabezado del proyecto, haga clic en el nombre del estado en el campo **Estado** y, a continuación, seleccione un nuevo estado.

   ![Cambiar estado del proyecto](assets/change-project-status-in-header-drop-down-nwe-350x371.png)

   O

   Haga clic en el menú **Más** ![Menú más](assets/qs-more-menu.png) junto al nombre del proyecto, haga clic en **Editar**, seleccione un nuevo estado en el campo **Estado** y, a continuación, haga clic en **Guardar**.

   El estado del proyecto se actualiza al estado seleccionado.
