---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo
description: Como Administrador de recursos, puede asignar trabajo a los usuarios y administrar sus asignaciones diarias, semanales o mensuales desde el Distribuidor de cargas de trabajo.
author: Lisa
feature: Resource Management
exl-id: 9649e482-af24-4516-9a69-ef12b2f1d579
source-git-commit: d2268e50080ddbe306731d034d88fd29b712b86d
workflow-type: tm+mt
source-wordcount: '2859'
ht-degree: 0%

---

# Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo

<!-- Audited: 01/2024 -->

<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa para todos los clientes de o en el entorno de producción para los clientes que habilitaron versiones rápidas de.</span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Activar o desactivar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Para obtener más información sobre la versión actual, consulte [Información general sobre la versión del segundo trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

Como Administrador de recursos, puede asignar trabajo a los usuarios y administrar sus asignaciones diarias, semanales o mensuales desde el Distribuidor de cargas de trabajo para asegurarse de que se les asigna una cantidad de horas que se ajusta a sus programaciones disponibles.

## Requisitos de acceso {#access-requirements}

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Al utilizar el Distribuidor de cargas de trabajo en el área de Recursos, necesita lo siguiente:</p>
   <p>Nuevo: estándar</p>
   <p>O</p>
   <p>Actual: plan</p>
   <p>Al utilizar el Distribuidor de cargas de trabajo de un equipo o proyecto, necesita lo siguiente:</p>
   <p>Nuevo: estándar</p>
   <p>O</p>
   <p>Actual: Trabajo</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuración del nivel de acceso</td> 
   <td> <p>Edite el acceso a lo siguiente:</p> 
    <ul> 
     <li> <p>Administración de recursos</p> </li> 
     <li> <p>Proyectos</p> </li> 
     <li> <p>Tareas</p> </li> 
     <li> <p>Problemas</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Aportar permisos o superiores que incluyan Realizar asignaciones a las tareas y problemas para los que desee administrar asignaciones. </p> <p>O </p> <p>Administre permisos para las tareas para las que desea actualizar las horas planificadas, además de actualizar las asignaciones. Para obtener información sobre la actualización de horas planificadas en el Distribuidor de cargas de trabajo, consulte la <a href="#update-task-planned-hours-when-managing-user-allocations">Actualizar horas planificadas de la tarea al administrar las asignaciones de usuario</a> de este artículo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Comprender las asignaciones de usuarios

Las asignaciones de usuarios son cantidades de horas que indican el tiempo que un usuario debe pasar en un día, día de la semana, semana o mes determinados para completar el elemento de trabajo. Se incluyen en las horas planificadas del elemento de trabajo.

Este artículo describe cómo actualizar las asignaciones por horas diarias, semanales o mensuales para los usuarios asignados a tareas o problemas. Para obtener información sobre la administración de asignaciones generales para usuarios y roles de trabajo para tareas, consulte [Administrar horas de asignación de usuarios y funciones en las tareas](../../manage-work/tasks/assign-tasks/manage-allocation-hours-on-tasks.md).

### Resumen de asignación de usuarios {#user-allocation-overview}

Puede mostrar la asignación de usuarios como horas o como un valor porcentual en el Distribuidor de cargas de trabajo. Puede ajustar las horas o los porcentajes.

Las asignaciones de usuarios se incluyen en el número de horas planificadas de un elemento de trabajo. Para obtener información sobre las horas planificadas, consulte [Resumen de horas planificadas](../../manage-work/tasks/task-information/planned-hours.md).

Las horas planificadas para la tarea se distribuyen equitativamente entre todos los días dentro de la duración de la tarea para el usuario asignado a la tarea. Por ejemplo, si una tarea tiene una duración de 5 días y un total de 10 horas planificadas, el número de asignaciones diarias para la tarea es de 2 horas. La asignación semanal es de 10 horas. Esto significa que se asigna a un usuario para que trabaje en la tarea durante 2 horas al día. Sin embargo, puede cambiar manualmente la asignación diaria del usuario mediante el Distribuidor de cargas de trabajo.

>[!CAUTION]
>
>El Distribuidor de cargas de trabajo solo muestra hasta 1000 horas planificadas por elemento de trabajo por usuario y hasta 1000 días de la duración de un elemento. Las asignaciones del Distribuidor de cargas de trabajo se muestran como cero después de alcanzar el límite de 1000 horas o 1000 días. Se recomienda dividir las tareas en subtareas más pequeñas para acomodar un mayor número de horas planificadas o para duraciones de más de 1000 días.

Tenga en cuenta lo siguiente al localizar asignaciones diarias, semanales o mensuales para tareas o problemas en el Distribuidor de cargas de trabajo:

* Puede ver las asignaciones diarias, semanales y mensuales de los usuarios a sus elementos de trabajo. Habilite la vista Semana o Mes para mostrar las asignaciones semanales o mensuales.
* Puede usar el Distribuidor de cargas de trabajo para modificar la asignación diaria, semanal o mensual de los usuarios a las tareas o problemas. Para obtener información sobre cómo ajustar la vista del Distribuidor de cargas de trabajo, consulte [Navegación por el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

  >[!NOTE]
  >
  >Le recomendamos que tome una decisión sobre el lapso de tiempo (diario, semanal o mensual) que desea utilizar siempre al administrar las asignaciones de usuarios y que no cambie entre ellos para los mismos elementos de trabajo. Al actualizar las asignaciones semanales para el mismo usuario para el que ha actualizado anteriormente las asignaciones diarias, se cambia la asignación diaria para el usuario.

* Puede actualizar las asignaciones tanto de los días laborables como de los no laborables.
* Las marcas de tiempo para las fechas planificadas de inicio y planificadas de finalización de los elementos de trabajo, así como la programación del proyecto, son importantes cuando Workfront calcula automáticamente la asignación diaria para la tarea.

  >[!INFO]
  >
  > Por ejemplo, una tarea puede tener una duración de 2 días y 2 horas planificadas y tiene una hora de inicio planificada de 12:00 p.m. en el primer día de la duración con un usuario y una programación de proyecto que termina a las 5 p.m. La capacidad del usuario para el primer día es de 5 horas. La capacidad del usuario para el segundo día es de 8 horas (si la programación comienza a las 9 de la mañana).
  >
  >Workfront calcula la asignación de las dos horas durante los dos días de la duración mediante la fórmula siguiente:
  >
  >`Daily allocation hours = (Total Planned Hours / Total of available hours) * Daily available hours`
  >
  >Para nuestro ejemplo, las horas de asignación diarias para cada día son:
  >   
  >(2 / 13) * 5 = 0,77 horas de asignación para el primer día
  >
  >(2 / 13) * 8 = 1,23 horas de asignación para el segundo día
  >
  >En los cálculos anteriores, 13 es el total de horas disponibles para la tarea: 5 + 8 = 13

* Dos usuarios en zonas horarias o programaciones diferentes a las de los usuarios asignados pueden hacer que las cantidades asignadas aparezcan de forma diferente para dos usuarios que vean los mismos elementos de trabajo.

* Cuando un usuario tiene tiempo libre programado, el día o la parte del día se muestra en un fondo gris. Si el administrador de Workfront habilitó la configuración Tiempo libre del usuario en el área de Configuración para tener en cuenta el tiempo libre del usuario, las horas asignadas pasan al siguiente día disponible en la cronología. Si la configuración está deshabilitada, las horas asignadas permanecen en el día marcado como tiempo libre y el usuario se muestra como sobreasignado. Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  >[!TIP]
  >
  >Si el tiempo libre se marcó después de que el usuario se asignara a un elemento de trabajo, debe volver a calcular la escala de tiempo del proyecto para mostrar la asignación desplazada. Para obtener más información, consulte [Recalcular escalas de tiempo del proyecto](../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* Si hay varios usuarios asignados a la tarea, la cantidad de horas planificadas se distribuye equitativamente a cada usuario, en primer lugar, y luego equitativamente a cada día dentro de la duración de la tarea. Esta distribución se convierte en la asignación de cada usuario a la tarea.

  Por ejemplo, podrían darse los siguientes casos:

   * Para una tarea con una duración de 2 días y con 10 horas planificadas asignadas a un usuario, la asignación diaria para el usuario es de 5 horas por cada día de forma predeterminada.
   * Para una tarea con una Duración de 2 días y con 10 Horas planificadas asignadas a dos usuarios, la asignación diaria para cada usuario es de 2,5 horas para cada día de forma predeterminada.

* Si una tarea o un problema se completan antes de la fecha planificada de finalización, el número de horas asignadas para los días restantes se alcanza y no se cuenta para la asignación general del usuario. Esto solo se muestra cuando están habilitados tanto el icono Mostrar asignaciones como la configuración Mostrar fechas proyectadas. Para obtener más información sobre cómo habilitar la configuración en el Distribuidor de cargas de trabajo, consulte [Navegación por el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

  ![Horas asignadas superadas](assets/allocations-struck-through-highlighted.png)

* Cuando se sobreasigna a un usuario, sus horas asignadas se muestran con un fondo rojo en el campo del usuario.
* Cuando al usuario se le asigna o se le asigna una cantidad igual de horas a su tiempo disponible programado, las horas se muestran con un fondo azul.
* Puede mostrar la asignación de los usuarios en una vista de gráfico en la línea del usuario. Para obtener información sobre cómo habilitar la vista de gráficos para las asignaciones de usuarios, consulte la sección &quot;Navegar por el Distribuidor de cargas de trabajo&quot; en el artículo [Navegación por el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

  ![Gráfico de asignación de usuarios](assets/user-allocation-chart.png)

### Criterios que restablecen las asignaciones de usuario {#criteria-that-reset-user-allocations}

No todos los cambios de tareas almacenan en déclencheur las asignaciones modificadas para su redistribución. Sin embargo, hay ciertas acciones que podrían restablecer las asignaciones ya ajustadas en los recursos y redistribuirlas equitativamente a todos los días durante la duración del elemento de trabajo para cada uno de los usuarios asignados.

>[!NOTE]
>
>Si no ha modificado la distribución automática de asignaciones en elementos de trabajo, las horas se redistribuyen de manera uniforme entre todas las personas asignadas cuando hay un cambio en el número de personas asignadas, la duración de una tarea o la cantidad de horas planificadas en el elemento de trabajo.

#### Acciones que restablecen asignaciones ajustadas {#actions-that-reset-adjusted-allocations}

Las siguientes acciones restablecen o modifican las asignaciones diarias, semanales o mensuales para los usuarios después de ajustarlas manualmente como se describe en la sección [Modificar asignaciones de usuario](#modify-user-allocations) de este artículo:

* Cuando se acorta la longitud de un elemento de trabajo que acorta la cantidad de días en su Duración, las horas asignadas ajustadas de los días perdidos se agregan a la cantidad de asignación del último día del elemento de trabajo.
* Al cambiar la cantidad de horas planificadas en una asignación o en el elemento de trabajo, el nuevo número de horas planificadas se redistribuye uniformemente para toda la duración del elemento de trabajo.
* Cuando se agrega o se quita un usuario asignado a un elemento de trabajo y esto hace que cambien las horas planificadas de la tarea, los valores ajustados se redistribuyen uniformemente.

#### Acciones que no restablecen asignaciones ajustadas {#actions-that-do-not-reset-adjusted-allocations}

Los siguientes cambios realizados en un elemento de trabajo no almacenan en déclencheur las asignaciones ajustadas para su restablecimiento o modificación:

* Cuando se mueven los días de un elemento de trabajo pero la cantidad de días de la Duración no cambia, los valores asignados ajustados permanecen igual y se mueven a las nuevas fechas.
* Al aumentar la Duración de un elemento de trabajo que aumenta el número de días en su Duración, las horas asignadas ajustadas siguen siendo las mismas para los días ajustados. Se agregan días adicionales al elemento de trabajo con 0 horas asignadas.
* Cuando agrega o quita un usuario asignado a un elemento de trabajo y esto no hace que cambien las horas planificadas del elemento, los valores ajustados permanecen igual.

## Localizar horas planificadas en el Distribuidor de cargas de trabajo

Puede modificar las asignaciones de usuarios a tareas o problemas mediante el Distribuidor de cargas de trabajo al encontrar las horas planificadas de las tareas o problemas asignados a los usuarios.

Tenga en cuenta lo siguiente al ver las horas planificadas en el Distribuidor de cargas de trabajo:

* El total de horas planificadas para una tarea o un problema se muestra junto al nombre de la tarea o el problema a la izquierda del Distribuidor de cargas de trabajo.

* El total de horas planificadas para un proyecto se muestra junto al nombre del proyecto a la izquierda del Distribuidor de cargas de trabajo. Representa el total de horas planificadas para todas las tareas y problemas enumerados en el proyecto en el Distribuidor de cargas de trabajo y no todas las horas planificadas del proyecto.
* La cantidad de tiempo asignado diaria o semanalmente para todas las tareas y para todos los proyectos se muestra solo cuando habilita manualmente la configuración Mostrar asignaciones. Para obtener información sobre cómo habilitar la configuración en el Distribuidor de cargas de trabajo, consulte [Navegación por el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Modificar asignaciones de usuario {#modify-user-allocations}

Como parte de la asignación de trabajo a los usuarios, puede modificar las asignaciones de usuarios en el Distribuidor de cargas de trabajo para garantizar que nunca se sobreasignen o para garantizar un equilibrio preciso de horas entre los recursos. Para obtener información sobre cómo identificar si un usuario está sobreasignado, consulte la sección [Resumen de asignación de usuarios](#user-allocation-overview) en este artículo.

1. Asegúrese de que tiene tareas y problemas asignados a los usuarios. Para obtener información sobre la asignación de trabajo a los usuarios en el Distribuidor de cargas de trabajo, consulte [Información general sobre la asignación de trabajo en el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).
1. Vaya al Distribuidor de cargas de trabajo.
1. (Opcional) Haga clic en **Semana** o **Mes** para administrar asignaciones semanales o mensuales para los usuarios.

   ![Seleccionar semana o mes](assets/month-icon-on-toolbar-selected-wb-350x226.png)

1. En el **Trabajo asignado** , busque el usuario para el que desea modificar manualmente la asignación y haga clic en la flecha hacia la derecha situada a la izquierda del nombre de usuario para expandir el usuario.

   ![Expandir usuario](assets/wb-highlight-on-name-caret2.png)

1. Haga clic en la flecha que señala a la derecha situada a la izquierda del nombre del proyecto para expandir el proyecto y mostrar los elementos de trabajo a los que está asignado el usuario.

   >[!TIP]
   >
   >Solo puede modificar las asignaciones de usuarios para tareas y problemas. No se pueden modificar las asignaciones de usuario para los proyectos.

1. (Opcional) Haga clic en **Mostrar asignaciones** icono ![](assets/show-allocations-icon-small.png) para mostrar las asignaciones de todos los elementos de trabajo.

   El nombre de las tareas y de los proyectos se reemplaza por la asignación del usuario para la tarea o el proyecto.

1. (Opcional) Haga clic en **Configuración** icono ![](assets/gear-icon-settings.png) y seleccione cualquiera de las siguientes opciones:

   1. **Incluir horas de problemas**. Esto le permite administrar las asignaciones de problemas además de las asignaciones de tareas.
   1. **Mostrar trabajo completado**. Esto muestra los elementos que se han completado y que están programados durante la cronología para la que administra las asignaciones.
   1. **Mostrar el tiempo restante**. Cambia el número total de horas de cada usuario (en la línea de usuario). Con esta configuración habilitada, el Distribuidor de cargas de trabajo muestra las horas que cada usuario tiene disponibles para trabajar en lugar del número de horas que se le asignan.

      >[!TIP]
      >
      >Modificar asignaciones cuando esta configuración está habilitada hace que disminuya el número total en la línea del usuario.

   1. **Proyecto** en el **Seleccionar tema de color** sección. Esto muestra cada proyecto y sus respectivos elementos de trabajo en colores únicos y facilita la comprensión de qué elementos pertenecen a cada proyecto.
   1. **Porcentaje** en el **Mostrar asignación de usuarios en** sección. Muestra las asignaciones como un valor porcentual. La capacidad del usuario según la programación se considera del 100%. Por ejemplo, si un usuario está asociado con una programación de 8 horas al día, 8 horas equivalen al 100 % de la capacidad. Si desea asignar al usuario para que trabaje 4 horas en un día, debe actualizar su asignación al 50 %.

      >[!NOTE]
      >
      >El administrador de Workfront decide qué programación utilizar en el sistema para calcular la capacidad del usuario en el área de Administración de recursos de la configuración. Para obtener más información, consulte [Configurar preferencias de administración de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

1. Haga clic en **Más** menú ![](assets/qs-more-menu.png) para un elemento de trabajo, haga clic en **Editar asignaciones**.

   ![Menú Más para elemento de trabajo](assets/more-menu-on-task-wb-nwe.png)

   O

   Haga doble clic en el día, la semana o el mes en la barra de una tarea o un problema.

   Los cuadros de asignación se pueden editar.

1. Haga clic dentro del cuadro de cada asignación diaria, semanal o mensual para actualizar manualmente la cantidad de horas o el valor porcentual para el que desea que se asigne al usuario cada día, semana o mes y, a continuación, haga clic en **Guardar** icono ![](assets/checkmark-icon.png).

   >[!TIP]
   >
   >Haga clic en **Cancelar** icono ![](assets/cancel-allocations-wb.png) para eliminar las asignaciones que ha ajustado.

   ![Guardar o cancelar asignaciones ajustadas](assets/wb-contouring-with-check-and-x-boxes-350x63.png)

   Las asignaciones para la actualización de usuario.

   >[!TIP]
   >
   >Si una tarea o un problema se completan antes de la fecha planificada de finalización, el número de horas asignadas para los días restantes se alcanza y no se cuenta para la asignación general del usuario. Esto solo se muestra cuando tanto la variable **Mostrar asignaciones** y el icono **Mostrar fechas proyectadas** están activadas.

   Existen los siguientes escenarios:

   * Para las tareas con tipos de duración que no son simples o para los problemas, el total de las asignaciones debe coincidir con las horas planificadas para que pueda hacer clic en el icono de marca de verificación.
   * Para las tareas con un Tipo de duración simple, el total de las asignaciones puede ser mayor o menor que las Horas planificadas y puede hacer clic en el icono de la marca de verificación aunque no coincidan. Esto también actualiza la cantidad de horas planificadas para la tarea. Debe tener los permisos y el acceso correctos para actualizar las horas planificadas en las tareas desde el Distribuidor de cargas de trabajo.

     >[!TIP]
     >
     >Un icono de candado se muestra a la derecha del nombre de la tarea a medida que empieza a ajustar las asignaciones para indicar que la tarea tiene un tipo de duración simple.

     ![Icono de bloqueo](assets/lock-icon-on-simple-task-in-the-balancer.png)

   Para obtener más información sobre las condiciones que deben cumplirse para actualizar las horas planificadas en el Distribuidor de cargas de trabajo, consulte la [Actualizar horas planificadas de la tarea al administrar las asignaciones de usuario](#update-task-planned-hours-when-managing-user-allocations) de este artículo. Para obtener información sobre los tipos de duración de tareas, consulte [Información general sobre la duración y el tipo de duración de la tarea](../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Condicional) Si la tarea está asignada a más de un usuario, repita estos pasos para cada usuario asignado a la tarea para actualizar las asignaciones de cada usuario.

   Cualquier persona que tenga acceso para ver el Distribuidor de cargas de trabajo y vea los mismos usuarios y los mismos proyectos que administró ahora verá la asignación actualizada para los usuarios que administró.

>[!TIP]
>
><span class="preview">Aparece un icono de lápiz a la derecha del nombre del elemento de trabajo para indicar que se ajustó manualmente.</span>

![Icono de horas ajustadas manualmente](assets/icon-for-manually-adjusted-hours.png)

## Actualizar horas planificadas de la tarea al administrar las asignaciones de usuario {#update-task-planned-hours-when-managing-user-allocations}

Puede actualizar las horas planificadas de una tarea al administrar las asignaciones de usuarios en el Distribuidor de cargas de trabajo para la tarea. Esto sucede cuando el total de las horas asignadas actualizadas no coincide con el total original de las horas planificadas para una tarea.

>[!IMPORTANT]
>
>* Actualizar las horas planificadas de las tareas puede afectar al progreso del proyecto.
>* La actualización manual de las horas planificadas mediante el cambio de las asignaciones diarias puede afectar a las horas planificadas cuando se eliminen asignaciones de las tareas en el futuro. Para obtener más información, consulte [Resumen de horas planificadas](../../manage-work/tasks/task-information/planned-hours.md).
>
>* No es posible actualizar las horas planificadas de los problemas al actualizar las asignaciones en el Distribuidor de cargas de trabajo.

Esto es posible cuando existen las siguientes condiciones:

* Tiene los permisos y el acceso correctos para administrar las horas planificadas desde el Distribuidor de cargas de trabajo. Entre ellos se incluyen los siguientes:

   * Administrar permisos para las tareas.
   * Actualice las horas planificadas en el acceso del Distribuidor de cargas de trabajo en el área de Administración de recursos de su nivel de acceso.

  Para obtener más información sobre el acceso necesario para utilizar el Distribuidor de cargas de trabajo, consulte la [Requisitos de acceso](#access-requirements) de este artículo.

* La tarea tiene un Tipo de duración de Simple.

