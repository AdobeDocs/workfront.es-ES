---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: Información general sobre restricciones de tarea
description: Las restricciones de tarea determinan cuándo debe comenzar y finalizar una tarea en un proyecto.
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: 91d757513792604677d6285baafa795629b4506d
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 6%

---

# Información general sobre restricciones de tarea

<!-- Audited: 12/2023 -->

Las restricciones de tarea determinan cuándo debe comenzar y finalizar una tarea en un proyecto.

## Información general sobre las restricciones de tarea

A medida que crea el plan del proyecto, toma decisiones sobre la secuencia y el lapso de tiempo de las tareas del proyecto. Las tareas pueden funcionar independientemente de cualquier secuencia de tareas, pero podrían afectar a la cronología del proyecto. Las restricciones de tareas permiten a un administrador de proyectos planificar cuándo se pueden iniciar o finalizar determinadas tareas en un proyecto.

Según la delimitación que utilice, es posible que tenga que especificar una Fecha planificada de inicio, una Fecha planificada de finalización o ambas para la tarea.

Los tipos de restricción que requieren fechas definidas afectan a las relaciones de predecesoras.

>[!TIP]
>
>Considere la posibilidad de utilizar un tipo de delimitación que no requiera fechas específicas si utiliza relaciones de predecesoras entre tareas.

En la tabla siguiente se muestra cada restricción y su abreviatura. Las abreviaturas se utilizan en listas de tareas y al crear archivos de importación de KickStart. Haga clic en el título vinculado de cada restricción de tarea para obtener más información sobre ese tipo de restricción.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col>
 <thead> 
  <tr> 
   <th> <p><strong>Nombre de restricción</strong> </p> </th> 
   <th> <p><strong>Abreviatura</strong> </p> </th> 
   <th> <p><strong>Descripción</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">Información General Sobre La Restricción De Tarea: Lo Antes Posible</a> </p> </td> 
   <td scope="col"> <p>LAP</p> </td>
   <td scope="col"> <p>Coloca la hora de inicio de la tarea lo más cerca posible del comienzo del proyecto.</p> 
   <p>Es la delimitación predeterminada si el proyecto utiliza un modo de programación desde la fecha de inicio y si la fecha de inicio predeterminada del sistema para una nueva tarea está establecida en Basado en la fecha planificada del proyecto. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">Información general sobre la restricción de tarea: lo más tarde posible </a> </p> </td> 
   <td scope="col"> <p>LMTP</p> </td> 
   <td scope="col"> <p>Coloca la hora de finalización de la tarea lo más cerca posible del final del proyecto.</p> 
   <p>Esta es la delimitación predeterminada cuando el modo de programación del proyecto es desde la fecha de finalización y el valor predeterminado del sistema o grupo para la fecha de inicio de una tarea se establece en Basado en la fecha planificada del proyecto. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">Información general sobre la restricción de tarea: lo más temprano disponible</a> </p> </td> 
   <td scope="col"> <p>LMTD</p> </td> 
 <td scope="col"> <p>Programa una tarea para que comience lo antes posible después de considerar las relaciones de predecesoras.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">Información general sobre la restricción de tarea: última hora disponible</a> </p> </td> 
   <td scope="col"> <p>LMTP</p> </td> 
   <td scope="col"> <p>Programa una tarea para que comience en el último tiempo disponible después de considerar las relaciones predecesoras-sucesoras en el proyecto.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">Información general sobre la restricción de tarea: No iniciar antes del </a> </p> </td> 
   <td scope="col"> <p>NIAD</p> </td> 
   <td scope="col"> <p>Programa una tarea para que comience después de la fecha especificada.</p> 
   <p>Esta es la delimitación predeterminada si el modo de programación del proyecto es desde la fecha de inicio y si la fecha de inicio predeterminada del sistema o grupo para una nueva tarea está establecida en Hoy.   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">Información general sobre la restricción de tarea: no iniciar después de </a> </p> </td> 
   <td scope="col"> <p>NIDD</p> </td> 
   <td scope="col"> <p>Programa una tarea para que comience antes de la fecha especificada.</p> 
   <p>Esta es la delimitación predeterminada si el modo de programación del proyecto es desde la fecha de finalización y si el sistema o grupo predeterminado para la fecha de inicio de una tarea está establecido en Hoy. 
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">Información general sobre la restricción de tarea: no finalizar antes del </a> </p> </td> 
   <td scope="col"> <p>NTAD</p> </td>
   <td scope="col"> <p>Programa una tarea para que se complete después de la fecha especificada.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">Información general sobre la restricción de tarea: no finalizar después de</a> </p> </td> 
   <td scope="col"> <p>NTDD</p> </td> 
   <td scope="col"> <p>Programa una tarea para que se complete antes de la fecha especificada.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">Información general sobre la restricción de tarea: debe comenzar el </a> </p> </td> 
   <td scope="col"> <p>DIE</p> </td> 
   <td scope="col"> <p>Programa una tarea para que comience exactamente en una fecha específica.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">Información general sobre la restricción de tarea: debe finalizar el</a> </p> </td> 
   <td scope="col"> <p>DFE</p> </td> 
   <td scope="col"> <p>Programa una tarea para que finalice en una fecha específica.</p> </td>
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">Resumen de restricción de tarea: fechas fijas</a> </p> </td> 
   <td> <p>FFJS</p> </td> 
   <td> <p>Programa una tarea para que comience y termine en fechas específicas.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Información general sobre las restricciones predeterminadas

Al crear nuevas tareas, Workfront selecciona automáticamente una Restricción de tarea.

Workfront utiliza dos variables para decidir qué restricción de tarea está seleccionada de forma predeterminada para una nueva tarea:

* El campo **Programación de proyecto a partir de** en el proyecto.

  Para obtener información acerca del campo Programación del proyecto desde, vea [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

* La preferencia **Fecha de inicio** configurada por el administrador del grupo o Workfront en el área **Tareas y problemas** del programa de instalación **Setup**.

  Para obtener información acerca de las preferencias de tareas y problemas, consulte la sección [Nuevos valores predeterminados de tarea](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#new-task-defaults) en [Configurar las preferencias de tareas y problemas en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

En la tabla siguiente se muestra la delimitación de tareas predeterminada al elegir distintas variables para el proyecto y las nuevas tareas:

| Programación de proyecto de | Fecha de inicio de tarea | Predeterminado de restricción de tarea |
|---|---|---|
| Fecha de inicio | En función de la fecha planificada del proyecto | Lo antes posible |
| Fecha de inicio | Hoy | No iniciar antes del |
| Fecha de finalización | En función de la fecha planificada del proyecto | Lo más tarde posible |
| Fecha de finalización | Hoy | No iniciar después del |
