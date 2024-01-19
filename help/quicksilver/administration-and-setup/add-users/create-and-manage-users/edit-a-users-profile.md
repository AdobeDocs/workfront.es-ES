---
title: Edición del perfil de un usuario
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Como administrador de Adobe Workfront, puede crear nuevos usuarios y administrar los perfiles de los existentes.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '3381'
ht-degree: 0%

---

# Edición del perfil de un usuario

{{highlighted-preview}}

>[!IMPORTANT]
>
>El procedimiento descrito en esta página se aplica sólo a las organizaciones que aún no se han incorporado al Admin Console. Si su organización se ha incorporado a Adobe Admin Console, debe realizar esta acción a través de Adobe Admin Console.
>
>Para obtener instrucciones sobre cómo editar el perfil de un usuario en Adobe Admin Console, consulte la sección &quot;Editar detalles del usuario&quot; en el artículo [Administrar usuarios individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) o póngase en contacto con su administrador de Adobe Admin Console.
>
>Para obtener una lista de procedimientos que difieren en función de si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en la plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador de Adobe Workfront, puede crear usuarios y administrar los perfiles de los existentes. Para obtener información sobre la creación de usuarios, consulte [Adición de usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Nuevo: estándar</p>
   O
   <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe tener uno de los siguientes:</p> 
    <ul> 
     <li> <p>El nivel de acceso del administrador del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>. </p> </li> 
     <li> <p>El <b>Usuarios</b> objeto en su nivel de acceso configurado para <b>Editar</b> acceso, con <b>Crear</b> y al menos uno de los dos siguientes <b>Administrador de usuarios</b> opciones activadas en <b>Ajuste la configuración</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
     <ul><li> Administrador de usuarios (todos los usuarios)</li>
     <li>Administrador de usuarios (usuarios de grupo)</li></ul>
     <p>If  <b>Administrador de usuarios (usuarios de grupo)</b> está habilitada, debe ser administrador de grupo de un grupo en el que el usuario sea miembro para poder editar al usuario.</p> 
     <p>Para obtener más información sobre <b>Usuarios</b> configuración en un nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concesión de acceso a los usuarios</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table> 
*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Edición de un perfil de usuario

{{step-1-to-users}}

1. Seleccione el usuario y haga clic en el botón **Editar** icono ![](assets/edit-icon.png).

   Se muestra el cuadro Editar usuario.

1. En el **Editar usuario** , cambie la siguiente información y haga clic en **Guardar cambios** en cualquier momento:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Información personal </td> 
      <td> 
       <ul> 
        <li><p><b>Nombre</b></p></li>
        <li><p><b>Apellido</b></p></li> 
        <li> <p><b>Correo electrónico:</b> La dirección de correo electrónico de un usuario es también su nombre de usuario en Workfront. Este campo distingue entre mayúsculas y minúsculas y debe ser único. Si algún usuario intenta agregar una dirección de correo electrónico no única 3 veces en un intervalo de 10 minutos, aparecerá una respuesta reCAPTCHA.</p> <p> Seleccione el <b>No soy un robot</b> configuración antes de continuar.</p><p>Si utiliza la lista de permitidos de correo electrónico e introduce un dominio de correo electrónico que no está en la lista, el usuario no recibirá notificaciones por correo electrónico. Para obtener más información sobre la lista de permitidos, consulte <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Configuración de la lista de permitidos de correo electrónico</a>.</p> </li> 
        <li> <p><b>Restablecer contraseña</b>: haga clic en este vínculo para restablecer la contraseña del usuario. Debe escribir su propia contraseña para poder restablecer la contraseña de otro usuario.</p> <p>Para restablecer la contraseña de otro usuario, debe ser administrador de Workfront o de un grupo.</p> <p><b>NOTA</b>:  
          <ul> 
           <li> <p>Si es administrador de un grupo, sólo puede restablecer las contraseñas de los usuarios de los grupos en los que esté designado como administrador. Además, el permiso Administración de usuarios (usuarios de grupo) debe estar habilitado en su nivel de acceso:</p> <p> <img src="assets/group-admin-user.png" > </p> <p>Esta configuración está deshabilitada de forma predeterminada. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </li> 
           <li> <p>No puede restablecer la contraseña de un administrador de Workfront.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;sso configuration=""&gt; Nombre de usuario</b>: Si el administrador de Workfront ha habilitado una integración de SSO con Workfront, en este campo se muestra el nombre de usuario de SSO. El tipo de configuración de SSO habilitada para la instancia de Workfront se puede ver en este campo. </li> 
        <li> <p><b>SolamentePermitir &lt;sso configuration=""&gt; Autenticación</b>: Si el administrador de Workfront ha habilitado una integración de SSO con Workfront y ha actualizado todos los usuarios para SSO, este campo está seleccionado de forma predeterminada. El tipo de configuración de SSO habilitada para la instancia de Workfront se puede ver en este campo.</p> <p>Cuando se selecciona este campo, el usuario debe iniciar sesión en Workfront con sus credenciales de SSO. Si lo desmarca, podrán iniciar sesión en Workfront con sus credenciales de Workfront.</p> <p>Para obtener más información sobre la configuración de Workfront con una solución de SSO, consulte <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Información general sobre el inicio de sesión único en Adobe Workfront</a></p> <p>Para obtener más información sobre la actualización de usuarios para SSO, consulte <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Actualizar usuarios para el inicio de sesión único</a>.</p> 
        <p><b>NOTA</b>:</p> 
        <p> Si es administrador de un grupo, puede editar la variable &lt;sso configuration=""&gt; solo para los usuarios de los grupos en los que esté designado como tal. Además, el permiso de Administración de usuarios (usuarios de grupo) debe estar habilitado en su nivel de acceso.
        <p>Si es administrador de un grupo y tiene habilitado el permiso Administración de usuarios (todos los usuarios) en su nivel de acceso, puede editar el &lt;sso configuration=""&gt; campos para todos los usuarios.</p> </li> 
        <li><b>Información de trabajo:</b> Información sobre el trabajo, como el cargo (en el <b>Título</b> ) y de qué área de conocimiento es responsable el usuario (en el <b>Hablar conmigo sobre</b> field).</li> 
        <li><p><b>Información de contacto</b>: el número de teléfono del usuario (en el <b>Número de teléfono, Ext.</b>, y <b>Número de móvil</b> campos) y dirección (en el <b>Dirección, Ciudad, Estado, Código postal, País</b> campos ).</p>
        <p>Si el usuario está habilitado para Unified User Management (UUM) o Adobe Identity Management System (IMS), la variable <b>País</b> El campo de la sección Información de contacto solo acepta valores de código de país (por ejemplo, EE. UU., GB, IN).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Preferencias </td> 
      <td> 
       <ul> 
      <li> <p><b>Zona horaria:</b> Zona horaria del usuario.</p> <p>Para obtener información sobre cómo ayudar a los usuarios a colaborar en Workfront en diferentes zonas horarias, consulte <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Trabajo entre zonas horarias</a>.</p> </li> 
       <li><b>Configuración regional de correo electrónico</b>: la configuración regional de correo electrónico preferida del usuario. Esto afecta al formato de los números y las fechas de los correos electrónicos que llegan desde Workfront a este usuario.</li>

   <li><b>Recibir correos electrónicos de este entorno de prueba</b>: marque esta opción si desea recibir notificaciones por correo electrónico del entorno en el que ha iniciado sesión actualmente.
      <p><b>NOTA</b></p>
      <p>Esta opción solo está disponible en los entornos Vista previa y Zona protegida. Las notificaciones por correo electrónico están habilitadas en el entorno de producción de forma predeterminada. </p>
      </li>

   <li><b>Mostrar porcentaje completado al actualizar el estado</b>: marque esta opción si desea mostrar una barra de porcentaje completado dentro del área de Actualización de las tareas de este usuario, al utilizar la experiencia de comentarios heredada. Para obtener más información, consulte <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md">Nueva experiencia de comentarios</a>.</li> 
       <li><b>Enviar trabajo que me asigne a mí mismo a mi ficha Trabajando en</b>: marque esta opción si desea que todo lo que el usuario se asigna a sí mismo aparezca directamente en la lista Trabajando en del área de Inicio. El valor predeterminado es enumerar todo lo asignado a un usuario en sus listas Listo para comenzar o No listo en el área de Inicio.</li> 
       <li><b>Generar automáticamente revisiones al cargar documentos</b>: Marque esta opción si desea que los documentos que carga el usuario generen una prueba inmediatamente. </li>
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
      <li><b>Está activo:</b> Seleccione esta casilla para indicar que el usuario está activo. Los usuarios activos utilizan una licencia de Workfront. Al desactivar la casilla, se desactiva el usuario y se impide que inicie sesión en Workfront.</li> 
       <li> <p><b>Nivel de acceso:</b> Seleccione el nivel de acceso que desea asignar a este usuario.</p> 
       <p>Al asignar un nivel de acceso a un usuario, puede asignar un nivel igual o inferior al suyo propio.</p>
       <p>Por ejemplo, si el nivel de acceso es Plan, no puede asignar el nivel de acceso Administrador. Sin embargo, no puede asignar un nivel de acceso que, de forma predeterminada, sea inferior a su propio nivel de acceso si el administrador de Workfront ha habilitado permisos no predeterminados en el nivel de acceso que no están habilitados también en su propio nivel de acceso. </p>
       <p>Por ejemplo, si tiene una licencia de planificación sin acceso para eliminar tareas, no puede asignar a alguien una licencia de trabajo con acceso para eliminar tareas, aunque la licencia de trabajo sea inferior a la licencia de planificación. Para obtener más información, consulte  <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>. </p> 
       <p>Para obtener más información sobre los niveles de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configuración del acceso a Adobe Workfront</a>.</p>
       <p> <b>NOTA:</b></p> 
       <p> Si su organización utiliza el nuevo modelo de acceso (Estándar/Ligero/Colaborador), no puede reasignar un usuario Estándar o Ligero a un nivel de acceso Colaborador si ese usuario ya ha alcanzado su límite de decisiones en el mes. </p><p>Para obtener más información sobre el nuevo modelo de acceso, consulte <a href="../how-access-levels-work/access-level-overview.md" class="MCXref xref">Información general sobre nuevos niveles de acceso</a>. </p><p>Para obtener información sobre los límites de decisión, consulte <a href="/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md" class="MCXref xref">Información general sobre la decisión limitada de documentos y pruebas para usuarios no pagados</a>.</p></li> 
       <li> <p><b>Plantilla de diseño</b>: elija una plantilla de diseño para el usuario. Esta plantilla de diseño tiene prioridad sobre cualquier plantilla de diseño asignada al grupo de inicio, al equipo de inicio o a la función principal del usuario. Para obtener más información sobre la prioridad de asignación de las plantillas de diseño, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Creación y administración de plantillas de diseño</a>.</p> <p><b>NOTA</b>:  <p>La siguiente lista describe cómo la lista de plantillas disponibles en este campo depende de su acceso:</p> 
       <ul> 
       <li>Como administrador de Workfront, puede ver todas las plantillas de diseño de nivel de sistema y de grupo.</li> 
       <li>Como administrador de grupos, puede ver la plantilla de diseño de nivel de sistema, así como las asociadas a los grupos que administra.</li> 
       <li>Como usuario con una licencia de planificación y acceso para editar usuarios, solo puede ver plantillas de diseño de nivel de sistema.</li> 
       </ul> <p>Para obtener más información sobre las plantillas de diseño de nivel de grupo, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Creación y administración de plantillas de diseño</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organización </td> 
      <td> 
       <ul> 
      <li><b>Compañía</b>: la compañía del usuario. Los usuarios solo pueden asociarse con una compañía. Debe crear una compañía antes de poder asociarla a un usuario. En la lista solo se muestran las empresas activas. Para obtener información sobre la creación de empresas, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Crear y editar compañías</a>.</li> 
      <li><b>Informes para:</b> Si ha especificado una compañía para el usuario, también puede especificar el administrador directo del usuario en este campo. Un usuario solo puede tener un responsable. Este campo no se muestra si el usuario no está asociado primero con una empresa. </li> 
      <li><b>Subordinados directos:</b> Si ha especificado una compañía para el usuario, también puede especificar los informes directos del usuario. Un usuario puede tener varios informes directos. Este campo no se muestra si el usuario no está asociado primero con una empresa.</li> 
      <li><b>Equipo de inicio</b>: especifique el equipo de inicio del usuario. Los usuarios solo pueden tener un equipo de inicio. El equipo de inicio es importante a la hora de asignar una plantilla de diseño o al definir el botón Trabajar en ello para las tareas y problemas asignados al usuario. </li> 
      <li><b>Otros equipos</b>: los usuarios pueden pertenecer a varios equipos. Un usuario puede ver los elementos de trabajo asignados a cualquiera de sus equipos en el área de Inicio. </li> 
      <li> <p><b>Grupo de inicio:</b> Seleccione un grupo apropiado para asignar al usuario. Esto ofrece al usuario la posibilidad de acceder a los objetos compartidos con el grupo. También puede compartir plantillas de diseño con el grupo de inicio del usuario.</p> <p>Este campo es obligatorio. Todos los usuarios deben estar asociados a un grupo de inicio. Si no selecciona uno, el grupo se asigna como el grupo de inicio del nuevo usuario.</p> <p><b>NOTA</b>:</p> 
      <p> Puede asignar un grupo a un usuario solo si se cumple una de las siguientes condiciones:</p>
      <ul><li>usted es administrador de Workfront</li>
      <li>usted es el administrador del grupo</li>
      <li>el grupo es público.</li></ul> 
      <li> <p><b>Otros grupos</b>: los usuarios pueden pertenecer a varios grupos. Solo puede asignar un grupo a un usuario si es administrador de Workfront, si es el administrador del grupo o si el grupo es público.</p> <p><b>IMPORTANTE</b>:</p> 
      <p>Añadir un usuario a más de 100 grupos puede causar problemas de rendimiento en cualquier área de Workfront que cargue la lista de grupos.</p> <p>Para obtener más información sobre los grupos públicos, consulte <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Crear un grupo</a>.</p> <p>Para obtener más información sobre los grupos, consulte <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Información general de grupos</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planificación de recursos </td> 
      <td> 
       <ul>
       <li>
       <b>Tiempo de trabajo</b>: Representa el porcentaje del tiempo equivalente a tiempo completo (FTE) que el usuario está disponible para el trabajo real, sin incluir los gastos generales. El tiempo de trabajo debe ser un número decimal de hasta 1 y no puede ser 0. Por ejemplo, una disponibilidad del 20% para el trabajo real sería de 0,2.

   El valor predeterminado del campo es 1, lo que indica que un usuario emplea todo su valor de FTE en trabajo real relacionado con el proyecto.

   El sistema utiliza este número para calcular la disponibilidad del usuario para el trabajo real relacionado con el proyecto.

   Para obtener más información sobre la creación de programaciones en Workfront, consulte <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Creación de una programación</a>.

   Las excepciones de horario y los días libres también pueden afectar a la capacidad del usuario.

   Workfront calcula la disponibilidad de un usuario según las preferencias de Administración de recursos del área de Configuración. Para obtener más información, consulte <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferencias de administración de recursos</a>.

   <b>SUGERENCIA</b>

   Establezca el valor Tiempo de trabajo en 1 para indicar que el usuario está disponible para el trabajo relacionado con el proyecto en su equivalente a tiempo completo.
   </li> 
      <li> <b>Programar desactivación</b>: Marque esta casilla si desea programar la desactivación de este usuario en una fecha y a una hora determinadas. </li> 
       <li><b>Fecha programada de desactivación</b>: la fecha y la hora en que se desactiva el usuario. Para obtener información acerca de cómo programar usuarios para su desactivación, consulte la <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Programar usuarios para su desactivación</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desactivar o reactivar un usuario</a>.</li> 
       <li> <p><b>Rol principal</b>: Esta es la función principal que el usuario puede desempeñar en Workfront. Todas las tareas y problemas que se le asignan al usuario también se asignan a este rol. Las funciones del puesto son esenciales en la gestión de recursos. Solo puede actualizar este campo si dispone de una licencia de planificación con acceso de usuario administrativo o si es administrador de Workfront. Para obtener más información sobre la configuración de usuarios con acceso de usuario administrativo, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concesión de acceso a los usuarios</a>.</p> <p>En la lista solo se muestran los roles activos. </p> </li> 
       <li>Si seleccionó una <b>Rol principal</b>, el <b>Porcentaje de disponibilidad de FTE</b> se muestra el campo. Especifique qué porcentaje de tiempo de la programación del usuario se asigna a este rol. El valor predeterminado para el porcentaje de disponibilidad de FTE para el rol principal es 100%. </li> 
       <li> <p><b>Otros roles</b>: un usuario puede tener varios roles en Workfront. Las funciones del puesto son esenciales en la gestión de recursos. No hay límite en cuanto a las funciones que puede desempeñar un usuario. Sin embargo, se recomienda no asignar un usuario a un número excesivamente elevado de funciones del puesto, ya que la administración de recursos podría resultar demasiado compleja para estos usuarios.<p>En la lista solo se muestran los roles activos. Para obtener más información sobre las funciones, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar roles</a>.</p> <p>Solo puede actualizar este campo si dispone de una licencia de planificación con acceso de usuario administrativo o si es administrador de Workfront. <br>Para obtener más información sobre la configuración de usuarios con acceso de usuario administrativo, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concesión de acceso a los usuarios</a>.</p> </li> 
       <li> <p>(Condicional) Si ha seleccionado uno o varios <b>Otros roles</b>, el <b>Porcentaje de disponibilidad de FTE</b> El campo se muestra para cada rol. Especifique qué porcentaje de tiempo de la programación del usuario se asigna a cada rol. El valor predeterminado para el porcentaje de disponibilidad de FTE para los otros roles es 0%.</p> <p><b>NOTA</b>: si otros roles tienen una disponibilidad de FTE del 0%, no se muestran en el Planificador de recursos, a menos que los usuarios estén asignados a tareas de estos roles.</p> <p> <img alt="user_settings_roles_and_date_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>NOTA</b>: <p>La suma de todos <b>Porcentajes de disponibilidad de FTE</b> para todos los roles debe ser igual a 100%. Cada porcentaje de disponibilidad de FTE calcula las horas disponibles para cada rol por usuario en el Planificador de recursos. Las horas disponibles para cada rol por usuario dependen del tiempo disponible para el usuario.</p> <p>Workfront calcula el tiempo disponible para el usuario según el método que haya seleccionado el administrador de Workfront para calcular el valor de FTE en las Preferencias de administración de recursos.</p> <p>Para obtener información sobre el cálculo de la disponibilidad del usuario, consulte <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Información general sobre el cálculo de horas y FTE para usuarios y roles en el Planificador de recursos</a>.</p> <p>Para obtener información sobre cómo configurar las preferencias de Administración de recursos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurar preferencias de administración de recursos</a>.</p> </p>
       <span class="preview"><p>(Opcional) Las asignaciones de funciones en vigor por fecha se utilizan en los cálculos financieros si la función del usuario cambia durante un proyecto.</p><p>Clic <b>Definir funciones por fecha</b>, seleccione la <b>Rol principal</b> y <b>Otros roles</b>e introduzca el porcentaje de asignación para cada rol. Las funciones podrían ser las mismas que las funciones existentes (con porcentajes diferentes) o que las nuevas funciones. Seleccione el <b>Fecha de inicio</b> cuando estas funciones se activen. Esta puede ser una fecha futura. Cuando se activen las funciones más recientes, puede hacer clic en <b>Mostrar funciones anteriores</b> para ver las funciones inactivas anteriores.</p> </li></span>
       <li> <p><b>Programación</b>: asocie una programación al usuario. La programación del usuario calcula la cronología de las tareas que se le asignan.</p> <p>Debe crear una programación para poder asociarla a un usuario. Para obtener más información sobre la creación de programaciones, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Creación de una programación</a>.</p> <p><b>NOTA</b>: Recomendamos que la programación que asocie con el usuario coincida con la zona horaria del usuario.</p> </li> 
       <li> <p><b>Perfil de hoja de horas</b>: asocie un perfil de hoja de horas al usuario para garantizar que las hojas de horas se generen automáticamente para el usuario.</p> <p><b>NOTA</b>: La lista de perfiles disponibles en este campo depende de su acceso:
       <ul>
       <li>Como administrador de Workfront, puede ver todos los perfiles de hojas de horas a nivel del sistema y de grupo.</li>
       <li>Como administrador de grupos, puede ver perfiles de hojas de horas de nivel de sistema, así como los asociados a los grupos que administra.</li>
       <li>Como usuario con una licencia de planificación y acceso para editar usuarios, solo puede ver perfiles de hojas de horas en el sistema. Para obtener más información sobre los perfiles de hojas de horas de nivel de grupo, consulte <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">Crear, editar y asignar perfiles de hojas de horas</a>.</li>
      </ul></p> </li> 
       <li><b>Tipo de hora predeterminado</b>: seleccione el tipo de hora predeterminado para el usuario. Es el tipo de hora que se utiliza de forma predeterminada cuando el usuario registra la hora.</li> 
       <li><b>Tipos de horas disponibles</b>: seleccione los tipos de horas que deben estar disponibles para el usuario. Estos tipos de horas son visibles en todas partes en Workfront donde el usuario puede registrar el tiempo. Un usuario solo puede ver los tipos de horas que están habilitados en el nivel de proyecto y en el nivel de usuario. Para obtener más información sobre los tipos de horas disponibles para los usuarios, consulte <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Definir tipos de horas y disponibilidad para hojas de horas</a>.</li> 
       <li><b>Registrar tiempo en:</b> Seleccione si el usuario debe registrar el tiempo de los elementos de trabajo en horas o días. Para obtener más información, consulte <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">Configurar si se registran horas y días</a>.</li>

   <li> <b>ETC</b>: es el equivalente a tiempo completo del usuario. Workfront utiliza este número para calcular la disponibilidad del usuario según el horario predeterminado sólo cuando las Preferencias de Gestión de Recursos del sistema están definidas en El Horario por Defecto.

   <p>El valor de FTE indica la cantidad de tiempo que el usuario puede pasar en el trabajo. Esto incluye los gastos generales, así como el tiempo empleado en el trabajo del proyecto. Por ejemplo, el tiempo empleado en reuniones o en formación también se incluye en el ETC.</p>

   El valor de FTE debe ser un número decimal de hasta 1 y no puede ser 0. Por ejemplo, si el valor de FTE es 0,5 y el horario predeterminado en Workfront es 40 horas, el usuario estará disponible durante 20 horas a la semana.

   El valor predeterminado del campo es 1.

   Las excepciones de horario, el tiempo libre y el valor del Tiempo de trabajo pueden afectar a la disponibilidad del usuario.

   Workfront calcula la disponibilidad de un usuario según las preferencias de Administración de recursos del área de Configuración.

   Si las Preferencias de administración de recursos en el nivel del sistema se establecen en El horario del usuario, el valor especificado aquí se ignorará y el usuario se considerará disponible según lo especificado en su horario.

   Para obtener más información, consulte <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferencias de administración de recursos</a>.

   Para obtener más información sobre la creación de programaciones en Workfront, consulte <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Creación de una programación</a>.
   </li>

   <li><b>Conjuntos de recursos</b>: asocie el usuario a los conjuntos de recursos. Para obtener más información, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Asociar conjuntos de recursos a los usuarios </a>.</li>

   <li><b>Tasa de costo</b>: Cantidad de coste por hora para el usuario.
      <p>Para tasas de costo efectivas por fecha, haga clic en <strong>Agregar tarifa</strong>. Introduzca el valor de la tasa de coste para el período de tiempo y asigne una fecha de inicio y una fecha de finalización según sea necesario. La tarifa de costo 1 no tendrá fecha de inicio y la última tarifa de costo no tendrá fecha de finalización.</p><p>Algunas fechas se añaden automáticamente. Por ejemplo, si la Tasa de Coste 1 no tiene una fecha de finalización y agrega la Tasa de Coste 2 con una fecha de inicio del 1 de mayo de 2023, se agrega la fecha de finalización del 30 de abril de 2023 a la Tasa de Coste 1 para que no haya espacios.</p></li>

   <li><b>Tarifa de facturación</b>: Cantidad de facturación por hora para el usuario.
      <p>Para tarifas de facturación efectivas por fecha, haga clic en <strong>Agregar tarifa</strong>. Introduzca el valor de la tarifa de facturación para el período de tiempo y asigne una Fecha de Inicio y una Fecha de Finalización según sea necesario. La tarifa de facturación 1 no tendrá una fecha de inicio y la última tarifa de facturación no tendrá una fecha de finalización.</p> <p>Algunas fechas se añaden automáticamente. Por ejemplo, si la Tarifa de facturación 1 no tiene una fecha de finalización y agrega una segunda con una fecha de inicio del 1 de mayo de 2023, se agrega la fecha de finalización del 30 de abril de 2023 a la Tarifa de facturación 1 para que no existan brechas.</p><p> <img alt="Costes de usuario y tarifas de facturación" src="assets/edit-user-cost-billing-rate-2.png"> </p></li>

   </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formularios personalizados</td> 
      <td><p>Asocie un formulario personalizado de usuario existente a este usuario. Debe crear un formulario personalizado para poder asociarlo a un usuario. En la lista solo se muestran los formularios personalizados activos. Los campos que no tiene acceso para editar no se muestran en un formulario personalizado individual.</p> <p>Para obtener información sobre la creación de formularios personalizados, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Crear o editar un formulario personalizado</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Comentario</td> 
      <td>Escriba el comentario que desee enviar a los usuarios y al área de Actualizaciones de sus perfiles de usuario.</td> 
     </tr> 
    </tbody> 
   </table>
