---
product-area: projects
navigation-topic: plan-a-project
title: Información general sobre la planificación de un proyecto
description: Averigüe qué es un proyecto, cómo establecer su ámbito y estructura, así como conceptos clave como programaciones, escalas de tiempo y fechas de inicio y finalización.
author: Alina
feature: Work Management
recommendations: noDisplay, noCatalog
exl-id: 23372e16-3933-445d-977c-901f52299cb2
source-git-commit: 3cbcc2dd2efb457f5f0c4213110af54230a23eb0
workflow-type: tm+mt
source-wordcount: '1414'
ht-degree: 0%

---

# Información general sobre la planificación de un proyecto

<!--Audited: 01/2024-->

<!--
< see if you need to add something about approval settings and users's time off might add time to tasks' timelines - Ninja story 2019.3) </p>
-->

Un proyecto es un elemento de trabajo grande en Adobe Workfront. Puede desglosar un proyecto en tareas que sean elementos de trabajo más pequeños. Las tareas se pueden asignar a usuarios o equipos que puedan ser responsables de su finalización. Cuando todos los usuarios completan sus tareas, el proyecto también se completa.

Además de planificar las tareas de un proyecto, se incluyen muchos otros detalles en la planificación de proyectos. Desde determinar los impactos económicos hasta considerar la disponibilidad de recursos, hay muchos elementos de los proyectos que requieren atención.

## Establecer un ámbito de proyecto

La planificación del proyecto significa determinar exactamente qué objetivos principales debe lograr para completar el proyecto.

En las fases iniciales de un proyecto, es posible que aún no haya determinado si realmente debe realizar el proyecto. Puede que no sea rentable o que no tenga los recursos. En esta fase de planificación, puede crear un proyecto en Workfront sin añadir ninguna tarea y establecer el estado en Planificación.

Para obtener más información sobre cómo crear un proyecto, consulte el artículo [Crear un proyecto](../../../manage-work/projects/create-projects/create-project.md).

Tenga en cuenta las siguientes preguntas antes de planificar un proyecto:

* ¿Qué objetivos son obligatorios y cuáles son opcionales?
* ¿Tiene tiempo suficiente para lograr todos los objetivos o solo los objetivos principales?
* ¿Tiene presupuesto suficiente para lograr todos los objetivos ahora?

Con el caso comercial de un proyecto puede definir sus objetivos y asegurarse de que el proyecto se ajuste a la estrategia de su organización.

Para obtener más información acerca de cómo definir un caso empresarial para un proyecto, vea el artículo [Crear un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Una vez definido el ámbito general del proyecto, puede determinar si desea llevar a cabo el proyecto y comenzar a planificarlo.

## Planificación preliminar del proyecto

* [Definir la fecha de inicio y finalización del proyecto](#define-the-start-and-completion-date-of-the-project)
* [Definir la programación del proyecto](#define-the-project-schedule)
* [Administrar la información adicional necesaria para planificar el proyecto](#manage-additional-information-needed-for-planning-the-project)

### Defina la fecha de inicio y finalización del proyecto {#define-the-start-and-completion-date-of-the-project}

Al planificar un proyecto, una de las primeras cosas que debe determinar es la cronología: cuándo puede comenzar el proyecto y para qué hora debe completarse. Determine si hay una fecha límite establecida para cuándo debe finalizar el proyecto o si debe establecer un punto de partida y trabajar desde allí.

Puede programar un proyecto a partir de una fecha de inicio o a partir de la fecha de finalización. Puede establecer este atributo cuando cree inicialmente el proyecto y puede cambiarlo en cualquier momento editando el proyecto.

### Defina la programación del proyecto {#define-the-project-schedule}

Debe determinar una programación y asociarla al proyecto y a los usuarios responsables de completar las tareas del proyecto.

Considere la posibilidad de definir lo siguiente en una programación:

* Vacaciones
* Tiempo libre
* Número de horas disponibles para trabajar durante un día o una semana

Saber cuándo los usuarios están disponibles para trabajar es importante para comprender el progreso de las tareas en el proyecto.

Puede crear varias programaciones de proyectos y aplicar una programación predeterminada al proyecto. Se pueden aplicar programaciones personalizadas adicionales a diferentes personas.

Para obtener más información acerca de Programaciones, consulte el artículo [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

### Administrar la información adicional necesaria para planificar el proyecto {#manage-additional-information-needed-for-planning-the-project}

Al planificar un proyecto, hay información adicional que debe configurarse antes de que pueda comenzar a trabajar en él.

Considere la posibilidad de hacer las siguientes preguntas:

* ¿Existe una regulación que le ordene mantener un registro de los eventos y procesos? En caso afirmativo, ¿de qué debe hacer un seguimiento?\
  Workfront permite registrar ediciones, cambios de ámbito, cambios de estado y acciones para que pueda cumplir con las regulaciones específicas de su sector.\
  Para obtener más información sobre cómo definir qué actualizaciones rastrear en Workfront, consulte el artículo [Actualizaciones rastreadas por el sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

* ¿Hay alguna información que se le pida que rastree que no tenga un campo en Workfront en el que almacenarlo? Si es así, cree Forms personalizado para proyectos o tareas en los que pueda almacenar esta información.\
  Para obtener más información sobre la creación de formularios personalizados, consulte el artículo [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* ¿Hay algún punto de comprobación de aprobación que deba otorgarse antes de que pueda continuar el trabajo en un proyecto? Si es así, cree procesos de aprobación para proyectos o tareas que pueda utilizar mientras crea el proyecto.\
  Para obtener más información acerca de los procesos de aprobación, vea el artículo [Crear un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Crear la cronología del proyecto

Después de determinar los objetivos principales de un proyecto y de decidir si merece la pena ejecutarlo, debe calcular la cronología de cada objetivo. Cada objetivo puede convertirse en una de las tareas del proyecto.

Esto ayuda a priorizar los objetivos y a planificar la estructura de desglose de trabajo en consecuencia. La estructura de desglose de trabajo define la cronología del proyecto.\
Para obtener más información acerca de cómo crear tareas en un proyecto, vea la sección [Definir tareas](#define-tasks).

Tenga en cuenta lo siguiente al crear la cronología del proyecto:

* Desglose los objetivos más grandes en tareas secundarias y defina sus fechas de inicio y finalización.
* Determine si los objetivos dependen de otros objetivos.

  Puede configurar esas dependencias como predecesoras.

  Por ejemplo, podría tener un proyecto para construir un edificio de apartamentos. Uno de sus objetivos incluye la fontanería y otro es poner los cimientos. Una de sus tareas de fontanería es conectar a la línea principal de agua de la ciudad y esto debe hacerse antes de poner los cimientos. Sin embargo, la mayoría de sus otras tareas de fontanería no se pueden hacer hasta después de poner los cimientos. En este caso, debe considerar la posibilidad de utilizar predecesoras para comprender cuándo puede comenzar un objetivo una vez finalizado su requisito previo.

  Cuando se utilizan tareas principales para organizar objetivos, se puede crear una tarea para cada objetivo principal y agregar subtareas cuando se llega a la fase de dividir los objetivos principales en tareas individuales. Esto mantiene organizadas las tareas que forman parte del objetivo del proyecto.

  Para obtener más información acerca de las tareas predecesoras, vea [Información general sobre las tareas predecesoras](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Considere los objetivos más importantes para su proyecto y márquelos como tareas de hito.

  Se recomienda utilizar las tareas principales como hitos.

  Para obtener más información acerca del uso de tareas de hitos, vea [Crear una ruta de hitos](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* Defina una cronología para cada objetivo. Si trabaja con tareas principales, cada tarea secundaria debe tener una fecha de inicio y de finalización definidas. Hora entre la primera fecha de inicio de una tarea y la última fecha de finalización de una tarea en el mismo proyecto que resulta en la escala de tiempo del proyecto.

## Definición de tareas {#define-tasks}

A medida que define los objetivos del proyecto y las tareas asociadas con ellos, estará creando la cronología del proyecto.

Puede crear tareas en un proyecto de las siguientes maneras:

* Agregar tareas a un proyecto en edición en línea.
* Utilice una plantilla con tareas de plantilla definidas y agréguela al proyecto.

  Las Tareas de plantilla pasan a ser las Tareas del proyecto.

  Para obtener más información acerca de cómo crear tareas, vea el artículo [Crear tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Al definir tareas, tenga en cuenta lo siguiente:

* Defina la cronología de cada tarea. Esto se captura en el campo Duración de cada tarea.

  Para obtener información acerca de la duración de la tarea, vea el artículo [Información general sobre la duración de la tarea y el tipo de duración](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* Defina la relación principal-secundario entre las tareas.
* Defina la relación de predecesoras entre las tareas.
* Asocie una ruta de hitos al proyecto y asocie un hito a su tarea correspondiente.

  Para obtener más información acerca del uso de tareas de hitos, vea el artículo [Crear una ruta de hitos](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* Defina la cantidad de trabajo necesario para completar cada tarea. Esto se captura en el campo Horas planificadas de cada tarea.

  Para obtener más información sobre las horas planificadas, consulte el artículo [Resumen de horas planificadas](../../../manage-work/tasks/task-information/planned-hours.md).

* Asigne cada tarea a un usuario o equipo responsable de completarla.
* Compruebe la disponibilidad de los usuarios que está asignando a las tareas. Asegúrese de que son libres para trabajar y de que no están sobreasignados para poder completar las tareas asignadas. Si los usuarios están sobreasignados o tienen tiempo libre en sus programaciones, siga uno de estos procedimientos:

   * Reduzca las horas planificadas de cada tarea.
   * Agregue más usuarios a una tarea para asegurarse de que se puede completar durante el tiempo asignado para ella.
   * Reasigne las tareas a usuarios que estén disponibles sin otras restricciones.\
     Para obtener más información acerca de cómo planificar los recursos del proyecto, vea el artículo [Planificación de recursos: índice de artículos](../../../resource-mgmt/resource-planning/resource-planning-overview.md).\
     Para obtener más información sobre cómo programar los recursos para que realicen el trabajo en un proyecto, vea [Resumen del Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
