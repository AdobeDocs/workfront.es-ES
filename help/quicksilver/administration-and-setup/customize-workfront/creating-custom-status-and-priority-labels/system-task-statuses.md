---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Estados de tareas del sistema
description: Se requieren los tres estados de tareas del sistema integrados en Workfront, lo que significa que puede desbloquearlos, cambiarles el nombre y reordenarlos, pero no puede ocultarlos ni eliminarlos. También puede agregar nuevos estados de tareas del sistema para que coincidan con las necesidades de su organización. Cambiar el estado de una tarea suele ser un proceso manual, pero a veces el estado de una tarea cambia automáticamente, según otros factores que estén ocurriendo en el sistema.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b8c751c3-aed3-4836-a888-f3f8a5f08421
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Estados de tareas del sistema

Se requieren los tres estados de tareas del sistema integrados en Workfront, lo que significa que puede desbloquearlos, cambiarles el nombre y reordenarlos, pero no puede ocultarlos ni eliminarlos.

También puede agregar nuevos estados de tareas del sistema para que coincidan con las necesidades de su organización.

Cambiar el estado de una tarea suele ser un proceso manual. Sin embargo, hay veces que se describen en la siguiente lista en las que el estado de una tarea cambia automáticamente, según otros factores que estén ocurriendo en el sistema.

La instancia de Workfront proporciona los siguientes estados de tareas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Estado de tarea del sistema</th> 
   <th>Cuando se produce este estado</th> 
   <th>Acciones que se producen cuando una tarea está en este estado</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Nuevo (estado obligatorio)</td> 
   <td>Este es el estado predeterminado de cada tarea recién creada.</td> 
   <td>Si la tarea se encuentra en un proyecto con el estado Actual, la tarea se mostrará en la ficha Solicitudes de trabajo de los usuarios asignados a las tareas. Los usuarios ahora pueden empezar a trabajar en la tarea.</td> 
  </tr> 
  <tr> 
   <td>En curso (estado requerido)</td> 
   <td>Puede colocar una tarea en este estado para indicar que se ha iniciado el trabajo en esa tarea.</td> 
   <td> <p>Cuando marca una tarea como En curso, la tarea muestra un valor para la Fecha de inicio real.</p> <p>El progreso de la tarea no se registrará hasta que actualice manualmente el porcentaje completado de la tarea.</p> </td> 
  </tr> 
  <tr> 
   <td>Completado (estado obligatorio)</td> 
   <td> <p>Puede marcar manualmente una tarea como completada cuando se complete el trabajo en ella.</p> <p>Cuando el modo de seguimiento de una tarea está establecido en Autocompletar, la tarea se marca automáticamente como Completada cuando alcanza la fecha planificada de finalización.</p> </td> 
   <td> <p>Cuando se completa una tarea, el porcentaje completado de la tarea se marca como 100%. La tarea se eliminará de la lista Mi trabajo del usuario asignado en el área de Inicio cuando se complete.</p> <p>Cuando marca una tarea como Completada, la tarea muestra un valor para la Fecha real de finalización.</p> <p><b>NOTA</b>: Si la tarea tiene problemas incompletos y cambia el estado de la tarea a Completo, el estado cambiará automáticamente a Completo - Problemas pendientes.</p> </td> 
  </tr> 
 </tbody> 
</table>
