---
product-area: projects
navigation-topic: plan-a-project
title: Información general sobre el plan de un proyecto
description: Información general sobre el plan de un proyecto
author: Alina
feature: Work Management
exl-id: 23372e16-3933-445d-977c-901f52299cb2
source-git-commit: 1834439ed43fb97c5287fc33abf860de77683e1b
workflow-type: tm+mt
source-wordcount: '1410'
ht-degree: 0%

---

# Información general sobre el plan de un proyecto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: see if you need to add something about approval settings and users's time off might add time to tasks' timelines - Ninja story 2019.3) </p>
-->

Un proyecto es un elemento de trabajo de gran tamaño en Adobe Workfront. Puede desglosar un proyecto en tareas que sean elementos de trabajo más pequeños, como tareas. Las tareas se pueden asignar a usuarios o equipos responsables de su finalización. Cuando todos los usuarios completan sus tareas, el proyecto también se completa.

Además de planificar las tareas en un proyecto, se incluyen muchos otros detalles en la planificación de proyectos. Desde la determinación de los efectos económicos hasta la consideración de la disponibilidad de recursos, hay muchos elementos de proyectos que necesitan atención. 

## Establecer un ámbito de proyecto

La planificación del proyecto significa determinar exactamente cuáles son los principales objetivos que debe alcanzar para completar el proyecto.

En las fases iniciales de un proyecto, es posible que aún no haya determinado si realmente debe hacerlo. Puede que no sea rentable o que no disponga de los recursos necesarios. En esta fase de planificación, puede crear un proyecto en Workfront sin añadir tareas y establecer el estado en planificación. 

Para obtener más información sobre la creación de un proyecto, consulte el artículo [Crear un proyecto](../../../manage-work/projects/create-projects/create-project.md).

Tenga en cuenta las siguientes preguntas antes de planificar un proyecto: 

* ¿Qué objetivos son obligatorios y cuáles son opcionales?
* ¿Tiene tiempo suficiente para alcanzar todos los objetivos o sólo los objetivos básicos?
* ¿Tienes suficiente presupuesto para lograr todos los objetivos ahora? 

Con el caso empresarial de un proyecto, puede definir sus objetivos y asegurarse de que el proyecto se ajuste a la estrategia de su organización. 

Para obtener más información sobre la definición de un caso de negocio para un proyecto, consulte el artículo [Creación de un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Una vez definido el ámbito general del proyecto, puede determinar si desea realizar el proyecto y empezar a planificarlo. 

## Planificación preliminar del proyecto

* [Definir la fecha de inicio y finalización del proyecto](#define-the-start-and-completion-date-of-the-project)
* [Definir la programación del proyecto](#define-the-project-schedule)
* [Administrar la información adicional necesaria para planificar el proyecto](#manage-additional-information-needed-for-planning-the-project)

### Definir la fecha de inicio y finalización del proyecto {#define-the-start-and-completion-date-of-the-project}

Al planificar un proyecto, una de las primeras cosas que debe determinar es la cronología: cuándo puede iniciarse el proyecto y a qué hora debe completarse. Determine si hay un plazo determinado para cuándo debe finalizar el proyecto o si debe establecer un punto de partida y trabajar desde allí. 

Puede programar un proyecto desde una fecha de inicio o desde la fecha de finalización. Puede configurar este atributo cuando cree el proyecto por primera vez y puede cambiarlo en cualquier momento editando el proyecto.

### Definir la programación del proyecto {#define-the-project-schedule}

Debe determinar una programación y asociarla al proyecto, así como a los usuarios responsables de completar las tareas del proyecto. 

Considere la posibilidad de definir lo siguiente en una programación:

* Vacaciones
* Tiempo de espera
* Número de horas disponibles para trabajar durante un día o una semana

Saber cuándo los usuarios están disponibles para trabajar es importante para comprender el progreso de sus tareas en el proyecto. 

Puede crear varias programaciones de proyectos y aplicar una programación predeterminada al proyecto. Pueden aplicarse programaciones personalizadas adicionales a diferentes personas.

Para obtener más información sobre las programaciones, consulte el artículo [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

### Administrar la información adicional necesaria para planificar el proyecto {#manage-additional-information-needed-for-planning-the-project}

Al planificar un proyecto, hay que configurar información adicional para poder empezar a trabajar en él. 

Considere la posibilidad de hacer las siguientes preguntas:

* ¿Existe alguna norma que obligue a mantener un registro de los eventos y procesos? En caso afirmativo, ¿qué debe rastrear?\
   Workfront permite registrar ediciones, cambios de ámbito, cambios de estado y acciones para poder cumplir con las regulaciones específicas de su sector.\
   Para obtener más información sobre la definición de las actualizaciones para rastrear en Workfront, consulte el artículo [Actualizaciones rastreadas por el sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

* ¡¿Se necesita alguna información para realizar un seguimiento que no tenga un campo en Workfront para almacenarlo en?! Si es así, cree Forms personalizado para proyectos o tareas en los que pueda almacenar esta información.\
   Para obtener más información sobre la creación de formularios personalizados, consulte el artículo [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* ¿Hay puntos de comprobación de aprobación que se deban conceder antes de que pueda continuar el trabajo en un proyecto? En caso afirmativo, cree Procesos de aprobación para proyectos o tareas que pueda utilizar mientras crea el proyecto.\
   Para obtener más información sobre los procesos de aprobación, consulte el artículo [Creación de un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Crear la cronología del proyecto

Después de determinar los principales objetivos de un proyecto y de decidir que vale la pena seguir con él, debe calcular la cronología de cada objetivo. Cada objetivo puede convertirse en una de sus tareas en el proyecto.

Esto le ayuda a priorizar sus objetivos y a planificar su estructura de desglose de trabajo en consecuencia. La estructura de desglose de trabajo define la cronología del proyecto.\
Para obtener más información sobre la creación de tareas en un proyecto, consulte el artículo [Definir tareas](#define-tasks).

Tenga en cuenta lo siguiente al crear la cronología del proyecto:

* Desglose objetivos más grandes en tareas secundarias y defina sus fechas de inicio y finalización.
* Determine si sus objetivos dependen de otros objetivos.

   Puede configurar esas dependencias como predecesoras.

   Por ejemplo, puede tener un proyecto para construir un edificio de departamentos. Uno de sus objetivos incluye la fontanería y otro es sentar las bases. Una de sus tareas de fontanería es conectar con la principal línea de agua de la ciudad y esto debe hacerse antes de poner los cimientos. Sin embargo, la mayoría de las demás tareas de fontanería no se pueden realizar hasta que no se haya puesto la base. En este caso, debe considerar la posibilidad de utilizar predecesores para comprender cuándo puede iniciarse un objetivo una vez finalizado su requisito previo.

   Cuando se utilizan tareas principales para organizar objetivos, se puede crear una tarea para cada objetivo principal y añadir subtareas cuando se llega a la etapa de dividir objetivos principales en tareas individuales. Esto mantiene las tareas que forman parte del objetivo organizado dentro del proyecto. 

   Para obtener más información sobre las predecesoras de tareas, consulte [Descripción general de las predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Considere los objetivos más importantes para su proyecto y marque como tareas hitos.

   Se recomienda usar tareas principales como hitos.

   Para obtener más información sobre el uso de tareas de hitos, consulte [Crear una ruta de hitos](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* Defina una cronología para cada objetivo. Si trabaja con tareas principales, cada tarea secundaria debe tener definida una fecha de inicio y finalización. La hora entre la fecha inicial más temprana de una tarea y la última fecha de finalización de una tarea en el mismo proyecto resulta en la cronología del proyecto. 

## Definir tareas {#define-tasks}

Al definir los objetivos del proyecto y las tareas asociadas a ellos, se crea la cronología del proyecto. 

Puede crear tareas en un proyecto de las siguientes maneras:

* Agregue tareas a un proyecto en la edición en línea.
* Utilice una plantilla con tareas de plantilla definidas y agréguela al proyecto. 

   Las tareas de plantilla se convierten en las tareas del proyecto. 

   Para obtener más información sobre la creación de tareas, consulte el artículo [Crear tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Al definir tareas, tenga en cuenta lo siguiente:

* Defina la cronología de cada tarea. Esto se captura en el campo Duration de cada tarea.

   Para obtener información sobre la duración de la tarea, consulte el artículo [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* Defina la relación padre-hijo entre las tareas.
* Defina la relación predecesora entre las tareas.
* Asocie una ruta de Milestone al proyecto y asocie un hito a su tarea respectiva. 

   Para obtener más información sobre el uso de tareas de hitos, consulte el artículo [Crear una ruta de hitos](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* Defina la cantidad de trabajo necesaria para completar cada tarea. Esto se captura en el campo Horario planificado de cada tarea.

   Para obtener más información sobre las horas planificadas, consulte el artículo [Información general sobre las horas planificadas](../../../manage-work/tasks/task-information/planned-hours.md).

* Asigne cada tarea a un usuario o equipo responsable de completarla. 
* Compruebe la disponibilidad de los usuarios que asigna a las tareas. Asegúrese de que son libres de trabajar y de que no están sobreasignados para poder completar las tareas asignadas. Si los usuarios están sobreasignados o tienen tiempo libre en sus programaciones, tenga en cuenta una de las siguientes opciones:

   * Reduzca las horas planificadas de cada tarea.
   * Agregue más usuarios a una tarea para asegurarse de que se pueda completar durante el tiempo asignado.
   * Vuelva a asignar las tareas a usuarios que no estén disponibles sin otras restricciones.\
      Para obtener más información sobre la planificación de los recursos del proyecto, consulte el artículo [Planificación de recursos en Adobe Workfront](../../../resource-mgmt/resource-planning/resource-planning-overview.md).\
      Para obtener más información sobre la programación de recursos para realizar el trabajo en un proyecto, consulte el artículo [Programación de recursos](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md).
