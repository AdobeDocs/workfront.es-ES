---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Agregar usuarios
description: Como administrador de Workfront o usuario con acceso administrativo completo, puede agregar usuarios en Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: 9bcd792139f8f2f0198da943e5c63a2add32e856
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 1%

---

# Agregar usuarios

>[!IMPORTANT]
>
>El procedimiento descrito en esta página solo se aplica a organizaciones que aún no se han incorporado al Admin Console. Si su organización se ha incorporado a Adobe Admin Console, debe realizar esta acción a través de Adobe Admin Console.
>
>Para obtener instrucciones sobre cómo agregar un usuario en Adobe Admin Console:
>
>* Consulte [Crear usuarios en Workfront con Adobe Admin Console](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create)
>* Consulte la sección &quot;Agregar usuarios&quot; en el artículo [Administrar usuarios individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* Póngase en contacto con su administrador de Adobe Admin Console.
>
>Para obtener una lista de procedimientos que difieren en función de si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en plataformas (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Puede agregar usuarios en Adobe Workfront creando usuarios individuales desde cero o copiando a los existentes.

Para obtener información sobre cómo importar varios usuarios simultáneamente, consulte [Importar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

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

## Requisitos previos

Antes de agregar un usuario, recopile la información sobre el usuario que aparece a continuación y determine qué información desea asociar con ese usuario:

* ¿Cuál es la información personal del usuario? Como mínimo, necesita lo siguiente:

   * Nombre completo
   * Un nombre de usuario
   * Contraseña predeterminada
   * Dirección de correo electrónico

   >[!NOTE]
   >
   >Puede determinar si los usuarios pueden ver la información de contacto de otros usuarios ajustando la configuración Vista de usuarios al especificar los niveles de acceso para los objetos de Workfront. Para obtener más información, consulte [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* ¿Cuál es la posición del nuevo usuario dentro de la empresa? ¿Esta persona tiene algún informe directo? ¿A quién informa esta persona?
* ¿Qué función laboral cumple la persona? ¿Existe esta función de trabajo en Workfront? ¿Hay un límite en el número de personas que pueden desempeñar esta función laboral? Para obtener información sobre la creación de funciones de trabajo, consulte [Crear y administrar funciones de trabajo](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
* ¿Qué nivel de acceso debe tener el usuario? ¿Ya existe o necesita crear uno nuevo? Para obtener más información, consulte [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
* ¿En qué grupo de inicio debería estar este usuario? ¿Debería estar la persona en más de un grupo? Para obtener información sobre los grupos, consulte [Información general sobre grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* ¿En qué equipo de casa debería estar este usuario? ¿Debería la persona estar en más de un equipo? Para obtener información sobre los equipos, consulte [Información general sobre equipos](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* ¿Qué información personalizada necesita asociar con este usuario?

   Si la información sobre los usuarios se captura en los campos personalizados que ha creado, debe tener un formulario personalizado listo al crear un usuario. Para obtener información sobre los formularios personalizados, consulte [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Crear un usuario desde cero

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Usuarios** ![](assets/users-icon-in-main-menu.png).

1. Haga clic en **Nuevo usuario > Nuevo usuario** para agregar un usuario que aún no se haya agregado a Workfront.

   O

   Haga clic en **Nuevo usuario > Importar usuarios** para agregar usuarios cargando un archivo de importación de hoja de cálculo.

   Si va a importar usuarios, no es necesario que siga estos pasos. Para obtener más información, consulte [Importar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. En el **Nuevo usuario** que aparece, haga clic en **Mostrar opciones avanzadas** y, a continuación, configure las opciones disponibles para introducir la información de la persona.

   Para obtener información sobre estas opciones, consulte [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Realice una de las siguientes acciones:

   * Leave **Enviar un correo electrónico de invitación a esta persona** activada. Si lo hace, el usuario recibe un correo electrónico en el que puede seguir un vínculo para crear su propia contraseña para Workfront. Los usuarios que no acepten la invitación por correo electrónico y creen una contraseña de Workfront aparecen como No registrados en Workfront.
   * Deshabilitar **Enviar un correo electrónico de invitación a esta persona** y, a continuación, escriba un **Contraseña** para la persona y confírmela en el **Confirmar contraseña** en la ventana Deberá compartir esta contraseña con el usuario fuera de Workfront.

   >[!NOTE]
   >
   >Si el administrador de Workfront ha habilitado la integración de SSO con Workfront, la opción Solo permitir &lt;sso configuration=&quot;&quot;> El campo Autenticación está oculto si se desactiva la invitación por correo electrónico. El ID de federación o &lt;sso configuration=&quot;&quot;> El campo Nombre de usuario permanece visible.

   >[!NOTE]
   Si su organización se ha incorporado al Admin Console y usted agrega un usuario a través de Workfront, no tiene la opción de enviar una invitación por correo electrónico.
   Los nuevos usuarios de Adobe se añaden al Admin Console y el Admin Console envía un correo electrónico para invitarlos a completar el proceso de registro. Todos los usuarios deben completar el proceso de registro para acceder a cualquier sistema de Adobe.
   Para los usuarios de Adobe existentes, es posible que el usuario reciba o no un correo electrónico acerca de la disponibilidad de Workfront. Se trata de una preferencia controlada por el administrador de Adobe del producto.

1. Haga clic en **Agregar este usuario**.

   O

   Haga clic en **Agregar usuario de persona e iniciar otro** para guardar el nuevo usuario y agregar otro.

## Copiar un usuario para crear uno nuevo

Puede crear un usuario copiando un usuario existente.

>[!NOTE]
Cuando crea un usuario de esta forma, toda la información se copia del usuario original al usuario recién creado, excepto lo siguiente:
* La información de la sección Información personal .
* Cuando inicie sesión, muestre: La pestaña de aterrizaje predeterminada para el nivel de acceso está seleccionada en esta casilla.
* Subordinados directos
>


Para crear un nuevo usuario copiando uno existente:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Usuarios** ![](assets/users-icon-in-main-menu.png).
1. Seleccione el usuario que desea copiar y, a continuación, haga clic en el icono Copiar ![](assets/copy-icon.png).
1. En el **Nuevo usuario** que se muestra, edite los campos disponibles para el nuevo usuario.

   Para obtener información sobre todos los campos asociados a un usuario, consulte [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Haga clic en **Agregar este usuario**.

   O

   Haga clic en **Agregar usuario de persona e iniciar otro** para guardar el nuevo usuario y agregar otro.

Esto crea una nueva cuenta en Workfront para el usuario.

Si ha seleccionado la opción para enviar una invitación al usuario, debe recibir un correo electrónico en el que pueda seguir un vínculo para crear su contraseña de Workfront.

>[!NOTE]
Si su organización se ha incorporado al Admin Console y usted agrega un usuario a través de Workfront, no tiene la opción de enviar una invitación por correo electrónico.
Los nuevos usuarios de Adobe se añaden al Admin Console y el Admin Console envía un correo electrónico para invitarlos a completar el proceso de registro. Todos los usuarios deben completar el proceso de registro para acceder a cualquier sistema de Adobe.
Para los usuarios de Adobe existentes, es posible que el usuario reciba o no un correo electrónico acerca de la disponibilidad de Workfront. Se trata de una preferencia controlada por el administrador de Adobe del producto.
