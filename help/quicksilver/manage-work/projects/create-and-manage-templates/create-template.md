---
product-area: templates
navigation-topic: templates-navigation-topic
title: Crear una plantilla de proyecto
description: Puede crear y eliminar plantillas desde el área Plantillas. Al crear una plantilla nueva, puede introducir la información de todas las tareas y de la configuración futura del proyecto. Esta información se transferirá a cualquier proyecto que cree a partir de la plantilla.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 96%

---

# Crear una plantilla de proyecto

<!-- Audited: 1/2024 -->

Puede crear y eliminar plantillas desde el área Plantillas. Al crear una plantilla nueva, puede introducir la información de todas las tareas y de la configuración futura del proyecto. Esta información se transferirá a cualquier proyecto que cree a partir de la plantilla.

>[!NOTE]
>
>Una plantilla y sus tareas no tienen fechas reales, sino una indicación de qué día (a partir de cuándo podría comenzar el proyecto futuro) podría comenzar una tarea y en qué día debería haberse completado la tarea. Cuando se utilizan plantillas para crear proyectos futuros, los proyectos recibirán fechas reales. Para obtener más información, consulte [Crear un proyecto](../create-projects/create-project.md).


Puede crear una nueva plantilla de las siguientes maneras:

* Desde cero, como se describe en este artículo.
* Desde proyectos existentes, guardando un proyecto como plantilla.

  Para obtener más información sobre cómo crear plantillas a partir de proyectos existentes, consulte [Guardar un proyecto como plantilla](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* Copiándolo desde otra plantilla.

  Para obtener más información sobre cómo copiar una plantilla existente, consulte [Copiar una plantilla de proyecto](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Mediante la importación de modelos. Debe ser administrador de Workfront para importar modelos. Para obtener más información, consulte [Configurar un modelo](../../../administration-and-setup/blueprints/configure-template-package.md).

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
   <td> <p>Estándar </p><p>Plan</p> <p>Debe ser administrador del sistema para importar plantillas de modelos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a las plantillas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>De forma predeterminada, tiene permisos de administración para las plantillas que crea</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
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
   <td> <p>New: Standard </p><p>Or </p><p>Current: Plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You must be a system administrator to import templates from Blueprints</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>You have Manage permissions to the templates you create, by default</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Creación de una plantilla

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Plantillas**.

1. Haga clic en **Nueva plantilla**.

   La plantilla no tiene título.

   ![Nueva plantilla](assets/create-template-nwe-2022-350x102.png)

1. Especifique un nombre para la nueva plantilla en el encabezado de la plantilla y, a continuación, presione **Intro.**
1. Haga clic en la sección **Tareas de plantilla** en el panel izquierdo.
1. Haga clic en **Empezar a añadir tareas de plantillas**.

   O

   Haga clic en **Nueva tarea de plantilla** para empezar a añadir tareas a la plantilla.

   El proceso de añadir tareas de plantilla a una plantilla es idéntico al de añadir tareas a un proyecto.

   Para obtener más información sobre cómo añadir tareas a un proyecto, consulte [Crear tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >No puede añadir tareas recurrentes a una plantilla.

1. (Opcional) Haga clic en el icono **Gráfico de Gantt** en la esquina superior derecha de la Lista de tareas para ver una representación visual de la lista de tareas de la plantilla.

   >[!TIP]
   >
   >No puede editar tareas directamente desde este gráfico Gantt.

1. Para agregar información a la nueva plantilla, haz clic en el **icono Más** del menú ![Más](assets/more-icon.png) y, a continuación, haz clic en **Editar**.

   Para obtener información sobre cómo editar una plantilla, consulte [Editar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. Haga clic en **Guardar cambios**.
1. (Opcional) Si desea añadir elementos adicionales a la plantilla, consulte la sección [Añadir elementos adicionales a una plantilla](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#add-additional-items-to-a-template) en el artículo [Editar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Configuración de plantilla determinada por asociación de grupo

La asociación de una plantilla de proyecto con un grupo (o la ausencia de un grupo) afecta al modo en que las preferencias del proyecto, la tarea y el problema determinan ciertas configuraciones de la plantilla. Para obtener más información, consulte la sección [Crear y modificar plantillas de proyecto de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#create-and-modify-a-groups-project-templates) en el artículo [Crear y modificar plantillas de proyecto de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
