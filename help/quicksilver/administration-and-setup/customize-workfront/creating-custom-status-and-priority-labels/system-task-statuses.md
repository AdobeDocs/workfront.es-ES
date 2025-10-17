---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Estados de tareas del sistema
description: Los tres estados de tareas del sistema integrados en Workfront son obligatorios, lo que significa que puede desbloquearlos, cambiarles el nombre y reordenarlos, pero no puede ocultarlos ni eliminarlos. También puede añadir nuevos estados de tareas del sistema para que coincidan con las necesidades de la organización. Cambiar el estado de una tarea suele ser un proceso manual, pero a veces este cambia automáticamente, según otros factores que se estén produciendo en el sistema.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: b8c751c3-aed3-4836-a888-f3f8a5f08421
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 94%

---

# Estados de tareas del sistema

Los tres estados de tareas del sistema integrados en Workfront son obligatorios, lo que significa que puede desbloquearlos, cambiarles el nombre y reordenarlos, pero no puede ocultarlos ni eliminarlos.

También puede añadir nuevos estados de tareas del sistema para que coincidan con las necesidades de la organización.

Cambiar el estado de una tarea suele ser un proceso manual. Sin embargo, en ocasiones (se describen en la siguiente lista), el estado de una tarea cambia automáticamente, según otros factores que se estén produciendo en el sistema.

La instancia de Workfront proporciona los siguientes estados de tareas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Estado de tarea del sistema</th> 
   <th>Cuando se produce este estado</th> 
   <th>Acciones que se producen cuando una tarea se encuentra en este estado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nueva (estado obligatorio)</td> 
   <td>Este es el estado predeterminado de cada tarea recién creada.</td> 
   <td>Si la tarea se encuentra en un proyecto con el estado Actual, se mostrará en la pestaña Solicitudes de trabajo de los usuarios asignados a las tareas. Los usuarios ahora pueden empezar a trabajar en la tarea.</td> 
  </tr> 
  <tr> 
   <td>En curso (estado obligatorio)</td> 
   <td>Puede poner una tarea en este estado para indicar que se ha iniciado el trabajo de esa tarea.</td> 
   <td> <p>Cuando marca una tarea como En curso, la tarea muestra un valor de fecha de inicio real.</p> <p>El progreso de la tarea no se registrará hasta que actualice manualmente el porcentaje completado de la tarea.</p> </td> 
  </tr> 
  <tr> 
   <td>Completado (estado obligatorio)</td> 
   <td> <p>Puede marcar manualmente una tarea como completada cuando se complete el trabajo de esa tarea.</p> <p>Cuando el modo de seguimiento de una tarea está establecido en Autocompletar, la tarea se marca automáticamente como completada cuando alcanza la fecha planificada de finalización.</p> </td> 
   <td> <p>Cuando se completa una tarea, su porcentaje completado se marca como 100 %. La tarea se eliminará de la lista Mi trabajo del usuario asignado en el área de Inicio cuando se complete.</p> <p>Cuando se marca una tarea como completada, la tarea muestra un valor de fecha real de finalización.</p> <p><b>NOTA</b>: Si la tarea tiene problemas no completados y se cambia su estado a Completada, el estado cambiará automáticamente a Completada - Problemas pendientes.</p> </td> 
  </tr> 
 </tbody> 
</table>
