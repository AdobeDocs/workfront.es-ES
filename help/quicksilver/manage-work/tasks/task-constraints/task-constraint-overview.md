---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: Información general sobre la restricción de tareas
description: Las restricciones de tareas determinan cuándo una tarea debe iniciarse y finalizar en un proyecto.
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 10%

---

# Información general sobre la restricción de tareas

Las restricciones de tareas determinan cuándo una tarea debe iniciarse y finalizar en un proyecto.

## Información general sobre las restricciones de tareas

A medida que crea el plan del proyecto, toma decisiones sobre la secuencia y el lapso de tiempo de las tareas en el proyecto. Las tareas pueden funcionar independientemente de cualquier secuencia de tareas, pero pueden afectar a la cronología del proyecto. Las restricciones de tareas permiten a un administrador de proyectos planificar cuándo se pueden iniciar o completar determinadas tareas en un proyecto.

Según la restricción que utilice, es posible que tenga que especificar una Fecha de Inicio Planificado, una Fecha de Finalización Planificada o ambas para la tarea.

Los tipos de restricción que requieren fechas definidas afectan a las relaciones predecesoras.

>[!TIP]
>
>Considere la posibilidad de utilizar un tipo de restricción que no requiera fechas específicas si utiliza relaciones predecesoras entre tareas.

La tabla siguiente muestra cada restricción y su abreviatura. Las abreviaturas se utilizan en listas de tareas y al crear archivos de importación de Inicio rápido. Haga clic en el título vinculado de cada restricción de tarea para obtener más información sobre ese tipo de restricción.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Nombre de restricción</strong> </p> </th> 
   <th> <p><strong>Abreviación</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">Información general sobre la restricción de tareas: Lo antes posible</a> </p> </td> 
   <td scope="col"> <p>LAP</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">Información general sobre la restricción de tareas: Tan Tarde como sea posible </a> </p> </td> 
   <td scope="col"> <p>LMTP</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">Información general sobre la restricción de tareas: Hora disponible más temprana</a> </p> </td> 
   <td scope="col"> <p>LMTD</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">Información general sobre la restricción de tareas: Última hora disponible</a> </p> </td> 
   <td scope="col"> <p>LMTP</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">Información general sobre la restricción de tareas: Iniciar antes de</a> </p> </td> 
   <td scope="col"> <p>NIAD</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">Información general sobre la restricción de tareas: Iniciar a más tardar</a> </p> </td> 
   <td scope="col"> <p>NIDD</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">Información general sobre la restricción de tareas: Finalizar no antes del</a> </p> </td> 
   <td scope="col"> <p>NTAD</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">Información general sobre la restricción de tareas: Finalizar a más tardar</a> </p> </td> 
   <td scope="col"> <p>NTDD</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">Información general sobre la restricción de tareas: Debe comenzar el</a> </p> </td> 
   <td scope="col"> <p>DIE</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">Información general sobre la restricción de tareas: Debe finalizar el</a> </p> </td> 
   <td scope="col"> <p>DFE</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">Información general sobre la restricción de tareas: Fechas fijas</a> </p> </td> 
   <td> <p>FFJS</p> </td> 
  </tr> 
 </tbody> 
</table>

## Información general sobre las restricciones predeterminadas

Al crear nuevas tareas, Workfront selecciona automáticamente una restricción de tareas.

Workfront usa dos variables para decidir qué restricción de tareas está seleccionada de forma predeterminada para una nueva tarea:

* La variable **Programación del proyecto desde** del proyecto.

   Para obtener información sobre el campo Programar desde, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

* La variable **Fecha de inicio** configurado por el administrador de grupo o Workfront en la variable **Tareas y problemas** área de **Configuración**.

   Para obtener información sobre las preferencias de Tareas y problemas, consulte la sección &quot;Nuevos valores predeterminados de tarea&quot; en [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

La tabla siguiente muestra la Restricción de tareas predeterminada al elegir distintas variables para el proyecto y las nuevas tareas:

| Programación del proyecto desde | Fecha de inicio de la tarea | Restricción de tarea predeterminada |
|---|---|---|
| Fecha de inicio | En función de la fecha planificada del proyecto | Lo antes posible |
| Fecha de inicio | Hoy | No iniciar antes del |
| Fecha de finalización | En función de la fecha planificada del proyecto | Tan tarde como sea posible |
| Fecha de finalización | Hoy | No iniciar después del |
