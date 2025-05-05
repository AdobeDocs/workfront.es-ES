---
title: Editar el perfil de un usuario
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Como administrador de Adobe Workfront, puede crear nuevos usuarios y administrar los perfiles de los existentes.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: bb6697241701160f878dc3fde2c7dd4d57ec097e
workflow-type: tm+mt
source-wordcount: '3325'
ht-degree: 94%

---

# Editar el perfil de un usuario

{{highlighted-preview}}

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Manage users individually](https://helpx.adobe.com/es/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

Como administrador de Adobe Workfront, puede crear usuarios y administrar los perfiles de los existentes. Para obtener información sobre cómo crear usuarios, consulte [Añadir usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Para obtener información acerca de los usuarios que actualizan sus propios perfiles, vea [Configurar mis opciones](/help/quicksilver/workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

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

## Editar el perfil de un usuario

{{step-1-to-users}}

1. Seleccione al usuario y luego haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png).

   Aparece el cuadro Editar usuario.

1. En el cuadro **Editar usuario**, cambie la siguiente información y haga clic en **Guardar cambios** en cualquier momento:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Información personal </td> 
      <td> 
       <ul> 
        <li><p><b>Nombre</b></p></li>
        <li><p><b>Apellido</b></p><p><b>NOTA:</b></p><p>La edición del nombre de un usuario en Workfront no edita el nombre del usuario en Adobe Admin Console.</p></li> 
        <li> <p><b>Dirección de correo electrónico:</b> la dirección de correo electrónico de un usuario también es su nombre de usuario en Workfront. Este campo distingue entre mayúsculas y minúsculas y debe ser único. Si algún usuario intenta añadir una dirección de correo electrónico no única tres veces en un intervalo de 10 minutos, aparecerá una respuesta reCAPTCHA.</p> <p> Seleccione el ajuste <b>No soy un robot</b> antes de continuar.</p><p>Si utiliza la lista de permitidos de correo electrónico e introduce un dominio de correo electrónico que no aparece en la lista, el usuario no recibirá notificaciones por correo electrónico. Para obtener más información sobre la lista de permitidos, consulte <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Configuración de la lista de permitidos de correo electrónico</a>.</p><p>Si su organización se ha migrado a Adobe Admin Console, no puede editar la dirección de correo electrónico de un usuario en Workfront. La dirección de correo electrónico del usuario se establece en Adobe Admin Console. </li> 
        <li> <p><b>Restablecer contraseña</b>: haga clic en este vínculo para restablecer la contraseña del usuario. Debe introducir su propia contraseña para poder restablecer la contraseña de otro usuario.</p> <p>Para restablecer la contraseña de otro usuario, debe ser administrador de Workfront o de grupos.</p> <p><b>NOTA</b>:  
          <ul> 
           <li> <p>Si es administrador de grupos, solo puede restablecer las contraseñas de los usuarios de los grupos para los que haya sido designado administrador. Además, el permiso de administrador de usuarios (usuarios de grupo) debe estar habilitado en su nivel de acceso:</p> <p> <img src="assets/group-admin-user.png" > </p> <p>Esta opción está desactivada de forma predeterminada. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creación o modificación de niveles de acceso personalizados</a>.</p> </li> 
           <li> <p>No puede restablecer la contraseña de un administrador de Workfront.</p> </li> 
          </ul> </p> </li> 
        <li><b>Nombre de usuario de &lt;Configuración de SSO&gt;</b>: si el administrador de Workfront ha habilitado una integración de SSO con Workfront, el nombre de usuario de SSO se mostrará en este campo. El tipo de configuración de SSO habilitada para la instancia de Workfront se puede ver en este campo. </li> 
        <li> <p> <b>Permitir solo la autenticación de &lt;configuración de SSO&gt;</b>: si el administrador de Workfront ha habilitado una integración de SSO con Workfront y ha actualizado todos los usuarios para SSO, este campo está seleccionado de forma predeterminada. El tipo de configuración de SSO habilitada para la instancia de Workfront se puede ver en este campo.</p> <p>Cuando se selecciona este campo, el usuario debe iniciar sesión en Workfront con sus credenciales de SSO. Si lo desmarca, podrán iniciar sesión en Workfront con sus credenciales de Workfront.</p> <p>Para obtener más información acerca de cómo configurar Workfront con una solución de SSO, consulte <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Información general sobre el inicio de sesión único en Adobe Workfront</a></p> <p>Para obtener más información sobre cómo actualizar usuarios para SSO, consulte <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Actualizar usuarios para el inicio de sesión único</a>.</p> 
        <p><b>NOTA</b>:</p> 
        <p> Si es administrador de grupos, puede editar los campos de &lt;Configuración de SSO&gt; solo para los usuarios de los grupos en los que haya sido designado como tal. Además, el permiso de Administrador de usuarios (usuarios de grupo) debe estar habilitado en su nivel de acceso.
        <p>Si es administrador de grupos y tiene habilitado el permiso Administrador de usuarios (todos los usuarios) en su nivel de acceso, puede editar los campos de &lt;Configuración de SSO&gt; para todos los usuarios.</p> </li> 
        <li><b>Información de trabajo:</b> información sobre el trabajo, como el título del trabajo (en el campo <b>Título</b>) y de qué área de especialización es responsable el usuario (en el campo <b>Añadir comentarios sobre</b>).</li> 
        <li><p><b>Información de contacto</b>: el número de teléfono del usuario (en los campos <b>Número de teléfono, Ext.</b> y <b>número de móvil</b>) y dirección (en los campos <b>Dirección, Ciudad, Estado, Código postal, País</b>).</p>
        <p>Si el usuario está habilitado para Unified User Management (UUM) o Adobe Identity Management System (IMS), el campo <b>País</b> de la sección Información de contacto solo acepta valores de código de país (por ejemplo, EE. UU., GB, IN).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Preferencias </td> 
      <td> 
       <ul> 
      <li> <p><b>Zona horaria:</b> especifique la zona horaria.</p> <p>Para obtener información acerca de cómo ayudar a los usuarios a colaborar en Workfront en diferentes zonas horarias, consulte <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Trabajar en diferentes zonas horarias</a>.</p> </li>

   <li><p><b>Configuración regional del correo electrónico</b>: la configuración regional de correo electrónico preferida del usuario. Esto afecta al formato de los números y de las fechas de los correos electrónicos que llegan desde Workfront a este usuario.</p>
      <p><b>NOTA:</b> Cuando su organización se encuentra en la experiencia unificada de Adobe, las preferencias de idioma del usuario se almacenan en su perfil de Adobe y no se utiliza la configuración regional del correo electrónico. Para obtener información sobre el acceso a estas preferencias, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiencia unificada de Adobe para Workfront</a>.</p></li>

   <li><b>Recibir correos electrónicos de este entorno de prueba</b>: marque esta opción si desea recibir notificaciones por correo electrónico del entorno en el que ha iniciado sesión.
      <p><b>NOTA</b></p>
      <p>Esta actualización solo está disponible en los entornos de vista previa y zona protegida. Las notificaciones por correo electrónico están habilitadas en el entorno de producción de forma predeterminada. </p>
      </li>

   </li> 
       <li><b>Enviar trabajo que me asigne a mí mismo a mi ficha Trabajando en</b>: Esta configuración hace referencia a una característica en desuso que se ha eliminado de Workfront.</li> 
       <li><b>Generar revisiones automáticamente al cargar documentos</b>: marque esta opción si quiere que los documentos que el usuario carga generen inmediatamente una revisión. </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificaciones</td> 
      <td> <p>Seleccione las notificaciones por correo electrónico que deben habilitarse para el nuevo usuario.</p> <p>Puede seleccionar notificaciones de resumen instantáneas y diarias.</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configurar notificaciones de eventos para todos los usuarios del sistema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Acceso</td> 
      <td> 
       <ul> 
      <li><b>Activo:</b> seleccione este recuadro para indicar que el usuario está activo.  Los usuarios activos utilizan una licencia de Workfront. Al borrar el cuadro, se desactiva el usuario y se impide que inicie sesión en Workfront.</li> 
       <li> <p><b>Nivel de acceso:</b> seleccione el nivel de acceso que desea asignar a este usuario.</p> 
       <p>Al asignar un nivel de acceso a un usuario, puede asignarle un nivel igual o inferior al suyo propio.</p>
       <p>Por ejemplo, si el nivel de acceso es Plan, no puede asignar el nivel de acceso Administrador. Sin embargo, no puede asignar un nivel de acceso que, de forma predeterminada, sea inferior a su propio nivel de acceso si el administrador de Workfront ha habilitado permisos no predeterminados en el nivel de acceso que no están habilitados también en su propio nivel de acceso. </p>
       <p>Por ejemplo, si tiene una licencia Plan sin acceso para eliminar tareas, no puede asignar a alguien una licencia de trabajo con acceso para eliminar tareas, aunque la licencia de trabajo sea inferior a la licencia Plan. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creación y modificación de niveles de acceso personalizados</a>. </p> 
       <p>Para obtener más información acerca de los niveles de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configurar el acceso a Adobe Workfront</a>.</p>
       <p> <b>NOTA:</b></p> 
       <p> Si su organización utiliza el nuevo modelo de acceso (Standard/Light/Contributor), no puede reasignar un usuario Standard o Light a un nivel de acceso Contributor si dicho usuario ya ha alcanzado su límite de decisiones del mes. </p><p>Para obtener más información sobre el nuevo modelo de acceso, consulte <a href="../how-access-levels-work/access-level-overview.md" class="MCXref xref">Información general sobre los nuevos niveles de acceso</a>. </p><p>Para obtener información sobre los límites de decisión, consulte <a href="/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md" class="MCXref xref">información general sobre decisiones limitadas de documentos y de la revisión para usuarios sin pago</a>.</p></li> 
       <li> <p><b>Plantilla de diseño</b>: elija una plantilla de diseño para el usuario. Esta plantilla de diseño tiene prioridad sobre cualquier plantilla de diseño asignada al grupo de inicio, al equipo de inicio o a la función principal del usuario. Para obtener más información sobre la prioridad de asignación de las plantillas de diseño, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Crear y administrar plantillas de diseño</a>.</p> <p><b>NOTA</b>:  <p>La siguiente lista describe cómo la lista de plantillas disponibles en este campo depende de su acceso:</p> 
       <ul> 
       <li>Como administrador de Workfront, puede ver todas las plantillas de diseño de nivel de sistema y de grupo.</li> 
       <li>Como administrador de grupos, puede ver la plantilla de diseño de nivel de sistema, así como las asociadas con los grupos que administra.</li> 
       <li>Como usuario con una licencia Plan y de acceso para editar usuarios, solo puede ver plantillas de diseño de nivel de sistema.</li> 
       </ul> <p>Para obtener más información acerca de las plantillas de diseño de nivel de grupo, vea <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Crear y administrar plantillas de diseño</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organización </td> 
      <td> 
       <ul> 
      <li><b>Compañía</b>: la compañía del usuario. Los usuarios solo pueden asociarse con una compañía. Debe crear una compañía antes de poder asociarla a un usuario. En la lista solo se muestran las compañías activas. Para obtener información acerca de cómo crear compañías, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Crear y editar compañías</a>.</li> 
      <li><b>Informa a:</b> si ha especificado una compañía para el usuario, también puede especificar el administrador directo del usuario en este campo. Un usuario solo puede tener un administrador. Este campo no se muestra si el usuario no está asociado primero con una compañía. </li> 
      <li><b>Informes directos:</b> si ha especificado una compañía para el usuario, también puede especificar los informes directos del usuario. Un usuario puede tener varios informes directos. Este campo no se muestra si el usuario no está asociado primero con una compañía.</li> 
      <li><b>Equipo de inicio</b>: especifique el equipo de inicio del usuario. Los usuarios solo pueden tener un equipo de inicio. El equipo de inicio es importante a la hora de asignar una plantilla de diseño o al definir el botón Trabajar en ello para las tareas y problemas asignados al usuario. </li> 
      <li><b>Otros equipos</b>: los usuarios pueden pertenecer a varios equipos. Un usuario puede ver los elementos de trabajo asignados a cualquiera de sus equipos en el área de Inicio. </li> 
      <li> <p><b>Grupo de inicio:</b> seleccione un grupo apropiado para asignar al usuario. Esto ofrece al usuario la posibilidad de acceder a los objetos compartidos con el grupo. También puede compartir plantillas de diseño con el grupo de inicio del usuario.</p> <p>Este campo es obligatorio. Todos los usuarios deben estar asociados a un grupo de inicio. Si no selecciona uno, el grupo de inicio se asignará como el grupo de inicio del nuevo usuario.</p> <p><b>NOTA</b></p> 
      <p> Puede asignar un grupo a un usuario solo si se cumple una de las siguientes condiciones:</p>
      <ul><li>es administrador de Workfront</li>
      <li>es el administrador del grupo</li>
      <li>el grupo es público.</li></ul> 
      <li> <p><b>Otros grupos</b>: los usuarios pueden pertenecer a varios grupos. Solo puede asignar un grupo a un usuario si es administrador de Workfront, si es el administrador de grupos o si el grupo es público.</p> <p><b>IMPORTANTE</b>:</p> 
      <p>Añadir un usuario a más de 100 grupos puede causar problemas de rendimiento en cualquier área de Workfront que cargue la lista de grupos.</p> <p>Para obtener más información sobre los grupos públicos, consulte <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Crear un grupo</a>.</p> <p>Para obtener más información sobre los grupos, consulte <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Información general sobre los grupos</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planificación de recursos </td> 
      <td> 
       <ul>
       <li>
       <b>Tiempo de trabajo</b>: representa el porcentaje del tiempo Equivalente a jornada completa (EJC) que el usuario está disponible para el trabajo real, sin incluir los gastos generales. El tiempo de trabajo debe ser un número decimal de hasta 1 y no puede ser 0. Por ejemplo, una disponibilidad del 20% para el trabajo real sería de 0,2.

   El valor predeterminado del campo es 1, lo que indica que un usuario emplea todo su FTE en trabajo real relacionado con el proyecto.

   El sistema utiliza este número para calcular la disponibilidad del usuario para el trabajo real relacionado con el proyecto.

   Para obtener más información sobre cómo crear programaciones en Workfront, consulte <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Crear programación</a>.

   Las excepciones de programación y los días libres también pueden afectar a la capacidad del usuario.

   Workfront calcula la disponibilidad de un usuario según las preferencias de Administración de recursos del área de Configuración. Para obtener más información, consulte <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferencias de administración de recursos</a>.

   <b>SUGERENCIA</b>

   Establezca el valor Tiempo de trabajo en 1 para indicar que el usuario está disponible para el trabajo relacionado con el proyecto en su equivalente a jornada completa
   </li> 
      <li> <b>Programar desactivación</b>: marque este recuadro si desea programar la desactivación de este usuario en una fecha y a una hora determinadas. </li> 
       <li><b>Fecha de desactivación programada</b>: fecha y hora en que se desactiva el usuario. Para obtener información sobre cómo programar usuarios para la desactivación, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Programar usuarios para la desactivación</a> en <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desactivar o reactivar un usuario</a>.</li> 
       <li> <p><b>Función principal</b>: la función principal que el usuario puede cumplir en Workfront. Todas las tareas y problemas que se le asignan al usuario también se asignan a esta función. Las funciones de trabajo son esenciales en la administración de recursos. Solo puede actualizar este campo si dispone de una licencia de planificación con acceso de usuario administrativo o si es administrador de Workfront. Para obtener más información sobre la configuración de usuarios con acceso de usuario administrativo, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a usuarios</a>.</p> <p>En la lista solo se muestran las funciones activas. </p> </li> 
       <li>Si seleccionó una <b>Función principal</b>, se muestra el campo <b>Porcentaje de disponibilidad de FTE</b>. Especifique qué porcentaje de tiempo de la programación del usuario se asigna a esta función. El valor predeterminado para el porcentaje de disponibilidad de FTE para la función principal es 100%. </li> 
       <li> <p><b>Otras funciones</b>: un usuario puede tener varias funciones en Workfront. Las funciones de trabajo son esenciales en la administración de recursos. No hay límite en cuanto a las funciones que puede desempeñar un usuario. Sin embargo, se recomienda no asignar un usuario a un número excesivamente elevado de funciones del puesto, ya que la administración de recursos podría resultar demasiado compleja para estos usuarios.<p>En la lista solo se muestran las funciones activas. Para obtener más información sobre las funciones, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar funciones</a>.</p> <p>Solo puede actualizar este campo si dispone de una licencia de planificación con acceso de usuario administrativo o si es administrador de Workfront. <br>Para obtener más información sobre cómo configurar usuarios con acceso de usuario administrativo, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a usuarios</a>.</p> </li> 
       <li> <p>(Condicional) Si ha seleccionado una o varias <b>Otras funciones</b>, se muestra el campo <b>Porcentaje de disponibilidad de FTE</b> para cada función. Especifique qué porcentaje de tiempo de la programación del usuario se asigna a cada función. El valor predeterminado para el porcentaje de disponibilidad de FTE para las otras funciones es 0 %.</p> <p><b>NOTA</b>: Si otras funciones tienen una disponibilidad de FTE del 0 %, no se mostrarán en el Planificador de recursos, a menos que los usuarios estén asignados a tareas en estas funciones.</p> <p> <img alt="user_settings_roles_and_dte_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>NOTA</b>: <p>La suma de todos los <b>porcentajes de disponibilidad de FTE</b> para todas las funciones debe ser igual a 100 %. Cada porcentaje de disponibilidad de FTE calcula las horas disponibles para cada función por usuario en el Planificador de recursos. Las horas disponibles para cada función por usuario dependen del tiempo disponible para el usuario.</p> <p>Workfront calcula el tiempo disponible para el usuario según el método que haya seleccionado el administrador de Workfront para calcular el valor de FTE en las Preferencias de administración de recursos.</p> <p>Para obtener información acerca de cómo calcular la disponibilidad del usuario, vea <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Información general sobre el cálculo de horas y FTE para usuarios y roles en el Planificador de recursos</a>.</p> <p>Para obtener información acerca de cómo configurar las preferencias de Administración de recursos, vea <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurar las preferencias de Administración de recursos</a>.</p> </p>
       <span class="preview"><p>(Opcional) Las asignaciones de funciones efectivas por fecha se utilizan en los cálculos financieros si la función del usuario cambia durante un proyecto.</p><p>Haga clic en <b>Definir funciones por fecha</b>, seleccione la <b>Función principal</b> y <b>Otras funciones</b> e introduzca el porcentaje de asignación para cada función. Las funciones podrían ser las mismas que las funciones existentes (con porcentajes diferentes) o que las nuevas funciones. Seleccione la <b>fecha de inicio</b> cuando estas funciones se vuelvan activas. Esta puede ser una fecha futura. Cuando se activen las funciones más recientes, puede hacer clic en <b>Mostrar funciones anteriores</b> para ver las funciones anteriores e inactivas.</p> </li></span>
       <li> <p><b>Horario</b>: asocie un horario al usuario. La programación del usuario calcula la cronología de las tareas que se le asignan.</p> <p>Debe crear una programación para poder asociarla a un usuario. Para obtener más información acerca de cómo crear programaciones, vea <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Crear una programación</a>.</p> <p><b>NOTA</b>: Se recomienda que la programación que asocia con el usuario coincida con la zona horaria del usuario.</p> </li> 
       <li> <p><b>Perfil de plantilla de horas</b>: asocie un perfil de plantilla de horas con el usuario para garantizar que las plantillas de horas se generen automáticamente para el usuario.</p> <p><b>NOTA</b>: La lista de perfiles que tiene disponibles en este campo depende de su acceso:
       <ul>
       <li>Como administrador de Workfront, puede ver todos los perfiles de plantilla de horas a nivel del sistema y de grupo.</li>
       <li>Como administrador de grupos, puede ver perfiles de plantillas de horas de nivel del sistema, así como los asociados con los grupos que administra.</li>
       <li>Como usuario con una licencia de planificación y acceso para editar usuarios, solo puede ver perfiles de plantilla de horas en el sistema. Para obtener más información sobre los perfiles de plantilla de horas de nivel de grupo, consulte <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">Crear, editar y asignar perfiles de plantilla de horas</a>.</li>
      </ul></p> </li> 
       <li><b>Tipo de hora predeterminado</b>: seleccione el tipo de hora predeterminado para el usuario. Es el tipo de hora que se utiliza de forma predeterminada cuando el usuario registra la hora.</li> 
       <li><b>Tipos de horas disponibles</b>: seleccione los tipos de horas que deben estar disponibles para el usuario. Estos tipos de horas son visibles en todas partes en Workfront donde el usuario puede registrar el tiempo. Un usuario solo puede ver los tipos de horas que están habilitados en el nivel de proyecto y en el nivel de usuario. Para obtener más información acerca de los tipos de horas que están disponibles para los usuarios, consulte <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Definir tipos de horas y disponibilidad</a>.</li> 
       <li><b>Registrar tiempo en:</b> seleccione si el usuario debe registrar tiempo en elementos de trabajo en horas o días. Para obtener más información, consulte <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">Configurar si el tiempo se registra en horas o días</a>.</li>

   <li> <b>EJC</b>: es el Equivalente a jornada completa del usuario. Workfront utiliza este número para calcular la disponibilidad del usuario según el horario predeterminado, solo cuando las Preferencias de administración de recursos del sistema están definidas en El horario predeterminado.

   <p>El valor de FTE indica la cantidad de tiempo que el usuario puede pasar en el trabajo. Esto incluye la sobrecarga, así como el tiempo empleado en el trabajo del proyecto. Por ejemplo, el tiempo empleado en reuniones o en formación también se incluye en el EJC.</p>

   El valor de FTE debe ser un número decimal de hasta 1 y no puede ser 0. Por ejemplo, si el valor de EJC es 0,5 y el horario predeterminado en Workfront son 40 horas, el usuario estará disponible durante 20 horas a la semana.

   El valor predeterminado del campo es 1.

   Las excepciones de horario, los días libres y el valor del Tiempo de trabajo pueden afectar a la disponibilidad del usuario.

   Workfront calcula la disponibilidad de un usuario según las preferencias de Administración de recursos del área de Configuración.

   Si las Preferencias de administración de recursos en el nivel del sistema se establecen en El horario del usuario, el valor especificado aquí se ignorará y el usuario se considerará disponible según lo especificado en su horario.

   Para obtener más información, consulte <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar las preferencias de administración de recursos</a>.

   Para obtener más información acerca de cómo crear programaciones en Workfront, consulte <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Crear programación</a>.
   </li>

   <li><b>Conjuntos de recursos</b>: asocie el usuario con los conjuntos de recursos. Para obtener más información, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Asociar conjuntos de recursos a los usuarios</a>.</li>

   <li><b>Tarifa de coste</b>: cantidad de coste por hora para el usuario.
      <p>Para ver las tarifas de coste efectivas por fecha, haga clic en <strong>Añadir tarifa</strong>. Introduzca el valor de la tarifa de coste para el período de tiempo y asigne una fecha de inicio y una fecha de finalización según sea necesario. La tarifa de coste 1 no tendrá fecha de inicio y la última tasa de coste no tendrá fecha de finalización.</p><p>Algunas fechas se añaden automáticamente. Por ejemplo, si la tarifa de coste 1 no tiene una fecha de finalización y añade la tarifa de coste 2 con una fecha de inicio del 1 de mayo de 2023, se añade la fecha de finalización del 30 de abril de 2023 a la tarifa de coste 1 para que no existan brechas.</p></li>

   <li><b>Tarifa de facturación</b>: la cantidad de facturación por hora para el usuario.
      <p>Para ver las tarifas de facturación vigentes por fecha, haga clic en <strong>Añadir tarifa</strong>. Introduzca el valor de la tarifa de facturación para el período de tiempo y asigne una Fecha de inicio y una Fecha de finalización según sea necesario. La tarifa de facturación 1 no tendrá una fecha de inicio y la última tarifa de facturación no tendrá una fecha de finalización.</p> <p>Algunas fechas se añaden automáticamente. Por ejemplo, si la tarifa de facturación 1 no tiene una fecha de finalización y añade una segunda con una fecha de inicio del 1 de mayo de 2023, se añade la fecha de finalización del 30 de abril de 2023 a la tarifa de facturación 1 para que no existan brechas.</p><p> <img alt="Costes de usuario y tarifas de facturación" src="assets/edit-user-cost-billing-rate-2.png"> </p></li>

   </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formularios personalizados</td> 
      <td><p>Asocie un formulario personalizado de usuario existente con este usuario. Debe crear un formulario personalizado para poder asociarlo a un usuario. En la lista solo se muestran los formularios personalizados activos. Los campos que no tiene acceso para editar no se muestran en un formulario personalizado individual.</p> <p><strong>Nota:</strong> Las características de formulario personalizadas avanzadas, como los campos de búsqueda externa y los campos nativos de Workfront, solo están disponibles cuando abre el registro de usuario en la página de detalles, no en el cuadro de diálogo Editar usuario. (En la lista de usuarios, haga clic en el nombre del usuario para abrir los detalles).</p> <p>Para obtener información sobre cómo crear formularios personalizados, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md" class="MCXref xref">Crear un formulario personalizado</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Comentario</td> 
      <td>Escriba el comentario que desee enviar a los usuarios y al área de Actualizaciones de sus perfiles de usuario.</td> 
     </tr> 
    </tbody> 
   </table>
