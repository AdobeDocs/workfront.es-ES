---
product-area: projects
navigation-topic: task-information
title: Actualizar retraso de redistribución de tareas
description: A veces, puede haber conflictos entre las programaciones de tareas de un proyecto. Puede nivelar recursos o solucionar conflictos de recursos reprogramando recursos y tareas para que todas las tareas se puedan completar dentro de una programación realista. Para obtener información sobre las tareas de redistribución, consulte Recursos de nivel en el Diagrama de Gantt .
author: Alina
feature: Work Management
exl-id: 6695448c-76ce-460c-aa59-63a3d5e2e18d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 3%

---

# Actualizar retraso de redistribución de tareas

A veces, puede haber conflictos entre las programaciones de tareas de un proyecto. Puede nivelar recursos o solucionar conflictos de recursos reprogramando recursos y tareas para que todas las tareas se puedan completar dentro de una programación realista. Para obtener información sobre las tareas de redistribución, consulte [Recursos de nivel en el diagrama de Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

Como administrador de proyectos o como usuario asignado de tareas, también puede agregar un Retraso de Nivelación en tareas individuales para tener en cuenta cualquier conflicto de planificación o recurso. En otras palabras, una tarea podría programarse con un retraso para garantizar que, cuando Adobe Workfront escale las tareas, una programación más realista supere los conflictos de recursos.

Al añadir un retraso de redistribución a una tarea, se ajusta la Fecha de finalización prevista de la tarea. Para obtener información sobre la fecha de finalización prevista, consulte [Información general sobre la fecha de finalización prevista para proyectos, tareas y problemas](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas y proyectos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en Tareas </p> <p>Contribute o permisos superiores para Proyectos</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Agregar un retraso de redistribución a una tarea

1. Vaya a una tarea para la que desee agregar un retraso de redistribución.
1. Haga clic en el **Más icono** a la derecha del nombre de la tarea y haga clic en **Editar**.

   ![](assets/qs-task-edit-icon-highlighted-350x154.png)

1. Haga clic en **Configuración**.

   ![](assets/leveling-delay-edit-task-nwe-350x345.png)

1. Especifique la variable **Retraso de redistribución**, en horas, elija una unidad de tiempo.\
   Este es el momento en que el recurso se retrasa al iniciar la tarea debido a conflictos de recursos.

   Seleccione entre las siguientes opciones para las unidades de tiempo:

   * minutos
   * Horas. Este es el valor predeterminado.
   * Días
   * Semanas
   * Meses
   * Minutos transcurridos
   * Horas transcurridas
   * Días transcurridos
   * Semanas transcurridas
   * Meses transcurridos

   >[!TIP]
   >
   >El tiempo transcurrido es una unidad de tiempo para la duración de una tarea. Es la hora entre la Fecha de Inicio Planificado y la Fecha de Finalización Planificada de una tarea que incluye festivos, fines de semana y tiempo libre. En otras palabras, el tiempo transcurrido es el paso de días naturales.

1. Haga clic en **Guardar**. 

 
