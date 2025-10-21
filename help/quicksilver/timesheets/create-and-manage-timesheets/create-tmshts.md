---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Crear hoja de horas de un solo uso
description: Puede crear manualmente una plantilla de horas de un solo uso si desea una plantilla de horas que no sea recurrente. Cuando llegue la fecha de finalización de la plantilla de horas y necesite más plantillas, debe crear otras nuevas.
author: Lisa
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1062'
ht-degree: 90%

---

# Crear una plantilla de horas de un solo uso

<!--Audited: 6/2025-->

Puede crear manualmente una plantilla de horas de un solo uso si desea una plantilla de horas que no sea recurrente. Cuando llegue la fecha de finalización de la plantilla de horas y necesite más plantillas, debe crear otras nuevas.

Para obtener información sobre cómo crear un perfil de plantilla de horas que genere plantillas de horas recurrentes para los usuarios sin ninguna otra intervención por su parte (recomendado), consulte [Crear, editar y asignar perfiles de plantillas de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Para obtener información sobre la generación manual de hojas de horas para todos los usuarios del sistema asociados con un perfil de hoja de horas, consulte [Generar manualmente hojas de horas](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

>[!NOTE]
>
>* No se pueden crear plantillas de horas de un solo uso para grupos.
>* Al crear una plantilla de horas de un solo uso, no puede seleccionar tipos de horas generales específicos para incluirlos en la plantilla de horas. Todos los tipos de hora generales que están activados en el sistema se muestran en plantillas de horas creadas manualmente.
>
>Si desea seleccionar solo ciertos tipos generales de horas para mostrarlos en sus plantillas de horas, utilice un perfil de plantilla de horas. Para obtener más información sobre los perfiles de plantillas de horas, consulte [Crear, editar y asignar perfiles de plantillas de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

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
   <td>
   <p>Estándar</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td><p>Acceso administrativo a hojas de horas</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear una plantilla de horas de un solo uso

{{step1-to-timesheets}}

El filtro **Todos** está seleccionado de manera predeterminada. Esto muestra todas las plantillas de horas que tiene acceso de visualización.

![Lista de hojas de horas con una hoja de horas seleccionada](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Opcional) Realice una de las siguientes acciones para actualizar el filtro en la lista de plantillas de horas:

   * Seleccione **Aprobaciones de Mis plantillas de horas** en la esquina superior derecha de la página para ver solamente las plantillas de horas que usted apruebe

     O

     Seleccione **Mis plantillas de horas** para ver solamente sus plantillas de horas.

     Esto es válido para los filtros Aprobaciones de Mis hojas de horas o de Mis hojas de horas a la lista de hojas de horas.

     ![Botones de filtro en Mis hojas de horas en la página Lista de hojas de horas](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-nwepng.png) para aplicar un filtro diferente o crear uno nuevo. Para obtener información sobre cómo crear o actualizar filtros, consulte [Crear o editar filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Las opciones Aprobaciones de Mis hojas de horas y Mis hojas de horas no se muestran en la parte superior de la lista de hojas de horas ni en la lista de filtros si su administrador de Workfront o su administrador de grupos ha eliminado los filtros Aprobaciones de Mis hojas de horas y Mis hojas de horas de Controles de Lista en el área Configuración o de la Plantilla de diseño. Para obtener más información, consulte los siguientes artículos:
   > 
   >   * [Personalizar filtros, vistas y agrupaciones mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Opcional) Haga clic en el icono **Buscar** ![Icono de búsqueda](assets/search-icon.png) para escribir una palabra clave y buscar una hoja de horas específica. Por ejemplo, puede buscar un lapso de tiempo de la plantilla de horas con el nombre del propietario.

1. (Opcional) Haga clic en los iconos **Ver** ![Ver icono](assets/view-icon.png) o **Agrupar** ![Icono de agrupación](assets/grouping.png) para aplicar una vista o agrupación diferente o para crear una nueva.

   Para obtener información sobre la creación de filtros, vistas o agrupaciones, consulte los siguientes artículos:

   * [Crear o editar filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Crear o editar vistas en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Creación de agrupaciones en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Haga clic en **Nueva plantilla de horas** al principio de la lista de hojas de horas.

   Especifique la siguiente información:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>Crear plantilla de horas para</strong> </td> 
      <td>Comience a introducir el nombre del usuario, una función o un equipo para el que esté creando la plantilla de horas y haga clic en ellos cuando se muestren en la lista.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Fecha de inicio</strong> </td> 
      <td>Esta la fecha de inicio de la plantilla de horas.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Fecha de finalización</strong> </td> 
      <td> Esta es la fecha de finalización de la plantilla de horas.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Aprobadores</strong> </td> 
      <td>Los aprobadores aprueban la plantilla de horas de los usuarios asociados con ella. Solo los usuarios con derechos administrativos de plantilla de horas pueden establecerse como aprobadores. Para obtener más información sobre los derechos administrativos sobre las plantillas de horas, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.<br>Empiece a introducir los nombres de los aprobadores de plantillas de horas y haga clic en ellos cuando aparezcan en la lista.<br>Puede tener varios aprobadores en una plantilla de horas. En este caso, una vez que uno de los aprobadores apruebe la plantilla de horas, esta se marcará como <strong>Cerrada</strong> y desaparecerá de la lista de aprobaciones de plantillas de horas de todos los aprobadores restantes.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Puede editar el tiempo</strong> </td>

   <td> <p>Seleccione esta opción si desea permitir que los aprobadores editen las horas en la plantilla de horas.</p>

   Esta opción funciona junto con **Restringir la edición de plantillas de horas a propietarios y administradores** del área Configuración > Plantilla de horas y horas > Preferencias. Para obtener más información, consulte <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configurar preferencias de plantillas de horas y de horas</a>.

   Se dan los siguientes escenarios:

   <ul>
      <li>Cuando la opción <b>Restringir la edición de plantillas de horas a propietarios y administradores</b> está habilitada:</li>
   <ul><li>Los aprobadores solo pueden aprobar y rechazar plantillas de horas, independientemente de si <b>Puede editar el tiempo</b> está habilitado o no. </li>
   <li>Los administradores de propietarios de plantillas de horas solo pueden ver las plantillas de horas de sus informes directos.</li></ul>
   <li>Cuando la opción <b>Restringir la edición de plantillas de horas a propietarios y administradores</b> está deshabilitada:</li>
   <ul><li>Cuando la opción <b>Puede editar el tiempo</b> está habilitada, los aprobadores pueden enviar, reabrir o cerrar la plantilla de horas, así como editar el tiempo.</li>
   <li>Cuando la opción <b>Puede editar el tiempo</b> está deshabilitada, los aprobadores no pueden enviar, reabrir o cerrar la plantilla de horas, ni editar la hora. Los aprobadores solo pueden aprobar o rechazar la plantilla de horas. </li>
   <li>Los administradores de los propietarios de las plantillas de horas pueden enviar, recuperar, volver a abrir y editar las plantillas de horas de sus informes directos.</li></ul>
   </ul>

   <p><b>NOTA</b>

   Una vez enviada una plantilla de horas para su aprobación, ya no se pueden editar las horas. Para devolver una plantilla de horas enviada a un estado editable, recupere la plantilla de horas o solicite al aprobador que la rechace. Para obtener más información, consulte <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Enviar una plantilla de horas para su aprobación</a> y <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Aprobar una plantilla de horas</a>.</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">Tiempo adicional</span> </td> 
      <td>Puede elegir ocultar el cuadro Horas extra en la plantilla de horas. Esta opción está desactivada de forma predeterminada.</td> 
      </tr> 
      </tbody> 
   </table>

1. Haga clic en **Crear plantilla de horas**.

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## Cuando las tareas y problemas aparecen en las plantillas de horas de los usuarios

Una tarea o problema asignado a un usuario aparece automáticamente en la plantilla de horas de un usuario si la tarea o problema cumple cualquiera de los siguientes criterios:

* El usuario ha registrado horas en la tarea o problema
* Las fechas planificadas para la tarea o problema se encuentran dentro de las fechas de la plantilla de horas
* La tarea o problema tiene una fecha de inicio real (el estado de la tarea o problema es En curso)
* La tarea o el problema están anclados a la plantilla de horas
* La fecha planificada de finalización se encuentra dentro del intervalo de fecha de la plantilla de horas y el estado es En curso

Si las preferencias **Rellenar previamente las plantillas de horas con…** (ubicadas en las preferencias de Plantillas de horas y Horas) no están seleccionadas, la plantilla de horas mostrará los problemas y tareas que tengan el estado En curso. Para obtener más información acerca de las preferencias de plantillas de horas y de horas, consulte [Configurar preferencias de plantillas de horas y de horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
