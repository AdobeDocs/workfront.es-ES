---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Estados de tareas del sistema
description: Los tres estados de tareas del sistema integrados en Workfront son obligatorios, lo que significa que puede desbloquearlos, cambiarles el nombre y reordenarlos, pero no puede ocultarlos ni eliminarlos. También puede agregar nuevos estados de tareas del sistema para adaptarlos a las necesidades de su organización. El cambio del estado de una tarea suele ser un proceso manual, pero a veces el estado de una tarea cambia automáticamente, según otros factores que estén ocurriendo en el sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b8c751c3-aed3-4836-a888-f3f8a5f08421
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# Estados de tareas del sistema

Los tres estados de tareas del sistema integrados en Workfront son obligatorios, lo que significa que puede desbloquearlos, cambiarles el nombre y reordenarlos, pero no puede ocultarlos ni eliminarlos.

También puede agregar nuevos estados de tareas del sistema para adaptarlos a las necesidades de su organización.

El cambio del estado de una tarea suele ser un proceso manual. Sin embargo, en la siguiente lista se describen tiempos en los que el estado de una tarea cambia automáticamente, según otros factores que estén ocurriendo en el sistema.

Con la instancia de Workfront se proporcionan los siguientes estados de tareas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Estado de la tarea del sistema</th> 
   <th>Cuando se produce este estado</th> 
   <th>Acciones que se producen cuando una tarea está en este estado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nuevo (estado requerido)</td> 
   <td>Este es el estado predeterminado de cada tarea recién creada.</td> 
   <td>Si la tarea está en un proyecto con el estado Actual, la tarea se muestra en la pestaña Solicitudes de trabajo de los usuarios asignados a las tareas. Los usuarios ahora pueden empezar a trabajar en la tarea.</td> 
  </tr> 
  <tr> 
   <td>In Progress (estado requerido)</td> 
   <td>Puede colocar una tarea en este estado para indicar que se ha iniciado el trabajo en esa tarea.</td> 
   <td> <p>Cuando marca una tarea como En curso, la tarea muestra un valor para la Fecha de inicio real.</p> <p>El progreso en la tarea no se registra hasta que se actualiza manualmente el porcentaje completado de la tarea.</p> </td> 
  </tr> 
  <tr> 
   <td>Completar (estado requerido)</td> 
   <td> <p>Puede marcar manualmente una tarea como completada cuando se haya completado el trabajo en ella.</p> <p>Cuando el modo de seguimiento de una tarea se establece en Autocompletar, la tarea se marca automáticamente como Completada cuando alcanza la fecha de finalización planeada.</p> </td> 
   <td> <p>Cuando se completa una tarea, el porcentaje completado de la tarea se marca como 100%. La tarea se elimina de la lista de trabajo del usuario asignado en el área principal cuando se completa.</p> <p>Cuando marca una tarea como Completada, la tarea muestra un valor para la Fecha de Finalización Real.</p> <p><b>NOTA</b>: Si la tarea tiene problemas incompletos y cambia el estado de la tarea a Complete, el estado cambia automáticamente a Complete - Pending Issues.</p> </td> 
  </tr> 
 </tbody> 
</table>
