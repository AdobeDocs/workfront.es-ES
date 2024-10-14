---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Crear hoja de horas de un solo uso
description: Puede crear manualmente una plantilla de horas de un solo uso si desea una plantilla de horas que no sea recurrente. Cuando llegue la fecha de finalización de la plantilla de horas y necesite más plantillas, debe crear otras nuevas.
author: Alina
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: 2ccf2775a858371aacdb6e8637fd5a30a212a82d
workflow-type: tm+mt
source-wordcount: '1058'
ht-degree: 0%

---

# Crear hoja de horas de un solo uso

Puede crear manualmente una plantilla de horas de un solo uso si desea una plantilla de horas que no sea recurrente. Cuando llegue la fecha de finalización de la plantilla de horas y necesite más plantillas, debe crear otras nuevas.

Para obtener información sobre cómo crear un perfil de hoja de horas que genere hojas de horas recurrentes para los usuarios sin ninguna otra intervención por su parte (recomendado), consulte [Crear, editar y asignar perfiles de hoja de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

>[!NOTE]
>
>* No se pueden crear plantillas de horas de un solo uso para grupos.
>  <!--
>  <span>Making sure with Lilit that this is correct</span>>
>  -->
>* Al crear una plantilla de horas de un solo uso, no puede seleccionar tipos de horas generales específicos para incluirlos en la plantilla de horas. Todos los tipos de horas generales que se activan en el sistema se muestran en hojas de horas creadas manualmente.
>
>  Si desea seleccionar solo ciertos tipos generales de horas para mostrarlos en sus hojas de horas, utilice un perfil de hoja de horas. Para obtener más información sobre los perfiles de hojas de horas, consulte [Crear, editar y asignar perfiles de hojas de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
>

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nuevo: estándar </p>
   <p>Actual: plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe tener acceso administrativo a las hojas de horas. </p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a ciertas áreas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso a la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear hoja de horas de un solo uso

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Plantillas de horas**. El filtro **Todos** está seleccionado de manera predeterminada. Esto muestra todas las hojas de horas que tiene acceso a ver.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Opcional) Realice una de las siguientes acciones para actualizar el filtro en la lista de plantillas de horas:

   * Seleccione **Mis aprobaciones de hojas de horas** en la esquina superior derecha de la página para ver solamente las hojas de horas que usted apruebe

     O

     Seleccione **Mis hojas de horas** para ver solamente sus hojas de horas.

     Esto aplica los filtros Mis aprobaciones de hojas de horas o Mis hojas de horas a la lista de hojas de horas.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Haga clic en el icono Filtro ![](assets/filter-nwepng.png) para aplicar un filtro diferente o crear uno nuevo. Para obtener información sobre cómo crear o actualizar filtros, consulte [Crear o editar filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Las opciones Mis aprobaciones de hojas de horas y Mis hojas de horas no se muestran en la parte superior de la lista de hojas de horas ni en la lista de filtros si el administrador de Workfront o de un grupo ha eliminado los filtros Mis aprobaciones de hojas de horas y Mis hojas de horas de los controles de Lista en el área Configuración o de la plantilla Diseño. Para obtener más información, consulte los siguientes artículos:
   > 
   >   * [Personalizar filtros, vistas y agrupaciones mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Opcional) Haga clic en el icono **Buscar** ![](assets/search-icon.png) para escribir una palabra clave y buscar una hoja de horas específica. Por ejemplo, puede buscar un marco de tiempo de hoja de horas con el nombre del propietario.

1. (Opcional) Haga clic en los iconos **Ver** ![](assets/view-icon.png) o **Agrupar** ![](assets/grouping.png) para aplicar una vista o agrupación diferente o para crear una nueva.

   Para obtener información sobre la creación de filtros, vistas o agrupaciones, consulte los siguientes artículos:

   * [Crear o editar filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Crear o editar vistas en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Creación de agrupaciones en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Haga clic en **Nueva hoja de horas** al principio de la lista de hojas de horas.

   Especifique la siguiente información:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>Crear hoja de horas para</strong> </td> 
      <td>Comience a introducir el nombre del usuario, un rol o un equipo para el que está creando la plantilla de horas y haga clic en ellos cuando se muestren en la lista.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Fecha de inicio</strong> </td> 
      <td>Es la fecha de inicio de la hoja de horas.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Fecha de finalización</strong> </td> 
      <td> Fecha de finalización de la plantilla de horas.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Aprobadores</strong> </td> 
      <td>Los aprobadores son usuarios que aprueban la hoja de horas de los usuarios asociados con ella. Solo los usuarios con derechos administrativos de hoja de horas pueden establecerse como aprobadores. Para obtener más información sobre los derechos administrativos de la hoja de horas, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder acceso administrativo a los usuarios a ciertas áreas</a>.<br>Empiece a introducir los nombres de los aprobadores de hojas de horas y haga clic en ellos cuando aparezcan en la lista.<br>Puede tener varios aprobadores en una hoja de horas. En este caso, una vez que uno de los aprobadores aprueba la hoja de horas, esta se marca como <strong>Cerrada</strong> y desaparece de la lista de aprobaciones de hojas de horas de todos los aprobadores restantes.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Puede editar el tiempo</strong> </td>

   <td> <p>Seleccione esta opción si desea permitir que los aprobadores editen las horas en la hoja de horas.</p>

   Esta opción funciona junto con **Restringir la edición de hojas de horas a propietarios y administradores** en el área Configuración > Hoja de horas y horas > Preferencias. Para obtener más información, consulte <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configurar la hoja de horas y las preferencias de horas</a>.

   Existen los siguientes escenarios:

   <ul>
      <li>Cuando la opción <b>Restringir la edición de hojas de horas a propietarios y administradores</b> esté habilitada:</li>
   <ul><li>Los aprobadores solo pueden aprobar y rechazar hojas de horas, independientemente de si <b>Puede editar el tiempo</b> está habilitado o no. </li>
   <li>Los administradores de propietarios de hojas de horas solo pueden ver las hojas de horas de sus subordinados directos.</li></ul>
   <li>Cuando la opción <b>Restringir la edición de hojas de horas a propietarios y administradores</b> esté deshabilitada:</li>
   <ul><li>Cuando la opción <b>Puede editar la hora</b> está habilitada, los aprobadores pueden enviar, reabrir o cerrar la hoja de horas y pueden editar la hora.</li>
   <li>Si la opción <b>Puede editar la hora</b> está deshabilitada, los aprobadores no podrán enviar, volver a abrir ni cerrar la hoja de horas y no podrán editar la hora. Los aprobadores solo pueden aprobar o rechazar la hoja de horas. </li>
   <li>Los administradores de los propietarios de las hojas de horas pueden enviar, recuperar, volver a abrir y editar las hojas de horas de sus subordinados directos.</li></ul>
   </ul>

   <p><b>NOTA</b>

   Una vez enviada una hoja de horas para su aprobación, ya no puede editar las horas. Para devolver una hoja de horas enviada a un estado editable, recupere la hoja de horas o pida al aprobador que la rechace. Para obtener más información, consulte <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Enviar una hoja de horas para su aprobación</a> y <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Aprobar una hoja de horas</a>.</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">Horas extra</span> </td> 
      <td>Puede elegir ocultar el cuadro Horas extra en la hoja de horas. Esta opción está desactivada de forma predeterminada.</td> 
      </tr> 
      </tbody> 
   </table>

1. Haga clic en **Crear hoja de horas**.

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## Cuando las tareas y los problemas aparecen en las plantillas de horas de los usuarios

Una tarea o un problema asignado a un usuario aparece automáticamente en la plantilla de horas de un usuario si la tarea o el problema cumple cualquiera de los siguientes criterios:

* El usuario ha registrado horas en la tarea o el problema
* Las fechas planificadas para la tarea o el problema se encuentran dentro de las fechas de la hoja de horas
* La tarea o el problema tienen una fecha de inicio real (el estado de la tarea o el problema es En curso)
* La tarea o el problema están anclados a la plantilla de horas
* La fecha planificada de finalización se encuentra dentro del intervalo de fechas de la hoja de horas y el estado es En curso

Si las **hojas de horas rellenadas previamente con preferencias de ...** (ubicadas en las preferencias de Hojas de horas y Horas) no están seleccionadas, la hoja de horas mostrará los problemas y las tareas que tengan el estado En curso. Para obtener más información acerca de Plantillas de horas y Preferencias de horas, consulte [Configurar preferencias de horas y hojas de horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
