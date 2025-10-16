---
user-type: administrator
product-area: system-administration;user-management
keywords: grupo,preferencias,tarea,grupos,problema,desbloquear
navigation-topic: create-and-manage-groups
title: Configurar las preferencias de horas y hojas de horas para un grupo
description: En el nivel del sistema, un administrador de Adobe Workfront puede desbloquear la plantilla de horas y las secciones de preferencias de horas Preferencias generales y Rellenar de forma previa las hojas de horas con. Esto permite a los administradores de grupos configurar las opciones de esas secciones de forma independiente para sus propios grupos.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: a42a167447d2f11b5502e4a0953b5e7eec2e67b1
workflow-type: tm+mt
source-wordcount: '1336'
ht-degree: 97%

---

# Configurar las plantillas de horas y las preferencias de horas de un grupo

Un administrador de Adobe Workfront puede desbloquear las siguientes secciones de la plantilla de horas y las preferencias de horas en el nivel del sistema para que los administradores de grupos puedan configurarlas de forma independiente para sus propios grupos:

* Preferencias generales
* Dónde pueden registrar el tiempo los usuarios
* Rellenar previamente las plantillas de horas

Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

Las siguientes secciones de la página Plantilla de horas y Preferencias de horas solo se pueden configurar en el nivel del sistema y no se pueden desbloquear para los grupos:

* Proyectos, tareas y problemas eliminados

Para obtener información sobre cómo los administradores de Workfront desbloquean preferencias de horas y plantillas de horas, consulte la sección [Desbloquear las preferencias de horas y plantillas de horas para grupos](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) del artículo [Configuración de preferencias de horas y plantillas de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

>[!TIP]
>
>La configuración a nivel de grupo también es posible para las preferencias de proyecto y para las preferencias de tarea y problema.  Para obtener información, consulte [Configurar las preferencias del proyecto de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) y [Configurar las preferencias de tareas y problemas para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de grupo del grupo o administrador del sistema.</td>
  </tr>
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Plantilla de horas y preferencia de horas del grupo

Tenga en cuenta la siguiente información sobre la configuración de una plantilla de horas o preferencia de horas desbloqueadas para un grupo:

* Si es administrador de grupos y configura una plantilla de horas o una preferencia de horas para su grupo, esto afectará a las personas que usen el grupo como su grupo de inicio.
* Normalmente, una preferencia desbloqueada permanecerá desbloqueada indefinidamente. Si el administrador de Workfront volviese a bloquearla, la configuración del sistema volverá a tener efecto y se perderá la configuración de las preferencias realizadas por los administradores del grupo.
* Una plantilla de horas hereda la plantilla de horas y las preferencias de horas configuradas para el grupo de inicio del propietario de la plantilla de horas.

  <!--
  Add example here?
  -->

* Una vez que un administrador de Workfront desbloquea una preferencia en el nivel del sistema y usted la configura para su grupo, puede bloquearla para asegurarse de que todos los miembros de los grupos por debajo del suyo estén usando la misma configuración. Esto es similar a la capacidad que tiene un administrador de Workfront para configurar y bloquear preferencias para todos los miembros del sistema. Para obtener más información, consulte [Bloquear o desbloquear una hoja de horas y preferencia de horas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

## Configurar una hoja de horas o preferencia de horas desbloqueadas para un grupo

>[!TIP]
>
>Si es administrador de Workfront, puede omitir los pasos del 1 al 4 desde Configuración > Plantilla de horas trabajadas y horas > Preferencias y, a continuación, buscar el nombre del grupo en el cuadro de la parte superior de la página.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![Grupos](assets/groups-icon.png).

1. Haga clic en el nombre del grupo cuya hoja de horas o preferencias de horas desee configurar.
1. En el panel izquierdo, haga clic en **Horas y plantillas de horas trabajadas**.

1. En la página que se muestra, en la sección **Preferencias generales**, configure cualquiera de las siguientes opciones:

   >[!TIP]
   >
   >Si al pasar el puntero por encima de una preferencia se mostrase ayuda contextual indicando que está bloqueada, pida al administrador de Workfront que la desbloquee para todos los grupos de la organización.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Registrar tiempo para fechas futuras</td> 
      <td> <p>Permite a los usuarios registrar tiempo para fechas futuras en todo el sistema en:</p> 
       <ul> 
       <li>Cualquier proyecto, tarea y problema a los que tengan acceso para registrar tiempo, independientemente del grupo del proyecto</li> 
       <li>Sus plantillas de horas como hora general</li>
       </ul> 
       <p>Esto resulta útil cuando los usuarios planean estar fuera de la oficina y desean registrar esas horas de antemano.</p> 
       <p><b>NOTA</b>: No puede evitar que los usuarios registren la hora en tareas o problemas que se hayan cerrado o cancelado. Solo puede evitar que los usuarios registren el tiempo en proyectos completos o inactivos. Le recomendamos que utilice filtros en listas de tareas y problemas para excluir de la visibilidad a los usuarios los que se hayan completado o cancelado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Añadir gastos de una plantilla de horas</td> 
      <td> <p>Permite que los usuarios registren tanto el tiempo como los gastos en la plantilla de horas.</p> 
      <p>Cuando esta preferencia está habilitada para un grupo y el grupo se establece como el grupo de inicio para ciertos usuarios, aparece un icono de gastos junto a los proyectos y las tareas de las plantillas de horas de esos usuarios. Los usuarios pueden hacer clic en este icono para añadir o editar gastos para el proyecto o la tarea.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Asignar funciones a entradas de horas manualmente.</td> 
      <td> <p>Permite que los usuarios seleccionen manualmente cualquier rol asignado en su perfil de usuario o asignado al objeto.</p> <p><b>IMPORTANTE</b>:  
        <ul> 
         <li>Si deshabilita esta configuración después de asignar las funciones a las entradas de horas, los usuarios deben ajustar las horas registradas en varios roles en la pestaña Horas del proyecto, la tarea o el problema.</li> 
         <li>Si el usuario no tiene una función asignada en su perfil y hay una tarea asignada como Propietario de la tarea en el cuadro de diálogo Asignaciones avanzadas, esa función aparece cuando el usuario registra tiempo en la tarea.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Restrinja la edición de la plantilla de horas trabajadas a los propietarios y administradores.</td> 
      <td> <p>Restrinja la edición a los propietarios de plantillas de horas, independientemente del grupo del proyecto y de los administradores de Workfront. Si se deshabilita esta opción, las plantillas de horas también se pueden editar:</p> 
       <ul> 
        <li> <p>Usuarios con acceso administrativo a hojas de horas y horas en su nivel de acceso</p> </li> 
        <li> <p>Aprobadores de hojas de horas si “Puede editar horas” está habilitado en la hoja de horas</p> </li> 
        <li> <p>El administrador del responsable del parte de horas</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Restrinja la edición de la plantilla de horas trabajadas a los propietarios y administradores.</td> 
      <td>Restrinja la edición al usuario que introduce las horas y a los administradores de Workfront. Esta configuración se aplica a la ficha Horas de un proyecto o de un informe de horas.</td> 
     </tr> 
    </tbody> 
   </table>

1. En la sección **Donde los usuarios pueden registrar el tiempo**, configure cualquiera de las siguientes opciones:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">Registrar tiempo directamente en los proyectos.</td> 
      <td>Permite a los usuarios registrar tiempo en el proyecto (tanto en la pestaña Actualizaciones como en la plantilla de horas). Si desea restringir el tiempo de registro de los usuarios en el nivel de proyecto, deje esta opción sin marcar.</td>
     </tr>
     <tr>
      <td role="rowheader">Registrar tiempo en proyectos completos.</td>
      <td>Permite a los usuarios registrar el tiempo de un proyecto que se ha marcado como completado. Si esta opción está deshabilitada, los usuarios no podrán registrar el tiempo de trabajo que hayan completado en los proyectos en el estado Completado.</td>
     </tr>
     <tr>
      <td role="rowheader">Registrar tiempo en proyectos inactivos.</td> 
      <td>Cuando esta opción está habilitada, los usuarios pueden registrar horas en los proyectos con el estado Inactivo.</td>
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >Esta preferencia se aplica según la configuración de las preferencias del grupo de inicio del usuario. Si esta configuración está habilitada en las preferencias de grupo de inicio del usuario, podrá registrar tiempo directamente en los proyectos, incluidos los proyectos completados o inactivos, independientemente de si las preferencias de grupo del proyecto lo permiten o no.

1. En la sección **Rellenar previamente plantillas de horas**, configure cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Trabajo que se encuentra en un lapso temporal de &lt;número de semanas&gt; del intervalo de trabajo de la plantilla de horas</td> 
      <td> <p>Define el número de semanas antes y después del intervalo de fechas de la plantilla de horas que contiene las fechas de las tareas y problemas asignados al usuario. La configuración predeterminada es 1 semana y puede ampliar este intervalo a 4 semanas. Esto significa que la plantilla de horas se rellena previamente con tareas y problemas que tienen fechas entre cuatro semanas antes del rango de fechas de la plantilla de horas y hasta cuatro semanas después del rango de fechas de la hoja de tiempo, si selecciona 4 semanas para su rango. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tareas y problemas que se han completado</td> 
      <td>Si normalmente se asignan varios recursos a una sola tarea, recomendamos esta configuración. Esto significa que cuando un recurso registra tiempo en la tarea y la marca como completa, los otros recursos asignados a la tarea aún pueden encontrar la tarea o el problema en su hoja de tiempo para registrar sus horas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tareas y problemas con fechas planificadas que se encuentren en el rango de fechas de la plantilla de horas</td> 
      <td> <p>Cuando se selecciona, la plantilla de horas incluye tareas y problemas que tengan una Fecha de inicio y de finalización planificada que se encuentre dentro del intervalo de fechas de la plantilla de horas.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> Tareas con fechas proyectadas que se encuentren en el rango de fechas de la plantilla de horas</td> 
      <td> <p>Cuando se selecciona, la plantilla de horas incluye tareas que tengan una fecha de inicio o de finalización proyectada dentro del lapso de tiempo del proyecto, incluso si la fecha planificada del problema o tarea está fuera del rango de fechas de la plantilla de horas.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.
