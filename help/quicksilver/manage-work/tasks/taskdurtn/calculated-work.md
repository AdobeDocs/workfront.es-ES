---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Información general de tipo de duración: Trabajo calculado'
description: Trabajo calculado es un tipo de duración que puede establecer para una tarea en Adobe Workfront. Para obtener información general sobre los tipos de duración en Workfront, consulte Información general sobre la duración de la tarea y el tipo de duración.
author: Alina
feature: Work Management
exl-id: f521c2f5-8d58-44c0-af18-6940ad0950ea
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 93%

---

# Información general sobre el tipo de duración: Trabajo calculado

Trabajo calculado es un tipo de duración que puede establecer para una tarea en Adobe Workfront. Para obtener información general acerca de los tipos de duración en Workfront, consulte [Información general sobre la duración de la tarea y el tipo de duración](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Información general sobre el tipo de duración Trabajo calculado

Trabajo calculado determina la cantidad de esfuerzo (horas planificadas) necesario para completar la tarea. Le recomendamos que utilice el tipo de duración Trabajo calculado cuando los recursos asignados a la tarea se asignen a toda la duración de la tarea.

Su Workfront o un administrador de grupo pueden establecer el tipo de duración predeterminado de su sistema o grupo como Trabajo calculado. En este caso, todas las tareas nuevas se crearán con este tipo de duración. Para obtener información sobre cómo cambiar las preferencias de tareas y problemas como parte de las preferencias de proyectos de nivel de sistema o de grupo, consulte [Configurar las preferencias de tareas y problemas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

A medida que se añaden recursos a una tarea, el gerente del proyecto puede esperar que aumente el esfuerzo planificado. A modo de ejemplo, una reunión de planificación de una hora con tres recursos representa tres horas totales de trabajo necesario, y una reunión de planificación de una hora con diez recursos representa diez horas de trabajo necesario. Esto supone que cada recurso se asigna a la tarea con una asignación del 100 %.

## Revise la fórmula para calcular el trabajo necesario cuando se utiliza el tipo de duración Trabajo calculado

Cuando se utiliza el tipo de duración de Trabajo calculado en una tarea, Workfront calcula la cantidad de trabajo para cada tarea utilizando las dos fórmulas siguientes. Las fórmulas difieren según el porcentaje de tiempo que cada recurso tenga asignado a la tarea y el número de recursos que haya asignado a cada tarea:

* Fórmula simplificada: suponiendo que tiene un recurso asignado a la tarea y que está asignado a la tarea durante el 100 % de su tiempo disponible, el valor de Trabajo necesario para cada tarea se calcula mediante la siguiente fórmula:

```
Work Required (Planned Hours) = (Duration of the task in hours) x (The number of resources assigned to the task)
```

* Fórmula compleja: si asigna cada recurso con varias asignaciones, la fórmula tiene en cuenta estas asignaciones y tiene en cuenta estas variaciones:

```
Work Required (Planned Hours) = SUM[(Duration of the task in hours) x (Percent allocated towards tasks for each resource)]
```

## Revisar el efecto de añadir o quitar recursos de la tarea

Al añadir o quitar asignados a una tarea con el tipo de duración Trabajo calculado, la duración se puede editar manualmente. A medida que se añaden o quitan asignados de la tarea, cambian las Horas planificadas.

En el ejemplo siguiente, el valor de Horas habituales por día laborable se establece en 8 en Preferencias del proyecto, en Configuración. Cada tarea tiene una duración de 1 día. A medida que cambia el número asignado, las horas planificadas cambian según el número de asignados a una tarea determinada:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Número de asignados (cada uno asignado al 100 %)</strong> </p> </th> 
   <th> <p><strong>Duración</strong> </p> </th> 
   <th> <p><strong>Horas planificadas</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>1</p> </td> 
   <td> <p>1 día</p> </td> 
   <td> <p>8 horas</p> <p>(1 día x 8 horas por día laborable x 1 asignado = 8 horas planificadas)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>2</p> </td> 
   <td> <p>1 día</p> </td> 
   <td> <p>16 horas</p> <p>(1 día x 8 horas por día laborable x 2 asignados = 16 horas planificadas)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>3</p> </td> 
   <td> <p>1 día</p> </td> 
   <td> <p>24 horas</p> <p>(1 día x 8 horas por día laborable x 3 asignados = 24 horas planificadas)</p> </td> 
  </tr> 
 </tbody> 
</table>

En este caso, cada asignado se asigna al 100 % a la tarea Trabajo calculado.

![](assets/calcwork-350x71.png)

## Cambiar el tipo de duración de una tarea a Trabajo calculado

Para obtener información sobre el cambio del tipo de duración de una tarea, consulte [Actualizar el tipo de duración de una tarea](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

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
