---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Información general de tipo de duración: Condicionada por el esfuerzo'
description: '"Condicionada por el esfuerzo" es un tipo de duración que puede establecer para una tarea en Adobe Workfront. Para obtener información general sobre los tipos de duración en Workfront, consulte Información general sobre la duración de la tarea y el tipo de duración.'
author: Alina
feature: Work Management
exl-id: 3c8534f7-02d0-4404-a37b-0ef6360e8efc
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 95%

---

# Información general sobre el tipo de duración: Condicionada por el esfuerzo

&quot;Condicionada por el esfuerzo&quot; es un tipo de duración que puede establecer para una tarea en Adobe Workfront. Para obtener información general acerca de los tipos de duración en Workfront, consulte [Información general sobre la duración de la tarea y el tipo de duración](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Descripción general del tipo de duración Condicionada por el esfuerzo

Su Workfront o un administrador de grupo pueden establecer el tipo de duración predeterminado de su sistema o grupo como Condicionada por el esfuerzo. En este caso, todas las tareas nuevas se crearán con este tipo de duración. Para obtener información sobre cómo cambiar las preferencias de tareas y problemas como parte de las preferencias de proyectos de nivel de sistema o de grupo, consulte [Configurar las preferencias de tareas y problemas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

En este escenario, existe el riesgo de acortar arbitrariamente el plan del proyecto, a menos que usted, como jefe de proyecto, se tome el tiempo para considerar si la tarea es en realidad una tarea Condicionada por el esfuerzo.

Utilice Condicionada por el esfuerzo para:

* Determinar la Duración planificada en función del número de recursos disponibles para trabajar en la tarea. La duración es igual a las horas planificadas. La duración planificada es igual a las horas planificadas divididas por el número de personas asignadas.

  El nivel de esfuerzo aplicado a la tarea determina la división del trabajo y la duración.

* Registre el número total de horas invertidas en una tarea cuando se asignan varios recursos.

  A medida que se agregan recursos, disminuye la Duración planificada de la tarea. (El principio de &quot;muchas manos hacen que la luz funcione&quot; ilustra el efecto que este tipo de duración tiene en la duración planificada de una tarea.)

Las secciones siguientes proporcionan información más detallada sobre cómo Workfront calcula la duración planificada de una tarea Condicionada por el esfuerzo y el efecto que tiene añadir recursos a la tarea con este tipo de duración.

## Información general de la fórmula del tipo de duración Condicionada por el esfuerzo

La fórmula para calcular la Duración planificada para una tarea con un tipo de duración Condicionada por el esfuerzo depende del porcentaje de asignación de cada recurso asignado a la tarea. En el caso de una tarea condicionada por el esfuerzo, Workfront calcula las horas planificadas de la tarea, que siempre son las mismas que la duración de la tarea:

```
Planned Hours (in hours) = Duration (in days)
```

Puede ajustar manualmente la duración de la tarea.

Workfront presupone que hay 8 horas laborables en un día laborable. El administrador de su Workfront o de su grupo define las horas por día laborable con la configuración Horas típicas por día laborable en Preferencias del proyecto, en Configuración. Para obtener más información sobre cómo cambiar las preferencias de tareas y problemas como parte de las preferencias de proyectos de nivel de sistema, consulte [Configurar las preferencias de tareas y problemas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!TIP]
>
>Workfront tiene en cuenta la programación para cada recurso asignado a la tarea para determinar el porcentaje de asignación de cada recurso para la tarea. Para obtener información acerca de cómo crear y asignar programaciones a los usuarios, vea [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Considere los siguientes escenarios:

* [Los recursos se asignan al 100% a la tarea](#resources-are-allocated-100-to-the-task)
* [Los recursos se asignan con varios porcentajes de tiempo a la tarea](#resources-are-allocated-for-various-percentages-of-time-to-the-task)

### Los recursos se asignan a la tarea al 100% {#resources-are-allocated-100-to-the-task}

Esta fórmula supone que todos los recursos se asignan al 100% a la tarea.

```
Planned Duration = (Planned Hours / Number of Resources) / 8
```

Este cálculo presupone que el número de horas en un día laborable normal es de 8. La ecuación incluye este valor para que la duración planificada se muestre en días.

### Los recursos se asignan con varios porcentajes de tiempo a la tarea {#resources-are-allocated-for-various-percentages-of-time-to-the-task}

Dado que cada recurso asignado puede tener un nivel de asignación único, la fórmula real tiene en cuenta estos valores de asignación:

```
Planned Duration = (Planned Hours / SUM(Percent allocation for each resource for the task)) / 8
```

Este cálculo presupone que el número de horas en un día laborable normal es de 8. La ecuación incluye este valor para que la duración planificada se muestre en días.

## El efecto de añadir más recursos a una tarea

Al añadir o eliminar personas asignadas a una tarea con el tipo de duración Condicionada por el esfuerzo, la duración y las horas planificadas no cambian. Sin embargo, la duración planificada sí cambia.

En el ejemplo siguiente, el valor de Horas típicas por día laborable se establece en 8 en las Preferencias del proyecto, en la configuración del sistema. Como la duración es de 3 días, las horas planificadas se establecen en 24 (3 días x 8 horas por día laborable = 24 horas planificadas).

>[!NOTE]
>
>Al utilizar la Restricción de tarea de fechas fijas, la duración planificada permanece igual cuando añade o elimina usuarios asignados y, en su lugar, se ajustan la duración y las horas planificadas. Al utilizar cualquier restricción de tarea que no sea Fechas fijas, se ajusta la duración planificada.

La siguiente tabla ilustra cómo cambia la duración planificada al añadir recursos a la tarea:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p><strong>Número de usuarios asignados (cada uno asignado al 100%)</strong> </p> </th> 
   <th> <p><strong>Duración</strong> </p> </th> 
   <th> <p><strong>Horas planificadas</strong> </p> </th> 
   <th><strong>Duración planificada</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> </td> 
   <td> <p>1</p> </td> 
   <td> <p>3 días</p> </td> 
   <td> <p>24 horas</p> <p>(3 días x 8 horas por día laborable = 24 horas planificadas)</p> </td> 
   <td> <p>3 días</p> <p>(24 horas planificadas / 1 persona asignada = 3 días)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>2</p> </td> 
   <td> <p>3 días</p> </td> 
   <td> <p>24 horas</p> <p>(3 días x 8 horas por día laborable = 24 horas planificadas)</p> </td> 
   <td> <p>1,5 días</p> <p>(24 horas planificadas / 2 usuarios asignados = 12 horas o 1,5 días)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>3</p> </td> 
   <td> <p>3 días</p> </td> 
   <td> <p>24 horas</p> <p>(3 días x 8 horas por día laborable = 24 horas planificadas)</p> </td> 
   <td> <p>1 día</p> <p>(24 horas planificadas / 3 personas asignadas = 8 horas o 1 día)</p> </td> 
  </tr> 
 </tbody> 
</table>

## Cambiar el tipo de duración de una tarea a condicionada por el esfuerzo

Para obtener información acerca de cómo cambiar el tipo de duración de una tarea, vea [Actualizar el tipo de duración de una tarea](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Effort Driven</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong><strong>Changes</strong>.</li>
</ol>
-->
