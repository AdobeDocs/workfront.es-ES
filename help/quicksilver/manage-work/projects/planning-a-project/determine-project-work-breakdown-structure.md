---
product-area: projects
navigation-topic: plan-a-project
title: Determinar la estructura de desglose de trabajo en un proyecto
description: La definición de una estructura de desglose de trabajo (EDT) para un proyecto es un conjunto de actividades que, en última instancia, describe el plan del proyecto. La EDT divide el resultado del proyecto en elementos de trabajo manejables, que se pueden utilizar para definir hitos y organizar asignaciones de trabajo.
author: Alina
feature: Work Management
exl-id: a76c468d-6373-4dab-93ff-a0b3734f368c
source-git-commit: dfd8dd07e1a88da872550163051e703f6aea5f74
workflow-type: tm+mt
source-wordcount: '1748'
ht-degree: 1%

---

# Determinar la estructura de desglose de trabajo en un proyecto

La definición de una estructura de desglose de trabajo (EDT) para un proyecto es un conjunto de actividades que, en última instancia, describe el plan del proyecto. La EDT divide el resultado del proyecto en elementos de trabajo manejables, que se pueden utilizar para definir hitos y organizar asignaciones de trabajo.

Debe tener una licencia de planificación con acceso de edición en Proyectos para crear la estructura de desglose de trabajo de un proyecto. Es posible que se necesite un acceso adicional a otras áreas de Adobe Workfront, en función de cuántas actividades realice al crear la EDT.

Se recomienda mantener el proyecto en estado de Planificación mientras se realizan cambios en la estructura de desglose de trabajo para evitar que se notifiquen déclencheur a los usuarios del equipo del proyecto.

## Definición de las entregas del proyecto

El propósito de un proyecto es proporcionar resultados tangibles a las partes interesadas internas y externas. Las entregas de un proyecto son los resultados que desea lograr al completar el proyecto. Los resultados casi siempre están asociados con al menos un resultado, y todos los resultados deben asociarse con un proyecto.

Los entregables del proyecto pueden ser bienes de consumo, producción intelectual (como informes) o servicios. Por ejemplo, si el ámbito del proyecto es construir una casa, algunos de los entregables pueden incluir:

* creación de planos arquitectónicos
* terminación de fontanería
* trabajo eléctrico
* derramamiento de la base
* trabajo encuadramiento
* cerrando la venta de la vivienda.

Según su tamaño y ámbito, un proyecto puede estar formado por varios entregables.

Una vez identificados los entregables, puede empezar a desglosarlos en tareas. Las tareas son los resultados que se obtienen para ofrecer el resultado general del proyecto. Al definir las tareas, debe tener en cuenta los siguientes parámetros:

* Cantidad de tiempo necesaria para finalizar.
* Presupuesto necesario para completar el trabajo.
* Recursos necesarios para completar el trabajo.
* Programación de los recursos en función de la cronología lógica de las tareas.

A medida que defina las tareas, asegúrese de no planificar demasiado trabajo para una tarea individual. Si el trabajo requerido en una tarea es de más de 40 horas (una semana de trabajo típica), es posible que tenga que desglosar esa cantidad de trabajo en subtareas. La finalización de todas las subtareas completará la tarea principal.

Para definir los resultados de la EDT y los entregables en Workfront, se recomienda realizar las siguientes actividades para crear una vista jerárquica de las tareas del proyecto:

* Si aún no lo ha hecho, cree un nuevo proyecto.\
  Para obtener información sobre cómo crear un proyecto, consulte el artículo [Creación de un proyecto](../../../manage-work/projects/create-projects/create-project.md).

* Cree tareas para todos los elementos de acción necesarios para completar cada resultado y entrega.\
  Para obtener información sobre la creación de tareas, consulte el artículo [Creación de tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md) .

* A partir de las tareas que acaba de crear, identifique cuáles son los resultados principales y asócielos a hitos.\
  Para obtener información sobre la creación de tareas de hitos, consulte los artículos [Creación de una trayectoria del hito](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) y [Asociar hitos a tareas](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

* Desglose las tareas con un ámbito demasiado grande en subtareas. Asociarlos con el elemento principal que define la entrega\
  Para obtener información sobre cómo crear subtareas, vea el artículo [Creación de subtareas](../../../manage-work/tasks/create-tasks/create-subtasks.md).

* Identificar relaciones de dependencia entre subtareas y entre hitos.\
  En una relación de dependencia, el inicio de una tarea depende de la finalización de otra tarea o grupo de tareas.\
  Para obtener información sobre las dependencias entre tareas, consulte los artículos [Información general sobre predecesoras de tareas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) y [Crear una relación de predecesoras en la lista de tareas](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

* Determine si en algún momento de la duración del proyecto se necesitan aprobaciones y revisiones. Cree procesos de aprobación para satisfacer esta necesidad.\
  Para obtener información sobre las aprobaciones, consulte el artículo [Crear un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Calcular las restricciones de horario y horario de trabajo

Una vez creado el hito básico y la estructura de tareas del proyecto, puede calcular el tiempo que tardará en completar el proyecto general definiendo las restricciones y duraciones de las tareas.

Tenga en cuenta lo siguiente:

* Las restricciones de tareas definen cuándo debe comenzar o finalizar el trabajo en una tarea.

  Para obtener información sobre la definición de delimitaciones de tareas, vea el artículo [Información general sobre restricciones de tarea](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* La duración de una tarea es el periodo de tiempo disponible para completar una tarea. Al calcular la Duración, es posible que desee introducir un valor que tenga en cuenta la posibilidad de un retraso. Si se han completado proyectos similares en el pasado, es posible que tenga una buena idea de dónde establecer este valor.

  Como la duración es una estimación, asegúrese de establecer valores de tiempo optimistas para tener en cuenta los factores que podrían afectar a la tarea, como el clima, los cortes de energía, las dificultades del proveedor u otros eventos imprevistos. Además, asegúrese de tener en cuenta si hay alguna tarea predecesora o de dependencia asociada y cómo pueden establecer restricciones en el trabajo y afectar a la finalización de la tarea.

  Según el tipo de duración de la tarea, puede modificar la duración de una tarea durante la duración de un proyecto, pero esto también afectará a la cronología del proyecto. Para obtener información sobre la duración de una tarea, consulte el artículo [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) .

## Asignar tareas

Después de definir la duración y las restricciones de cada tarea, puede determinar quién tiene el tiempo y las habilidades para realizar el trabajo. Puede asignar tareas a las siguientes entidades en Workfront:

* Usuarios\
  Solo los usuarios con un nivel de acceso de Planificador o Trabajador pueden asignarse a tareas. Aunque puede asignar tareas a los solicitantes y a los revisores, no pueden completarlas. Por este motivo, no se recomienda asignarles tareas.

  Para obtener información sobre los niveles de acceso y cómo definen lo que los usuarios pueden hacer con los objetos de Workfront, consulte [Información general sobre niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

* Roles
* Equipos

Para obtener información sobre la asignación de tareas, consulte los artículos de la [Asignar tareas](../../../manage-work/tasks/assign-tasks/assign-tasks-1.md) sección.

## Administración de recursos

La administración de recursos en Workfront le permite determinar si hay personal suficiente para completar el proyecto. Cuando se agregan usuarios a un proyecto, Workfront muestra el uso de cada usuario. Los gerentes de recursos pueden ver el número total de horas que la persona está asignada a otros proyectos durante el marco de tiempo del proyecto.

>[!NOTE]
>
>Siempre que el proyecto tenga un estado de Planificación, las tareas asignadas a los usuarios no aparecen en sus listas de tareas.

Al principio de un año o trimestre fiscal, puede que desee administrar los recursos en un nivel superior, en varios proyectos, sin tener conocimientos de una estructura de desglose de trabajo específica.\
Para obtener información sobre cómo planificar el uso de los recursos en un nivel superior, consulte el artículo [Introducción a la planificación de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planning.md).

Cuando administra los recursos en el contexto de la creación de la estructura de desglose de trabajo de un proyecto y se asegura de que cada tarea se asigna al recurso correcto, está listo para programar los recursos para el trabajo que se debe realizar.\
Para obtener información sobre cómo programar los recursos, consulte los artículos de la [Índice de artículos del Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/workload-balancer.md) sección.

## Estimar las finanzas del proyecto

Workfront calculará los costes planificados para cada tarea y los costes globales de un proyecto. Los costes planificados para una tarea incluyen todos los gastos de la tarea más el coste del empleado o rol asignado a la tarea. Las tarifas por hora de la tarea, el rol y el empleado se asignan durante la creación de la tarea, el rol y el usuario.

Para obtener información sobre las finanzas del proyecto, consulte la sección [Finanzas del proyecto](../../../manage-work/projects/project-finances/project-finances-overview.md) .

## Determinar puntos de aprobación para el proyecto

Al crear los procesos de aprobación en Workfront, puede establecer puntos de revisión para el proyecto a fin de supervisar el progreso y las posibles áreas problemáticas. A través del proceso de aprobación, los propietarios del proyecto pueden discernir qué tareas se retrasan y se adelantan, ver las pistas de auditoría que enumeran quién cambió el estado de una tarea y ver los historiales de problemas, incluidos cómo se resolvieron los problemas y cuándo se cerraron. Al revisar un proyecto, los propietarios del proyecto pueden determinar qué pasos deben seguir y actualizar el plan del proyecto, si es necesario.

Para obtener información sobre las aprobaciones, consulte el artículo [Crear un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

## Ver su WBS

Para comprender la EDT de un proyecto, desea ver los siguientes elementos de tarea:

* Secuencia de tareas y escala de tiempo (fechas planificadas de inicio y finalización y duración de las tareas)
* Dependencias de predecesoras
* Relación principal y secundaria
* Asignaciones

Una vez completada la EDT, puede verla en una lista de tareas a nivel de proyecto o en un informe.

* [Ver la EDT en una lista de tareas](#view-the-wbs-in-a-task-list)
* [Ver la EDT en un informe de tareas](#view-the-wbs-in-a-task-report)

### Ver la EDT en una lista de tareas {#view-the-wbs-in-a-task-list}

Puede ver la lista de tareas en el nivel de proyecto.

1. Vaya al proyecto para el que desea ver la estructura de desglose de trabajo.
1. Seleccione el **Tareas** pestaña.
1. (Opcional) Seleccione **Nada** en el **Agrupación** menú desplegable.

   La estructura de desglose de trabajo no muestra la sangría de las tareas en la EDT.

1. Desde el **Ver** menú desplegable y seleccione la opción **Desglose de trabajo** vista.

   La estructura de desglose de trabajo se muestra en la segunda columna de la vista seleccionada.

   ![Estructura de desglose de trabajo en una lista de tareas](assets/work-breakdown-structure.png)

### Ver la EDT en un informe de tareas {#view-the-wbs-in-a-task-report}

Puede generar un informe de tareas y mostrar la EDT de las tareas realizando una de las siguientes acciones:

* Aplique la vista Estructura del desglose de trabajo existente al informe.
* Agregue la columna Estructura del desglose de trabajo a cualquier informe personalizado.

>[!TIP]
>
>Se recomienda agregar una agrupación de proyecto para aclarar a qué proyectos pertenecen las tareas. La sangría de las tareas no se muestra en un informe de tareas.

Para obtener información sobre la creación de informes, consulte el artículo [Creación de un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Guardar la EDT de un proyecto como plantilla

Si trabaja en otros proyectos que siguen programaciones de trabajo similares a la EDT que acaba de crear, es posible que desee guardar el proyecto como plantilla. Una plantilla ahorrará tiempo y esfuerzo al crear futuros proyectos relacionados.

Si su organización tiene poca rotación, considere la posibilidad de esperar hasta que se realicen las asignaciones de los usuarios para guardar la plantilla. Independientemente de cuándo se guarde un proyecto como plantilla, las asignaciones de usuarios o las tareas específicas se pueden quitar al adjuntar la plantilla a un nuevo proyecto.

Los siguientes elementos de una estructura de desglose de trabajo se pueden guardar en una plantilla para su uso futuro con otro proyecto:

* Dependencias de predecesoras
* Asignaciones (incluidos Propietario del proyecto, Patrocinador y Administrador de recursos)
* Procesos de aprobación
* Restricciones de tarea
* Documentos
* Gastos y otra información financiera
* Metas
* Tipos de horas
* Estructura de cola de solicitudes
* Notificaciones de recordatorio
* Riesgos
* Tarifas de facturación
* Compartir información
* Formularios personalizados

Para obtener información sobre cómo guardar proyectos como plantillas, consulte el artículo [Crear plantilla a partir de proyecto](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md) .
