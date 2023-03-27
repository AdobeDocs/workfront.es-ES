---
title: Edición del perfil de un usuario
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Como administrador de Adobe Workfront, puede crear usuarios nuevos y administrar los perfiles de los existentes.
author: Courtney, Alina
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: fed4713d1e9044879db6d34dc4725245a2516634
workflow-type: tm+mt
source-wordcount: '2786'
ht-degree: 0%

---

# Edición del perfil de un usuario


>[!IMPORTANT]
>
>El procedimiento descrito en esta página solo se aplica a organizaciones que aún no se han incorporado al Admin Console. Si su organización se ha incorporado a Adobe Admin Console, debe realizar esta acción a través de Adobe Admin Console.
>
>Para obtener instrucciones sobre la edición del perfil de un usuario en Adobe Admin Console, consulte la sección &quot;Editar detalles del usuario&quot; en el artículo [Administrar usuarios individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) o póngase en contacto con su administrador de Adobe Admin Console.
>
>Para obtener una lista de procedimientos que difieren en función de si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en plataformas (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador de Adobe Workfront, puede crear usuarios nuevos y administrar los perfiles de los existentes. Para obtener información sobre la creación de usuarios, consulte [Agregar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Los usuarios con una licencia de Plan también pueden crear y administrar usuarios. Para obtener información sobre el acceso necesario para editar usuarios, consulte [Conceder acceso a los usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe tener una de las siguientes opciones:</p> 
    <ul> 
     <li> <p>Nivel de acceso del administrador del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>. </p> </li> 
     <li> <p><b>Usuarios</b> en el nivel de acceso configurado para <b>Editar</b> acceso, con <b>Crear</b> y al menos uno de los dos <b>Administrador de usuarios</b> opciones activadas en <b>Ajustar la configuración</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De estas dos opciones, si es Usuario <b>Administración (usuarios del grupo)</b> está activada, debe ser administrador de grupo de un grupo al que pertenezca el usuario.</p> <p>Para obtener más información sobre la variable <b>Usuarios</b> configuración en un nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Editar un perfil de usuario

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Usuarios** ![](assets/users-icon-in-main-menu.png).
1. Seleccione el usuario y, a continuación, haga clic en el icono Editar ![](assets/edit-icon.png).

1. En el **Editar usuario** que se muestra, cambie cualquiera de la siguiente información y haga clic en **Guardar cambios**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Información personal </td> 
      <td> 
       <ul> 
        <li><b>Nombre</b>, <b>Apellidos</b></li> 
        <li> <p><b>Dirección de correo electrónico:</b> La dirección de correo electrónico de un usuario también es su nombre de usuario en Workfront. Este campo distingue entre mayúsculas y minúsculas y debe ser único. Si algún usuario intenta agregar una dirección de correo electrónico no única 3 veces dentro de una ventana de 10 minutos, aparecerá una respuesta de reCAPTCHA.</p> <p>Si utiliza la lista de permitidos de correo electrónico e introduce un dominio de correo electrónico que no está en la lista, el usuario no recibirá notificaciones por correo electrónico. Para obtener más información sobre la lista de permitidos, consulte <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Configurar la lista de permitidos de correo electrónico</a>.</p> </li> 
        <li> <p><b>Restablecer contraseña</b>: Haga clic en este vínculo para restablecer la contraseña del usuario. Se le pedirá su propia contraseña antes de poder restablecer la contraseña de un usuario.</p> <p>Para restablecer la contraseña de otro usuario, debe ser administrador de Workfront o administrador de grupo.</p> <p><b>NOTA</b>:  
          <ul> 
           <li> <p>Si es un administrador de grupos, puede restablecer las contraseñas solo para los usuarios de los grupos en los que esté designado como tal. Además, el permiso del administrador de usuarios (usuarios del grupo) debe estar habilitado en el nivel de acceso:</p> <p> <img src="assets/group-admin-user.png" > </p> <p>Esta configuración está deshabilitada de forma predeterminada. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </li> 
           <li> <p>No puede restablecer la contraseña de un administrador de Workfront.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;sso configuration=""&gt; Nombre de usuario</b>: Si el administrador de Workfront ha habilitado una integración de SSO con Workfront, en este campo aparece el nombre de usuario de SSO. El tipo de configuración SSO habilitada para su instancia de Workfront se puede ver en este campo. </li> 
        <li> <p><b>OnlyAllow &lt;sso configuration=""&gt; Autenticación</b>: Si el administrador de Workfront ha habilitado una integración de SSO con Workfront y ha actualizado todos los usuarios para SSO, este campo está seleccionado de forma predeterminada. El tipo de configuración SSO habilitada para su instancia de Workfront se puede ver en este campo.</p> <p>Cuando se selecciona este campo, el usuario debe iniciar sesión en Workfront con sus credenciales de SSO. Al desmarcarlo, podrán iniciar sesión en Workfront con sus credenciales de Workfront.</p> <p>Para obtener más información sobre la configuración de Workfront con una solución SSO, consulte <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Información general sobre el inicio de sesión único en Adobe Workfront</a></p> <p>Para obtener más información sobre la actualización de usuarios para SSO, consulte <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Actualización de usuarios para el inicio de sesión único</a>.</p> <p><b>NOTA</b>: Si es administrador de grupos, puede editar la variable &lt;sso configuration=""&gt; solo para los usuarios de los grupos en los que esté designado como tal. Además, el permiso Administración de usuarios (usuarios del grupo) debe estar habilitado en su nivel de acceso.
        <p>Si es un administrador de grupo y tiene el permiso Administrador de usuarios (todos los usuarios) habilitado en su nivel de acceso, puede editar la variable &lt;sso configuration=""&gt; para todos los usuarios.</p> </li> 
        <li><b>Información del trabajo:</b> Información sobre el trabajo, como la titularidad del trabajo y el área de experiencia que es responsable el usuario.</li> 
        <li><p><b>Información de contacto</b>: El número de teléfono y la dirección del usuario.</p>
        <p>Si el usuario está habilitado para la administración unificada de usuarios (UUM) o el sistema Identity Management de Adobe (IMS), la variable <b>País</b> en la sección Información de contacto solo acepta valores de código de país (por ejemplo, EE. UU., GB, IN).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Preferencias </td> 
      <td> 
       <ul> 
      <li> <p><b>Zona horaria:</b> Zona horaria del usuario.</p> <p>Para obtener información sobre cómo ayudar a los usuarios a colaborar en Workfront en zonas horarias, consulte <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Trabajo en zonas horarias</a>.</p> </li> 
       <li><b>Configuración regional de correo electrónico</b>: La configuración regional de correo electrónico preferida del usuario. Esto afecta al formato de los números y las fechas de los correos electrónicos procedentes de Workfront.</li>

   <li><b>Recibir correos electrónicos de este entorno de prueba</b>: Marque esta opción si desea recibir notificaciones por correo electrónico del entorno en el que ha iniciado sesión.
      <p><b>NOTA</b></p>
      Esta opción solo está disponible en los entornos Preview y Sandbox. Las notificaciones por correo electrónico están habilitadas en el entorno de producción de forma predeterminada. 
      </li>

   <li><b>Mostrar porcentaje completado en el estado de actualización</b>: Marque esta opción si desea mostrar una barra de porcentaje completado dentro del área Actualizar de las tareas de este usuario.</li> 
       <li><b>Enviar trabajo que me asigne a mi misma en la pestaña Trabajar en</b>: Seleccione esta opción si desea que todo lo que el usuario se asigna aparezca directamente en la ficha Trabajar en . El valor predeterminado es mostrar todo lo asignado a un usuario en la pestaña Solicitud de trabajo .</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificaciones</td> 
      <td> <p>Seleccione las notificaciones por correo electrónico que deben habilitarse para el nuevo usuario.</p> <p>Puede seleccionar notificaciones de compendio instantáneo y diario.</p> <p>Para obtener más información, consulte <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configurar notificaciones de eventos para todos los miembros del sistema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Acceso</td> 
      <td> 
       <ul> 
      <li><b>Está activo:</b> Seleccione este cuadro para indicar que el usuario está activo. Los usuarios activos utilizan una licencia de Workfront. Al desmarcar la casilla, se desactiva el usuario.</li> 
       <li> <p><b>Nivel de acceso:</b> Seleccione el nivel de acceso que desea asignar a este usuario.</p> 
       <p>Al asignar un nivel de acceso a un usuario, puede asignar un nivel igual o inferior a su propio nivel de acceso. (Por ejemplo, si el nivel de acceso es Planificador, no puede asignar el nivel de acceso Administrador). Sin embargo, no puede asignar un nivel de acceso que, de forma predeterminada, sea menor que su propio nivel de acceso si el administrador de Workfront ha habilitado permisos no predeterminados en el nivel de acceso que no estén también habilitados en su propio nivel de acceso (a través de la configuración de la Ajustar, tal como se describe en <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>). </p> 
       <p>Para obtener más información sobre los niveles de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configuración del acceso a Adobe Workfront</a>.</p> </li> 
       <li> <p><b>Plantilla de diseño</b>: Elija una plantilla de diseño para el usuario. Esta plantilla de diseño tiene prioridad sobre cualquier plantilla de diseño asignada al grupo principal del usuario, al equipo principal o a la función de trabajo principal. Para obtener más información sobre la prioridad de asignación de las plantillas de diseño, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Creación y administración de plantillas de diseño</a>.</p> <p><b>NOTA</b>:  <p>La lista de plantillas disponibles en este campo depende del acceso:</p> 
       <ul> 
       <li>Como administrador de Workfront, puede ver todas las plantillas de diseño de nivel de sistema y de grupo.</li> 
       <li>Como administrador de grupo, puede ver la plantilla de diseño a nivel de sistema, así como las asociadas con los grupos que administra.</li> 
       <li>Como usuario con una licencia de Plan y acceso para editar usuarios, solo puede ver plantillas de diseño a nivel de sistema.</li> 
       </ul> <p>Para obtener más información sobre las plantillas de diseño de nivel de grupo, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Creación y administración de plantillas de diseño</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organización </td> 
      <td> 
       <ul> 
      <li><b>Empresa</b>: Empresa del usuario. Los usuarios solo pueden asociarse con una empresa. Debe crear una empresa para poder asociarla con un usuario. En la lista solo aparecen las empresas activas. Para obtener información sobre la creación de empresas, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Crear y editar empresas</a>.</li> 
      <li><b>Informes para:</b> Si ha especificado una empresa para el usuario, también puede especificar el administrador directo del usuario en este campo. Un usuario solo puede tener un administrador.</li> 
      <li><b>Informes directos:</b> Si ha especificado una empresa para el usuario, también puede especificar los informes directos del usuario. Un usuario puede tener varios informes directos.</li> 
      <li><b>Equipo principal</b>: Especifique el equipo de inicio del usuario. Los usuarios solo pueden tener un equipo de inicio.</li> 
      <li><b>Otros equipos</b>: Los usuarios pueden pertenecer a varios equipos.</li> 
      <li> <p><b>Grupo de inicio:</b> Seleccione un grupo apropiado para asignar al usuario. Esto permite al usuario acceder a los objetos que se comparten con el grupo.</p> <p>Este campo es obligatorio. Todos los usuarios deben estar asociados a un grupo principal. Si no selecciona uno, el grupo se asigna como grupo principal del nuevo usuario.</p> <p><b>NOTA</b>: Puede asignar un grupo a un usuario solo si es administrador de Workfront, administrador del grupo o público.</p> </li> 
      <li> <p><b>Otros grupos</b>: Los usuarios pueden pertenecer a varios grupos. Puede asignar un grupo a un usuario solo si es administrador de Workfront, administrador del grupo o público.</p> <p><b>IMPORTANTE</b>: Agregar un usuario a más de 100 grupos puede causar problemas de rendimiento en cualquier área de Workfront que carga la lista de grupos.</p> <p>Para obtener más información sobre los grupos públicos, consulte <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Crear un grupo</a>.</p> <p>Para obtener más información sobre los grupos, consulte <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Información general sobre grupos</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planificación de recursos </td> 
      <td> 
       <ul>
       <li>
       <b>Tiempo de trabajo</b>: Representa el porcentaje del tiempo equivalente a tiempo completo (FTE) que el usuario está disponible para el trabajo real, sin incluir la sobrecarga. El tiempo de trabajo debe ser un número decimal de hasta 1 y no puede ser 0. Por ejemplo, un 20% de disponibilidad para el trabajo real sería 0,2.

   El valor predeterminado del campo es 1, lo que indica que un usuario gasta todo su FTE en trabajo real relacionado con el proyecto.

   El sistema utiliza este número para calcular la disponibilidad del usuario para el trabajo real relacionado con el proyecto.

   Para obtener más información sobre la creación de programaciones en Workfront, consulte <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Crear una programación</a>.

   Las excepciones de programación y el tiempo de espera también pueden afectar a la capacidad del usuario.

   Workfront calcula la disponibilidad de un usuario según las preferencias de Administración de recursos del área de configuración. Para obtener más información, consulte <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar las preferencias de Administración de recursos</a>.

   <b>SUGERENCIA</b>

   Establezca el valor Tiempo de trabajo en 1 para indicar que el usuario está disponible para trabajos relacionados con el proyecto con todo su equivalente de tiempo completo.
   </li> 
      <li> <b>Desactivación de programación</b>: Marque esta casilla si desea programar la desactivación de este usuario después de un periodo de tiempo. </li> 
       <li><b>Fecha de desactivación programada</b>: La fecha después de la cual se desactiva el usuario. Para obtener información sobre cómo programar usuarios para la desactivación, consulte la <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Programar usuarios para su desactivación</a> en <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desactivar o reactivar un usuario</a>.</li> 
       <li> <p><b>Función principal</b>: Esta es la función de trabajo principal que el usuario puede cumplir en Workfront. Todas las tareas y problemas a los que está asignado el usuario también se asignan a esta función de trabajo. Las funciones de los puestos de trabajo son esenciales en la gestión de los recursos. Este campo solo se puede actualizar si tiene una licencia de Plan con acceso administrativo de usuario o si es administrador de Workfront. Para obtener más información sobre la configuración de usuarios con acceso administrativo a los usuarios, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</p> <p>En la lista solo se muestran los roles de trabajo activos. </p> </li> 
       <li>Si seleccionó un <b>Función principal</b>, el <b>Porcentaje de disponibilidad de FTE</b> se muestra. Especifique qué porcentaje de tiempo de la programación del usuario se asigna a esta función de trabajo. El valor predeterminado para el Porcentaje de disponibilidad de FTE para la función principal es del 100%. </li> 
       <li> <p><b>Otras funciones</b>: Un usuario puede tener varias funciones de trabajo en Workfront. Las funciones de los puestos de trabajo son esenciales en la gestión de los recursos. No hay límite para la cantidad de funciones de trabajo que un usuario puede desempeñar. Sin embargo, se recomienda no asignar un usuario a un número excesivamente grande de funciones de trabajo, ya que la administración de recursos puede llegar a ser demasiado compleja para estos usuarios.<p>En la lista solo se muestran los roles de trabajo activos. Para obtener más información sobre las funciones de trabajo, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar funciones de trabajo</a>.</p> <p>Este campo solo se puede actualizar si tiene una licencia de Plan con acceso administrativo de usuario o si es administrador de Workfront. <br>Para obtener más información sobre la configuración de usuarios con acceso administrativo a los usuarios, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</p> </li> 
       <li> <p>(Condicional) Si ha seleccionado una o varias <b>Otras funciones</b>, el <b>Porcentaje de disponibilidad de FTE</b> se muestra para cada función. Especifique qué porcentaje de tiempo de la programación del usuario se asigna a cada rol de trabajo. El valor predeterminado del Porcentaje de disponibilidad de FTE para las otras funciones es 0%.</p> <p><b>NOTA</b>: Si Otras funciones tienen una disponibilidad del 0% de FTE, no se muestran en el Planificador de recursos, a menos que se asignen a los usuarios tareas en estas funciones.</p> <p> <img alt="user_settings_roles_and_date_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>NOTA</b>: <p>La suma de todos <b>Porcentajes de disponibilidad de FTE</b> para todas las funciones debe ser igual al 100 %. Cada porcentaje de disponibilidad de FTE calcula las horas disponibles para cada función por usuario en el Planificador de recursos. Las horas disponibles para cada función por usuario dependen del tiempo disponible para el usuario.</p> <p>Workfront calcula el tiempo disponible para el usuario según el método que haya seleccionado el administrador de Workfront para calcular el FTE en las preferencias de administración de recursos.</p> <p>Para obtener información sobre el cálculo de disponibilidad para el usuario, consulte <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Descripción general del cálculo de horas y FTE para usuarios y funciones en el planificador de recursos</a>.</p> <p>Para obtener información sobre la configuración de las preferencias de Administración de recursos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurar las preferencias de Administración de recursos</a>.</p> </p> </li> 
       <li> <p><b>Programación</b>: Asocie una programación al usuario. La programación del usuario calcula la cronología de las tareas a las que se asigna el usuario.</p> <p>Debe crear una programación para poder asociarla con un usuario. Para obtener más información sobre la creación de programaciones, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Crear una programación</a>.</p> <p><b>NOTA</b>: Se recomienda que la programación que asocie al usuario coincida con el huso horario del usuario.</p> </li> 
       <li> <p><b>Perfil de hoja de horas</b>: Asocie un perfil de parte de horas al usuario para asegurarse de que las hojas de horas se generan automáticamente para el usuario.</p> <p><b>NOTA</b>: La lista de perfiles que tiene disponibles en este campo depende del acceso:
       <ul>
       <li>Como administrador de Workfront, puede ver todos los perfiles de hoja de horas a nivel de sistema y de grupo.</li>
       <li>Como administrador de grupos, puede ver los Perfiles de hojas de horas a nivel de sistema, así como los asociados a los grupos que administra.</li>
       <li>Como usuario con una licencia de Plan y acceso para editar usuarios, solo puede ver Perfiles de parte de horas a nivel de sistema. Para obtener más información sobre los perfiles de hojas de horas de nivel de grupo, consulte <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">Crear, editar y asignar perfiles de parte de horas</a>.</li>
      </ul></p> </li> 
       <li><b>Tipo de hora predeterminado</b>: Seleccione el tipo de hora predeterminado para el usuario. Este es el tipo de hora que se utiliza de forma predeterminada cuando el usuario registra la hora.</li> 
       <li><b>Tipos de hora disponibles</b>: Seleccione los tipos de hora que deben estar disponibles para el usuario. Estos tipos de hora son visibles en todas partes en Workfront donde el usuario puede registrar la hora. Un usuario solo puede ver los tipos de hora habilitados en el nivel de proyecto, así como en el nivel de usuario. Para obtener más información sobre los tipos de hora disponibles para los usuarios, consulte <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Definir tipos de hora y disponibilidad para hojas de hora</a>.</li> 
       <li><b>Iniciar sesión:</b> Seleccione si el usuario debe iniciar sesión en los elementos de trabajo en horas o días. Para obtener más información, consulte <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">Configure si la hora se registra en horas o días</a>.</li>

   <li> <b>FTE</b>: Es el equivalente de tiempo completo del usuario. Workfront utiliza este número para calcular la disponibilidad del usuario según la programación predeterminada solo cuando las preferencias de administración de recursos a nivel de sistema están establecidas en la programación predeterminada.

   <p>El FTE indica la cantidad de tiempo que el usuario puede pasar en el trabajo. Esto incluye los gastos generales, así como el tiempo empleado en el trabajo del proyecto. Por ejemplo, el tiempo que se pasa en las reuniones o la formación también se incluye en el ETC.</p>

   El FTE debe ser un número decimal de hasta 1 y no puede ser 0. Por ejemplo, si el valor de FTE es 0,5 y el programa predeterminado en Workfront es 40 horas, el usuario estará disponible 20 horas a la semana.

   El valor predeterminado del campo es 1.

   Las excepciones de programación, el tiempo libre y el valor del tiempo de trabajo pueden afectar a la disponibilidad del usuario.

   Workfront calcula la disponibilidad de un usuario según las preferencias de Administración de recursos del área de configuración.

   Si las Preferencias de Gestión de Recursos a nivel de sistema se establecen en La programación del usuario, se ignora el valor que especifique aquí y se considera que el usuario está disponible según lo especificado en su programación.

   Para obtener más información, consulte <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar las preferencias de Administración de recursos</a>.

   Para obtener más información sobre la creación de programaciones en Workfront, consulte <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Crear una programación</a>.
   </li>

   <li><b>Grupos de recursos</b>: Asocie el usuario a grupos de recursos. Para obtener más información, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Asociación de grupos de recursos con usuarios </a>.</li> 
        <li><b>Costo por hora</b>: Cantidad de coste por hora para el usuario. </li> 
        <li><b>Facturación por hora</b>: El importe de la facturación por hora para el usuario.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formularios personalizados</td> 
      <td>Asocie un formulario personalizado de usuario existente a este usuario. Debe crear un formulario personalizado para poder asociarlo a un usuario. En la lista solo aparecen los formularios personalizados activos. Para obtener información sobre la creación de formularios personalizados, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Crear o editar un formulario personalizado</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Comentario</td> 
      <td> <p>Escriba el comentario que desea enviar a los usuarios y al área Actualizaciones de sus perfiles de usuario.</p> </td> 
     </tr> 
    </tbody> 
   </table>
