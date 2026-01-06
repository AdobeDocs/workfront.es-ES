---
product-area: templates
navigation-topic: templates-navigation-topic
title: Información general sobre plantillas de proyecto
description: Puede utilizar plantillas de proyecto para capturar la mayoría de los procesos, la información y la configuración repetibles asociados con los proyectos de su organización.
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 96%

---

# Información general sobre plantillas de proyecto

<!-- Audited: 12/2023 -->

Puede utilizar plantillas de proyecto para capturar la mayoría de los procesos, la información y la configuración repetibles asociados con los proyectos de su organización.

Defina tareas, temas de colas, formularios personalizados y adjunte documentos en plantillas.

Después de crear plantillas, adjúntelas a proyectos existentes o utilícelas para crear nuevos proyectos. Toda la información de la plantilla se transfiere a los proyectos creados con ella.

## Ventajas del uso de plantillas en Adobe Workfront

A continuación, se indican algunas de las ventajas del uso de plantillas para crear proyectos:

* Se ahorra tiempo y esfuerzo a la hora de crear nuevos proyectos repetitivos.
* Dispone de información coherente en todos los proyectos de ámbito similar.
* Resulta útil en la creación de informes sobre proyectos. Por ejemplo, es posible crear informes sobre proyectos que compartan la misma plantilla para comparar su progreso y mejorar la forma en que deberían completarse.
* Además de definir la configuración futura del proyecto, es posible añadir la siguiente información para el mismo en una plantilla:

   * Tareas
   * Documentos
   * Rutas de aprobación
   * Detalles de la cola
   * Temas de la cola
   * Grupos de temas
   * Reglas de enrutamiento
   * Formularios personalizados
   * Información sobre la compañía y grupo

## Prácticas recomendadas para la creación de plantillas

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is not an extensive list, but we are updating it as we go.)</p>
-->

Es necesario tener en cuenta lo siguiente al crear plantillas:

* No asignar usuarios a tareas de plantilla. Aunque puede dejar las tareas sin asignar, le recomendamos que asigne funciones a las tareas. Esto le dará una idea de qué usuarios podrían asignarse a las tareas al crear el proyecto con la plantilla.
* Asigne siempre un valor de duración y horas planificadas a las tareas de plantilla. Cada tarea del proyecto debería estar asociada a una duración que especifique cuánto tiempo permanecerá abierta la tarea y a un valor de hora planificada que indique cuánto tiempo realmente tardará la tarea en completarse. Las tareas que no tengan esta información no se podrán presupuestar correctamente para los recursos al utilizar las herramientas de administración de recursos de Workfront.

  Para obtener información sobre la duración, consulte los siguientes artículos:

   * [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Información general sobre la duración de un proyecto](../../../manage-work/projects/planning-a-project/project-duration.md)

  Para obtener información sobre las horas planificadas, consulte [Información general sobre horas planificadas](../../../manage-work/tasks/task-information/planned-hours.md).

* Añada las relaciones predecesoras entre las tareas al final, cuando tenga una comprensión clara del plan del proyecto futuro en su totalidad. La adición de predecesoras a las tareas de plantilla es similar a la adición de predecesoras a las tareas de un proyecto.

  Para obtener información acerca de cómo añadir predecesoras a las tareas, consulte [Información general sobre predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Indique con quién se compartirá la plantilla para uso futuro y con quién se compartirán los proyectos que se creen a partir de la plantilla. Para obtener información acerca de cómo compartir plantillas, consulte [Compartir plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* Utilice procesos de aprobación globales y añádalos a la plantilla y a las tareas de plantilla, si fuera posible. Con esto se ahorrará tiempo cuando se necesite que las tareas o el proyecto futuro pasen por las mismas aprobaciones.

  Para obtener información sobre la creación de aprobaciones, consulte [Creación de procesos de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  Para obtener información acerca de cómo asociar un proceso de aprobación a un elemento de trabajo, consulte [Asociación de procesos de aprobación nuevos o existentes con trabajos](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Formas de crear plantillas

Puede crear una nueva plantilla de las siguientes maneras:

* Desde cero\
  Para obtener más información sobre cómo crear plantillas nuevas desde cero, consulte [Creación de plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/create-template.md).

* Desde proyectos existentes, guardando un proyecto como plantilla.\
  Para obtener más información sobre cómo crear plantillas a partir de proyectos existentes, consulte [Creación de plantillas a partir de proyectos](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md).

* Copiándolo desde otra plantilla.\
  Para obtener más información sobre cómo copiar una plantilla existente, consulte [Copiar una plantilla de proyecto](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Utilizando nuestras plantillas de ejemplo.\
  Para obtener más información sobre cómo crear sus plantillas con nuestras plantillas de ejemplo, consulte [Crear plantillas de proyecto a partir de ejemplos](../../../manage-work/projects/create-and-manage-templates/create-templates-from-examples.md).
