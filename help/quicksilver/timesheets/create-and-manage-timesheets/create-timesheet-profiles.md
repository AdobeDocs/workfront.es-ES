---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Crear, editar y asignar perfiles de hojas de horas
description: Puede crear, editar y asignar perfiles de hojas de horas que generen hojas de horas recurrentes para los usuarios sin que usted tenga que intervenir más. Esto le ahorra tiempo y garantiza la coherencia entre los usuarios.
author: Alina
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 9b6552fe496a1602786cdc6b6050d02cd367a531
workflow-type: tm+mt
source-wordcount: '1519'
ht-degree: 1%

---

# Crear, editar y asignar perfiles de hojas de horas

Puede crear, editar y asignar perfiles de hojas de horas que generen hojas de horas recurrentes para los usuarios sin que usted tenga que intervenir más. Esto le ahorra tiempo y garantiza que los siguientes elementos sean coherentes entre los usuarios:

* Lapso de tiempo de hoja
* Aprobadores
* Tipos de horas generales

Para obtener más información sobre cómo crear una plantilla de horas manualmente, consulte [Crear hoja de horas de un solo uso](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

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

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Crear o editar un perfil de hoja de horas

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>Para habilitar los cambios de perfil de hoja de horas en las hojas de horas actuales, debe eliminar las hojas de horas existentes y luego generar otras nuevas. Para obtener instrucciones, consulte [Eliminación de plantillas de horas en Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) y [Generar manualmente hojas de horas](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. Si está creando o editando un perfil de hoja de horas para utilizarlo en todo el sistema, haga clic en **Hoja de horas y horas**.

   O

   Si está creando o editando un perfil de plantilla de horas para un grupo, haga clic en **Grupos** y, a continuación, haga clic en el nombre del grupo.

1. Clic **Perfiles de hoja de horas**.
1. Para crear un nuevo perfil de hoja de horas, haga clic en **Nuevo perfil**.

   O

   Para editar un perfil de plantilla de horas existente, seleccione el perfil de plantilla de horas que desee editar y haga clic en **Editar**.

   Se muestra el perfil de hoja de horas nuevo o existente.


1. En el **Establecer detalles** pestaña, escriba un **Nombre** y **Descripción** para el perfil de la plantilla de horas y proporcione la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Grupo con acceso de administración</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>Si está creando un perfil de hoja de horas de nivel de sistema, deje este campo en blanco.</p> <p>Cualquier usuario que pueda editar cuentas de usuario puede adjuntar una plantilla de horas de nivel del sistema a otros usuarios.</p> <p>Solamente un administrador de Workfront puede editar un perfil de hoja de horas de nivel de sistema.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>Si está creando un perfil de hoja de horas para un grupo que administra, identifique el grupo aquí.</p> <p>Esto no asigna el perfil de plantilla de horas a los usuarios del grupo; solo permite a los administradores del grupo modificar el perfil de plantilla de horas. Asignará el perfil a los usuarios en el paso 6.</p> <p><b>NOTA</b>

   Cuando los usuarios fuera del grupo adjuntan perfiles de plantilla de horas a otros usuarios, no podrán ver ni adjuntar este perfil de plantilla de horas.</p> </li>
   </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Crear hojas de horas</strong> </td> 
      <td> <p> <p>Especifique cuándo el perfil de hoja de horas debe generar las hojas de horas. Se puede configurar una hoja de horas para que se genere automáticamente de forma semanal, quincenal, semestral o mensual. Seleccione el día de la semana en el que desea que se produzca la plantilla de horas.</p>
      <p>Una hoja de horas semanal comienza en la fecha en que se genera. Por ejemplo, si crea hojas de horas semanales todos los jueves, el primer día de la semana en la hoja de horas es el jueves.</p>
      <p><b>NOTA</b></p>

   <p>Workfront siempre crea dos plantillas de horas a la vez: la primera incluye siempre la fecha actual y la segunda comienza cuando termina el lapso de tiempo de la primera.</p> </p> </td> 
    </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Aprobadores</strong></p> </td> 
      <td> <p> <p>Los aprobadores son usuarios que aprueban la hoja de horas de los usuarios asociados con ella. Puede identificar hasta 7 usuarios como aprobadores en una hoja de horas. La identificación de varios usuarios resulta útil para garantizar que un aprobador esté disponible cuando alguien esté fuera de la oficina. Se notifica a todos los aprobadores cuando un usuario envía la plantilla de horas para su aprobación. Solo se requiere un usuario para aprobar la plantilla de horas.</p> <p>Solo los usuarios con derechos administrativos de hoja de horas pueden establecerse como aprobadores. Para obtener más información sobre los derechos administrativos de plantillas de horas, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> <p>Utilice el menú desplegable para seleccionar el aprobador de la plantilla de horas (si se requiere un aprobador). Puede seleccionar las siguientes opciones:</p> 
      <ul> 
      <li><strong>Ninguno</strong>: no es necesario aprobar la plantilla de horas.</li> 
      <li><strong>Su responsable</strong>: Es el aprobador predeterminado, establecido por el sistema. En este caso, el usuario designado como su responsable aprueba la plantilla de horas cuando se envía para su aprobación.</li> 
      <li><strong>Personas específicas:</strong> Puede designar a usuarios concretos, por su nombre, como aprobadores de plantillas de horas. Puede tener varios aprobadores en una hoja de horas. En este caso, una vez que uno de los aprobadores aprueba la plantilla de horas, esta se marca como <strong>Cerrado</strong> y desaparece de la lista de aprobaciones de hojas de horas de todos los aprobadores restantes.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Puede editar el tiempo </strong> </td> 
      <td> <p> <p>Seleccione esta opción para permitir que los aprobadores editen las horas en la hoja de horas.

   Esta opción funciona junto con la variable **Restringir la edición de hojas de horas a propietarios y administradores** en el área Configuración > Hoja de horas y Horas > Preferencias. Para obtener más información, consulte <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configurar preferencias de horas y hojas de horas</a>.

   Existen los siguientes escenarios:

   <ul>
      <li>Si la variable <b>Restringir la edición de hojas de horas a propietarios y administradores</b> La opción está activada:</li>
      <ul><li>Los aprobadores solo pueden aprobar y rechazar plantillas de horas, independientemente de si <b>Puede editar el tiempo</b> está activada o no. </li>
      <li>Los administradores de propietarios de hojas de horas solo pueden ver las hojas de horas de sus subordinados directos.</li></ul>
      <li>Si la variable <b>Restringir la edición de hojas de horas a propietarios y administradores</b> La opción está desactivada:</li>
    <ul><li>Si la variable <b>Puede editar el tiempo</b> está activada, los aprobadores pueden enviar, volver a abrir o cerrar la plantilla de horas y editar la hora.</li>
      <li>Si la variable <b>Puede editar el tiempo</b> está desactivada, los aprobadores no pueden enviar, volver a abrir ni cerrar la plantilla de horas y no pueden editar la hora. Los aprobadores solo pueden aprobar o rechazar la hoja de horas. </li>
      <li>Los administradores de los propietarios de las hojas de horas pueden enviar, recuperar, volver a abrir y editar las hojas de horas de sus subordinados directos.</li></ul>
      </ul>

   <p><b>NOTA</b>

   Una vez enviada una hoja de horas para su aprobación, ya no puede editar las horas. Para devolver una hoja de horas enviada a un estado editable, recupere la hoja de horas o pida al aprobador que la rechace. Para obtener más información, consulte <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Enviar hoja de horas para su aprobación</a> y<a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Aprobar una hoja de horas</a>.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Tipos de horas disponibles</strong> </td> 
      <td><p>Esta configuración solo hace referencia a los tipos de horas generales y no a los específicos del proyecto. </p>
      <p>De forma predeterminada, los usuarios ven todas las horas generales en una hoja de horas. Sin embargo, si su organización desea que solo se muestren horas generales específicas para un conjunto determinado de usuarios, puede seleccionar las horas generales que necesitan ver en sus plantillas de horas seleccionándolas en el perfil de plantilla de horas en este campo. Si desea deshabilitar todas las horas generales, anule la selección de todos los tipos de horas para generar la hoja de horas sin una sección para las horas generales.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Horas extra</span> </td> 
      <td>Puede elegir ocultar el cuadro Horas extra en las plantillas de horas. Esta opción está desactivada de forma predeterminada.</td> 
     </tr> 
    </tbody> 
    </table>

1. Haga clic en **Asignar personas** para asociar el perfil de la plantilla de horas con usuarios, grupos o equipos específicos (si es administrador de Workfront). Empiece a escribir el nombre del usuario, grupo o equipo y, a continuación, haga clic en él cuando aparezca en la lista desplegable.

   Si es administrador de un grupo, puede asignar el perfil de la plantilla de horas a los grupos que administre, pero no a los equipos. Para obtener más información, consulte [Limitaciones para un administrador de grupo que asigna un perfil de hoja de horas](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) en este artículo.

   >[!NOTE]
   >
   >* También puede asociar un usuario con un perfil de plantilla de horas editando el perfil del usuario. Para obtener más información, consulte [Edición del perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* Cuando se agrega un grupo, sólo aparece el nombre del grupo en la ficha Asignar personas, no la lista de miembros del grupo. Si desea ver los miembros del grupo enumerados aquí, haga clic en Guardar cambios y, a continuación, haga clic en el nombre del perfil de hoja de horas que acaba de crear.
   >* Cuando termina estos pasos, el perfil de hoja de horas genera hojas de horas únicamente para los usuarios o miembros del grupo asignados que no tienen hojas de horas existentes para el periodo actual.

1. Clic **Guardar cambios**.

   La primera vez que el perfil de hoja de horas genera hojas de horas, se crean 2 hojas de horas por cada usuario. Después, cada vez que genera nuevas plantillas de horas, se crea una por usuario.

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## Limitaciones para un administrador de grupo que asigna un perfil de hoja de horas {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

Si es administrador de un grupo y la opción de acceso administrativo Plantillas de horas y horas está desactivada en su nivel de acceso, puede crear perfiles de plantillas de horas, pero puede asignarlos únicamente a:

* Grupos que administra
* Usuarios individuales a los que tiene acceso para editar que están en un grupo que administra

Para estos grupos y usuarios, no tendrá acceso a las plantillas de horas que genera el perfil de plantilla de horas.

Además, si la opción Administración de usuarios (Usuarios del grupo) también está desactivada en su nivel de acceso, puede asignar el perfil de plantilla de horas a un grupo que administre, pero esto solo afecta a los usuarios del grupo al que tenga acceso para editar. Si el grupo contiene usuarios a los que no tiene acceso para editar, no se les asigna el perfil de plantilla de horas junto con el resto del grupo.

Para obtener información sobre la opción Hojas de horas y horas en su nivel de acceso, consulte [Conceder a los usuarios acceso administrativo a determinadas áreas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Para obtener información sobre la opción Administración de usuarios (usuarios de grupo) en su nivel de acceso, consulte [Concesión de acceso a los usuarios](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Varios perfiles de hojas de horas recurrentes

Puede tener más de un perfil de hoja de horas para su organización si hay:

* Períodos de pago únicos para diferentes conjuntos de usuarios
* Aprobadores únicos para diferentes conjuntos de usuarios
* Requisitos generales de horas únicos para diferentes conjuntos de usuarios

No se puede asociar a un usuario con más de un perfil de hoja de horas a la vez. 
