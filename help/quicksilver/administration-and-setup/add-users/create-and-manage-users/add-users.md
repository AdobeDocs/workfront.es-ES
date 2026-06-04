---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Agregar usuarios
description: Como persona con la función de administrador de Workfront o usuario con acceso administrativo total, puede añadir usuarios en Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
TQID: https://experienceleague.adobe.com/TeDJRpOI2i7PQIb-ImUyHTTi0ETJ7pZcOVRM3WMQhWY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1221
ht-degree: 77%

---

# Agregar usuarios

<!--Audited 2/2024-->

>[!IMPORTANT]
>
>* **Debe crear administradores de sistema mediante Adobe Admin Console.**
>
>   Para obtener instrucciones sobre cómo crear administradores de sistemas en Adobe Admin Console, consulte [Administrar usuarios en Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).
>
>   Los administradores de grupo de las organizaciones que se han incorporado a Adobe Admin Console pueden utilizar este procedimiento para crear usuarios y enviarlos para su aprobación por parte de la administración.
>
>   Para obtener una lista de procedimientos que difieren según si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración entre Adobe Workfront y Adobe Business Platform](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
>* **Si su organización utiliza el inicio de sesión único (SSO)**, le recomendamos que cree usuarios y los asigne a Workfront en Adobe Admin Console. Es posible crear estos usuarios en Workfront, pero puede haber problemas para transferir esa información a Adobe Admin Console, según la configuración de Admin Console de su organización.
>   Después de crear el usuario en Adobe Admin Console, puede configurar la información del usuario en Workfront, como la asignación de funciones, grupos, equipos y niveles de acceso.
>* **Si su organización no utiliza el inicio de sesión único (SSO)**, puede añadir usuarios que no sean administradores del sistema directamente en Workfront. Es posible agregar usuarios en Adobe Admin Console, pero añadirlos en Workfront le permite establecer su nivel de acceso mientras los crea, lo que le puede ahorrar tiempo.



<!--

You can add users in Adobe Workfront by creating individual users from scratch or by copying existing users.

For information about how to import multiple users simultaneously, see [Import users](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

-->

Como administrador de Adobe, puede añadir usuarios en Adobe Workfront agregándolos al perfil de producto de Workfront en Adobe Admin Console. Para obtener instrucciones, consulte [Administrar usuarios en Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Debe tener uno de los siguientes elementos:</p> 
    <ul> 
     <li> <p>El nivel de acceso de administrador del sistema. </li> 
     <li> <p>Configuración de <b>usuarios</b> en su nivel de acceso configurado para el acceso de <b>Edición</b>, con <b>Crear</b> y al menos una de las dos opciones de <b>Administrador de usuarios</b> habilitadas en <b>Ajustar la configuración</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De estas dos opciones, si <b>Administrador de usuarios (usuarios de grupo)</b> está habilitado, debe ser administrador de grupo de un grupo al que pertenezca el usuario.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Antes de añadir un usuario, recopile la información sobre el usuario enumerada a continuación y determine qué información desea asociar a ese usuario:

* ¿Cuál es la información personal del usuario? Como mínimo, necesita lo siguiente:

   * Nombre completo
   * Nombre de usuario
   * Contraseña predeterminada
   * Dirección de correo electrónico

  >[!NOTE]
  >
  >Puede determinar si los usuarios pueden ver la información de contacto de otros usuarios ajustando la opción Vista de usuarios al especificar niveles de acceso para objetos de Workfront. Para obtener más información, consulte [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* ¿Cuál es la posición del nuevo usuario en la compañía? ¿Tiene esta persona subordinados directos? ¿A quién rinde cuentas esta persona?
* ¿Qué función desempeña la persona? ¿Existe esta función en Workfront? ¿Hay un límite en el número de personas que pueden desempeñar esta función? Para obtener información sobre la creación de funciones, consulte [Crear y administrar funciones](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
* ¿Qué nivel de acceso debe tener el usuario? ¿Ya existe o necesita crear uno nuevo? Para obtener más información, consulte [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
* ¿En qué grupo de inicio debe estar este usuario? ¿Debe la persona estar en más de un grupo? Para obtener información acerca de los grupos, consulte [Información general sobre los grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* ¿En qué equipo de inicio debe estar este usuario? ¿Debería estar esta persona en más de un equipo? Para obtener más información sobre los equipos, vea [Información general sobre los equipos](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* ¿Qué información personalizada necesita asociar con este usuario?

  Si la información sobre los usuarios se captura en los campos personalizados que ha creado, debe tener preparado un formulario personalizado al crear un usuario. Para obtener información acerca de los formularios personalizados, vea [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Crear un usuario desde cero

{{step-1-to-users}}

1. Haga clic en **Nuevo usuario > Nuevo usuario** para añadir un usuario que aún no se haya añadido a Workfront.

   O

   Haga clic en **Nuevo usuario > Importar usuarios** para añadir usuarios al cargar un archivo de importación de hoja de cálculo.

   Si está importando usuarios, no es necesario que continúe con estos pasos. Para obtener más información, consulte [Importar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. En el cuadro **Nuevo usuario** que aparece, haga clic en **Mostrar opciones avanzadas** y, a continuación, configure las opciones disponibles para escribir la información de la persona.

   Para obtener más información acerca de estas opciones, vea [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Realice una de las siguientes acciones:

   * Deje la opción **Enviar invitación por correo electrónico a esta persona** habilitada. En este caso, el usuario recibe un correo electrónico en el que puede seguir un vínculo para crear su propia contraseña para Workfront. Los usuarios que no aceptan la invitación por correo electrónico y crean una contraseña de Workfront aparecen como No registrados en Workfront.
   * Deshabilite **Enviar invitación por correo electrónico a esta persona**, luego escriba una **Contraseña** para esta y confírmela en el cuadro **Confirmar contraseña**. Deberá compartir esta contraseña con el usuario fuera de Workfront.

   >[!NOTE]
   >
   >* Si el administrador de Workfront ha habilitado una integración de SSO con Workfront, el campo Permitir solo la autenticación &lt;Configuración de SSO> se oculta si se desactiva la invitación por correo electrónico. El campo Identificador de federación o &lt;Configuración de SSO> Nombre de usuario permanece visible.
   >
   >* Como su organización se ha incorporado a Admin Console y usted agrega un usuario a través de Workfront, no tiene la opción de enviar una invitación por correo electrónico.
   >
   >   Para los usuarios de Adobe existentes, el usuario puede recibir o no un correo electrónico sobre la disponibilidad de Workfront. Esta es una preferencia que controla el administrador de Adobe del producto.

1. Haga clic en **Agregar esta persona**.

   O

   Haga clic en **Agregar persona y comenzar otra** para guardar el nuevo usuario y añadir otro.

   >[!NOTE]
   >
   >* Si es usted administrador de grupos y añade un usuario a una organización que se ha incorporado a Adobe Admin Console, las opciones de este paso son **Enviar usuario para la aprobación de Admin** y **Enviar para aprobación y empezar otro**. El usuario se crea con un estado de Desactivado y Pendiente de aprobación.
   > 
   >* Si el usuario no abandona los estados Desactivado y Aprobación pendiente en unos minutos y una actualización de la pantalla no elimina el distintivo Aprobación pendiente, puede aprobarlo manualmente.
   >
   >   1. Vaya a Configuración > Usuarios.
   >   1. Seleccione el usuario o usuarios en la lista Usuarios.
   >   1. Haga clic en el menú de tres puntos del encabezado de la lista.
   >   1. Seleccione **Aprobar**.
   >   1. Espere unos minutos y actualice la página.


## Copiar un usuario existente para crear uno nuevo

Puede crear un usuario copiando un usuario existente.

>[!NOTE]
>
>Cuando crea un usuario de esta manera, toda la información se copia del usuario original al usuario recién creado, excepto para los siguientes casos:
>
>* La información de la sección Información personal.
>* Al iniciar sesión, se muestra la pestaña de aterrizaje predeterminada del nivel de acceso está seleccionada en este cuadro.
>* Subordinados directos
>

Para crear un nuevo usuario copiando uno existente:

{{step-1-to-users}}

1. Seleccione el usuario que desea copiar y luego haga clic en el icono Copiar ![Icono Copiar](assets/copy-icon.png).
1. En el cuadro **Copiar usuario** que aparece, edite los campos disponibles para el nuevo usuario.

   Para obtener información acerca de todos los campos asociados con un usuario, vea [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Haga clic en **Agregar esta persona**.

   O

   Haga clic en **Agregar persona y comenzar otra** para guardar el nuevo usuario y añadir otro.

Esto crea una nueva cuenta en Workfront para el usuario.

Si ha seleccionado la opción para enviar una invitación al usuario, este debería recibir un correo electrónico donde pueda seguir un vínculo para crear su contraseña de Workfront.

>[!NOTE]
>
>Como su organización se ha incorporado a Admin Console y usted agrega un usuario a través de Workfront, no tiene la opción de enviar una invitación por correo electrónico.
>
>Para los usuarios de Adobe existentes, el usuario puede recibir o no un correo electrónico sobre la disponibilidad de Workfront. Esta es una preferencia que controla el administrador de Adobe del producto.
