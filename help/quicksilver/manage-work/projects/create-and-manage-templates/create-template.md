---
product-area: templates
navigation-topic: templates-navigation-topic
title: Crear una plantilla de proyecto
description: Puede crear y eliminar plantillas desde el área Plantillas. Al crear una plantilla nueva, puede introducir la información de todas las tareas y de la configuración futura del proyecto. Esta información se transferirá a cualquier proyecto que cree a partir de la plantilla.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 2%

---

# Crear una plantilla de proyecto

<!-- Audited: 1/2024 -->

Puede crear y eliminar plantillas desde el área Plantillas. Al crear una plantilla nueva, puede introducir la información de todas las tareas y de la configuración futura del proyecto. Esta información se transferirá a cualquier proyecto que cree a partir de la plantilla.

>[!NOTE]
>
>Una plantilla y sus tareas no tienen fechas reales, sino una indicación de qué día (a partir de cuándo podría comenzar el proyecto futuro) podría comenzar una tarea y en qué día debería completarse la tarea. Al utilizar plantillas para crear proyectos futuros, los proyectos recibirán fechas reales. Para obtener más información, consulte [Crear un proyecto](../create-projects/create-project.md).


Puede crear una nueva plantilla de las siguientes maneras:

* Desde cero, como se describe en este artículo.
* Desde proyectos existentes, guardando un proyecto como plantilla.

  Para obtener más información sobre cómo crear plantillas a partir de proyectos existentes, vea [Guardar un proyecto como plantilla](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* Copiándolo desde otra plantilla.

  Para obtener más información sobre cómo copiar una plantilla existente, vea [Copiar una plantilla de proyecto](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Mediante la importación de modelos. Debe ser administrador de Workfront para importar modelos. Para obtener más información, consulte [Configurar un modelo](../../../administration-and-setup/blueprints/configure-template-package.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Nuevo: estándar </p><p>O </p><p>Actual: plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Debe ser administrador del sistema para importar plantillas de modelos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a plantillas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>De forma predeterminada, tiene permisos de administración para las plantillas que crea</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creación de una plantilla

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Plantillas**.

1. Haga clic en **Nueva plantilla**.

   La plantilla no tiene título.

   ![Nueva plantilla](assets/create-template-nwe-2022-350x102.png)

1. Especifique un nombre para la nueva plantilla en el encabezado de la plantilla y, a continuación, presione **Intro.**
1. Haga clic en la sección **Tareas de plantilla** del panel izquierdo.
1. Haga clic en **Comenzar a agregar tareas de plantilla**.

   O

   Haga clic en **Nueva tarea de plantilla** para empezar a agregar tareas a la plantilla.

   Agregar tareas de plantilla a una plantilla es idéntico a agregar tareas a un proyecto.

   Para obtener más información sobre cómo agregar tareas a un proyecto, vea [Crear tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >No puede agregar tareas recurrentes a una plantilla.

1. (Opcional) Haga clic en el icono **Diagrama de Gantt** en la esquina superior derecha de la Lista de tareas para ver una representación visual de la lista de tareas de la plantilla.

   >[!TIP]
   >
   >No puede editar tareas directamente desde este gráfico Gantt.

1. Para agregar información a la nueva plantilla, haga clic en el menú **Más** ![](assets/more-icon.png) y, a continuación, haga clic en **Editar**.

   Para obtener información sobre cómo editar una plantilla, consulte [Editar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. Haga clic en **Guardar cambios**.
1. (Opcional) Si desea agregar elementos adicionales a la plantilla, consulte la sección [Agregar elementos adicionales a una plantilla](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#add-additional-items-to-a-template) en el artículo [Editar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Configuración de plantilla determinada por asociación de grupo

La asociación de una plantilla de proyecto con un grupo (o la falta de un grupo) afecta a la forma en que las preferencias de proyecto, tarea y problema determinan ciertas configuraciones en la plantilla. Para obtener más información, vea la sección [Crear y modificar plantillas de proyecto de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#create-and-modify-a-groups-project-templates) en el artículo [Crear y modificar plantillas de proyecto de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
