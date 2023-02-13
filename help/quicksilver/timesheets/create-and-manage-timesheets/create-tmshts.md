---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Crear un parte de horas de un solo uso
description: Puede crear manualmente un parte de horas de un solo uso si desea un parte de horas que no sea recurrente. Cuando se llega a la fecha de finalización del parte de horas y se necesitan más partes de horas, se deben crear otras nuevas.
author: Alina
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 1%

---

# Crear un parte de horas de un solo uso

Puede crear manualmente un parte de horas de un solo uso si desea un parte de horas que no sea recurrente. Cuando se llega a la fecha de finalización del parte de horas y se necesitan más partes de horas, se deben crear otras nuevas.

Para obtener información sobre la creación de un perfil de parte de horas que genere partes de horas recurrentes para los usuarios sin ninguna otra intervención por su parte (recomendado), consulte [Crear, editar y asignar perfiles de parte de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

>[!NOTE]
>
>* Las hojas de horas de un solo uso no se pueden crear para grupos.

>  <!--
>  <span>Making sure with Lilit that this is correct</span>>
>  -->
>* Al crear un parte de horas de un solo uso, no se pueden seleccionar tipos de horas generales específicos para incluirlos en el parte de horas. Todos los tipos de horas generales que se activan en el sistema se muestran en partes de horas creadas manualmente.
>
>  Si desea seleccionar solo determinados tipos de hora generales para mostrarlos en las hojas de horas, utilice un perfil de parte de horas. Para obtener más información sobre los perfiles de hojas de horas, consulte [Crear, editar y asignar perfiles de parte de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Requisitos de acceso

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
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe tener acceso administrativo a las hojas de horas. </p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> <p><b> NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Crear un parte de horas de un solo uso

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Hojas de tiempo**. La variable **Todo** está seleccionado de forma predeterminada. Esto muestra todas las partes de horas a las que tiene acceso para ver.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Opcional) Realice una de las siguientes acciones para actualizar el filtro en la lista de partes de horas:

   * Select **Aprobaciones de Mi parte de horas** en la esquina superior derecha de la página para ver solo las partes de horas que aprueba

      O

      Select **Mis hojas de hora** para ver solo sus partes de horas.

      Esto aplica los filtros Mis aprobaciones de parte de horas o Mi parte de horas a la lista de partes de horas.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Haga clic en el icono Filtro ![](assets/filter-nwepng.png) para aplicar un filtro diferente o crear uno nuevo. Para obtener información sobre cómo crear o actualizar filtros, consulte [Crear o editar filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >Las opciones Mis aprobaciones de parte de horas y Mis hojas de horas no se muestran en la parte superior de la lista de hojas de horas ni en la lista de filtros si el administrador de Workfront o un administrador de grupo han eliminado los filtros Mis aprobaciones de parte de horas y Mis hojas de horas de los controles de lista del área Configuración o de la plantilla Diseño. Para obtener más información, consulte los siguientes artículos:
   > 
   >   * [Personalización de filtros, vistas y grupos mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)



1. (Opcional) Haga clic en el **Buscar** icono ![](assets/search-icon.png) para escribir una palabra clave y buscar un parte de horas específico. Por ejemplo, puede buscar un lapso de tiempo de parte de horas con el nombre del propietario.

1. (Opcional) Haga clic en el **Ver** ![](assets/view-icon.png) o **Agrupación** ![](assets/grouping.png) para aplicar una vista o agrupación diferente o para crear una nueva.

   Para obtener información sobre la creación de filtros, vistas o agrupaciones, consulte los siguientes artículos:

   * [Crear o editar filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Crear o editar vistas en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Crear agrupaciones en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Haga clic en **Nueva hoja de horas** en la parte superior de la lista de partes de horas.

   Especifique la siguiente información:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>Crear hoja de horas para</strong> </td> 
      <td>Comience a introducir el nombre del usuario, una función de trabajo o un equipo para el que esté creando el parte de horas y haga clic en ellos cuando se muestren en la lista.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Fecha de inicio</strong> </td> 
      <td>Esta es la fecha de inicio del parte de horas.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Fecha de finalización</strong> </td> 
      <td> Esta es la fecha de finalización del parte de horas.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Aprobadores</strong> </td> 
      <td>Los aprobadores son usuarios que aprueban el parte de horas para los usuarios asociados al parte de horas. Solo los usuarios con derechos administrativos de parte de horas pueden configurarse como aprobadores. Para obtener más información sobre los derechos administrativos del parte de horas, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.<br>Comience a introducir los nombres de los aprobadores de hojas de horas y haga clic en ellos cuando aparezcan en la lista.<br>Puede tener varios aprobadores en un parte de horas. En este caso, después de que uno de los aprobadores apruebe el parte de horas, el parte de horas se marca como <strong>Cerrado</strong> y desaparece de la lista de aprobaciones de parte de horas de todos los aprobadores restantes.</td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Puede editar el tiempo</strong> </td>

   <td> <p>Seleccione esta opción si desea permitir que los aprobadores editen las horas en el parte de horas.</p>

   Esta opción funciona junto con la variable **Restringir la edición de hojas de horas a propietarios y administradores** en el área Configuración > Horario y horas > Preferencias . Para obtener más información, consulte <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configuración de las preferencias de horas y horas</a>.

   Existen los siguientes escenarios:

   <ul>
      <li>Cuando la variable <b>Restringir la edición de hojas de horas a propietarios y administradores</b> está activada:</li>
   <ul><li>Los aprobadores solo pueden aprobar y rechazar el parte de horas, independientemente de si la variable <b>Puede editar el tiempo</b> está activada o no. </li>
   <li>Los administradores de los propietarios de hojas de horas solo pueden ver las hojas de horas de sus informes directos.</li></ul>
   <li>Cuando la variable <b>Restringir la edición de hojas de horas a propietarios y administradores</b> está desactivada:</li>
   <ul><li>Cuando la variable <b>Puede editar el tiempo</b> está activada, los aprobadores pueden enviar, volver a abrir o cerrar el parte de horas y editar la hora.</li>
   <li>Cuando la variable <b>Puede editar el tiempo</b> está desactivado, los aprobadores no pueden enviar, volver a abrir ni cerrar el parte de horas y no pueden editar la hora. Los aprobadores solo pueden aprobar o rechazar el parte de horas. </li>
   <li>Los administradores de los propietarios de hojas de horas pueden enviar, recuperar, volver a abrir y editar las hojas de horas de sus informes directos.</li></ul>
   </ul>

   <p><b>NOTA</b>

   Una vez que envíe un parte de horas para su aprobación, ya no podrá editar las horas. Para devolver un parte de horas enviado a un estado editable, recuerde el parte de horas o haga que el aprobador rechace el parte de horas. Para obtener más información, consulte <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Enviar un parte de horas para su aprobación</a> y <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Aprobar un parte de horas</a>.</p> </p>

   </td> 
      </tr>

   <tr>

   <td role="rowheader"><span style="font-weight: bold;">Horas extra</span> </td> 
      <td>Puede elegir ocultar el cuadro Tiempo extra del parte de horas. Esta opción está desactivada de forma predeterminada.</td> 
      </tr> 
      </tbody> 
   </table>

1. Haga clic en **Crear hoja de horas**.

<!--the content in the table above will need to match the content in the Create timesheet profiles article-->

## Cuando las tareas y los problemas aparecen en las hojas de horas de los usuarios

Una tarea o problema asignado a un usuario aparece automáticamente en el parte de horas de un usuario si la tarea o el problema cumple cualquiera de los siguientes criterios:

* El usuario ha registrado horas en la tarea o el problema
* Las fechas planificadas de la tarea o el problema se encuentran dentro de las fechas del parte de horas
* La tarea o el problema tienen una fecha de inicio real (la tarea o el estado del problema están en curso)
* La tarea o el problema está anclado en el parte de horas
* La fecha de finalización planeada se encuentra dentro del intervalo de fechas del parte de horas y el estado está en curso

Si la variable **Rellenar previamente hojas de hora con ...** Las preferencias (que se encuentran en las preferencias Hojas de hora y Hora) no están seleccionadas, el parte de horas muestra los problemas y tareas que tienen el estado En curso. Para obtener más información sobre las preferencias de horas y hojas de horas, consulte [Configuración de las preferencias de horas y horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
