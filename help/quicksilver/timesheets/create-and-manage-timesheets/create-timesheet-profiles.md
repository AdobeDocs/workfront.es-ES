---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Crear, editar y asignar perfiles de plantillas de horas
description: Puede crear, editar y asignar perfiles de hojas de horas que generen hojas de horas recurrentes para sus usuarios sin ninguna intervención por su parte. Esto le ahorra tiempo y garantiza la coherencia entre los usuarios.
author: Lisa
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 611c3c947855610cf86cdcbf96d1e9d847e34f38
workflow-type: tm+mt
source-wordcount: '1668'
ht-degree: 66%

---

# Crear, editar y asignar perfiles de plantillas de horas

<!--Audited: 06/2025-->

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa de espacio aislado y se va a lanzar en un despliegue gradual en Producción.</span>

Puede crear, editar y asignar perfiles de hojas de horas que generen hojas de horas recurrentes para sus usuarios sin ninguna intervención por su parte. Esto le permite ahorrar tiempo y garantiza la coherencia de los siguientes elementos entre los usuarios:

* Lapso de tiempo de la plantilla de horas
* Aprobadores
* Tipos de hora generales

Para obtener más información sobre cómo crear manualmente una hoja de horas, consulte [Crear una hoja de horas de un solo uso](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
   <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nuevo: estándar </p>
 <p>o</p> 
<p>Actual: plan </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe tener acceso administrativo a las plantillas de horas. </p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear o editar un perfil de plantilla de horas

<!--Old info: 
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>Para habilitar los cambios de perfil de hoja de horas en las hojas de horas actuales, tiene que eliminar las hojas de horas existentes antes de realizar los cambios en los perfiles de hoja de horas y luego generar nuevas hojas de horas. Para obtener instrucciones, consulte [Eliminar hojas de horas en Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) y [Generar manualmente hojas de horas](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

{{step-1-to-setup}}

1. Si crea o edita un perfil de hoja de horas para utilizarlo en todo el sistema, haga clic en **Hoja de horas y horas**.

   O

   Si crea o edita un perfil de hoja de horas para un grupo, haga clic en **Grupos** y luego haga clic en el nombre del grupo.

1. Haga clic en **Perfiles de plantilla de horas**.
1. Para crear un perfil de hoja de horas, haz clic en **Nuevo perfil**.

   O

   Para editar un perfil de plantilla de horas existente, seleccione el perfil de plantilla de horas que desee editar y luego haga clic en **Editar**.

   Se muestra la página de perfil de hoja de horas nueva o existente.

1. Actualice la siguiente información:

   * **Nombre**: agregue un nombre para el perfil de hoja de horas. Podría ser el nombre de un equipo o un grupo cuyas personas compartan el mismo periodo de tiempo para sus plantillas de horas. Este campo es obligatorio.
   * **Descripción**: agrega más información sobre el perfil de hoja de horas.
   * **Grupo con acceso de administración**: Si está creando un perfil de hoja de horas de nivel de sistema, deje este campo en blanco.

     Cualquier usuario que pueda editar cuentas de usuario puede adjuntar una plantilla de horas a nivel de sistema a otros usuarios.

     Solamente un administrador de Workfront puede editar un perfil de plantilla de horas a nivel de sistema.

     Si está creando un perfil de plantilla de horas para un grupo que administra, identifique el grupo aquí.

     Esto no asigna el perfil de plantilla de horas a los usuarios del grupo; solo permite a los administradores del grupo modificar el perfil de plantilla de horas. Asignará el perfil a los usuarios en el paso 6.

     >[!NOTE]
     >
     >Cuando los usuarios fuera del grupo adjunten perfiles de plantilla de horas a otros usuarios, no podrán ver ni adjuntar este perfil de plantilla de horas.

   * **Crear hojas de horas**: especifique cuándo el perfil de la hoja de horas debe generar las hojas de horas. Se puede configurar una hoja de horas para que se genere automáticamente de forma semanal, quincenal, semestral o mensual. Seleccione el día de la semana en el que desea que se genere la plantilla de horas.

     Una plantilla de horas semanal comienza en la fecha en que se genera. Por ejemplo, si crea plantillas de horas semanales todos los jueves, el primer día de la semana en la plantilla de horas es el jueves.

     >[!NOTE]
     >
     >Workfront siempre crea dos plantillas de horas a la vez: la primera incluye siempre la fecha actual y la segunda comienza cuando termina el lapso de tiempo de la primera.

   * **Aprobadores**: Los aprobadores son usuarios que aprueban la hoja de horas para los usuarios asociados con la hoja de horas. Puede identificar hasta siete usuarios como aprobadores en una plantilla de horas. La identificación de varios usuarios resulta útil para garantizar que un aprobador esté disponible cuando alguien esté fuera de la oficina. Se notifica a todos los aprobadores cuando un usuario envía la plantilla de horas para su aprobación. Solo se requiere un usuario para aprobar la plantilla de horas.

     Solo los usuarios con derechos administrativos de plantilla de horas pueden establecerse como aprobadores. Para obtener más información sobre los derechos administrativos sobre las plantillas de horas, consulte [Conceder a los usuarios acceso administrativo a determinadas áreas](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

     Utilice el menú desplegable para seleccionar el aprobador de la plantilla de horas (si se requiere un aprobador). Puede seleccionar entre las siguientes opciones:

      * **Ninguno**: no es necesario aprobar la hoja de horas.
      * **Su administrador**: este es el aprobador predeterminado, establecido por el sistema. En este caso, el usuario designado como su responsable aprueba la plantilla de horas cuando se envía para su aprobación.
      * **Personas específicas**: puede designar a usuarios específicos, por su nombre, como aprobadores de hojas de horas. Puede tener varios aprobadores en una plantilla de horas. En este caso, una vez que uno de los aprobadores apruebe la plantilla de horas, esta se marcará como **Cerrada** y desaparecerá de la lista de aprobaciones de plantillas de horas de todos los aprobadores restantes.

   * **Puede editar el tiempo**: seleccione esta opción para permitir que los aprobadores editen las horas en la hoja de horas.

     Esta opción funciona junto con **Restringir la edición de plantillas de horas a propietarios y administradores** del área Configuración > Plantilla de horas y horas > Preferencias. Para obtener más información, consulte [Configurar preferencias de plantillas de horas y de horas](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

     Se dan los siguientes escenarios:

     Cuando la opción **Restringir la edición de plantillas de horas a propietarios y administradores** está habilitada:

      * Los aprobadores solo pueden aprobar y rechazar plantillas de horas, independientemente de si la opción Puede editar las horas está activada o no.
      * Los administradores de propietarios de plantillas de horas solo pueden ver las plantillas de horas de sus informes directos.

     Cuando la opción **Restringir la edición de plantillas de horas a propietarios y administradores** está deshabilitada:

      * Cuando **Puede editar la hora** está habilitada, los aprobadores pueden enviar, reabrir o cerrar la hoja de horas y pueden editar la hora.
      * Si **Puede editar la hora** está deshabilitada, los aprobadores no podrán enviar, volver a abrir ni cerrar la hoja de horas y no podrán editar la hora. Los aprobadores solo pueden aprobar o rechazar la plantilla de horas.
      * Los administradores de los propietarios de las plantillas de horas pueden enviar, recuperar, volver a abrir y editar las plantillas de horas de sus informes directos.

     >[!NOTE]
     >
     >Una vez enviada una plantilla de horas para su aprobación, ya no se pueden editar las horas. Para devolver una plantilla de horas enviada a un estado editable, recupere la plantilla de horas o solicite al aprobador que la rechace. Para obtener más información, consulte [Enviar una plantilla de horas para su aprobación](/help/quicksilver/timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md) y [Aprobar una plantilla de horas](/help/quicksilver/timesheets/create-and-manage-timesheets/timesheet-approvals.md).

   * **Horas extra**: puede elegir ocultar el cuadro Horas extra en las hojas de horas. Esta opción está desactivada de forma predeterminada.
   * **Tipos de horas disponibles**: esta configuración solo hace referencia a tipos de horas generales y no a tipos de horas específicos de proyectos.

     De forma predeterminada, los usuarios ven todas las horas generales en una hoja de horas. Sin embargo, si su organización desea que solo se muestren horas generales específicas para un conjunto determinado de usuarios, puede seleccionar las horas generales que necesitan ver en sus plantillas de horas seleccionándolas en el perfil de plantilla de horas en este campo. Si desea deshabilitar todas las horas generales, anule la selección de todos los tipos de horas para generar la plantilla de horas sin una sección para las horas generales.

   * **Notificaciones de recordatorio**: agregue una notificación de recordatorio. Workfront enviará recordatorios a los usuarios para pedirles que completen o aprueben sus plantillas de horas. Debe crear notificaciones de recordatorio antes de poder asociarlas a un perfil de hoja de horas.

1. Al crear perfiles de hojas de horas de nivel de grupo en Producción, haga clic en la ficha **Asignar personas** para asociar el perfil de hojas de horas con usuarios, grupos o equipos específicos (si es administrador de Workfront). <!--To associate the timesheet profile with specific users, groups, or (if you are a Workfront administrator) teams, scroll towards the bottom of the page and find the **Assign People** section.-->

   <span class="preview">Al crear perfiles de hojas de horas de nivel de grupo en Vista previa, desplácese hacia la parte inferior de la página y busque la sección **Asignar personas**.</span>

   Al crear perfiles de hojas de horas para el sistema, desplácese hacia la parte inferior de la página y busque la sección **Asignar personas**.

   Empiece a escribir el nombre del usuario, grupo o equipo y, a continuación, haga clic en él cuando aparezca en la lista desplegable.

   Si es administrador de un grupo, puede asignar el perfil de la plantilla de horas a los grupos que administre, pero no a los equipos. Para obtener más información, consulte [Limitaciones para un administrador de grupo que asigna un perfil de plantilla de horas](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) en este artículo.

   >[!NOTE]
   >
   >* También puede asociar un usuario con un perfil de plantilla de horas editando el perfil del usuario. Para obtener más información, consulte [Editar el perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* Cuando se añade un grupo, solo aparece el nombre del grupo en la pestaña Asignar personas, no la lista de integrantes del grupo. Si desea ver los integrantes del grupo enumerados aquí, haga clic en Guardar cambios y, a continuación, haga clic en el nombre del perfil de plantilla de horas que acaba de crear.
   >* Cuando termina estos pasos, el perfil de plantilla de horas genera plantillas de horas únicamente para los usuarios o integrantes del grupo asignados que no tienen plantillas de horas existentes para el período actual.

1. Haga clic en **Guardar**.

1. En la parte superior de la lista de perfiles de hojas de horas, haga clic en el icono **Más** ![Icono de Más](assets/more-icon.png) y luego haga clic en **Generar hojas de horas**.

   En la parte inferior de la pantalla aparece una confirmación de que las plantillas de horas se han generado correctamente. Se generan nuevas plantillas de horas en función de los nuevos perfiles que haya creado.

   Para obtener más información, consulte [Generar hojas de horas manualmente](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

   La primera vez que el perfil de plantilla de horas genera plantillas de horas, se crean dos plantillas de horas para cada usuario, tanto para el periodo de tiempo que incluye la hora actual como para el siguiente periodo de tiempo.

   Después, cada vez que genera nuevas plantillas de horas, se crea una por usuario.

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## Limitaciones para un administrador de grupo que asigna un perfil de plantilla de horas {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

Si es administrador de grupos y la opción de acceso administrativo Plantillas de horas y horas está desactivada en su nivel de acceso, puede crear perfiles de plantillas de horas, pero, asignarlos, únicamente a:

* Grupos que administra
* Usuarios individuales a los que tiene acceso para editar y que están en un grupo que administra

Para estos grupos y usuarios, no tendrá acceso a las hojas de horas que genera el perfil de plantilla de horas.

Además, si la opción Administración de usuarios (usuarios de grupo) también está desactivada en su nivel de acceso, puede asignar el perfil de plantilla de horas a un grupo que administre, pero esto solo afectará a los usuarios del grupo al que tenga acceso para editar. Si el grupo contiene usuarios a los que no tiene acceso para editar, no se les asignará el perfil de plantilla de horas junto con el resto del grupo.

Para obtener información acerca de la opción Hojas de horas y horas en su nivel de acceso, consulte [Conceder a los usuarios acceso administrativo a ciertas áreas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Para obtener información acerca de la opción Administración de usuarios (usuarios de grupo) en su nivel de acceso, consulte [Conceder acceso a usuarios](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Varios perfiles de plantillas de horas recurrentes

Puede tener más de un perfil de plantilla de horas para su organización si tiene lo siguiente:

* Períodos de pago únicos para diferentes conjuntos de usuarios
* Aprobadores únicos para diferentes conjuntos de usuarios
* Requisitos horarios generales únicos para distintos grupos de usuarios

No se puede asociar a un usuario con más de un perfil de plantilla de horas a la vez.

<!--
<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td> <p> Add a name for the timesheet profile. It could be the name of a team or a group whose people share the same timeframe for their timesheets. </p> <p>This ia a required field.</p> </td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td> <p> Add more information about the timesheet profile.     
      </p> </td> 
     </tr>

   <tr> 
   <td role="rowheader"><strong>Group with Administration Access</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>If you are creating a system-level timesheet profile, leave this field blank.</p> <p>Any user who can edit user accounts can attach a system-level timesheet to other users.</p> <p>Only a Workfront administrator can edit a system-level timesheet profile.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>If you are creating a timesheet profile for a group you administer, identify the group here.</p> <p>This does not assign the timesheet profile to the users in the group; it only allows the group's administrators to modify the timesheet profile. You will assign the profile to users in Step 6.</p>

   <p><b>NOTE</b>: When users outside the group are attaching timesheet profiles to other users, they won't be able to see or attach this timesheet profile.</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Create timesheets</strong> </td> 
      <td> <p> <p>Specify when the timesheet profile should generate the timesheets. A timesheet can be set to automatically generate on a weekly, bi-weekly, semi-monthly, or monthly basis. Select the day of the week when you want the timesheet to be produced.</p>
      <p>A weekly timesheet begins on the date it is generated. For example, if you create weekly timesheets every Thursday, the first day of the week on the timesheet is Thursday.</p>
    
      
   <p><b>NOTE</b>: Workfront always creates two timesheets at a time: the first timesheet always includes the current date, and the second timesheet starts when the time frame of the first one ends.</p> </p> </td> 
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Approvers</strong></p> </td> 
      <td> <p> <p>Approvers are users who approve the timesheet for the users associated with the timesheet. You can identify up to 7 users as approvers on a timesheet. Identifying multiple users is useful to ensure an approver is available when someone is out of the office. All approvers are notified when a user submits the timesheet for approval. Only one user is required to approve the timesheet in order for it to be approved.</p> <p>Only users with timesheet administrative rights can be set as approvers. For more information about timesheet administrative rights, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p>Use the drop-down menu&nbsp;to select&nbsp;the approver&nbsp;for the timesheet (if an approver is required). You can select from the following options:</p> 
      <ul> 
      <li><strong>None</strong>: The timesheet does not need to&nbsp;be approved.</li> 
      <li><strong>Their Manager</strong>: This is the default approver, set by the system. In this case, the user designated as their manager approves the timesheet when it is submitted for approval.</li> 
      <li><strong>Specific People:</strong>&nbsp;You can designate specific users, by name, as timesheet approvers. You can have multiple approvers on a timesheet. In this case, after&nbsp;one of the approvers approves the timesheet, the timesheet is marked as <strong>Closed</strong> and it disappears from the timesheet approvals list of all the remaining approvers.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Can edit time </strong> </td> 
      <td> <p> <p>Select this option to allow the approvers to edit hours on the timesheet. 

   <p>This option works together with the **Restrict timesheet editing to owners and admins** setting in the Setup > Timesheet & Hours > Preferences area. For more information, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configure timesheet and hour preferences</a>.</p>

   <p>The following scenarios exist: </p>

   <ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is enabled:</li>
      <ul><li>Approvers can only approve and reject timesheet, regardless of whether the <b>Can edit time</b> is enabled or not. </li>
      <li>Timesheet owners' managers can only view their direct reports' timesheets.</li></ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is disabled:</li>
    <ul><li>When the <b>Can edit time</b> is enabled, approvers can submit, reopen, or close the timesheet and can edit the time.</li>
      <li>When the <b>Can edit time</b> is disabled, approvers cannot submit, reopen, or close the timesheet and cannot edit the time. Approvers can only approve or reject the timesheet. </li>
      <li>Timesheet owners' managers can submit, recall, reopen, and edit their direct reports' timesheets.</li></ul>
      </ul>

   <p>

   <b>NOTE</b>: Once you submit a timesheet for approval, you can no longer edit the hours. To return a submitted timesheet to an editable state, recall the timesheet or have the approver reject the timesheet. For more information, see <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Submit a timesheet for approval</a> and <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Approve a timesheet</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Overtime</strong> </td> 
      <td>You can choose to hide the Overtime box in timesheets. This option is disabled by default.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Available Hour Types</strong> </td> 
      <td><p>This setting refers only to General Hour Types, and not to project-specific hour types. </p>
      <p>By default, users see all general hours on a timesheet. However, if your organization wants only specific general hours to be shown for a particular set of users, you can select the general hours that they need to see in their timesheets by selecting them in their timesheet profile in this field. If you want to disable all general hours, deselect all hour types to generate the timesheet without a section for general hours.</p></td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Reminder notifications</strong> </td> 
      <td> <p> Add a reminder notification. Workfront will send reminders to users to ask them to complete or approve their timesheets. You must create reminder notifications before you can associate them with a timesheet profile.  </p> </td> 
     </tr>
    </tbody> 
   </table>
-->