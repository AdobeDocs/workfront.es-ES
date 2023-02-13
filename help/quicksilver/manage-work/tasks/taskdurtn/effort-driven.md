---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Descripción general del tipo de duración: Impulsado por el esfuerzo'
description: El controlador de esfuerzo es un tipo de duración que se puede definir para una tarea en Adobe Workfront. Para obtener información general sobre los tipos de duración en Workfront, consulte Información general sobre la duración de la tarea y el tipo de duración.
author: Alina
feature: Work Management
exl-id: 3c8534f7-02d0-4404-a37b-0ef6360e8efc
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 1%

---

# Información general del tipo de duración: Impulsado por el esfuerzo

El controlador de esfuerzo es un tipo de duración que se puede definir para una tarea en Adobe Workfront. Para obtener información general sobre los tipos de duración en Workfront, consulte [Información general sobre la duración y el tipo de duración de la tarea](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Descripción general del tipo de duración impulsada por el esfuerzo

El administrador de Workfront o de un grupo puede establecer el tipo de duración predeterminado del sistema o del grupo como impulsado por el esfuerzo. En este caso, todas las tareas nuevas se crearán con este tipo de duración. Para obtener información sobre cómo cambiar las preferencias de problemas y tareas como parte de las preferencias de proyecto de nivel de sistema o de grupo, consulte [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

En este escenario, existe el riesgo de acortar arbitrariamente el plan del proyecto, a menos que usted, como administrador del proyecto, dedique tiempo a considerar si la tarea es realmente una tarea impulsada por el esfuerzo.

Utilice el esfuerzo impulsado para:

* Determine la duración prevista en función del número de recursos disponibles para trabajar en la tarea. La duración es igual a horas planificadas. La duración planeada es igual a las horas planificadas divididas por el número de personas asignadas.

   El nivel de esfuerzo aplicado a la tarea determina la división del trabajo y la duración.

* Rastree el número total de horas empleado en una tarea cuando se asignan varios recursos.

   A medida que se añaden recursos, la duración planificada de la tarea disminuye. (El principio de &quot;muchas manos hacen que la luz funcione&quot; ilustra el efecto que este tipo de duración tiene en la duración prevista de una tarea.)

Las secciones siguientes proporcionan información más detallada sobre cómo calcula Workfront la duración prevista de una tarea impulsada por el esfuerzo y el efecto que tiene la adición de recursos en la tarea con este tipo de duración.

## Descripción general de la fórmula Tipo de duración impulsada por esfuerzo

La fórmula para calcular la duración prevista de una tarea con un tipo de duración impulsada por el esfuerzo depende del porcentaje de asignación de cada recurso asignado a la tarea. En el caso de una tarea impulsada por el esfuerzo, Workfront calcula las horas planificadas de la tarea y siempre son iguales a la duración de la tarea:

```
Planned Hours (in hours) = Duration (in days)
```

Puede ajustar manualmente la duración de la tarea.

Workfront supone que hay 8 horas laborables en un día laborable. El administrador de Workfront o de grupo define las horas por día laborable con la configuración Horas típicas por día laboral en Preferencias de proyecto en Configuración. Para obtener más información sobre cómo cambiar las preferencias de problemas y tareas como parte de las preferencias de proyecto de nivel de sistema, consulte [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!TIP]
>
>Workfront considera la programación de cada recurso asignado a la tarea para determinar el porcentaje de asignación de cada recurso para la tarea. Para obtener información sobre la creación y asignación de programaciones a los usuarios, consulte [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Consideremos los siguientes escenarios:

* [Los recursos se asignan al 100 % a la tarea](#resources-are-allocated-100-to-the-task)
* [Los recursos se asignan a diversos porcentajes de tiempo para la tarea](#resources-are-allocated-for-various-percentages-of-time-to-the-task)

### Los recursos se asignan al 100 % a la tarea {#resources-are-allocated-100-to-the-task}

Esta fórmula supone que todos los recursos se asignan al 100% de la tarea.

```
Planned Duration = (Planned Hours / Number of Resources) / 8
```

Este cálculo supone que el número de horas en un día de trabajo normal es de 8. La ecuación incluye este valor, de modo que la Duración planeada se muestre en días.

### Los recursos se asignan a diversos porcentajes de tiempo para la tarea {#resources-are-allocated-for-various-percentages-of-time-to-the-task}

Dado que cada recurso asignado puede tener un nivel de asignación único, la fórmula real tiene en cuenta estos valores de asignación:

```
Planned Duration = (Planned Hours / SUM(Percent allocation for each resource for the task)) / 8
```

Este cálculo supone que el número de horas en un día de trabajo normal es de 8. La ecuación incluye este valor, de modo que la Duración planeada se muestre en días.

## El efecto de añadir más recursos a una tarea

Al añadir o eliminar asignadores a una tarea con el tipo de duración impulsada por el esfuerzo, la duración y las horas planificadas no cambian. Sin embargo, la duración prevista sí cambia.

En el siguiente ejemplo, el valor de Horario típico por día laboral se establece en 8 en Preferencias de proyecto en la configuración del sistema. Como la duración es de 3 días, el valor de Horario planificado es de 24 (3 días x 8 horas por día laboral = 24 horas planificadas).

>[!NOTE]
>
>Cuando se utiliza la restricción de tareas Fechas fijas, la duración planeada permanece igual cuando se agregan o eliminan personas asignadas, y en su lugar se ajustan la duración y las horas planificadas. Cuando se utiliza cualquier restricción de tarea que no sea Fechas fijas, se ajusta la duración planeada.

La siguiente tabla ilustra cómo cambia la duración planificada con la adición de recursos a la tarea:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p><strong>Número de personas asignadas (cada 100% asignado)</strong> </p> </th> 
   <th> <p><strong>Duración</strong> </p> </th> 
   <th> <p><strong>Horas planificadas</strong> </p> </th> 
   <th><strong>Duración planificada</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> </td> 
   <td> <p>1</p> </td> 
   <td> <p>3 días</p> </td> 
   <td> <p>24 horas</p> <p>(3 días x 8 horas por día de trabajo = 24 horas previstas)</p> </td> 
   <td> <p>3 días</p> <p>(24 horas previstas / 1 persona asignada = 3 días)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>2</p> </td> 
   <td> <p>3 días</p> </td> 
   <td> <p>24 horas</p> <p>(3 días x 8 horas por día de trabajo = 24 horas previstas)</p> </td> 
   <td> <p>1,5 días</p> <p>(24 horas planificadas / 2 asignados = 12 horas o 1,5 días)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>3</p> </td> 
   <td> <p>3 días</p> </td> 
   <td> <p>24 horas</p> <p>(3 días x 8 horas por día de trabajo = 24 horas previstas)</p> </td> 
   <td> <p>1 día</p> <p>(24 horas planificadas / 3 asignados = 8 horas o 1 día)</p> </td> 
  </tr> 
 </tbody> 
</table>

## Cambiar el tipo de duración de una tarea a Impulsado por el esfuerzo

Para obtener información sobre cómo cambiar el tipo de duración de una tarea, consulte [Actualizar el tipo de duración de una tarea](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

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
