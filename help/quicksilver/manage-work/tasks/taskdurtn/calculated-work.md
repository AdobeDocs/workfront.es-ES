---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Descripción general del tipo de duración: Trabajo calculado'
description: Trabajo calculado es un tipo de duración que puede establecer para una tarea en Adobe Workfront. Para obtener información general sobre los tipos de duración en Workfront, consulte Información general sobre la duración de la tarea y el tipo de duración.
author: Alina
feature: Work Management
exl-id: f521c2f5-8d58-44c0-af18-6940ad0950ea
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 1%

---

# Información general del tipo de duración: Trabajo calculado

Trabajo calculado es un tipo de duración que puede establecer para una tarea en Adobe Workfront. Para obtener información general sobre los tipos de duración en Workfront, consulte [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Descripción general del tipo de duración de trabajo calculada

Trabajo calculado determina la cantidad de esfuerzo (horas planificadas) necesaria para completar la tarea. Se recomienda utilizar el Tipo de duración del trabajo calculado cuando los recursos asignados a la tarea se asignen durante toda la duración de la tarea.

El administrador de Workfront o de un grupo puede establecer el tipo de duración predeterminado del sistema o del grupo como Trabajo calculado. En este caso, todas las tareas nuevas se crearán con este tipo de duración. Para obtener información sobre cómo cambiar las preferencias de problemas y tareas como parte de las preferencias de proyecto de nivel de sistema o de grupo, consulte [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

A medida que se añaden recursos a una tarea, un administrador de proyectos puede esperar ver un aumento del esfuerzo planificado. A modo de ejemplo, una reunión de planificación de una hora con tres recursos representa tres horas de trabajo totales necesarias, y una reunión de planificación de una hora con diez recursos representa diez horas de trabajo necesarias. Esto supone que cada recurso está asignado a la tarea con una asignación del 100 %.

## Revise la fórmula para calcular el trabajo necesario al utilizar el tipo de duración de trabajo calculada

Cuando se utiliza el tipo de duración de trabajo calculada en una tarea, Workfront calcula la cantidad de trabajo para cada tarea mediante las dos fórmulas siguientes. Las fórmulas difieren según el porcentaje de tiempo que cada recurso se asigne a la tarea y la cantidad de recursos que haya asignado a cada tarea:

* Fórmula simplificada: Suponiendo que tenga un recurso asignado a la tarea y que se asigne a la tarea durante el 100 % de su tiempo disponible, el valor Trabajo requerido para cada tarea se calcula mediante la fórmula siguiente:

```
Work Required (Planned Hours) = (Duration of the task in hours) x (The number of resources assigned to the task)
```

* Fórmula compleja: Si asigna cada recurso con varias asignaciones, la fórmula tiene en cuenta estas asignaciones y tiene en cuenta estas variaciones:

```
Work Required (Planned Hours) = SUM[(Duration of the task in hours) x (Percent allocated towards tasks for each resource)]
```

## Revise el efecto de añadir o quitar recursos de la tarea

Al agregar o quitar asignadores a una tarea con el tipo de duración Trabajo calculado , la duración se puede editar manualmente. A medida que se añaden o eliminan asignaciones de la tarea, cambian las horas planificadas.

En el ejemplo siguiente, el valor de Horario típico por día de trabajo se establece en 8 en Preferencias de proyecto en Configuración. Cada tarea tiene una duración de 1 día. A medida que cambia el número de personas asignadas, el horario planificado cambia en función del número de personas asignadas a una tarea determinada:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Número de personas asignadas (cada 100% asignado)</strong> </p> </th> 
   <th> <p><strong>Duración</strong> </p> </th> 
   <th> <p><strong>Horas planificadas</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>1</p> </td> 
   <td> <p>1 día</p> </td> 
   <td> <p>8 horas</p> <p>(1 día x 8 horas por día de trabajo x 1 usuario asignado = 8 horas programadas)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>2</p> </td> 
   <td> <p>1 día</p> </td> 
   <td> <p>16 horas</p> <p>(1 día x 8 horas por día de trabajo x 2 cesionarios = 16 horas programadas)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>3</p> </td> 
   <td> <p>1 día</p> </td> 
   <td> <p>24 horas</p> <p>(1 día x 8 horas por día de trabajo x 3 personas asignadas = 24 horas programadas)</p> </td> 
  </tr> 
 </tbody> 
</table>

En este caso, cada usuario asignado está 100 % asignado a la tarea Trabajo calculado.

![](assets/calcwork-350x71.png)

## Cambiar el tipo de duración de una tarea a Trabajo calculado

Para obtener información sobre cómo cambiar el tipo de duración de una tarea, consulte [Actualizar el tipo de duración de una tarea](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3">Select <strong>Calculated Work</strong> from the drop-down menu.</li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong>.</li>
</ol>
-->
