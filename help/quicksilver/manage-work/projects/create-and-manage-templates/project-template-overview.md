---
product-area: templates
navigation-topic: templates-navigation-topic
title: Información general sobre la plantilla del proyecto
description: Puede utilizar plantillas de proyecto para capturar la mayoría de los procesos, la información y la configuración repetibles asociados a los proyectos de su organización.
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 1%

---

# Información general sobre la plantilla del proyecto

Puede utilizar plantillas de proyecto para capturar la mayoría de los procesos, la información y la configuración repetibles asociados a los proyectos de su organización.

Puede definir tareas, poner en cola temas, formularios personalizados y adjuntar documentos en la plantilla.

Después de crear plantillas, puede adjuntarlas a proyectos existentes o puede utilizarlas para crear nuevos proyectos. Toda la información de la plantilla se transfiere a los proyectos que se crean con ella.

## Ventajas del uso de plantillas en Adobe Workfront

A continuación se indican algunas de las ventajas de utilizar plantillas para crear sus proyectos:

* Le ahorra tiempo y esfuerzo al crear nuevos proyectos que son repetitivos.
* Tiene información coherente en todos los proyectos que tienen un alcance similar.
* Resulta útil al crear informes de proyectos. Por ejemplo, puede crear informes sobre proyectos que comparten la misma plantilla, comparar su progreso y encontrar mejoras en cómo se pueden completar.
* Además de definir la futura configuración del proyecto, puede añadir la siguiente información para el proyecto futuro en una plantilla:

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

* No asigne usuarios a tareas de plantilla. Aunque puede dejar las tareas sin asignar, le recomendamos que asigne funciones de trabajo a las tareas. Esto le dará una idea de qué usuarios pueden asignarse a las tareas cuando cree el proyecto con la plantilla.
* Asigne siempre a las tareas de plantilla un valor Duración y Horario planificado . Cada tarea del proyecto debe asociarse con una duración durante cuánto tiempo la tarea puede permanecer abierta y con un valor de hora planeada durante cuánto tiempo tardará realmente en completarse la tarea. Las tareas sin esta información no se pueden presupuestar correctamente para los recursos al utilizar herramientas de administración de recursos en Workfront.

   Para obtener información sobre la duración, consulte los siguientes artículos:

   * [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Descripción general de la duración del proyecto](../../../manage-work/projects/planning-a-project/project-duration.md)

   Para obtener información sobre las horas planificadas, consulte [Información general sobre las horas planificadas](../../../manage-work/tasks/task-information/planned-hours.md).

* Añada las relaciones predecesoras entre las tareas al final, cuando tenga una idea clara del futuro plan de proyecto en su totalidad. Añadir predecesores a tareas de plantilla es similar a añadir predecesores a tareas de un proyecto.

   Para obtener información sobre cómo agregar predecesores a tareas, consulte [Descripción general de las predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Indique con quién se debe compartir la plantilla para un uso futuro y con quién se deben compartir los proyectos que se crearán a partir de la plantilla. Para obtener información sobre cómo compartir plantillas, consulte [Compartir plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* Utilice procesos de aprobación globales y agréguelos a sus tareas de plantilla y plantilla si es posible. Esto ahorrará tiempo cuando las tareas o el proyecto futuro tengan que pasar por las mismas aprobaciones.

   Para obtener información sobre la creación de aprobaciones, consulte [Creación de un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   Para obtener información sobre cómo asociar un proceso de aprobación a un elemento de trabajo, consulte [Asociar un proceso de aprobación nuevo o existente al trabajo](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Formas de crear plantillas

Puede crear una nueva plantilla de las siguientes maneras:

* Desde cero.\
   Para obtener más información sobre la creación de una nueva plantilla desde cero, consulte [Creación de una plantilla de proyecto](../../../manage-work/projects/create-and-manage-templates/create-template.md).

* A partir de proyectos existentes, guardando un proyecto como plantilla.\
   Para obtener más información sobre la creación de plantillas a partir de proyectos existentes, consulte [Crear plantilla del proyecto](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md).

* Copiándolo desde otra plantilla.\
   Para obtener más información sobre cómo copiar una plantilla existente, consulte [Copiar una plantilla de proyecto](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Mediante el uso de las plantillas de ejemplo.\
   Para obtener más información sobre la creación de plantillas con las plantillas de ejemplo, consulte [Creación de plantillas de proyecto a partir de ejemplos](../../../manage-work/projects/create-and-manage-templates/create-templates-from-examples.md).
