---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Crear, editar y asignar perfiles de plantillas de horas
description: Puede crear, editar y asignar perfiles de hojas de horas que generen hojas de horas recurrentes para sus usuarios sin ninguna intervención por su parte. Esto le ahorra tiempo y garantiza la coherencia entre los usuarios.
author: Lisa
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 764200970aeb8d121cd99a8d4239e0b9853670a9
workflow-type: tm+mt
source-wordcount: '1635'
ht-degree: 79%

---

# Crear, editar y asignar perfiles de plantillas de horas

<!--Audited: 06/2025-->

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


1. Haga clic en la ficha **Establecer detalles** y, a continuación, actualice la siguiente información: <!-- at the Production release, change the order of some of these rows, as they changed in the unshimmed UI-->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Nombre</strong> </td> 
      <td> <p> Añada un nombre para el perfil de la plantilla de horas. Podría ser el nombre de un equipo o un grupo cuyas personas compartan el mismo periodo de tiempo para sus plantillas de horas. </p> <p>Es un campo obligatorio.</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Descripción</strong> </td> 
      <td> <p> Añada más información sobre el perfil de la plantilla de horas.     
      </p> </td> 
     </tr>

   <tr> 
   <td role="rowheader"><strong>Grupo con acceso de administración</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>Si está creando un perfil de plantilla de horas a nivel de sistema, deje este campo en blanco.</p> <p>Cualquier usuario que pueda editar cuentas de usuario puede adjuntar una plantilla de horas a nivel de sistema a otros usuarios.</p> <p>Solamente un administrador de Workfront puede editar un perfil de plantilla de horas a nivel de sistema.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>Si está creando un perfil de plantilla de horas para un grupo que administra, identifique el grupo aquí.</p> <p>Esto no asigna el perfil de plantilla de horas a los usuarios del grupo; solo permite a los administradores del grupo modificar el perfil de plantilla de horas. Asignará el perfil a los usuarios en el paso 6.</p>

   <p><b>NOTA</b>: cuando los usuarios fuera del grupo están adjuntando perfiles de plantilla de horas a otros usuarios, no podrán ver ni adjuntar este perfil de plantilla de horas.</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Crear hojas de horas</strong> </td> 
      <td> <p> <p>Especifique cuándo el perfil de la plantilla de horas debe generar las hojas de horas. Se puede configurar una hoja de horas para que se genere automáticamente de forma semanal, quincenal, semestral o mensual. Seleccione el día de la semana en el que desea que se genere la plantilla de horas.</p>
      <p>Una plantilla de horas semanal comienza en la fecha en que se genera. Por ejemplo, si crea plantillas de horas semanales todos los jueves, el primer día de la semana en la plantilla de horas es el jueves.</p>


   <p><b>NOTA</b>: Workfront siempre crea dos hojas de horas a la vez: la primera hoja de horas siempre incluye la fecha actual y la segunda hoja de horas comienza cuando finaliza el lapso de tiempo de la primera.</p> </p> </td> 
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Aprobadores</strong></p> </td> 
      <td> <p> <p>Los aprobadores aprueban la plantilla de horas de los usuarios asociados con ella. Puede identificar hasta siete usuarios como aprobadores en una plantilla de horas. La identificación de varios usuarios resulta útil para garantizar que un aprobador esté disponible cuando alguien esté fuera de la oficina. Se notifica a todos los aprobadores cuando un usuario envía la plantilla de horas para su aprobación. Solo se requiere un usuario para aprobar la plantilla de horas.</p> <p>Solo los usuarios con derechos administrativos de plantilla de horas pueden establecerse como aprobadores. Para obtener más información sobre los derechos administrativos de la plantilla de horas, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> <p>Utilice el menú desplegable para seleccionar el aprobador de la plantilla de horas (si se requiere un aprobador). Puede seleccionar entre las siguientes opciones:</p> 
      <ul> 
      <li><strong>Ninguno</strong>: no es necesario aprobar la plantilla de horas.</li> 
      <li><strong>Su administrador</strong>: este es el aprobador predeterminado, establecido por el sistema. En este caso, el usuario designado como su responsable aprueba la plantilla de horas cuando se envía para su aprobación.</li> 
      <li><strong>Personas específicas:</strong> puede designar a usuarios específicos, por su nombre, como aprobadores de plantillas de horas. Puede tener varios aprobadores en una plantilla de horas. En este caso, una vez que uno de los aprobadores aprueba la plantilla de horas, esta se marca como <strong>Cerrada</strong> y desaparece de la lista de aprobaciones de plantillas de horas de todos los aprobadores restantes.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Puede editar el tiempo</strong> </td> 
      <td> <p> <p>Seleccione esta opción para permitir que los aprobadores editen las horas en la plantilla de horas.

   <p>Esta opción funciona junto con la configuración **Restringir la edición de plantillas de horas a propietarios y administradores** en el área Configuración &gt; Plantilla de horas y horas &gt; Preferencias. Para obtener más información, consulte <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configurar preferencias de plantillas de horas y de horas</a>.</p>

   <p>Se dan los siguientes escenarios: </p>

   <ul>
      <li>Cuando la opción <b>Restringir la edición de plantillas de horas a propietarios y administradores</b> está habilitada:</li>
      <ul><li>Los aprobadores solo pueden aprobar y rechazar plantillas de horas, independientemente de si <b>Puede editar el tiempo</b> está habilitado o no. </li>
      <li>Los administradores de propietarios de plantillas de horas solo pueden ver las plantillas de horas de sus informes directos.</li></ul>
      <li>Cuando la opción <b>Restringir la edición de plantillas de horas a propietarios y administradores</b> está deshabilitada:</li>
    <ul><li>Cuando la opción <b>Puede editar el tiempo</b> está habilitada, los aprobadores pueden enviar, reabrir o cerrar la plantilla de horas, así como editar el tiempo.</li>
      <li>Cuando la opción <b>Puede editar el tiempo</b> está deshabilitada, los aprobadores no pueden enviar, reabrir o cerrar la plantilla de horas, ni editar la hora. Los aprobadores solo pueden aprobar o rechazar la plantilla de horas. </li>
      <li>Los administradores de los propietarios de las plantillas de horas pueden enviar, recuperar, volver a abrir y editar las plantillas de horas de sus informes directos.</li></ul>
      </ul>

   <p>

   <b>NOTA</b>: Una vez que envíe una hoja de horas para su aprobación, ya no podrá editar las horas. Para devolver una plantilla de horas enviada a un estado editable, recupere la plantilla de horas o solicite al aprobador que la rechace. Para obtener más información, consulte <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Enviar hoja de horas para su aprobación</a> y <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Aprobar una hoja de horas</a>.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Tipos de horas disponibles</strong> </td> 
      <td><p>Esta configuración solo hace referencia a tipos de horas generales y no a tipos de horas específicos del proyecto. </p>
      <p>De forma predeterminada, los usuarios ven todas las horas generales en una hoja de horas. Sin embargo, si su organización desea que solo se muestren horas generales específicas para un conjunto determinado de usuarios, puede seleccionar las horas generales que necesitan ver en sus plantillas de horas seleccionándolas en el perfil de plantilla de horas en este campo. Si desea deshabilitar todas las horas generales, anule la selección de todos los tipos de horas para generar la plantilla de horas sin una sección para las horas generales.</p></td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Notificaciones de recordatorio</strong> </td> 
      <td> <p> Añada una notificación de recordatorio. Workfront enviará recordatorios a los usuarios para pedirles que completen o aprueben sus plantillas de horas. Debe crear notificaciones de recordatorio antes de poder asociarlas a un perfil de hoja de horas.  </p> </td> 
     </tr>

   <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Horas extra</span> </td> 
      <td>Puede elegir ocultar el cuadro Horas extra en las plantillas de horas. Esta opción está desactivada de forma predeterminada.</td> 
     </tr> 
    </tbody> 
    </table>

1. Al crear perfiles de hojas de horas de nivel de grupo, haga clic en la ficha **Asignar personas** para asociar el perfil de hojas de horas con usuarios, grupos o equipos específicos (si es administrador de Workfront). <!--Keep the reference to the group upon release to Prod, for now, until they unshim the group Timesheet Profiles-->

   Al crear perfiles de hojas de horas para el sistema, desplácese hacia la parte inferior de la página y busque la sección **Asignar personas**. <!--Keep the reference to the system when releasing to Prod, until they unshim the group Timesheet Profile-->

   Empiece a escribir el nombre del usuario, grupo o equipo y, a continuación, haga clic en él cuando aparezca en la lista desplegable.

   Si es administrador de un grupo, puede asignar el perfil de la plantilla de horas a los grupos que administre, pero no a los equipos. Para obtener más información, consulte [Limitaciones para un administrador de grupo que asigna un perfil de plantilla de horas](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) en este artículo.

   >[!NOTE]
   >
   >* También puede asociar un usuario con un perfil de plantilla de horas editando el perfil del usuario. Para obtener más información, consulte [Editar el perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* Cuando se añade un grupo, solo aparece el nombre del grupo en la pestaña Asignar personas, no la lista de integrantes del grupo. Si desea ver los integrantes del grupo enumerados aquí, haga clic en Guardar cambios y, a continuación, haga clic en el nombre del perfil de plantilla de horas que acaba de crear.
   >* Cuando termina estos pasos, el perfil de plantilla de horas genera plantillas de horas únicamente para los usuarios o integrantes del grupo asignados que no tienen plantillas de horas existentes para el período actual.

1. Haga clic en **Guardar**.

1. En la parte superior de la lista de perfiles de hojas de horas, haga clic en el icono **Más** ![Icono de más](assets/more-icon.png) para perfiles de hojas de horas de nivel de sistema o en **Más** para perfiles de hojas de horas de grupo y, a continuación, haga clic en **Generar hojas de horas**.

   En la parte inferior de la pantalla aparece una confirmación de que las plantillas de horas se han generado correctamente. Se generan nuevas plantillas de horas en función de los nuevos perfiles que haya creado.

   Para obtener más información, consulte [Generar hojas de horas manualmente](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

   La primera vez que el perfil de plantilla de horas genera plantillas de horas, se crean 2 plantillas de horas para cada usuario, tanto para el periodo de tiempo que incluye la hora actual como para el siguiente periodo de tiempo.

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
