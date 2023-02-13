---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Editar perfiles de usuario de forma masiva
description: Como administrador de Adobe Workfront, puede editar las cuentas de usuario de forma masiva.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '2194'
ht-degree: 0%

---

# Editar perfiles de usuario de forma masiva

>[!IMPORTANT]
>
>El procedimiento descrito en esta página solo se aplica a organizaciones que aún no se han incorporado al Admin Console. Si su organización se ha incorporado a Adobe Admin Console, debe realizar esta acción a través de Adobe Admin Console.
>
>Para obtener instrucciones sobre la edición del perfil de un usuario en Adobe Admin Console, consulte la sección &quot;Editar detalles del usuario&quot; en el artículo [Usuarios de carga masiva](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) o póngase en contacto con su administrador de Adobe Admin Console.
>
>Para obtener una lista de procedimientos que difieren en función de si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en plataformas (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Puede editar las cuentas de usuario de forma masiva. Al editar usuarios de forma masiva, solo los campos que seleccione específicamente se actualizarán con la misma información para todos los usuarios seleccionados. Todos los demás campos que deje sin seleccionar permanecen igual para cada usuario individual, incluso si son diferentes para cada usuario.

>[!NOTE]
>
>* No puede editar de forma masiva la sección Información personal de los perfiles de los usuarios porque dicha información debe ser única para cada usuario.
>* Para garantizar la precisión de los datos y un rendimiento óptimo, le recomendamos que no seleccione más de 2000 usuarios al mismo tiempo para una edición masiva.
>


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

## Editar cuentas de usuario de forma masiva

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Usuarios** ![](assets/users-icon-in-main-menu.png).

1. Seleccione más de un usuario y, a continuación, haga clic en el icono Editar ![](assets/edit-icon.png).

1. En el **Editar usuario** cambie cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Preferencias</td> 
      <td> 
       <ul> 
        <li><b>Zona horaria:</b> Zona horaria de los usuarios.</li> 
        <li><b>Configuración regional</b>: La configuración regional preferida de los usuarios. Esto afecta al formato de los números y las fechas de los correos electrónicos procedentes de Workfront.</li> 
        <li><b>Mostrar porcentaje completado en el estado de actualización</b>: Marque esta opción si desea mostrar una barra de porcentaje completado dentro del flujo de actualización de tareas para todos los usuarios.</li> 
        <li><b>Enviar trabajo que me asigne a mi misma en la pestaña Trabajar en</b>: Marque esta opción si desea que todo lo que los usuarios se asignan a sí mismos aparezca directamente en la pestaña Trabajar en . El valor predeterminado es mostrar todo lo asignado a un usuario en la pestaña Solicitud de trabajo .</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificaciones</td> 
      <td>Seleccione las notificaciones por correo electrónico que deben habilitarse para el nuevo usuario.<p>Puede seleccionar notificaciones de compendio instantáneo y diario. Todas las notificaciones diarias del compendio se entregan en algún momento después de la misma hora para todos los usuarios seleccionados. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configurar notificaciones de eventos para todos los miembros del sistema</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Acceso</td> 
      <td> 
       <ul> 
        <li><b>Está activo:</b> Seleccione este campo para indicar si los usuarios están activos. Los usuarios activos utilizan una licencia de Workfront. Al anular la selección del campo, se desactivan los usuarios.</li> 
        <li> 
        <p><b>Nivel de acceso:</b> Seleccione el nivel de acceso que desea asignar a estos usuarios. Todos los usuarios seleccionados tendrán el mismo nivel de acceso.
        </p> 
        <p>Al asignar un nivel de acceso a los usuarios, puede asignar un nivel igual o inferior a su propio nivel de acceso. (Por ejemplo, si el nivel de acceso es Planificador, no puede asignar el nivel de acceso Administrador). </p>
        <p>Sin embargo, no puede asignar un nivel de acceso inferior al suyo si el administrador de Workfront ha habilitado permisos en el nivel de acceso que no están también habilitados en el suyo propio (a través de la configuración de Ajuste, como se describe en <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>).</p> 
        <p>Para obtener más información sobre los niveles de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configuración del acceso a Adobe Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Plantilla de diseño</b>: Elija una plantilla de diseño para los usuarios. La plantilla de diseño asignada a los usuarios tendrá prioridad sobre cualquier plantilla de diseño asignada a su grupo principal, equipo doméstico o función de trabajo principal. Para obtener más información sobre la prioridad de asignación de la plantilla de diseño, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Creación y administración de plantillas de diseño</a>.</p> 
        <p><b>NOTA</b>: La lista de plantillas de diseño disponibles en este campo depende del acceso:
          <ul>
           <li>Como administrador de Workfront, puede ver todas las plantillas de diseño a nivel de sistema y de grupo.</li>
           <li>Como administrador de grupo, puede ver las plantillas de diseño de nivel de sistema, así como las asociadas con los grupos que administra.</li>
           <li><p>Como usuario con licencia de Planificador y acceso para editar usuarios, solo puede ver plantillas de diseño a nivel de sistema. </p>
           <p>Para obtener información sobre las plantillas de diseño de nivel de grupo, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Creación y administración de plantillas de diseño</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organización</td> 
      <td> 
       <ul> 
        <li><b>Empresa</b>: Empresa de los usuarios. Los usuarios solo pueden asociarse con una empresa. Debe crear una empresa para poder asociarla con un usuario. En la lista solo aparecen las empresas activas. Para obtener información sobre la creación de empresas, consulte Explicación y administración de empresas.</li> 
        <li><b>Equipo principal</b>: Especifique el equipo principal de los usuarios. Los usuarios solo pueden tener un equipo de inicio. </li> 
        <li><b>Otros equipos</b>: Los usuarios pueden pertenecer a varios equipos. </li> 
        <li> <p><b>Grupo de inicio:</b> Seleccione un grupo apropiado para asignar a los usuarios como su grupo de inicio. Esto permite al usuario acceder a los objetos que se comparten con el grupo.</p> <p><b>NOTA</b>: Se trata de un campo obligatorio. Los usuarios no pueden estar asociados a un grupo de inicio.</p> <p>Puede asignar un grupo a usuarios solo en las siguientes situaciones:</p> 
         <ul> 
          <li>Es administrador de Workfront.</li> 
          <li>Usted es el administrador de ese grupo.</li> 
          <li>El grupo es público.</li> 
         </ul> </li> 
        <li> <p><b>Otros grupos</b>: Los usuarios pueden pertenecer a varios grupos. Puede asignar un grupo a un usuario solo en las siguientes situaciones:</p> 
         <ul> 
          <li>Es administrador de Workfront.</li> 
          <li>Usted es el administrador de ese grupo.</li> 
          <li> <p>El grupo es público. </p> 
          <p>Para obtener más información sobre los grupos públicos, consulte <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Crear un grupo</a>.</p> 
          <p>Para obtener más información sobre los grupos, consulte <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Información general sobre grupos</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planificación de recursos</td> 
      <td> 
       <ul> 
        <li><b>Desactivación de programación</b>: Marque esta casilla si desea programar que los usuarios se desactiven después de un periodo de tiempo.</li> 
        <li><b>Fecha de desactivación programada</b>: La fecha después de la cual se desactivan los usuarios. Para obtener más información sobre la programación de usuarios para la desactivación, consulte la sección <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Programar usuarios para su desactivación</a> en <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desactivar o reactivar un usuario</a>.</li> 
        <li> <p><b>Función principal</b>: Esta es la función de trabajo principal que tiene un usuario en Workfront. De forma predeterminada, todas las tareas y problemas a los que se asignan los usuarios también se asignan a esta función de trabajo. Las funciones de los puestos de trabajo son esenciales en la gestión de los recursos. Para obtener más información sobre las funciones de trabajo, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar funciones de trabajo</a></p> <p>Este campo solo se puede actualizar si tiene una licencia de Plan con acceso administrativo de usuario o si es administrador de Workfront. Para obtener más información sobre la configuración de usuarios con acceso administrativo a los usuarios, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</p> </li> 
        <li>(Condicional) Si seleccionó un <b>Función principal</b>, el <b>Porcentaje de disponibilidad de FTE</b> se muestra. Especifique qué porcentaje de tiempo de las programaciones de los usuarios se asigna a esta función de trabajo. El valor predeterminado para el Porcentaje de disponibilidad de FTE para la función principal es del 100%.</li> 
        <li> <p><b>Otras funciones</b>: Los usuarios pueden tener varias funciones de trabajo en Workfront. Las funciones de los puestos de trabajo son esenciales en la gestión de los recursos. No hay límite para la cantidad de funciones de trabajo que un usuario puede desempeñar. Sin embargo, se recomienda no asignar un usuario a un número excesivamente grande de funciones de trabajo, ya que la administración de recursos puede llegar a ser demasiado compleja para estos usuarios.</p> <p>Para obtener más información sobre las funciones de trabajo, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar funciones de trabajo</a>.</p> <p>Este campo solo se puede actualizar si tiene una licencia de Plan con acceso administrativo de usuario o si es administrador de Workfront. Para obtener más información sobre la configuración de usuarios con acceso administrativo a los usuarios, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</p> </li> 
        <li> <p>(Condicional) Si ha seleccionado una o varias <b>Otras funciones</b>, el <b>Porcentaje de disponibilidad de FTE</b> se muestra para cada función. Especifique qué porcentaje de tiempo de las programaciones de los usuarios se asigna a cada rol de trabajo. El valor predeterminado del Porcentaje de disponibilidad de FTE para las otras funciones es 0%.</p> <p><b>NOTA</b>:  
          <ul> 
           <li>Si Otras funciones tienen una disponibilidad del 0% de FTE, no se muestran en el Planificador de recursos, a menos que se asignen a los usuarios tareas en estas funciones.</li> 
           <li> <p>La suma de todos los porcentajes de disponibilidad de FTE para todas las funciones debe ser igual al 100%. Cada porcentaje de disponibilidad de FTE calcula las horas disponibles para cada función por usuario en el Planificador de recursos. Las horas disponibles para cada función por usuario dependen del tiempo disponible para el usuario.</p> <p>Workfront calcula el tiempo disponible para el usuario según el método que haya seleccionado el administrador de Workfront para calcular el FTE en las preferencias de administración de recursos.</p> <p>Para obtener más información sobre el cálculo de la disponibilidad para el usuario, consulte <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Descripción general del cálculo de horas y FTE para usuarios y funciones en el planificador de recursos</a>.</p> <p>Para obtener más información sobre la configuración de las preferencias de Administración de recursos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurar las preferencias de Administración de recursos</a>.</p> </li> 
          </ul> </p> </li> 
        <li> <p><b>Programación</b>: Asocie una programación a los usuarios. La programación de los usuarios calcula la cronología de las tareas a las que se asignan los usuarios.</p> <p>Un administrador de Workfront o un administrador de grupo deben crear una programación para poder asociarla con los usuarios.</p> <p>Seleccione una programación de sistema o de grupo para asignarla a los usuarios seleccionados.</p> <p>Para obtener más información sobre las programaciones de grupos y niveles del sistema, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Crear una programación</a>.</p> <p><b>IMPORTANTE</b>: Workfront utiliza la programación de un usuario únicamente cuando la opción Calcular disponibilidad de recursos mediante está establecida en la programación del usuario. Para obtener información acerca de cómo afecta la configuración Calcular disponibilidad de recursos usando a la programación que se usa para la Administración de recursos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurar las preferencias de Administración de recursos</a>.</p> </li> 
        <li> <p><b>Perfil de hoja de horas</b>: Asocie un perfil de parte de horas a los usuarios. Esto garantiza que las hojas de horas se generen automáticamente para los usuarios.</p> 
        <p><b>NOTA</b>:  
          <ul> 
           <li>La lista de perfiles de hojas de horas que tiene disponibles en este campo depende del acceso:
            <ul>
             <li>Como administrador de Workfront, puede ver todos los perfiles de hojas de horas a nivel de sistema y de grupo.</li>
             <li><p>Como administrador de grupos, puede ver perfiles de parte de horas de nivel de sistema, así como los asociados a los grupos que administra.</p></li>
             <li><p>Como usuario con licencia de Planificador y acceso para editar usuarios, solo puede ver perfiles de hojas de horas a nivel de sistema.</p></li>
            </ul></li> 
           <li>Si es administrador de grupos, todos los usuarios que edite deben ser miembros de un grupo que administre.</li> 
          </ul> </p> </li> 
        <li><b>Tipo de hora predeterminado</b>: Seleccione el tipo de hora predeterminado para los usuarios. Este es el tipo de hora que se utiliza de forma predeterminada cuando los usuarios registran la hora.</li> 
        <li> <p><b>Tipos de hora disponibles</b>: Seleccione los tipos de hora que deben estar disponibles para el usuario. Estos tipos de hora son visibles en todas partes en Workfront donde los usuarios pueden registrar la hora. Un usuario solo puede ver los tipos de hora habilitados en el nivel de proyecto, así como en el nivel de usuario.</p> 
        <p>Para obtener más información sobre los tipos de hora disponibles para los usuarios, consulte <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Definir tipos de hora y disponibilidad para hojas de hora</a>.</p> 
        </li> 
        <li> <p><b>FTE</b>: El número que especifique aquí se tiene en cuenta para calcular la disponibilidad del usuario en función de la programación predeterminada solo cuando las preferencias de administración de recursos a nivel de sistema están configuradas como <b>La programación predeterminada</b>.</p> 
        <p>Por ejemplo, si el valor de FTE es 0,5 y el programa predeterminado es 40 horas, el usuario estará disponible para trabajar 20 horas a la semana. Para obtener más información acerca de cómo las excepciones de programación o el tiempo de inactividad pueden afectar a la disponibilidad del usuario cuando se selecciona la programación predeterminada, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurar las preferencias de Administración de recursos</a>. </p> 
        <p>Si las Preferencias de Gestión de Recursos a nivel de sistema están establecidas en <b>Programación del usuario</b>, el valor que especifique aquí se ignorará y el usuario se considerará disponible según lo especificado en su programación. En este caso, el FTE del usuario para el planificador de recursos se calcula mediante la fórmula siguiente:</p>
        <p><code style="font-style: normal;">User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code> </p> <p>Para obtener más información sobre el cálculo de FTE de usuario, consulte <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Descripción general del cálculo de horas y FTE para usuarios y funciones en el planificador de recursos</a>.</p> <p>Para obtener más información sobre la creación de programaciones en Workfront, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Crear una programación</a>.</p> <p>Para obtener más información sobre la configuración de las preferencias de administración de recursos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurar las preferencias de Administración de recursos</a>.</p> 
        </li> 
        <li> <p><b>Grupos de recursos</b>: Asocie a los usuarios con grupos de recursos.</p> <p><b>NOTA</b>: En este campo solo aparecen los grupos de recursos comunes a todos los usuarios seleccionados. Si los usuarios seleccionados no tienen grupos de recursos compartidos, este campo está vacío. Si este campo está vacío, los grupos de recursos que especifique aquí sobrescribirán sus grupos de recursos individuales.</p> 
        <p>Para obtener más información sobre los grupos de recursos, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resumen de los grupos de recursos </a>.</p> </li> 
        <li><b>Costo por hora</b>: Cantidad de coste por hora para el usuario. </li> 
        <li><b>Facturación por hora</b>: El importe de la facturación por hora para el usuario.</li> 
        <li><b>Forms personalizado</b>: Asocie un formulario personalizado de usuario existente a los usuarios. Debe crear un formulario personalizado para poder asociarlo a un usuario. En la lista solo aparecen los formularios personalizados activos. Para obtener información sobre la creación de formularios personalizados, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Crear o editar un formulario personalizado</a>.</li> 
        <li><b>Comentario</b>: Introduzca un comentario en el campo proporcionado. Todos los usuarios seleccionados recibirán una notificación en la aplicación, así como una notificación por correo electrónico con su comentario. El comentario se muestra en la pestaña Actualizaciones del perfil de los usuarios.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) En la **Forms personalizado** seleccione **Volver a calcular expresiones personalizadas** para garantizar que todos los campos personalizados calculados de los formularios personalizados adjuntos a los usuarios seleccionados estén actualizados.

1. Haga clic en **Guardar cambios**.
