---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Información general sobre el esfuerzo de trabajo
description: Información general sobre el esfuerzo de trabajo
author: Alina
feature: Work Management
exl-id: 70f51e4b-43cc-427a-99e4-ebb056bb1070
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1512'
ht-degree: 0%

---

# Información general sobre el esfuerzo de trabajo

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the UI >> in the Project/ Template edit box > Tasks area> Learn more) </p>
-->

Como administrador de proyectos, puede decidir cómo desea calcular la cantidad de trabajo necesario para que las tareas se completen en un proyecto. Calcule la cantidad de trabajo necesario para completar tareas utilizando uno de los siguientes indicadores:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Horas planificadas</td> 
   <td> <p> Entrada numérica manual o cálculo de Adobe Workfront que muestra el número de horas que tardarían los recursos asignados a una tarea en completarla. </p> <p>Tenga en cuenta lo siguiente sobre las horas programadas: </p> 
    <ul> 
     <li>Este es el método predeterminado. </li> 
     <li>Puede actualizar manualmente las horas planificadas solo para tareas con un tipo de duración de asignación calculada o simple. </li> 
    </ul> <p>Para obtener información sobre las horas planificadas, consulte <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Información general sobre las horas planificadas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Esfuerzo de trabajo </td> 
   <td> <p>Etiqueta manual que define si se requiere que un usuario realice un esfuerzo diario pequeño, medio o grande para completar una tarea. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The level of effort is estimated to be a percentage of the daily amount of working time. (NOTE: keep this drafted. Vazgen said it's not needed, but waiting for feedback from users)
      </MadCap:conditionalText>
     --> </p> <p>Tenga en cuenta lo siguiente sobre el esfuerzo de trabajo:</p> 
    <ul> 
     <li>Este campo solo está disponible para tareas con un tipo de duración simple. </li> 
     <li>Puede habilitar el uso de esta etiqueta y definir el porcentaje de tiempo de trabajo asociado a ella en el nivel de proyecto. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

En este artículo se describe qué es el esfuerzo de trabajo y cómo debe utilizarlo al estimar la cantidad de trabajo para sus tareas.

>[!NOTE]
>
>Las horas planificadas y el esfuerzo de trabajo se influyen entre sí. Actualizar las horas planificadas puede actualizar el esfuerzo de trabajo y actualizar el esfuerzo de trabajo puede actualizar las horas planificadas de la tarea.

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos y tareas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para un proyecto y sus tareas</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones para utilizar el esfuerzo de trabajo

* Cuando las tareas del proyecto tienen 0 horas planificadas y se habilita la opción Utilizar esfuerzo de trabajo para calcular automáticamente las horas planificadas de la tarea en el proyecto, el nivel predeterminado de esfuerzo de trabajo asociado a ellas será Medio. Las horas planificadas se actualizan automáticamente para las tareas Tipo de duración simple . Para obtener más información, consulte la sección  [Niveles de trabajo](#levels-of-work-effort) en este artículo.
* Cuando las tareas del proyecto tienen horas planificadas superiores a 0 y se habilita la opción Utilizar esfuerzo de trabajo para calcular automáticamente las horas planificadas de la tarea en el proyecto, el nivel de esfuerzo de trabajo se actualiza según la cantidad de horas planificadas sin cambiar la cantidad de horas planificadas para las tareas de tipo de duración simple. Para obtener más información, consulte la sección [Cómo calcula Workfront el esfuerzo de trabajo en función de las horas planificadas](#how-workfront-calculates-work-effort-based-on-planned-hours) en este artículo.
* Cuando las tareas del proyecto tienen 0 horas planificadas y se habilita la opción Utilizar esfuerzo de trabajo para calcular automáticamente las horas planificadas de la tarea en el proyecto y, a continuación, actualizar el nivel de esfuerzo de trabajo de medio a pequeño o grande, también se actualiza el horario planificado. Para obtener más información, consulte la sección [Cómo calcula Workfront las horas programadas en función del esfuerzo laboral](#how-workfront-calculates-planned-hours-based-on-work-effort) en este artículo.
* Cuando se insertan tareas de edición y se modifican al mismo tiempo los campos Horario planificado y Esfuerzo de trabajo para la tarea, las horas planificadas se actualizan con el valor especificado, mientras que el valor Esfuerzo de trabajo se calcula en función de las horas planificadas actualizadas.
* Al actualizar el valor Esfuerzo de Trabajo de una tarea, la Duración ya no se calcula automáticamente en función de las horas planificadas. Para obtener más información sobre cómo se calcula la duración para las tareas de duración simple, consulte [Información general del tipo de duración: Sencilla](../../../manage-work/tasks/taskdurtn/simple-duration-type.md).
* Cuando se cambia el tipo de duración de una tarea de Simple a cualquier otro tipo, el campo Esfuerzo de trabajo se oculta en la tarea. Las horas programadas permanecen sin cambios.
* No se puede actualizar el nivel de esfuerzo de trabajo en una tarea principal. El nivel Esfuerzo de Trabajo de una tarea principal se calcula automáticamente en función del número de horas planificadas para las tareas que es un resumen de todas las tareas secundarias. Para obtener información sobre las tareas principales, consulte [Crear subtareas](../../../manage-work/tasks/create-tasks/create-subtasks.md).

## Habilitar utilizando el esfuerzo de trabajo en lugar de horas planificadas

1. Vaya a un proyecto y haga clic en el **Más** menú ![](assets/more-icon.png)y haga clic en **Editar**.
1. Haga clic en **Configuración de tareas** y, a continuación, seleccione la opción **Utilice Esfuerzo de Trabajo para calcular automáticamente las horas planificadas de la tarea**. Esta opción está desactivada de forma predeterminada.

   ![](assets/nwe-work-effort-on-projects-350x182.png)

   Para obtener más información sobre cómo habilitar el uso de Esfuerzo de trabajo en un proyecto, consulte la sección &quot;Configuración de tareas&quot; en la sección [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md) artículo.

1. Haga clic en **Tareas** en el panel izquierdo y, a continuación, haga clic en el nombre de una tarea para acceder a ella.
1. Haga clic en el **Más** menú ![](assets/more-icon.png)y haga clic en **Editar**. Asegúrese de que la tarea tiene un tipo de duración simple.

   >[!TIP]
   >
   >También puede actualizar el esfuerzo de trabajo de una tarea en la sección Detalles de la tarea .

1. En el **Información general** , haga clic en el menú desplegable Esfuerzo de trabajo para corregir el esfuerzo necesario para completar la tarea.

   ![](assets/work-effort-on-edit-task-page-350x239.png)

   Para obtener más información sobre la actualización del campo Esfuerzo de trabajo en una tarea, consulte los siguientes artículos:

   * La sección &quot;Información general&quot; de la sección [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md) article
   * [Administrar información de tarea en el área Información general de detalles de tarea](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)

## Niveles de trabajo {#levels-of-work-effort}

Como administrador de proyectos, puede identificar tres niveles de esfuerzo de trabajo para sus proyectos. Cada nivel de esfuerzo equivale a un porcentaje del tiempo diario que los usuarios necesitan para completar la tarea.

Al configurar el nivel de trabajo, debe hacerse la pregunta: &quot;¿Cuánto tiempo debe pasar un usuario asignado a esta tarea a diario para realizarla a tiempo?&quot; 

La siguiente tabla ilustra los posibles niveles de esfuerzo de trabajo y sus porcentajes correspondientes predeterminados. Como administrador de proyectos, puede actualizar los porcentajes para adaptarlos a las necesidades de su organización. Para ello, edite un proyecto. Para obtener información sobre la edición de proyectos, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

Como administrador de Workfront, define las horas típicas por día laboral en el área Preferencias del proyecto de Configuración. Es la cantidad diaria de tiempo que se considera tiempo de trabajo. Para obtener información sobre la configuración de las preferencias de proyecto para la instancia de Workfront, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

>[!NOTE]
>
>En los ejemplos siguientes, suponemos que el administrador de Workfront ha establecido la cantidad típica de horas por día laboral en 8 horas.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Nivel de esfuerzo laboral</td> 
   <td>Valores de porcentaje</td> 
  </tr> 
  <tr> 
   <td>Pequeño </td> 
   <td>Un Pequeño nivel de esfuerzo para completar una tarea se establece en el 25% de las horas típicas por día laboral. Esto significa que una tarea asignada a este nivel de esfuerzo laboral debe tardar hasta dos horas al día en completarse en un día. <code>(0.25*8=2)</code></td> 
  </tr> 
  <tr> 
   <td>Medio</td> 
   <td> <p>Un nivel medio de esfuerzo para completar una tarea se establece en el 50% de las horas típicas por día laboral. Esto significa que una tarea asignada a este nivel de esfuerzo laboral debe tardar más de 2 horas y menos de 6 horas en completarse en un día. <code>(0.50*80=4)</code> </p> <p>Nota: Cuando el ajuste Utilizar esfuerzo de trabajo para calcular automáticamente las horas planificadas de la tarea está habilitado en el proyecto, esta es la configuración predeterminada para una tarea, si la tarea tenía 0 horas planificadas antes de que se activara esta configuración. Esto hace que la tarea Horario planificado se actualice a 4 horas. </p> </td> 
  </tr> 
  <tr> 
   <td>Grande</td> 
   <td>Un gran nivel de esfuerzo para completar una tarea se establece en el 75% de las horas típicas por día laboral. Esto significa que una tarea asignada a este nivel de esfuerzo laboral debe tardar 6 horas o más en completarse en un día. <code>(0.75*8=6)</code></td> 
  </tr> 
 </tbody> 
</table>

## Cómo calcula Workfront las horas programadas en función del esfuerzo laboral {#how-workfront-calculates-planned-hours-based-on-work-effort}

Cuando se habilita la opción Utilizar esfuerzo de trabajo para calcular automáticamente la tarea Horario planificado en un proyecto, Workfront calcula el número de horas planificadas para una tarea con un tipo de duración simple utilizando la fórmula siguiente:

```
Task Planned Hours = Number of days in task Duration * Work Effort percentage * Typical hours per work day
```

Por ejemplo, una tarea con una duración de 3 días y un esfuerzo de trabajo de medio tiene 12 horas planificadas:

```
Planned Hours = 3*4=12
```

donde el valor típico de horas por día laboral es de 8 horas.

>[!TIP]
>
>Cuando se asigna una tarea a varios recursos, las horas planificadas se distribuyen uniformemente a cada recurso durante cada día de la duración de la tarea.

## Cómo calcula Workfront el esfuerzo de trabajo en función de las horas planificadas {#how-workfront-calculates-work-effort-based-on-planned-hours}

Cuando habilita la opción Utilizar esfuerzo de trabajo para calcular automáticamente la tarea Horario planificado en un proyecto y ya tiene Horas planificadas en la tarea o edita el número de horas planificadas en la tarea, Workfront actualiza el valor de Esfuerzo de trabajo.

Workfront utiliza la fórmula siguiente para actualizar el nivel de esfuerzo laboral según el horario planificado:

```
Work Effort level = Task Planned Hours / Duration / Typical hours per work day
```

Por ejemplo, si tiene una tarea con una duración de 2 días y actualiza las horas planificadas de 8 a 20 horas, el esfuerzo de trabajo para la tarea se actualiza de Medio a Grande:

```
Work Effort level = 20 / 2 / 8 = 125 % = Large
```

## Localización del esfuerzo de trabajo para tareas y proyectos

* [Esfuerzo de trabajo para proyectos](#work-effort-for-projects)
* [Esfuerzo de trabajo para tareas](#work-effort-for-tasks)

### Esfuerzo de trabajo para proyectos {#work-effort-for-projects}

Puede ubicar la sección Esfuerzo de trabajo en un proyecto en la siguiente área:

* El área Configuración de tarea del cuadro Editar proyecto

### Esfuerzo de trabajo para tareas {#work-effort-for-tasks}

Puede ubicar el campo Trabajo de una tarea en las siguientes áreas:

* El área Información general del cuadro Editar tarea
* Área Información general de la sección Detalles de la tarea, en el área Tiempo de trabajo
* Una lista de tareas o un informe
