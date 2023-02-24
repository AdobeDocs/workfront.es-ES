---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Crear, editar y asignar perfiles de parte de horas
description: Puede crear, editar y asignar perfiles de hojas de horas que generen hojas de horas recurrentes para los usuarios sin ninguna otra intervención por su parte. Esto ahorra tiempo y garantiza la coherencia entre los usuarios.
author: Alina
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 43f1ad86784532ed3a5a3baa12d135ca35f16d21
workflow-type: tm+mt
source-wordcount: '1505'
ht-degree: 1%

---

# Crear, editar y asignar perfiles de parte de horas

Puede crear, editar y asignar perfiles de hojas de horas que generen hojas de horas recurrentes para los usuarios sin ninguna otra intervención por su parte. Esto ahorra tiempo y garantiza que los siguientes elementos sean coherentes entre los usuarios:

* Lapso de tiempo de hoja de horas
* Aprobadores
* Tipos de hora generales

Para obtener más información sobre la creación manual de un parte de horas, consulte [Crear un parte de horas de un solo uso](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

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
   <td> <p>Debe tener acceso administrativo a las hojas de horas. </p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p>  <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Crear o editar un perfil de hoja de horas

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>Para habilitar los cambios de perfil de parte de horas en hojas de horas actuales, debe eliminar las hojas de horas existentes y luego generar otras nuevas. Para obtener instrucciones, consulte [Eliminar partes de horas en Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) y [Generar hojas de hora manualmente](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Si está creando o editando un perfil de parte de horas para utilizarlo en todo el sistema, haga clic en **Hoja de horas y horas**.

   O

   Si crea o edita un perfil de parte de horas para un grupo, haga clic en **Grupos** y, a continuación, haga clic en el nombre del grupo.

1. Haga clic en **Perfiles de parte de horas**.
1. Para crear un nuevo perfil de parte de horas, haga clic en **Nuevo perfil**.

   O

   Para editar un perfil de parte de horas existente, seleccione el perfil de parte de horas que desee editar y haga clic en **Editar**.

   Se muestra el perfil de parte de horas nuevo o existente.


1. En el **Definir detalles** pestaña , escriba a **Nombre** y **Descripción** para el perfil del parte de horas y proporcione la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Grupo con acceso de administración</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>Si está creando un perfil de parte de horas de nivel de sistema, deje este campo en blanco.</p> <p>Cualquier usuario que pueda editar cuentas de usuario puede adjuntar un parte de horas del sistema a otros usuarios.</p> <p>Solo los administradores de Workfront pueden editar un perfil de parte de horas a nivel de sistema.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>Si está creando un perfil de parte de horas para un grupo que administra, identifique el grupo aquí.</p> <p>Esto no asigna el perfil de parte de horas a los usuarios del grupo; solo permite a los administradores del grupo modificar el perfil del parte de horas. En el paso 6, asignará el perfil a los usuarios.</p> <p><b>NOTA</b>

   Cuando los usuarios fuera del grupo adjuntan perfiles de parte de horas a otro usuario, no podrán ver ni adjuntar este perfil de parte de horas.</p> </li>
   </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Crear hojas de horas</strong> </td> 
      <td> <p> <p>Especifique cuándo debe generar el perfil del parte de horas los partes de horas. Se puede configurar un parte de horas para que se genere automáticamente con periodicidad semanal, quincenal, semestral o mensual. Seleccione el día de la semana en el que desea que se produzca el parte de horas.</p>
      <p>Un parte de horas semanal comienza en la fecha en que se genera. Por ejemplo, si crea hojas de horas semanales todos los jueves, el primer día de la semana en el parte de horas es jueves.</p>
      <p><b>NOTA</b></p>

   <p>Workfront siempre crea dos partes de horas a la vez: el primer parte de horas siempre incluye la fecha actual y el segundo parte de horas se inicia cuando finaliza el período de tiempo del primero.</p> </p> </td> 
    </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Aprobadores</strong></p> </td> 
      <td> <p> <p>Los aprobadores son usuarios que aprueban el parte de horas para los usuarios asociados al parte de horas. Puede identificar hasta 7 usuarios como aprobadores en un parte de horas. La identificación de varios usuarios es útil para garantizar que un aprobador esté disponible cuando alguien está fuera de la oficina. Se notifica a todos los aprobadores cuando un usuario envía el parte de horas para su aprobación. Solo se necesita un usuario para aprobar el parte de horas para que se apruebe.</p> <p>Solo los usuarios con derechos administrativos de parte de horas pueden configurarse como aprobadores. Para obtener más información sobre los derechos administrativos del parte de horas, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> <p>Utilice el menú desplegable para seleccionar el aprobador del parte de horas (si se requiere un aprobador). Puede seleccionar entre las siguientes opciones:</p> 
      <ul> 
      <li><strong>Ninguna</strong>: No es necesario aprobar el parte de horas.</li> 
      <li><strong>Su administrador</strong>: Este es el aprobador predeterminado configurado por el sistema. En este caso, el usuario designado como administrador aprueba el parte de horas cuando se envía para su aprobación.</li> 
      <li><strong>Personas específicas:</strong> Puede designar usuarios específicos, por nombre, como aprobadores de hojas de horas. Puede tener varios aprobadores en un parte de horas. En este caso, después de que uno de los aprobadores apruebe el parte de horas, el parte de horas se marca como <strong>Cerrado</strong> y desaparece de la lista de aprobaciones de parte de horas de todos los aprobadores restantes.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Puede editar el tiempo </strong> </td> 
      <td> <p> <p>Seleccione esta opción para permitir que los aprobadores editen las horas en el parte de horas.

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

   Una vez que envíe un parte de horas para su aprobación, ya no podrá editar las horas. Para devolver un parte de horas enviado a un estado editable, recuerde el parte de horas o haga que el aprobador rechace el parte de horas. Para obtener más información, consulte <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Enviar un parte de horas para su aprobación</a> y<a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Aprobar un parte de horas</a>.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Tipos de horas disponibles</strong> </td> 
      <td>De forma predeterminada, los usuarios ven todas las horas generales en un parte de horas. Sin embargo, si su organización desea que solo se muestren horas generales específicas para un conjunto determinado de usuarios, puede seleccionar las horas generales que deben ver en sus hojas de horas seleccionándolas en su perfil de parte de horas en este campo. Si desea deshabilitar todas las horas generales, anule la selección de todos los tipos de horas para generar el parte de horas sin una sección para las horas generales.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Horas extra</span> </td> 
      <td>Puede elegir ocultar el cuadro Tiempo extra en las hojas de horas. Esta opción está desactivada de forma predeterminada.</td> 
     </tr> 
    </tbody> 
    </table>

1. Haga clic en el **Asignar personas** para asociar el perfil del parte de horas con usuarios, grupos o equipos específicos (si es administrador de Workfront). Empiece a escribir el nombre del usuario, grupo o equipo y, a continuación, haga clic en él cuando aparezca en la lista desplegable.

   Si es administrador de grupos, puede asignar el perfil de parte de horas a los grupos que administre, pero no a los equipos. Para obtener más información, consulte [Limitaciones para un administrador de grupo que asigna un perfil de parte de horas](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) en este artículo.

   >[!NOTE]
   >
   >* También puede asociar un usuario con un perfil de parte de horas editando el perfil del usuario. Para obtener más información, consulte [Edición del perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* Cuando se agrega un grupo, solo aparece el nombre del grupo en la ficha Asignar personas, no la lista de miembros del grupo. Si desea ver los miembros del grupo enumerados aquí, haga clic en Guardar cambios y, a continuación, haga clic en el nombre del perfil del parte de horas que acaba de crear.
   >* Cuando termina estos pasos, el perfil de parte de horas genera partes de horas solo para los usuarios o miembros de grupo asignados que no tienen partes de horas existentes para el periodo actual.


1. Haga clic en **Guardar cambios**.

   La primera vez que el perfil de parte de horas genera hojas de horas, se crean 2 hojas de horas para cada usuario. A continuación, cada vez que genera nuevas hojas de horas, se crea un parte de horas por usuario.

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## Limitaciones para un administrador de grupo que asigna un perfil de parte de horas {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

Si es administrador de grupos y la opción de acceso administrativo Hojas de hora y horas está desactivada en el nivel de acceso, puede crear perfiles de hojas de horas, pero solo puede asignarlos a:

* Grupos que administra
* Usuarios individuales a los que tiene acceso para editar que se encuentran en un grupo que administra

Para estos grupos y usuarios, no tendrá acceso a las hojas de horas que genera el perfil de parte de horas.

Además, si la opción Administración de usuarios (usuarios del grupo) también está deshabilitada en el nivel de acceso, puede asignar el perfil del parte de horas a un grupo que administre, pero solo afecta a los usuarios del grupo a los que tenga acceso para editar. Si el grupo contiene usuarios a los que no tiene acceso para editar, no se les asigna el perfil del parte de horas junto con el resto del grupo.

Para obtener información sobre la opción Hojas de hora y horas en el nivel de acceso, consulte [Conceder a los usuarios acceso administrativo a determinadas áreas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Para obtener información sobre la opción Administrador de usuarios (usuarios del grupo) en el nivel de acceso, consulte [Conceder acceso a los usuarios](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Varios perfiles de hojas de horas recurrentes

Puede tener más de un perfil de parte de horas para su organización si hay:

* Periodos de pago únicos para diferentes conjuntos de usuarios
* Aprobadores únicos para diferentes conjuntos de usuarios
* Requisitos de horas generales únicas para diferentes conjuntos de usuarios

Un usuario no puede asociarse con más de un perfil de parte de horas a la vez. 
