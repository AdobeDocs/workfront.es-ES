---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Agregar usuarios
description: Como administrador de Workfront o usuario con acceso administrativo total, puede agregar usuarios en Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: 198129edd8690393e3214f5041b183b5516617a7
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 1%

---

# Agregar usuarios

<!--Audited 2/2024-->

>[!IMPORTANT]
>
>Si su organización se ha incorporado a Adobe Admin Console, debe crear administradores del sistema a través de Adobe Admin Console.
>
>Para obtener instrucciones sobre cómo crear administradores de sistemas en Adobe Admin Console, consulte [Administrar administradores de sistemas en Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).
>
>Los administradores de grupo de las organizaciones que se han incorporado a Adobe Admin Console pueden utilizar este procedimiento para crear usuarios y enviar al usuario para su aprobación por parte de la administración.
>
>Para obtener una lista de procedimientos que difieren según si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en la plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Puede añadir usuarios en Adobe Workfront creando usuarios individuales desde cero o copiando los existentes.

Para obtener información sobre cómo importar varios usuarios simultáneamente, vea [Importar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

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
   <td><p>Nuevo: estándar</p><p>O</p><p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe tener uno de los siguientes:</p> 
    <ul> 
     <li> <p>El nivel de acceso del administrador del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo completo a un usuario</a>. </p> </li> 
     <li> <p>Configuración de <b>usuarios</b> en su nivel de acceso configurado para el acceso de <b>Editar</b>, con <b>Crear</b> y al menos una de las dos opciones de <b>Administrador de usuarios</b> habilitadas en <b>Ajustar la configuración</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De estas dos opciones, si el usuario <b>Admin (usuarios del grupo)</b> está habilitado, debe ser administrador de un grupo del que el usuario sea miembro.</p> <p>Para obtener más información sobre la configuración de <b>Usuarios</b> en un nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a usuarios</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Requisitos previos

Antes de agregar un usuario, recopile la información sobre el usuario que se muestra a continuación y determine qué información desea asociar con ese usuario:

* ¿Cuál es la información personal del usuario? Como mínimo, necesita lo siguiente:

   * Nombre completo
   * Un nombre de usuario
   * Contraseña predeterminada
   * Dirección de correo electrónico

  >[!NOTE]
  >
  >Puede determinar si los usuarios pueden ver la información de contacto de otros usuarios ajustando la configuración de Vista de usuarios al especificar niveles de acceso para objetos de Workfront. Para obtener más información, vea [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* ¿Cuál es la posición del nuevo usuario dentro de la empresa? ¿Tiene esta persona algún informe directo? ¿A quién reporta esta persona?
* ¿Qué función desempeña la persona? ¿Existe esta función en Workfront? ¿Hay un límite en el número de personas que pueden desempeñar este rol? Para obtener información sobre cómo crear roles, consulte [Crear y administrar roles](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
* ¿Qué nivel de acceso debe tener el usuario? ¿Ya existe o necesita crear una nueva? Para obtener más información, vea [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
* ¿En qué grupo de inicio debe estar este usuario? ¿Debe la persona estar en más de un grupo? Para obtener información acerca de los grupos, vea [Información general de grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* ¿En qué equipo de inicio debe estar este usuario? ¿Debe la persona estar en más de un equipo? Para obtener información sobre los equipos, vea [Información general de los equipos](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* ¿Qué información personalizada necesita asociar con este usuario?

  Si la información sobre los usuarios se captura en los campos personalizados que ha creado, debe tener preparado un formulario personalizado al crear un usuario. Para obtener información acerca de los formularios personalizados, vea [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Crear un usuario desde cero

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Usuarios** ![](assets/users-icon-in-main-menu.png).

1. Haga clic en **Nuevo usuario > Nuevo usuario** para agregar un usuario que aún no se haya agregado a Workfront.

   O

   Haga clic en **Nuevo usuario > Importar usuarios** para agregar usuarios al cargar un archivo de importación de hoja de cálculo.

   Si está importando usuarios, no es necesario que continúe con estos pasos. Para obtener más información, consulte [Importar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. En el cuadro **Nuevo usuario** que aparece, haga clic en **Mostrar opciones avanzadas** y, a continuación, configure las opciones disponibles para escribir la información de la persona.

   Para obtener información acerca de estas opciones, vea [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Realice una de las siguientes acciones:

   * Dejar **Enviado un correo electrónico de invitación a esta persona** habilitado. En este caso, el usuario recibe un correo electrónico en el que puede seguir un vínculo para crear su propia contraseña para Workfront. Los usuarios que no aceptan la invitación por correo electrónico y crean una contraseña de Workfront aparecen como No registrados en Workfront.
   * Deshabilite **Envíe un correo electrónico de invitación a esta persona**, luego escriba una **Contraseña** para la persona y confírmela en el cuadro **Confirmar contraseña**. Deberá compartir esta contraseña con el usuario fuera de Workfront.

   >[!NOTE]
   >
   >* Si el administrador de Workfront ha habilitado una integración de SSO con Workfront, el campo Permitir solo la autenticación &lt;configuración de SSO> se oculta si desactiva la invitación por correo electrónico. El campo ID de federación o &lt;SSO Configuration> nombre de usuario permanece visible.
   >
   * Si su organización se ha incorporado al Admin Console y agrega un usuario a través de Workfront, no tiene la opción de enviar una invitación por correo electrónico.
   >
   Para los usuarios de Adobe existentes, el usuario puede recibir o no un correo electrónico sobre la disponibilidad de Workfront. Es una preferencia controlada por el administrador de Adobe para el producto.

1. Haga clic en **Agregar esta persona**.

   O

   Haga clic en **Agregar persona y comenzar otra** para guardar el nuevo usuario y agregar otro.

   >[!NOTE]
   >
   Si es administrador de un grupo y agrega un usuario a una organización que se ha incorporado a Adobe Admin Console, las opciones de este paso son **Enviar usuario para la aprobación del administrador** y **Enviar para aprobación e iniciar otro**. El usuario se crea con un estado de Desactivado y Pendiente de aprobación. Un administrador de Workfront debe aprobar el usuario, quien lo activa en Workfront y lo añade a Adobe Admin Console.

## Copiar un usuario para crear uno nuevo

Puede crear un usuario copiando un usuario existente.

>[!NOTE]
>
Cuando crea un usuario de esta manera, toda la información se copia del usuario original al usuario recién creado, excepto para lo siguiente:
>
* La información de la sección Información personal.
* Al iniciar sesión, mostrar: La pestaña de aterrizaje predeterminada del nivel de acceso está seleccionada en este cuadro.
* Subordinados directos
>

Para crear un nuevo usuario copiando uno existente:

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Usuarios** ![](assets/users-icon-in-main-menu.png).
1. Seleccione el usuario que desea copiar y luego haga clic en el icono Copiar ![](assets/copy-icon.png).
1. En el cuadro **Copiar usuario** que aparece, edite los campos disponibles para el nuevo usuario.

   Para obtener información acerca de todos los campos asociados con un usuario, vea [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Haga clic en **Agregar esta persona**.

   O

   Haga clic en **Agregar persona y comenzar otra** para guardar el nuevo usuario y agregar otro.

Esto crea una nueva cuenta en Workfront para el usuario.

Si ha seleccionado la opción para enviar una invitación al usuario, este debería recibir un correo electrónico donde pueda seguir un vínculo para crear su contraseña de Workfront.

>[!NOTE]
>
Si su organización se ha incorporado al Admin Console y agrega un usuario a través de Workfront, no tiene la opción de enviar una invitación por correo electrónico.
>
Para los usuarios de Adobe existentes, el usuario puede recibir o no un correo electrónico sobre la disponibilidad de Workfront. Es una preferencia controlada por el administrador de Adobe para el producto.
