---
product-area: projects
navigation-topic: plan-a-project
title: Determinar la estructura de desglose de trabajo de un proyecto
description: La definición de una estructura de desglose de trabajo (EDT) para un proyecto es un conjunto de actividades que en última instancia esbozan el plan del proyecto. El EDT divide el resultado del proyecto en elementos de trabajo manejables, que pueden utilizarse para definir hitos y organizar asignaciones de trabajo.
author: Alina
feature: Work Management
exl-id: a76c468d-6373-4dab-93ff-a0b3734f368c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1737'
ht-degree: 1%

---

# Determinar la estructura de desglose de trabajo de un proyecto

La definición de una estructura de desglose de trabajo (EDT) para un proyecto es un conjunto de actividades que en última instancia esbozan el plan del proyecto. El EDT divide el resultado del proyecto en elementos de trabajo manejables, que pueden utilizarse para definir hitos y organizar asignaciones de trabajo.

Debe tener una licencia de Plan con acceso de edición a Proyectos para crear la estructura de desglose de trabajo de un proyecto. Es posible que se necesite acceso adicional a otras áreas de Adobe Workfront, en función de cuántas actividades realice al crear el EDT.

Se recomienda mantener el proyecto en estado de Planning mientras se realizan cambios en la estructura de desglose de trabajo, para evitar notificaciones de déclencheur para los usuarios del equipo de proyecto.

## Definición de los resultados del proyecto

El objetivo de un proyecto es proporcionar resultados tangibles a las partes interesadas internas y externas. Los resultados de un proyecto son los que desea obtener completando el proyecto. Los resultados casi siempre están asociados con al menos un envío y todos los entregables deben estar asociados a un proyecto.

Los entregables del proyecto pueden ser bienes de consumo, producción intelectual (como informes) o servicios. Por ejemplo, si el ámbito del proyecto es crear una casa, algunos de los resultados pueden incluir:

* creación de planes arquitectónicos
* completar la instalación
* trabajo eléctrico
* verter la base
* trabajo de marco
* cerrar la venta de la casa.

Según su tamaño y alcance, un proyecto se puede componer de varios entregables.

Una vez identificados los entregables, puede empezar a desglosarlos en tareas. Las tareas son el resultado que obtiene para ofrecer el resultado general del proyecto. Al definir las tareas, tiene en cuenta los siguientes parámetros:

* Cantidad de tiempo necesaria para la finalización.
* Presupuesto necesario para completar el trabajo.
* Recursos necesarios para completar el trabajo.
* Programación de los recursos en función de la cronología lógica de las tareas.

A medida que define las tareas, asegúrese de no planificar demasiado trabajo para una tarea individual. Si el trabajo requerido en una tarea supera las 40 horas (una semana de trabajo típica), es posible que tenga que desglosar esa cantidad de trabajo en subtareas. La finalización de todas las subtareas completará la tarea principal.

Para definir los resultados y entregables de WBS en Workfront, le recomendamos que realice las siguientes actividades para crear una vista jerárquica de las tareas del proyecto:

* Si aún no lo ha hecho, cree un nuevo proyecto.\
   Para obtener información sobre la creación de un proyecto, consulte el artículo [Crear un proyecto](../../../manage-work/projects/create-projects/create-project.md).

* Cree tareas para todos los elementos de acción necesarios para completar cada resultado y entrega.\
   Para obtener información sobre la creación de tareas, consulte el artículo [Crear tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md) .

* A partir de las tareas que acaba de crear, identifique cuáles son los principales resultados y asócielos a hitos.\
   Para obtener información sobre la creación de tareas de hitos, consulte los artículos [Crear una ruta de hitos](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) y [Asociar hitos con tareas](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

* Desglose las tareas con un ámbito demasiado grande en subtareas. Asociarlos al elemento principal que define la entrega .\
   Para obtener información sobre la creación de subtareas, consulte el artículo [Crear subtareas](../../../manage-work/tasks/create-tasks/create-subtasks.md).

* Identifique las relaciones de dependencia entre subtareas y entre hitos.\
   En una relación de dependencia, el inicio de una tarea depende de la finalización de otra tarea o grupo de tareas.\
   Para obtener información sobre las dependencias de tareas, consulte los artículos [Descripción general de las predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) y [Crear una relación predecesora en la lista de tareas](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

* Determine si en algún momento de la duración del proyecto se necesitan aprobaciones y revisiones. Cree procesos de aprobación para satisfacer esta necesidad.\
   Para obtener información sobre las aprobaciones, consulte el artículo [Creación de un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Estimación de la programación de trabajo y las restricciones de programación

Una vez creado el hito básico y la estructura de tareas del proyecto, puede calcular el tiempo que tardará en completarse definiendo las restricciones y duraciones de las tareas.

Tenga en cuenta lo siguiente:

* Las restricciones de tareas definen cuándo debe comenzar o finalizar el trabajo en una tarea.

   Para obtener información sobre la definición de restricciones de tareas, consulte el artículo [Información general sobre la restricción de tareas](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* La duración de una tarea es el periodo de tiempo disponible para completarla. Al calcular la duración, puede que desee introducir un valor que tenga en cuenta la posibilidad de un retraso. Si proyectos similares se han completado en el pasado, es posible que tenga una buena idea de dónde establecer este valor.

   Como la duración es una estimación, asegúrese de establecer valores de tiempo optimistas para tener en cuenta los factores que podrían afectar a la tarea, como el clima, los cortes de energía, las dificultades del proveedor u otros eventos imprevistos. Además, asegúrese de considerar si hay tareas de predecesor o dependencia asociadas y cómo pueden imponer restricciones en el trabajo y afectar a la finalización de las tareas.

   Según el tipo de duración de la tarea, puede modificar la duración de una tarea durante la duración de un proyecto, pero esto también afectará a la escala de tiempo del proyecto. Para obtener información sobre la duración de una tarea, consulte el artículo [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) .

## Asignación de tareas

Después de definir la duración y las restricciones de cada tarea, puede determinar quién tiene el tiempo y las habilidades para realizar el trabajo. Puede asignar tareas a las siguientes entidades en Workfront:

* Usuarios\
   Solo se pueden asignar a las tareas los usuarios con un nivel de acceso de Planificador o Trabajador. Aunque puede asignar tareas a los solicitantes y revisores, no pueden completarlas. Por este motivo, no se recomienda asignarles tareas.

   Para obtener información sobre los niveles de acceso y cómo definen lo que los usuarios pueden hacer con los objetos de Workfront, consulte [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

* Roles
* Equipos

Para obtener información sobre la asignación de tareas, consulte los artículos de la sección [Asignación de tareas](../../../manage-work/tasks/assign-tasks/assign-tasks-1.md) para obtener más información.

## Administrar recursos

La administración de recursos en Workfront le permite determinar si hay personal adecuado para completar el proyecto. Cuando se agregan usuarios a un proyecto, Workfront muestra la utilización de cada usuario. Los administradores de recursos pueden ver la cantidad total de horas que la persona está asignada a otros proyectos durante el período de tiempo del proyecto.

>[!NOTE]
>
>Siempre que el proyecto tenga un estado de Planning, las tareas asignadas a los usuarios no aparecerán en sus listas de tareas.

Al principio de un año o trimestre fiscal, es posible que desee administrar los recursos en un nivel superior, en varios proyectos, sin tener conocimiento de una estructura de desglose de trabajo específica.\
Para obtener información sobre la planificación del uso de los recursos en un nivel superior, consulte el artículo [Introducción a la planificación de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planning.md).

Al administrar los recursos en el contexto de la creación de la estructura de desglose de trabajo de un proyecto y asegurarse de que cada tarea esté asignada al recurso correcto, está listo para programar los recursos para el trabajo que debe realizarse.\
Para obtener información sobre la programación de los recursos, consulte los artículos de la sección [Programación de recursos](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md) para obtener más información.

## Estimación de las finanzas de los proyectos

Workfront calculará los costes planeados para cada tarea y los costes generales de un proyecto. Los costes planeados para una tarea incluyen todos los gastos de la tarea más el coste del empleado o la función asignada a la tarea. Las tasas por hora para la tarea, la función y el empleado se asignan durante la tarea, la función y la creación del usuario.

Para obtener información sobre las finanzas del proyecto, consulte la sección [Finanzas del proyecto](../../../manage-work/projects/project-finances/project-finances-overview.md) .

## Determinar los puntos de aprobación del proyecto

Al crear Procesos de aprobación en Workfront, puede establecer puntos de revisión para el proyecto a fin de monitorizar el progreso y las posibles áreas problemáticas. A través del proceso de aprobación, los propietarios del proyecto pueden discernir qué tareas se tardan y empiezan, ver las pistas de auditoría que enumeran quién ha cambiado el estado de una tarea y ver historiales de problemas, incluido cómo se resolvieron los problemas y cuándo se cerraron. Tras revisar un proyecto, los propietarios del proyecto pueden determinar qué pasos tomar y actualizar el plan del proyecto, si es necesario.

Para obtener información sobre las aprobaciones, consulte el artículo [Creación de un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

## Ver el EDT

Para comprender el EDT de un proyecto, debe ver los siguientes elementos de tarea:

* Secuencia de tareas y cronología (fechas de inicio y finalización planificadas y duración de la tarea)
* Dependencias del predecesor
* Relación secundaria y principal
* Asignaciones

Una vez completado el EDT, puede verlo en una lista de tareas a nivel de proyecto o en un informe.

* [Ver el EDT en una lista de tareas](#view-the-wbs-in-a-task-list)
* [Ver el EDT en un informe de tareas](#view-the-wbs-in-a-task-report)

### Ver el EDT en una lista de tareas {#view-the-wbs-in-a-task-list}

Puede ver la lista de tareas en el nivel de proyecto.

1. Vaya al proyecto para el que desea ver la estructura de desglose de trabajo.
1. Seleccione el **Tareas** pestaña .
1. (Opcional) Seleccione **Nada** en el **Agrupación** menú desplegable.

   La estructura de desglose de trabajo no muestra la sangría de las tareas del EDT.

1. En el **Ver** menú desplegable y seleccione **Desglose de trabajo** vista.

   La estructura Desglose de trabajo aparece en la segunda columna de la vista seleccionada.

   ![](assets/wbs-view-on-task-list-nwe-350x87.png)

### Ver el EDT en un informe de tareas {#view-the-wbs-in-a-task-report}

Puede crear un informe de tareas y mostrar el EDT de las tareas realizando una de las siguientes acciones:

* Aplique al informe la vista Estructura de desglose de trabajo existente.
* Agregue la columna Estructura de desglose de trabajo a cualquier informe personalizado.

>[!TIP]
>
>Se recomienda añadir una agrupación de Project para añadir claridad a los proyectos a los que pertenecen las tareas. La sangría de las tareas no se muestra en un informe de tareas.

Para obtener información sobre la creación de informes, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Guardar el EDT de un proyecto como plantilla

Si trabaja en otros proyectos que siguen programas de trabajo similares a los del EDT que acaba de crear, puede que desee guardar el proyecto como una plantilla. Una plantilla ahorrará tiempo y esfuerzo al crear futuros proyectos relacionados.

Si su organización tiene poca rotación, considere la posibilidad de esperar hasta que se realicen asignaciones de usuario para guardar la plantilla. Independientemente de cuándo se guarde un proyecto como plantilla, las asignaciones de usuario o tareas específicas se pueden eliminar al adjuntar la plantilla a un nuevo proyecto.

Los siguientes elementos de una estructura de desglose de trabajo se pueden guardar en una plantilla para su uso futuro con otro proyecto:

* Dependencias del predecesor
* Asignaciones (incluidos Propietario del proyecto, Patrocinador y Administrador de recursos)
* Procesos de aprobación
* Restricciones de tareas
* Documentos
* Gastos y otra información financiera
* Metas
* Tipos de horas
* Estructura de la cola de solicitud
* Notificaciones de recordatorio
* Riesgos
* Tarifas de facturación
* Información compartida
* Formularios personalizados

Para obtener información sobre cómo guardar proyectos como plantillas, consulte el artículo [Crear plantilla del proyecto](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md) .
