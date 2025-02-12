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
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '2213'
ht-degree: 96%

---

# Editar perfiles de usuario de forma masiva

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

1. Seleccione más de un usuario y luego haga clic en el icono Editar ![Editar icono](assets/edit-icon.png).

1. En el cuadro **Editar usuario** que aparece, cambie cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Preferencias</td> 
      <td> 
       <ul> 
        <li><b>Zona horaria:</b> especifique la zona horaria del usuario.</li> 
        <li><b>Configuración regional</b>: la configuración regional preferida de los usuarios. Esto afecta al formato de los números y las fechas de los correos electrónicos procedentes de Workfront.</li> 
        <li><b>Enviar trabajo que me asigne a mí mismo a mi ficha Trabajando en</b>: Esta configuración hace referencia a una característica en desuso que se ha eliminado de Workfront.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificaciones</td> 
      <td>Seleccione las notificaciones por correo electrónico que deben habilitarse para el nuevo usuario.<p>Puede seleccionar notificaciones de resumen instantáneas y diarias. Todas las notificaciones de resumen diarias se envían en algún momento a la misma hora para todos los usuarios seleccionados. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configurar notificaciones de los eventos para todos los usuarios del sistema</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Acceso</td> 
      <td> 
       <ul> 
        <li><b>Activo:</b> seleccione este campo para indicar si los usuarios están activos.  Los usuarios activos utilizan una licencia de Workfront. Desmarcando el campo se desactivan los usuarios.</li> 
        <li> 
        <p><b>Nivel de acceso:</b> seleccione el nivel de acceso que desea asignar a estos usuarios. Todos los usuarios seleccionados tendrán el mismo nivel de acceso.
        </p> 
        <p>Al asignar un nivel de acceso a los usuarios, puede asignar un nivel igual o inferior al suyo propio. (Por ejemplo, si su nivel de acceso es Planificador, no puede asignar el nivel de acceso Administrador). </p>
        <p>Sin embargo, no puede asignar un nivel de acceso inferior al suyo propio si el administrador de Workfront ha habilitado permisos en el nivel de acceso que no están habilitados también en el suyo propio (a través de la configuración de ajuste, tal como se describe en <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear modificar niveles de acceso personalizados</a>).</p> 
        <p>Para obtener más información sobre los niveles de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configurar el acceso a Adobe Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Plantilla de diseño</b>: elija una plantilla de diseño para los usuarios. La plantilla de diseño asignada a los usuarios tendrá prioridad sobre cualquier plantilla de diseño asignada a su grupo de inicio, equipo de inicio o función principal. Para obtener más información sobre la prioridad de asignación de la plantilla de diseño, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Crear y administrar plantillas de diseño</a>.</p> 
        <p><b>NOTA</b>: La lista de plantillas de diseño que tiene disponibles en este campo depende de su acceso:
          <ul>
           <li>Como administrador de Workfront, puede ver todas las plantillas de diseño de nivel de sistema y de grupo.</li>
           <li>Como administrador de grupos, puede ver la plantilla de diseño de nivel de sistema, así como las asociadas con los grupos que administra.</li>
           <li><p>Como usuario con una licencia Planificador y acceso para editar usuarios, solo puede ver plantillas de diseño de nivel de sistema. </p>
           <p>Para obtener información acerca de las plantillas de diseño de nivel de grupo, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Crear y administrar plantillas de diseño</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organización</td> 
      <td> 
       <ul> 
        <li><b>Compañía</b>: la compañía de los usuarios. Los usuarios solo pueden asociarse con una compañía. Debe crear una compañía antes de poder asociarla a un usuario. En la lista solo se muestran las compañías activas. Para obtener información acerca de cómo crear compañías, consulte Explicación y administración de compañías.</li> 
        <li><b>Equipo de inicio</b>: especifique el equipo de inicio de los usuarios. Los usuarios solo pueden tener un equipo de inicio. </li> 
        <li><b>Otros equipos</b>: los usuarios pueden pertenecer a varios equipos. </li> 
        <li> <p><b>Grupo de inicio:</b> seleccione un grupo apropiado para asignárselo a los usuarios como su grupo de inicio. Esto ofrece al usuario la posibilidad de acceder a los objetos compartidos con el grupo.</p> <p><b>NOTA</b>: Este campo es obligatorio. No puede haber usuarios que no estén asociados a un grupo de inicio.</p> <p>Solo puede asignar un grupo a usuarios en las situaciones siguientes:</p> 
         <ul> 
          <li>Es usted administrador de Workfront.</li> 
          <li>Es usted el administrador de ese grupo.</li> 
          <li>El grupo es público.</li> 
         </ul> </li> 
        <li> <p><b>Otros grupos</b>: los usuarios pueden pertenecer a varios grupos. Solo puede asignar un grupo a un usuario en las situaciones siguientes:</p> 
         <ul> 
          <li>Es usted administrador de Workfront.</li> 
          <li>Es usted el administrador de ese grupo.</li> 
          <li> <p>El grupo es público. </p> 
          <p>Para obtener más información sobre los grupos públicos, consulte <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Crear un grupo</a>.</p> 
          <p>Para obtener más información sobre los grupos, consulte <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Información general sobre los grupos</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planificación de recursos</td> 
      <td> 
       <ul>

   <li>
       <b>Tiempo de trabajo</b>: representa el porcentaje del tiempo Equivalente a jornada completa (EJC) que el usuario está disponible para el trabajo real, sin incluir los gastos generales. El tiempo de trabajo debe ser un número decimal de hasta 1 y no puede ser 0. Por ejemplo, una disponibilidad del 20% para el trabajo real sería de 0,2.

   El valor predeterminado del campo es 1, lo que indica que un usuario emplea todo su FTE en trabajo real relacionado con el proyecto.

   El sistema utiliza este número para calcular la disponibilidad del usuario para el trabajo real relacionado con el proyecto.

   Para obtener más información sobre cómo crear programaciones en Workfront, consulte <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Crear programación</a>.

   Las excepciones de horario y los días libres también pueden afectar a la capacidad del usuario.

   Workfront calcula la disponibilidad de un usuario según las preferencias de Administración de recursos del área de Configuración. Para obtener más información, consulte <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferencias de administración de recursos</a>.

   <b>SUGERENCIA</b>

   Establezca el valor de Tiempo de trabajo en 1 para indicar que el usuario está disponible para realizar el trabajo relacionado con el proyecto en su equivalente a jornada completa.
   </li>

   <li><b>Programar desactivación</b>: marque esta casilla si desea programar la desactivación de usuarios después de un periodo de tiempo.</li> 
       <li><b>Fecha programada de desactivación</b>: fecha a partir de la cual se desactivan los usuarios. Para obtener más información sobre cómo programar la desactivación de usuarios, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Programar usuarios para la desactivación</a> en <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desactivar o reactivar usuarios</a>.</li> 
       <li> <p><b>Función principal</b>: esta es la función principal que un usuario tiene en Workfront. De forma predeterminada, todas las tareas y problemas a los que están asignados los usuarios también se asignan a esta función. Las funciones de trabajo son esenciales en la administración de recursos. Para obtener más información sobre las funciones, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar funciones</a>.</p> <p>Solo puede actualizar este campo si dispone de una licencia de planificación con acceso de usuario administrativo o si es administrador de Workfront. Para obtener más información sobre la configuración de usuarios con acceso de usuario administrativo, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a usuarios</a>.</p> </li> 
       <li>(Condicional) Si seleccionó una <b>Función principal</b>, se muestra el campo <b>Porcentaje de disponibilidad de FTE</b>. Especifique qué porcentaje de tiempo de las programaciones de los usuarios se asigna a esta función. El valor predeterminado para el porcentaje de disponibilidad de FTE para la función principal es 100%.</li> 
       <li> <p><b>Otras funciones</b>: los usuarios pueden tener varias funciones en Workfront. Las funciones de trabajo son esenciales en la administración de recursos. No hay límite en cuanto a las funciones que puede desempeñar un usuario. Sin embargo, se recomienda no asignar un usuario a un número excesivamente elevado de funciones del puesto, ya que la administración de recursos podría resultar demasiado compleja para estos usuarios.</p> <p>Para obtener más información sobre las funciones, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Crear y administrar funciones de trabajo</a>.</p> <p>Solo puede actualizar este campo si dispone de una licencia de planificación con acceso de usuario administrativo o si es administrador de Workfront. Para obtener más información sobre la configuración de usuarios con acceso de usuario administrativo, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</p> </li> 
       <li> <p>(Condicional) Si ha seleccionado una o varias <b>Otras funciones</b>, se muestra el campo <b>Porcentaje de disponibilidad de FTE</b> para cada función. Especifique qué porcentaje de tiempo del horario de los usuarios se asigna a cada función. El valor predeterminado para el porcentaje de disponibilidad de FTE para las otras funciones es 0 %.</p> <p><b>NOTA</b>:  
       <ul> 
       <li>Si otras funciones tienen una disponibilidad de FTE del 0 %, no se muestran en el Planificador de recursos, a menos que los usuarios estén asignados a tareas de estas funciones.</li> 
       <li> <p>La suma de todos los porcentajes de disponibilidad de FTE para todas las funciones debe ser igual al 100 %. Cada porcentaje de disponibilidad de FTE calcula las horas disponibles para cada función por usuario en el Planificador de recursos. Las horas disponibles para cada función por usuario dependen del tiempo disponible para el usuario.</p> <p>Workfront calcula el tiempo disponible para el usuario según el método que haya seleccionado el administrador de Workfront para calcular el valor de FTE en las Preferencias de administración de recursos.</p> <p>Para obtener más información sobre cómo calcular la disponibilidad del usuario, consulte <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Información general sobre el cálculo de horas y FTE para usuarios y funciones en el Planificador de recursos</a>.</p> <p>Para obtener más información acerca de cómo configurar las preferencias de Administración de recursos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurar preferencias de administración de recursos</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>Programación</b>: asocie una programación con los usuarios. La programación de los usuarios calcula la línea de tiempo de las tareas que se les asignan.</p> <p>Un administrador de Workfront o de grupos debe crear una programación para poder asociarla con los usuarios.</p> <p>Seleccione una programación de nivel del sistema o de grupo para asignarla a los usuarios seleccionados.</p> <p>Para obtener más información sobre las programaciones de grupo y de nivel del sistema, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Crear programación</a>.</p> <p><b>IMPORTANTE</b>: Workfront utiliza la programación de un usuario solamente cuando la opción Calcular disponibilidad de recursos mediante está establecida en El horario del usuario. Para obtener información acerca de cómo la opción Calcular disponibilidad de los recursos mediante afecta a la programación que se utiliza para la administración de recursos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurar preferencias de administración de recursos</a>.</p> </li> 
       <li> <p><b>Perfil de plantilla de horas</b>: asocie un perfil de plantilla de horas con los usuarios. Esto garantiza que las plantillas de horas se generen automáticamente para los usuarios.</p> 
       <p><b>NOTA</b>:  
       <ul> 
       <li>La lista de perfiles de plantillas de horas que tiene disponibles en este campo depende de su acceso:
       <ul>
       <li>Como administrador de Workfront, puede ver todos los perfiles de plantillas de horas de nivel del sistema y de nivel de grupo.</li>
       <li><p>Como administrador de grupos, puede ver perfiles de plantillas de horas de nivel del sistema, así como los asociados con los grupos que administra.</p></li>
       <li><p>Como usuario con una licencia de Planificador y acceso para editar usuarios, solo puede ver perfiles de plantillas de horas en el sistema.</p></li>
       </ul></li> 
       <li>Si es administrador de grupos, todos los usuarios que esté editando deben ser miembros de un grupo que administre.</li> 
       </ul> </p> </li> 
       <li><b>Tipo de hora predeterminado</b>: seleccione el tipo de hora predeterminado para los usuarios. Es el tipo de hora que se utiliza de forma predeterminada cuando los usuarios registran el tiempo.</li> 
       <li> <p><b>Tipos de horas disponibles</b>: seleccione los tipos de horas que deben estar disponibles para el usuario. Estos tipos de horas son visibles en todas partes en Workfront, donde los usuarios pueden registrar la hora. Un usuario solo puede ver los tipos de horas que están habilitados en el nivel de proyecto y en el nivel de usuario.</p> 
       <p>Para obtener más información acerca de los tipos de horas que están disponibles para los usuarios, consulte <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Definición de tipos de horas y disponibilidad</a>.</p> 
       </li> 
       <li> <b>FTE</b>: es el equivalente a jornada completa del usuario. Workfront utiliza este número para calcular la disponibilidad del usuario según el horario predeterminado, solo cuando las Preferencias de administración de recursos del sistema están definidas en El horario predeterminado.

   <p>El valor de FTE indica la cantidad de tiempo que el usuario puede pasar en el trabajo. Esto incluye la sobrecarga, así como el tiempo empleado en el trabajo del proyecto. Por ejemplo, el tiempo empleado en reuniones o en formación también se incluye en el EJC.</p>

   El valor de FTE debe ser un número decimal de hasta 1 y no puede ser 0. Por ejemplo, si el valor de EJC es 0,5 y el horario predeterminado en Workfront son 40 horas, el usuario estará disponible durante 20 horas a la semana.

   El valor predeterminado del campo es 1.

   Las excepciones de horario, los días libres y el valor del Tiempo de trabajo pueden afectar a la disponibilidad del usuario.

   Workfront calcula la disponibilidad de un usuario según las preferencias de Administración de recursos del área de Configuración.

   Si las Preferencias de administración de recursos en el nivel del sistema se establecen en El horario del usuario, el valor especificado aquí se ignorará y el usuario se considerará disponible según lo especificado en su horario.

   Para obtener más información, consulte <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar las preferencias de administración de recursos</a>.

   Para obtener más información acerca de cómo crear programaciones en Workfront, vea <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Crear una programación</a>.
   </li> 
       <li> <p><b>Conjuntos de recursos</b>: asocie los usuarios a los conjuntos de recursos.</p> <p><b>NOTA</b>: En este campo solo aparecen los conjuntos de recursos comunes a todos los usuarios seleccionados en este campo. Si los usuarios seleccionados no tienen conjuntos de recursos compartidos, este campo está vacío. Si este campo está vacío, los conjuntos de recursos que especifique aquí sobrescribirán sus conjuntos de recursos individuales.</p> 
       <p>Para obtener más información sobre los conjuntos de recursos, vea <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref">Información general sobre los conjuntos de recursos</a>.</p> </li> 
       <li><b>Coste por hora</b>: importe en coste por hora para el usuario. </li> 
       <li><b>Facturación por hora</b>: importe de facturación por hora para el usuario.</li> 
       <li><b>Formularios personalizado</b>: asocie un formulario personalizado de usuario existente con los usuarios. Debe crear un formulario personalizado para poder asociarlo a un usuario. En la lista solo se muestran los formularios personalizados activos. Para obtener información sobre cómo crear formularios personalizados, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Crear un formulario personalizado</a>.</li> 
       <li><b>Comentario</b>: escriba un comentario en el campo proporcionado. Todos los usuarios seleccionados recibirán una notificación dentro de la aplicación, así como una notificación por correo electrónico con su comentario. El comentario se muestra en la pestaña Actualizaciones del perfil de los usuarios.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) En la sección **Formularios personalizado**, seleccione la opción **Volver a calcular expresiones personalizadas** para asegurarse de que todos los campos personalizados calculados en formularios personalizados adjuntos a los usuarios seleccionados estén actualizados.

1. Haga clic en **Guardar cambios**.
