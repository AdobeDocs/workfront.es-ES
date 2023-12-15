---
product-area: templates
navigation-topic: templates-navigation-topic
title: Resumen de plantilla de proyecto
description: Puede utilizar plantillas de proyecto para capturar la mayoría de los procesos, la información y la configuración repetibles asociados con los proyectos de su organización.
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
source-git-commit: ca4da5302198d8fffc8b706baa3b3aeaa1f738e3
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 1%

---

# Resumen de plantilla de proyecto

<!-- Audited: 12/2023 -->

Puede utilizar plantillas de proyecto para capturar la mayoría de los procesos, la información y la configuración repetibles asociados con los proyectos de su organización.

Puede definir tareas, temas de colas, formularios personalizados y adjuntar documentos en la plantilla.

Después de crear las plantillas, puede adjuntarlas a proyectos existentes o puede utilizarlas para crear nuevos proyectos. Toda la información de la plantilla se transfiere a los proyectos creados con ella.

## Ventajas de usar plantillas en Adobe Workfront

A continuación se indican algunas de las ventajas de utilizar plantillas para crear proyectos:

* Le ahorra tiempo y esfuerzo al crear nuevos proyectos que son repetitivos.
* Tiene información coherente en todos los proyectos con un ámbito similar.
* Resulta útil a la hora de informar sobre proyectos. Por ejemplo, puede crear informes sobre proyectos que compartan la misma plantilla para comparar su progreso y encontrar mejoras en la forma de completarlos.
* Además de definir la configuración futura del proyecto, puede agregar la siguiente información para el proyecto futuro en una plantilla:

   * Tareas
   * Documentos
   * Rutas de aprobación
   * Detalles de cola
   * Temas de colas
   * Grupos de temas
   * Reglas de enrutamiento
   * Forms personalizado
   * Información de empresa y grupo

## Prácticas recomendadas para crear plantillas

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is not an extensive list, but we are updating it as we go.)</p>
-->

Tenga en cuenta lo siguiente al crear plantillas:

* No asignar usuarios a tareas de plantilla. Aunque puede dejar las tareas sin asignar, le recomendamos que asigne funciones a las tareas. Esto le dará una idea de qué usuarios podrían asignarse a las tareas cuando cree el proyecto con la plantilla.
* Asigne siempre un valor de Duración y Horas planificadas a las tareas de plantilla. Cada tarea del proyecto debe estar asociada con una duración para cuánto tiempo la tarea puede permanecer abierta y con un valor de Hora planificada para cuánto tiempo realmente tardará la tarea en completarse. Las tareas sin esta información no se pueden presupuestar correctamente para los recursos al utilizar las herramientas de administración de recursos en Workfront.

  Para obtener información sobre la duración, consulte los siguientes artículos:

   * [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Información general sobre la duración del proyecto](../../../manage-work/projects/planning-a-project/project-duration.md)

  Para obtener información sobre las horas planificadas, consulte [Resumen de horas planificadas](../../../manage-work/tasks/task-information/planned-hours.md).

* Agregue las relaciones de predecesoras entre las tareas al final, cuando tenga una comprensión clara del plan del proyecto futuro en su totalidad. Agregar predecesoras a tareas de plantilla es similar a agregar predecesoras a tareas de un proyecto.

  Para obtener información acerca de cómo agregar predecesoras a las tareas, vea [Información general sobre predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Indique con quién se debe compartir la plantilla para uso futuro y con quién se deben compartir los proyectos que se creen a partir de la plantilla. Para obtener información sobre cómo compartir plantillas, consulte [Compartir plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* Utilice procesos de aprobación globales y añádalos a las tareas de plantilla y plantilla, si es posible. Esto ahorrará tiempo cuando las tareas o el proyecto futuro necesiten pasar por las mismas aprobaciones.

  Para obtener información sobre la creación de aprobaciones, consulte [Crear un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  Para obtener información sobre cómo asociar un proceso de aprobación a un elemento de trabajo, consulte [Asociar un proceso de aprobación nuevo o existente con el trabajo](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Formas de crear plantillas

Puede crear una nueva plantilla de las siguientes maneras:

* Desde cero.\
  Para obtener más información sobre cómo crear una plantilla nueva desde cero, consulte [Creación de una plantilla de proyecto](../../../manage-work/projects/create-and-manage-templates/create-template.md).

* Desde proyectos existentes, guardando un proyecto como plantilla.\
  Para obtener más información sobre la creación de plantillas a partir de proyectos existentes, consulte [Crear plantilla a partir de proyecto](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md).

* Copiándolo desde otra plantilla.\
  Para obtener más información sobre cómo copiar una plantilla existente, consulte [Copiar una plantilla de proyecto](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Utilizando nuestras plantillas de ejemplo.\
  Para obtener más información sobre la creación de plantillas con nuestras plantillas de ejemplo, consulte [Crear plantillas de proyecto a partir de ejemplos](../../../manage-work/projects/create-and-manage-templates/create-templates-from-examples.md).
