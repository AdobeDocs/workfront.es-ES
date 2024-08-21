---
user-type: administrator
product-area: system-administration;user-management
keywords: grupo,preferencias,tarea,grupos,problema,desbloquear
navigation-topic: create-and-manage-groups
title: Configurar las preferencias de horas y hojas de horas para un grupo
description: En el nivel del sistema, un administrador de Adobe Workfront puede desbloquear las secciones de plantilla de horas y preferencias de horas Preferencias generales y Rellenar de forma previa las plantillas de horas con. Esto permite a los administradores de grupos configurar las opciones de esas secciones de forma independiente para sus propios grupos.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '1364'
ht-degree: 1%

---

# Configurar las preferencias de horas y hojas de horas de un grupo

Un administrador de Adobe Workfront puede desbloquear las siguientes secciones de la plantilla de horas y las preferencias de horas en el sistema para que los administradores de grupos puedan configurarlas de forma independiente para sus propios grupos:

* Preferencias generales
* Dónde pueden registrar el tiempo los usuarios
* Rellenar previamente las plantillas de horas

Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

Las siguientes secciones de la página Preferencias de plantilla de horas y horas solo se pueden configurar en el sistema y no se pueden desbloquear para grupos:

* Proyectos, tareas y problemas eliminados

Para obtener información sobre cómo un administrador de Workfront desbloquea una hoja de horas y preferencias de horas, consulte la sección [Desbloquear hoja de horas y preferencias de horas para grupos](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) en el artículo [Configurar preferencias de horas y hojas de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

>[!TIP]
>
>La configuración de nivel de grupo también es posible para las preferencias de proyecto y para las preferencias de tarea y problema. Para obtener más información, vea [Configurar las preferencias de proyecto para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) y [Configurar las preferencias de tarea y problema para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Debe ser administrador de grupo del grupo o de Workfront. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> y <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con su administrador de Workfront.

+++

## Agrupar preferencias de horas y hojas de horas

Tenga en cuenta la siguiente información sobre la configuración de una plantilla de horas o preferencia de horas desbloqueadas para un grupo:

* Si es administrador de un grupo y configura una plantilla de horas o una preferencia de horas para su grupo, esto afectará a las personas que usen el grupo como su grupo de inicio.
* Normalmente, una preferencia desbloqueada permanece desbloqueada indefinidamente. Si el administrador de Workfront vuelve a bloquearlo, la configuración del sistema vuelve a tener efecto y se pierde la configuración de las preferencias realizadas por los administradores del grupo.
* Una plantilla de horas hereda la plantilla de horas y las preferencias de horas configuradas para el grupo de inicio del propietario de la plantilla de horas.

  <!--
  Add example here?
  -->

* Una vez que un administrador de Workfront desbloquea una preferencia en el sistema y usted la configura para su grupo, puede bloquearla para asegurarse de que todos los miembros de los grupos debajo del suyo estén usando la misma configuración. Esto es paralelo a la capacidad que tiene un administrador de Workfront para configurar y bloquear una preferencia para todos los miembros del sistema. Para obtener más información, consulte [Bloquear o desbloquear una hoja de horas de grupo y preferencia de horas](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

## Configurar una hoja de horas o preferencia de horas desbloqueadas para un grupo

>[!TIP]
>
>Si es administrador de Workfront, puede omitir los pasos del 1 al 4 en Configuración > Plantilla de horas y Horas > Preferencias y, a continuación, buscar el nombre del grupo en el cuadro de la parte superior de la página.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos** ![](assets/groups-icon.png).

1. Haga clic en el nombre del grupo cuya hoja de horas o preferencias de hora desee configurar.
1. En el panel izquierdo, haga clic en **Hojas de horas y horas**.

1. En la página que se muestra, en la sección **Preferencias generales**, configure cualquiera de las siguientes opciones:

   >[!TIP]
   >
   >Si pasa el ratón por encima de una preferencia y se muestra información del objeto para indicarle que está bloqueada, puede pedir al administrador de Workfront que la desbloquee para todos los grupos de la organización.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Registrar tiempo para fechas futuras</td> 
      <td> <p>Permite a los usuarios registrar tiempo para fechas futuras en todo el sistema en:</p> 
       <ul> 
       <li>Proyectos, tareas y problemas a los que tengan acceso para registrar tiempo, independientemente del grupo del proyecto</li> 
       <li>Sus hojas de horas como Hora general</li>
       </ul> 
       <p>Esto resulta útil cuando los usuarios planean estar fuera de la oficina y desean registrar esa hora de antemano.</p> 
       <p><b>NOTA</b>: no puede evitar que los usuarios registren la hora en tareas o problemas que se hayan cerrado o cancelado. Solo puede evitar que los usuarios registren el tiempo en proyectos completos o inactivos. Le recomendamos que utilice filtros en listas de tareas y problemas para excluir de la visibilidad a los usuarios los que se hayan completado o cancelado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Agregar gastos de una hoja de horas</td> 
      <td> <p>Permite que los usuarios registren tanto el tiempo como los gastos en la hoja de horas.</p> 
      <p>Cuando esta preferencia está habilitada para un grupo y el grupo se establece como el grupo de inicio para ciertos usuarios, aparece un icono de gastos junto a los proyectos y las tareas de las hojas de horas de esos usuarios. Los usuarios pueden hacer clic en este icono para agregar o editar gastos para el proyecto o la tarea.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Asignar roles a entradas de horas manualmente</td> 
      <td> <p>Permite que los usuarios seleccionen manualmente cualquier rol asignado en su perfil de usuario o asignado al objeto.</p> <p><b>IMPORTANTE</b>:  
        <ul> 
         <li>Si deshabilita esta configuración después de asignar los roles a las entradas de horas, los usuarios deben ajustar las horas registradas en varios roles en la pestaña Horas del proyecto, tarea o problema.</li> 
         <li>Si el usuario no tiene una función de trabajo asignada en su perfil y hay una tarea asignada como Propietario de la tarea en el cuadro de diálogo Asignaciones avanzadas, esa función de trabajo aparece cuando el usuario registra tiempo en la tarea.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Restringir la edición de hojas de horas a propietarios y administradores</td> 
      <td> <p>Restrinja la edición a los propietarios de plantillas de horas, independientemente del grupo del proyecto y de los administradores de Workfront. Si se deshabilita esta opción, las plantillas de horas también se pueden editar:</p> 
       <ul> 
        <li> <p>Usuarios con acceso administrativo a hojas de horas y horas en su nivel de acceso</p> </li> 
        <li> <p>Aprobadores de hojas de horas si "Puede editar horas" está habilitado en la hoja de horas</p> </li> 
        <li> <p>El administrador del propietario de la plantilla de horas</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Restringir la edición de horas a propietarios y administradores</td> 
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
      <td role="rowheader">Registrar tiempo directamente en los proyectos</td> 
      <td>Permite a los usuarios registrar tiempo en el proyecto (tanto en la pestaña Actualizaciones como en la hoja de horas). Si desea restringir el tiempo de registro de los usuarios en el nivel de proyecto, deje esta opción sin marcar.</td>
     </tr>
     <tr>
      <td role="rowheader">Registrar tiempo en proyectos completos</td>
      <td>Permite a los usuarios registrar el tiempo de un proyecto que se ha marcado como completado. Si esta opción está deshabilitada, los usuarios no podrán registrar el tiempo de trabajo que hayan completado en los proyectos en el estado Completado.</td>
     </tr>
     <tr>
      <td role="rowheader">Registrar tiempo en proyectos inactivos</td> 
      <td>Cuando esta opción está habilitada, los usuarios pueden registrar horas en los proyectos con el estado Inactivo.</td>
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >Esta preferencia se aplica según la configuración de las preferencias del grupo de inicio del usuario. Si esta configuración está habilitada en las preferencias de grupo de inicio del usuario, podrá registrar tiempo directamente en los proyectos, incluidos los proyectos completados o inactivos, independientemente de si las preferencias de grupo del proyecto lo permiten o no.

1. En la sección **Rellenar previamente hojas de horas**, configure cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Trabajo que se encuentra dentro de un &lt;number of week&gt; del intervalo de trabajo de la plantilla de horas</td> 
      <td> <p>Define el número de semanas antes y después del intervalo de fechas de la hoja de horas que contiene las fechas de las tareas y problemas asignados al usuario. La configuración predeterminada es 1 semana y puede ampliar este intervalo a 4 semanas. Esto significa que la hoja de horas se rellena previamente con tareas y problemas que tienen fechas entre cuatro semanas antes del intervalo de fechas de la hoja de horas y hasta cuatro semanas después del intervalo de fechas de la hoja de horas, si selecciona 4 semanas para el intervalo de fechas. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tareas y problemas que se han completado</td> 
      <td>Si se suelen asignar varios recursos a una sola tarea, se recomienda esta configuración. Esto significa que cuando un recurso registra la hora con la tarea y la marca como completada, los demás recursos asignados a la tarea pueden encontrar la tarea o el problema en su hoja de horas para registrar sus horas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tareas y problemas con fechas planificadas que se encuentren en el rango de fechas de la hoja de horas</td> 
      <td> <p>Una vez seleccionada, la hoja de horas incluye tareas y problemas con una fecha planificada de inicio o una fecha de finalización que se encuentran dentro del intervalo de fechas de la hoja de horas.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> Tareas con fechas proyectadas que se encuentren en el rango de fechas de la hoja de horas</td> 
      <td> <p>Cuando se selecciona, la hoja de horas incluye tareas que tienen una Fecha proyectada de inicio o Fecha de finalización que se encuentra dentro del marco de tiempo del proyecto, incluso si la fecha planificada del problema o la tarea está fuera del intervalo de fechas de la hoja de horas.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.
