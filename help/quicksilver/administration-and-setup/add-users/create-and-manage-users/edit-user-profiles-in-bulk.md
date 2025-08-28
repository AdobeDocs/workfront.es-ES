---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Editar perfiles de usuario de forma masiva
description: Como administrador de Adobe Workfront, puede editar las cuentas de usuario de forma masiva.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: c7b91828e5a4f961fc48e857eb63756b9b38f664
workflow-type: tm+mt
source-wordcount: '2625'
ht-degree: 65%

---

# Editar perfiles de usuario de forma masiva

{{highlighted-preview}}

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

Puede editar las cuentas de usuario de forma masiva. Al editar usuarios de forma masiva, solo los campos que seleccione específicamente se actualizarán con la misma información para todos los usuarios seleccionados. Todos los demás campos que deje sin seleccionar permanecerán igual para cada usuario individual, aunque sean diferentes para cada usuario.

>[!NOTE]
>
>* No puede editar de forma masiva la sección Información personal de los perfiles de los usuarios porque esa información debe ser única para cada usuario.
>* Para garantizar la precisión de los datos y un rendimiento óptimo, se recomienda seleccionar un máximo de 2000 usuarios al mismo tiempo para una edición masiva.
>

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p><p>O</p><p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe tener uno de los siguientes elementos:</p> 
    <ul> 
     <li> <p>El nivel de acceso del administrador del sistema. </li> 
     <li> <p>Configuración de <b>usuarios</b> en su nivel de acceso configurado para el acceso de <b>Edición</b>, con <b>Crear</b> y al menos una de las dos opciones de <b>Administrador de usuarios</b> habilitadas en <b>Ajustar la configuración</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De estas dos opciones, si <b>Administrador de usuarios (usuarios de grupo)</b> está habilitado, debe ser administrador de grupo de un grupo al que pertenezca el usuario.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Editar cuentas de usuario de forma masiva

{{step-1-to-users}}

1. Seleccione más de un usuario y luego haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png).

1. En el cuadro **Editar usuario**, cambie la información en cualquiera de las secciones y haga clic en **Guardar cambios** <span class="preview">o **Guardar**</span> en cualquier momento.

### Preferencias

* **Zona horaria**: La zona horaria del usuario.

  Para obtener información acerca de cómo ayudar a los usuarios a colaborar en Workfront en diferentes zonas horarias, consulte [Trabajar en diferentes zonas horarias](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

* **Configuración regional del correo electrónico**: la configuración regional de correo electrónico preferida del usuario. Esto afecta al formato de los números y de las fechas de los correos electrónicos que llegan desde Workfront a este usuario.

  >[!NOTE]
  >
  >Cuando su organización se encuentra en la experiencia unificada de Adobe, las preferencias de idioma del usuario se almacenan en su perfil de Adobe y no se utiliza la configuración regional del correo electrónico. Para obtener información sobre el acceso a estas preferencias, consulte [Experiencia unificada de Adobe para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

### Notificaciones

Seleccione las notificaciones por correo electrónico que deben habilitarse para los usuarios.

Puede seleccionar notificaciones de resumen instantáneas y diarias. Todas las notificaciones de resumen diario se envían en algún momento después de la misma hora para todos los usuarios seleccionados.

Para obtener más información, consulte [Configurar notificaciones de los eventos para todos los usuarios del sistema](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

### Acceso

* **Está activo** / <span class="preview">**El usuario está activo**</span>: Habilite esta opción para indicar que los usuarios están activos.  Los usuarios activos utilizan una licencia de Workfront. Al deshabilitar el campo, se desactiva a los usuarios y se impide que inicien sesión en Workfront.

* **Nivel de acceso**: seleccione el nivel de acceso que desea asignar a estos usuarios. Todos los usuarios seleccionados tendrán el mismo nivel de acceso.

  Al asignar un nivel de acceso a los usuarios, puede asignar un nivel igual o inferior al suyo propio. (Por ejemplo, si el nivel de acceso es Estándar, no puede asignar el nivel de acceso Administrador.)

  Sin embargo, no puede asignar un nivel de acceso que, de forma predeterminada, sea inferior a su propio nivel de acceso si el administrador de Workfront ha habilitado permisos no predeterminados en el nivel de acceso que no están habilitados también en su propio nivel de acceso.

  Por ejemplo, si tiene una licencia estándar sin acceso para eliminar tareas, no puede asignar a alguien una licencia básica con acceso para eliminar tareas, aunque la licencia básica sea inferior a la licencia estándar. Para obtener más información, consulte [Creación o modificación de niveles de acceso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

  Para obtener más información sobre los niveles de acceso, consulte [Configurar el acceso a Adobe Workfront](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md).

  >[!NOTE]
  >
  >Si su organización utiliza el nuevo modelo de acceso (Standard/Light/Contributor), no puede reasignar un usuario Standard o Light a un nivel de acceso Contributor si dicho usuario ya ha alcanzado su límite de decisiones del mes.
  >
  >Para obtener más información sobre el nuevo modelo de acceso, consulte [Información general sobre los nuevos niveles de acceso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).
  >
  >Para obtener información sobre los límites de decisión, consulte [información general sobre decisiones limitadas de documentos y de la revisión para usuarios sin pago](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

* **Plantilla de diseño**: elija una plantilla de diseño para los usuarios. esta plantilla de diseño tiene prioridad sobre cualquier plantilla de diseño asignada a su grupo de inicio, equipo de inicio o función principal. Para obtener más información acerca de la prioridad de asignación de las plantillas de diseño, vea [Crear y administrar plantillas de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

  La siguiente lista describe cómo la lista de plantillas disponibles en este campo depende de su acceso:

   * Como administrador de Workfront, puede ver todas las plantillas de diseño de nivel de sistema y de grupo.
   * Como administrador de grupos, puede ver la plantilla de diseño de nivel de sistema, así como las asociadas con los grupos que administra.
   * Como usuario con una licencia estándar o de planificación y acceso para editar usuarios, solo puede ver plantillas de diseño de nivel de sistema.

     Para obtener más información acerca de las plantillas de diseño de nivel de grupo, vea [Crear y modificar plantillas de diseño de un grupo](/help/quicksilver/administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

### Organización

* **Compañía**: la compañía de los usuarios. Los usuarios solo pueden asociarse con una compañía. Debe crear una compañía antes de poder asociarla a un usuario. En la lista solo se muestran las compañías activas. Para obtener información acerca de cómo crear compañías, consulte [Crear y editar compañías](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* **Equipo de inicio**: especifique el equipo de inicio de los usuarios. Los usuarios solo pueden tener un equipo de inicio.
* **Otros equipos**: los usuarios pueden pertenecer a varios equipos.
* **Grupo de inicio** / <span class="preview">**Grupo de inicio actual**</span>: seleccione un grupo apropiado para asignar los usuarios. Esto proporciona a los usuarios la capacidad de acceder a los objetos compartidos con el grupo. También puede compartir plantillas de diseño con un grupo de inicio.

  Este campo es obligatorio. Todos los usuarios deben estar asociados a un grupo de inicio. Si no selecciona uno, el grupo de inicio se asigna como grupo de inicio.

  Puede asignar un grupo a un usuario solo si se cumple una de las siguientes condiciones:

   * es administrador de Workfront
   * es el administrador del grupo
   * el grupo es público

* **Otros grupos**: los usuarios pueden pertenecer a varios grupos. Solo puede asignar un grupo a un usuario si es administrador de Workfront, si es el administrador de grupos o si el grupo es público.

  >[!IMPORTANT]
  >
  >Añadir un usuario a más de 100 grupos puede causar problemas de rendimiento en cualquier área de Workfront que cargue la lista de grupos.

  Para obtener más información sobre los grupos públicos, consulte [Crear un grupo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

  Para obtener más información sobre los grupos, consulte [Información general sobre los grupos](/help/quicksilver/administration-and-setup/manage-groups/groups-overview/groups.md).

### Planificación de recursos

* **Tiempo de trabajo**: Representa el porcentaje de tiempo equivalente a tiempo completo (FTE) que los usuarios están disponibles para el trabajo real, sin incluir los gastos generales. El tiempo de trabajo debe ser un número decimal de hasta 1 y no puede ser 0. Por ejemplo, una disponibilidad del 20% para el trabajo real sería de 0,2.

  El valor predeterminado del campo es 1, lo que indica que un usuario emplea todo su FTE en trabajo real relacionado con el proyecto.

  El sistema utiliza este número para calcular la disponibilidad del usuario para el trabajo real relacionado con el proyecto.

  Para obtener más información sobre cómo crear programaciones en Workfront, consulte [Crear programación](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

  Las excepciones de programación y los días libres también pueden afectar a la capacidad del usuario.

  Workfront calcula la disponibilidad de un usuario según las preferencias de Administración de recursos del área de Configuración. Para obtener más información, consulte [Configurar preferencias de administración de recursos](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

  >[!TIP]
  >
  >Establezca el valor Tiempo de trabajo en 1 para indicar que el usuario está disponible para el trabajo relacionado con el proyecto en su equivalente a jornada completa

* **Programar desactivación** / <span class="preview">**Establecer fecha de desactivación**</span>: marque esta casilla / <span class="preview">haga clic en este botón</span> si desea programar la desactivación de estos usuarios en una fecha y a una hora determinadas.
* **Fecha programada de desactivación** / <span class="preview">**Fecha de desactivación**</span>: La fecha y la hora en que se desactivaron los usuarios. Para obtener información sobre cómo programar usuarios para la desactivación, consulte [Programar usuarios para la desactivación](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation) en [Desactivar o reactivar un usuario](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
* **Rol principal**: Este es el rol principal que los usuarios pueden cumplir en Workfront. Todas las tareas y problemas que se asignan a los usuarios también se asignan a este rol. Las funciones de trabajo son esenciales en la administración de recursos. Solo puede actualizar este campo si dispone de una licencia Standard o Plan con acceso de usuario administrativo o si es administrador de Workfront. Para obtener más información sobre la configuración de usuarios con acceso de usuario administrativo, consulte [Conceder acceso a usuarios](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

  En la lista solo se muestran las funciones activas.

* (Condicional) Si seleccionó una **Función principal**, se muestra el campo **Porcentaje de disponibilidad de FTE**. Especifique qué porcentaje de tiempo de las programaciones de los usuarios se asigna a esta función. El valor predeterminado para el porcentaje de disponibilidad de FTE para la función principal es 100%.
* **Otras funciones**: los usuarios pueden tener varias funciones en Workfront. Las funciones de trabajo son esenciales en la administración de recursos. No hay límite en cuanto a las funciones que puede desempeñar un usuario. Sin embargo, se recomienda no asignar un usuario a un número excesivamente elevado de funciones del puesto, ya que la administración de recursos podría resultar demasiado compleja para estos usuarios.

  En la lista solo se muestran las funciones activas. Para obtener más información sobre las funciones, consulte [Crear y administrar funciones](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

  Solo puede actualizar este campo si dispone de una licencia Standard o Plan con acceso de usuario administrativo o si es administrador de Workfront.

  Para obtener más información sobre la configuración de usuarios con acceso de usuario administrativo, consulte [Conceder acceso a los usuarios](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

* (Condicional) Si ha seleccionado una o varias **Otras funciones**, se muestra el campo **Porcentaje de disponibilidad de FTE** para cada función. Especifique qué porcentaje de tiempo del horario de los usuarios se asigna a cada función. El valor predeterminado para el porcentaje de disponibilidad de FTE para las otras funciones es 0 %.

  Si otras funciones tienen una disponibilidad de FTE del 0 %, no se muestran en el Planificador de recursos, a menos que los usuarios estén asignados a tareas de estas funciones.

  La suma de todos los **porcentajes de disponibilidad de FTE** para todas las funciones debe ser igual a 100 %. Cada porcentaje de disponibilidad de FTE calcula las horas disponibles para cada función por usuario en el Planificador de recursos. Las horas disponibles para cada función por usuario dependen del tiempo disponible para el usuario.

  Workfront calcula el tiempo disponible para el usuario según el método que haya seleccionado el administrador de Workfront para calcular el valor de FTE en las Preferencias de administración de recursos.

  Para obtener información acerca de cómo calcular la disponibilidad del usuario, vea [Información general sobre el cálculo de horas y FTE para usuarios y roles en el Planificador de recursos](/help/quicksilver/resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

  Para obtener información acerca de cómo configurar las preferencias de Administración de recursos, vea [Configurar las preferencias de Administración de recursos](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **Programación**: asocie una programación con los usuarios. La programación de los usuarios calcula la línea de tiempo de las tareas que se les asignan.

  Debe crear una programación para poder asociarla a los usuarios. Para obtener más información acerca de cómo crear programaciones, vea [Crear una programación](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

  >[!IMPORTANT]
  >
  >Workfront usa la programación de un usuario solamente cuando la opción **Calcular disponibilidad de recursos usando** está establecida en **La programación del usuario**. Para obtener información acerca de cómo afecta esta configuración a la programación que se usa para la administración de recursos, vea [Configurar las preferencias de administración de recursos](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **Perfil de hoja de horas**: asocie un perfil de hoja de horas con los usuarios para garantizar que las hojas de horas se generen automáticamente.

  La lista de perfiles disponibles en este campo depende de su acceso:

   * Como administrador de Workfront, puede ver todos los perfiles de plantilla de horas a nivel del sistema y de grupo.
   * Como administrador de grupos, puede ver perfiles de plantillas de horas de nivel del sistema, así como los asociados con los grupos que administra.
   * Como usuario con una licencia estándar o de planificación y acceso para editar usuarios, solo puede ver perfiles de hojas de horas en el sistema. Para obtener más información sobre los perfiles de plantilla de horas de nivel de grupo, consulte [Crear, editar y asignar perfiles de plantilla de horas](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Tipo de hora predeterminado**: seleccione el tipo de hora predeterminado para los usuarios. Es el tipo de hora que se utiliza de forma predeterminada cuando los usuarios registran el tiempo.
* **Tipos de horas disponibles**: seleccione los tipos de horas que deben estar disponibles para los usuarios. Estos tipos de horas son visibles en todas partes en Workfront, donde los usuarios pueden registrar la hora. Los usuarios solo pueden ver los tipos de horas que están habilitados en el nivel de proyecto y en el nivel de usuario. Para obtener más información acerca de los tipos de horas que están disponibles para los usuarios, consulte [Definición de tipos de horas y disponibilidad](/help/quicksilver/timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
* **ETC**: Este es el equivalente a tiempo completo de los usuarios. Workfront utiliza este número para calcular la disponibilidad de los usuarios según el horario predeterminado sólo cuando las Preferencias de Gestión de Recursos del sistema están definidas en El Horario por Defecto.

  El valor de FTE indica la cantidad de tiempo que los usuarios pueden pasar en el trabajo. Esto incluye la sobrecarga, así como el tiempo empleado en el trabajo del proyecto. Por ejemplo, el tiempo empleado en reuniones o en formación también se incluye en el EJC.

  El valor de FTE debe ser un número decimal de hasta 1 y no puede ser 0. Por ejemplo, si el valor de FTE es 0,5 y el horario predeterminado en Workfront es 40 horas, los usuarios estarán disponibles durante 20 horas a la semana.

  El valor predeterminado del campo es 1.

  Las excepciones de horario, el tiempo libre y el valor del tiempo de trabajo pueden afectar a la disponibilidad de los usuarios.

  Workfront calcula la disponibilidad de un usuario según las preferencias de Administración de recursos del área de Configuración.

  Si las Preferencias de administración de recursos en el nivel del sistema se establecen en El horario del usuario, el valor especificado aquí se ignorará y el usuario se considerará disponible según lo especificado en su horario.

  Para obtener más información, consulte [Configurar las preferencias de administración de recursos](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

  Para obtener más información acerca de cómo crear programaciones en Workfront, vea [Crear una programación](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* **Conjuntos de recursos**: Asocie los usuarios con los conjuntos de recursos.

  >[!NOTE]
  >
  >En este campo solo aparecen los conjuntos de recursos que son comunes a todos los usuarios seleccionados. Si los usuarios seleccionados no tienen conjuntos de recursos compartidos, este campo está vacío. Si este campo está vacío, los conjuntos de recursos que especifique aquí sobrescribirán sus conjuntos de recursos individuales.

  Para obtener más información sobre los conjuntos de recursos, consulte [Asociar conjuntos de recursos a los usuarios](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

* **Tarifa de coste**: cantidad de coste por hora para el usuario.

  Para ver las tarifas de coste efectivas por fecha, haga clic en **Añadir tarifa**. Introduzca el valor de la tarifa de coste para el período de tiempo y asigne una fecha de inicio y una fecha de finalización según sea necesario. La tarifa de coste 1 no tendrá fecha de inicio y la última tasa de coste no tendrá fecha de finalización.

  Algunas fechas se añaden automáticamente. Por ejemplo, si la tarifa de coste 1 no tiene una fecha de finalización y añade la tarifa de coste 2 con una fecha de inicio del 1 de mayo de 2023, se añade la fecha de finalización del 30 de abril de 2023 a la tarifa de coste 1 para que no existan brechas.

* **Tarifa de facturación**: la cantidad de facturación por hora para el usuario.

  Para ver las tarifas de facturación vigentes por fecha, haga clic en **Añadir tarifa**. Introduzca el valor de la tarifa de facturación para el período de tiempo y asigne una Fecha de inicio y una Fecha de finalización según sea necesario. La tarifa de facturación 1 no tendrá una fecha de inicio y la última tarifa de facturación no tendrá una fecha de finalización.

  Algunas fechas se añaden automáticamente. Por ejemplo, si la tarifa de facturación 1 no tiene una fecha de finalización y añade una segunda con una fecha de inicio del 1 de mayo de 2023, se añade la fecha de finalización del 30 de abril de 2023 a la tarifa de facturación 1 para que no existan brechas.

### Formularios personalizados

Asocie un formulario personalizado de usuario existente con los usuarios. Debe crear un formulario personalizado para poder asociarlo a un usuario. En la lista solo se muestran los formularios personalizados activos. Los campos que no tiene acceso para editar no se muestran en un formulario personalizado individual.

>[!NOTE]
>
>Las funciones de formulario personalizadas avanzadas, como los campos de búsqueda externa y los campos nativos de Workfront, solo están disponibles cuando abre el registro de usuario en la página de detalles, no en el cuadro de diálogo Editar usuario. (En la lista de usuarios, haga clic en el nombre del usuario para abrir los detalles).

Si lo desea, puede seleccionar la opción **Volver a calcular expresiones personalizadas** para asegurarse de que todos los campos personalizados calculados en los formularios personalizados que están adjuntos a los usuarios seleccionados estén actualizados.

Para obtener información sobre cómo crear formularios personalizados, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Comentario

Escriba el comentario que desee enviar a los usuarios y al área de Actualizaciones de sus perfiles de usuario.

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Preferences</td> 
      <td> 
       <ul> 
        <li><b>Time Zone:</b> The users' time zone.</li> 
        <li><b>Locale</b>: The users' preferred locale. This affects the format of numbers and dates in the emails that come from Workfront.</li> 
        <li><b>Send work I assign to myself to my Working On tab</b>: This setting refers to a deprecated feature that has been removed from Workfront.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td>Select the email notifications which should be enabled for the new user.<p>You can select instant as well as daily digest notifications. All the daily digest notifications are delivered sometime after the same time for all the users selected. For more information, see <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configure event notifications for everyone in the system</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Access</td> 
      <td> 
       <ul> 
        <li><b>Is Active:</b> Select this field to indicate whether the users are active. Active users use a Workfront license. Deselecting the field deactivates the users.</li> 
        <li> 
        <p><b>Access Level:</b> Select the access level to assign to these users. All users selected will have the same access level.
        </p> 
        <p>When you assign an access level to users, you can assign a level equal to or less than your own access level. (For example, if your access level is Planner, you cannot assign the Administrator access level.) </p>
        <p>However, you cannot assign an access level that is lower than your own if the Workfront administrator has enabled permissions on the access level that are not also enabled in your own (via the Fine-Tune settings, as described in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>).</p> 
        <p>For more information about access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configure access to Adobe Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Layout Template</b>: Choose a layout template for the users. The layout template assigned to the users will take precedence over any layout template assigned to their Home Group, Home Team or primary job role. For more information about the assignment priority of layout template, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> 
        <p><b>NOTE</b>:  The list of layout templates you have available in this field depends on your access:
          <ul>
           <li>As a Workfront administrator, you can see all system-level and group-level layout templates.</li>
           <li>As a group administrator, you can see system-level layout templates, as well as those associated with the groups that you manage.</li>
           <li><p>As a user with a Planner license and access to edit users, you can see only system-level layout templates. </p>
           <p>For information about group-level layout templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organization</td> 
      <td> 
       <ul> 
        <li><b>Company</b>: The company of the users. Users can be associated only with one company. You must create a company before you can associate it with a user. Only active companies display in the list. For information about creating companies, see Understanding and Managing Companies.</li> 
        <li><b>Home Team</b>: Specify the home team for the users. Users can only have one home team. </li> 
        <li><b>Other Teams</b>: Users can belong to multiple teams. </li> 
        <li> <p><b>Home Group:</b> Select an appropriate group to assign the users as their Home Group. This gives the user the ability to access objects that are shared with the group.</p> <p><b>NOTE</b>:  This is a required field. You cannot have users not associated with a Home Group.</p> <p>You can assign a group to users only in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li>The group is public.</li> 
         </ul> </li> 
        <li> <p><b>Other Groups</b>: Users can belong to multiple groups. You can assign a group to a user only  in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li> <p>The group is public. </p> 
          <p>For more information about public groups, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Create a group</a>.</p> 
          <p>For more information about groups, see <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Groups overview</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resource Planning</td> 
      <td> 
       <ul> 
      
      <li>
       <b>Work Time</b>: Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.

      The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work. 

      The system uses this number to calculate the availability of the user for actual, project-related work. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.

      Schedule exceptions and time off might also affect the user capacity. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      <b>TIP</b>

      Set the Work Time value to  1 to indicate that the user is available for project-related work their entire full-time equivalent.
      </li> 

      <li><b>Schedule Deactivation</b>: Check this box if you want to schedule users to be deactivated after a period of time.</li> 
       <li><b>Scheduled Deactivation Date</b>: The date after which the users become deactivated. For more information about scheduling users for deactivation, see the section <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Schedule users for deactivation</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</li> 
       <li> <p><b>Primary Role</b>: This is the primary job role that a user has in Workfront. Every task and issue that the users are assigned to is also assigned to this job role, by default. Job roles are essential in resource management. For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a></p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li>(Conditional) If you selected a <b>Primary Role</b>, the <b>Percentage of FTE Availability</b> field displays. Specify what percentage of time of the users' schedules is allocated to this job role. The default value for the Percentage of FTE Availability for the Primary Role is 100%.</li> 
       <li> <p><b>Other Roles</b>: Users can have multiple job roles in Workfront. Job roles are essential in resource management. There is no limit for how many job roles a user can fulfill. However, we recommend to not assign one user to an excessively large number of job roles, because resource management might become too complex for these users.</p> <p>For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li> <p>(Conditional) If you selected one or multiple <b>Other Roles</b>, the <b>Percentage of FTE Availability</b> field displays for each role. Specify what percentage of time of the users' schedules is allocated to each job role. The default value for the Percentage of FTE Availability for the Other Roles is 0%.</p> <p><b>NOTE</b>:  
       <ul> 
       <li>If Other Roles have a 0% FTE Availability, they do not display in the Resource Planner, unless the users are assigned to tasks in these roles.</li> 
       <li> <p>The sum of all Percentages of FTE Availability for all roles must equal 100%. Each Percentage of FTE Availability calculates the Available Hours for each role per user in the Resource Planner. The Available Hours for each role per user depends on the available time for the user.</p> <p>The available time for the user is calculated by Workfront depending on the method that has been selected by the Workfront administrator to calculate the FTE in the Resource Management Preferences.</p> <p>For more information about calculating availability for the user, see <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> <p>For more information about configuring Resource Management preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>Schedule</b>: Associate a schedule with the users. The schedule of the users calculates the timeline of the tasks the users are assigned to.</p> <p>A Workfront administrator or a group administrator must create a schedule before it can be associated with users.</p> <p>Select a system-level or a group schedule to assign it to the selected users.</p> <p>For more information about system-level and group schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> <p><b>IMPORTANT</b>: Workfront uses the schedule of a user only when the Calculate Resource Availability Using setting is set to The User's Schedule. For information about how the Calculate Resource Availability Using setting affects which schedule is used for Resource Management, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       <li> <p><b>Timesheet Profile</b>: Associate a Timesheet Profile with the users. This ensures that timesheets generate automatically for the users.</p> 
       <p><b>NOTE</b>:  
       <ul> 
       <li>The list of timesheet profiles you have available in this field depends on your access:
       <ul>
       <li>As a Workfront administrator, you can see all system-level and group-level timesheet profiles.</li>
       <li><p>As a group administrator, you can see system-level timesheet profiles, as well as those associated with the groups that you manage.</p></li>
       <li><p>As a user with a Planner license and access to edit users, you can see only system-level timesheet profiles.</p></li>
       </ul></li> 
       <li>If you are a group administrator, all of the users you are editing must be members of a group that you administer.</li> 
       </ul> </p> </li> 
       <li><b>Default Hour Type</b>: Select the default hour type for the users. This is the hour type that is used by default when the users log time.</li> 
       <li> <p><b>Available Hour Types</b>: Select the hour types that should be available to the user. These hour types are visible everywhere in Workfront where the users can log time. A user can only see the hour types that are enabled at the project level as well as the user level.</p> 
       <p>For more information about what hour types are available to users, see <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Define hour types and availability</a>.</p> 
       </li> 
       <li> <b>FTE</b>: This is the Full Time Equivalent of the user. Workfront uses this number to calculate the availability of the user based on the Default Schedule only when the Resource Management Preferences at the system level are set to The Default Schedule. 

      <p>The FTE indicates the amount of time that the user can spend at work. This includes overhead, as well as time spent on project work. For example, time that is spent in meetings, or training is also included in the FTE.</p> 

      The FTE must be a decimal number up to 1, and it cannot be 0. For example, if the FTE value is 0.5 and the Default Schedule in Workfront is 40 hours, the user is available for 20 hours a week. 

      The field's default is 1.

      Schedule exceptions, time off might, and the value of Work Time may affect the availability of the user. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area.

      If the Resource Management Preferences at the system level are set to The User's Schedule, the value you specify here is ignored and the user is considered to be available according to what is specified in their schedule. 

      For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.
      </li> 
       <li> <p><b>Resource Pools</b>: Associate the users with resource pools.</p> <p><b>NOTE</b>:  Only the resource pools that are common to all the users selected appear in this field. If the users selected have no shared resource pools, this field is empty. If this field is empty, the resource pools you specify here will overwrite their individual resource pools.</p> 
       <p>For more information about resource pools, see <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview </a>.</p> </li> 
       <li><b>Cost Per Hour</b>: The amount of cost per hour for the user. </li> 
       <li><b>Billing Per Hour</b>: The amount of billing per hour for the user.</li> 
       <li><b>Custom Forms</b>: Associate an existing user custom form with the users. You must create a custom form before you can associate it with a user. Only active custom forms display in the list. For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>.</li> 
       <li><b>Comment</b>: Enter a comment in the field provided. All users selected will receive an in-app notification as well as an email notification with your comment. The comment shows in the Updates tab of the users' profile.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
-->

