---
user-type: administrator
product-area: system-administration;user-management
keywords: grupo,preferencias,tarea,grupos,problema,desbloquear
navigation-topic: create-and-manage-groups
title: Configuración de las preferencias de horas y horas de un grupo
description: A nivel del sistema, un administrador de Adobe Workfront puede desbloquear las secciones de preferencias de horas y horas Preferencias generales y cumplimentar hojas de horas previamente con. Esto permite a los administradores de grupos configurar las opciones de esas secciones de forma independiente para sus propios grupos.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1203'
ht-degree: 5%

---

# Configuración de las preferencias de horas y horas de un grupo

Un administrador de Adobe Workfront puede desbloquear las siguientes secciones de las preferencias de horario y horario a nivel del sistema para que los administradores de grupo puedan configurarlas de forma independiente para sus propios grupos:

* Preferencias generales
* Rellenar de forma previa las hojas de horas con

Si hay algún grupo por encima del grupo que administra, sus administradores también pueden hacerlo por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

Las siguientes secciones de la página Preferencias de parte de horas y horas solo se pueden configurar a nivel del sistema y no se pueden desbloquear para grupos:

* Tiempo de registro
* Preferencias de eliminación de proyecto, tarea o problema

Para obtener información sobre cómo un administrador de Workfront desbloquea un parte de horas y una preferencia de hora, consulte la sección [Desbloquear preferencias de horas y horas para grupos](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) en el artículo [Configuración de las preferencias de horas y horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

>[!TIP]
>
>La configuración a nivel de grupo también es posible para las preferencias de proyecto y para las preferencias de tarea y problema. Para obtener más información, consulte [Configuración de las preferencias de un proyecto para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) y [Configuración de las preferencias de tarea y problema para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Debe ser administrador de grupo del grupo o administrador de Workfront. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> y <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con el administrador de Workfront.

## Agrupar preferencias de horas y horas

Tenga en cuenta la siguiente información sobre la configuración de un parte de horas o preferencia de hora desbloqueados para un grupo:

* Si es un administrador de grupo y configura un parte de horas o una preferencia de hora para su grupo, esto afecta a las personas que usan el grupo como su grupo principal.
* Normalmente, una preferencia desbloqueada permanece desbloqueada indefinidamente. Si el administrador de Workfront lo vuelve a bloquear, la configuración del sistema se aplica de nuevo y se pierde la configuración de las preferencias de los administradores del grupo.
* Un parte de horas hereda las preferencias de horas y hojas de horas configuradas para el grupo principal del propietario del parte de horas.

   <!--
  Add example here?
  -->

* Una vez que un administrador de Workfront desbloquea una preferencia a nivel de sistema y la configura para su grupo, puede bloquearla para asegurarse de que todos los miembros de los grupos debajo de la suya usen la misma configuración. Esto es paralelo a la capacidad que tiene un administrador de Workfront para configurar y bloquear una preferencia para todos los miembros del sistema. Para obtener más información, consulte [Bloquear o desbloquear un grupo de preferencias de horas y horas](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

## Configurar una hoja de horas o preferencia de hora desbloqueada para un grupo

>[!TIP]
>
>Si es administrador de Workfront, puede evitar los pasos del 1 al 4 accediendo a Configuración > Horario y horas > Preferencias y buscando el nombre del grupo en el cuadro de la parte superior de la página.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).

1. Haga clic en el nombre del grupo cuyas preferencias de horario u hora desee configurar.
1. En el panel izquierdo, haga clic en **Hojas de hora y horas**.

1. En la página que se muestra, en la sección **Preferencias generales** , configure cualquiera de las siguientes opciones:

   >[!TIP]
   >
   >Si pasa el ratón sobre una preferencia y aparece un aviso para decirle que está bloqueado, puede solicitar al administrador de Workfront que la desbloquee para todos los grupos de la organización.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Registrar tiempo para fechas futuras</td> 
      <td> <p>Permite a los usuarios registrar la hora de las fechas futuras en todo el sistema en:</p> 
       <ul> 
       <li>Todos los proyectos, tareas y problemas en los que tengan acceso al tiempo de registro, independientemente del grupo del proyecto</li> 
       <li>Sus partes de horas como hora general</li>
       </ul> 
       <p>Esto resulta útil cuando los usuarios planean estar fuera de la oficina y desean hacerlo antes.</p> 
       <p><b>NOTA</b>: No puede impedir que los usuarios inicien sesión en tareas o problemas que se hayan cerrado o cancelado. Solo puede evitar que los usuarios inicien sesión en proyectos completos o en ejecución. Se recomienda utilizar filtros en listas de tareas y problemas para excluir los que se han completado o cancelado de la visibilidad de los usuarios.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Agregar gastos de una hoja de horas</td> 
      <td> <p>Permite a los usuarios registrar el tiempo y los gastos en el parte de horas.</p> 
      <p>Cuando esta preferencia está habilitada para un grupo y el grupo está establecido como grupo principal para determinados usuarios, aparece un icono de gastos junto a los proyectos y tareas en las hojas de horas de esos usuarios. Los usuarios pueden hacer clic en este icono para añadir o editar los gastos del proyecto o la tarea.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Asignar roles a entradas de horas manualmente</td> 
      <td> <p>Permita a los usuarios seleccionar manualmente cualquier función de trabajo asignada en su perfil de usuario o asignada al objeto.</p> <p><b>IMPORTANTE</b>:  
        <ul> 
         <li>Si deshabilita esta configuración después de asignar funciones de trabajo a entradas de hora, los usuarios deben ajustar las horas registradas en las distintas funciones en la ficha Horas del proyecto, tarea o problema.</li> 
         <li>Si el usuario no tiene una función de trabajo asignada en su perfil y hay una tarea asignada como Propietario de la Tarea en el cuadro de diálogo Asignaciones avanzadas, esa función de trabajo aparece cuando el usuario inicia sesión en la tarea.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Restrinja la edición de la plantilla de horas trabajadas a los propietarios y administradores</td> 
      <td> <p>Restringir la edición a propietarios de hojas de horas, independientemente del grupo del proyecto y los administradores de Workfront. Cuando esta opción está deshabilitada, las hojas de horas también se pueden editar:</p> 
       <ul> 
        <li> <p>Usuarios con acceso administrativo a hojas de horas y horas en su nivel de acceso</p> </li> 
        <li> <p>Aprobadores de parte de horas si "Puede editar horas" está habilitado en el parte de horas</p> </li> 
        <li> <p>El administrador del propietario del parte de horas</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Restringir la edición de horas a propietarios y administradores</td> 
      <td>Restrinja la edición al usuario que ha introducido las horas y a los administradores de Workfront. Esta configuración se aplica a la ficha Horas de un proyecto o a un informe de horas.</td> 
     </tr> 
    </tbody> 
   </table>

1. En el **Rellenar partes de horas previamente con** , configure cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Trabajo que se encuentra dentro de &lt;number of="" weeks=""&gt; del rango de trabajo del parte de horas</td> 
      <td> <p>Define el número de semanas antes y después del intervalo de fechas del parte de horas que contiene fechas de tareas y problemas asignados al usuario. El valor predeterminado es 1 semana y se puede ampliar este intervalo a 4 semanas. Esto significa que el parte de horas se rellena previamente con tareas y problemas que tienen fechas entre cuatro semanas antes del intervalo de fechas del parte de horas y hasta cuatro semanas después del intervalo de fechas del parte de horas, si selecciona 4 semanas para el intervalo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tareas y problemas que se han completado</td> 
      <td>Si se asignan varios recursos a una sola tarea, se recomienda esta configuración. Esto significa que cuando un recurso registra la hora en la tarea y la marca como completa, los demás recursos asignados a la tarea aún pueden encontrar la tarea o el problema en su parte de horas, para registrar sus horas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tareas y problemas con fechas planificadas que se encuentren en el rango de fechas de la hoja de horas</td> 
      <td> <p>Cuando se selecciona, el parte de horas incluye tareas y problemas que tienen una Fecha de inicio planificada o una Fecha de finalización que se encuentra dentro del intervalo de fechas del parte de horas.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> Tareas con fechas proyectadas que se encuentren en el rango de fechas de la hoja de horas</td> 
      <td> <p>Cuando se selecciona, el parte de horas incluye tareas que tienen una Fecha de inicio prevista o una Fecha de finalización comprendida dentro del lapso de tiempo del proyecto, incluso si la fecha planificada del problema o la tarea queda fuera del intervalo de fechas del parte de horas.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.
