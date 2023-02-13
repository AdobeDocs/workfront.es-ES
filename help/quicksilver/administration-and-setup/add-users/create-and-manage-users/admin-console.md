---
title: Administrar usuarios en Adobe Admin Console
description: Como administrador de Adobe, puede crear usuarios de Adobe Workfront y administradores de sistemas mediante Adobe Admin Console.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: ae657964-d4a5-4c3b-afc6-8dde7695955d
source-git-commit: 9bcd792139f8f2f0198da943e5c63a2add32e856
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 0%

---

# Administrar usuarios en Adobe Admin Console

>[!IMPORTANT]
>
>La funcionalidad de este artículo solo está disponible si la instancia de Workfront de su organización se ha incorporado a la plataforma empresarial de Adobe.
>
>Para obtener una lista de procedimientos que difieren en función de si su organización ha sido incorporada a la plataforma empresarial de Adobe, consulte [Diferencias de administración basadas en plataformas (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador de Adobe, puede crear usuarios de Adobe Workfront y administradores de sistemas mediante Adobe Admin Console. La consola es una ubicación central para administrar las autorizaciones de Adobe en toda la organización. Para obtener más información, consulte la [Información general del Admin Console](https://helpx.adobe.com/es/enterprise/using/admin-console.html).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Derechos de administrador de Adobe</td> 
   <td> <p>Debe ser administrador de configuración de producto de productos de Adobe para su organización</p> </td> 
  </tr> 
 </tbody> 
</table>

## Requisitos previos

Antes de usar el Admin Console para Workfront, debe recibir un mensaje de correo electrónico que le invite a la consola.

1. Si es nuevo en el Adobe y ha recibido un correo electrónico que le informa de que ahora tiene derechos de administración para administrar el software y los servicios de Adobe de su organización, haga clic en el botón del correo electrónico para crear una cuenta de Adobe y abrir el Admin Console.

   O

   Si ya tiene una cuenta de Adobe, vaya a la [Página de Adobe Admin Console](https://adminconsole.adobe.com/).

## Acceda al área de usuario y administrador de la instancia de producción de Workfront {#access-the-user-and-admin-area-for-your-production-instance-of-workfront}

1. En el [Página de Adobe Admin Console](https://adminconsole.adobe.com/), seleccione **Productos** en la barra de navegación superior y, a continuación, seleccione la **Workfront** mosaico del producto.

   ![](assets/admin-product-1.png)

1. En la lista que aparece, seleccione el vínculo en la parte superior.

   Esta es la instancia de producción en la que trabajan los usuarios.

   ![](assets/instances-1.png)

   >[!TIP]
   >
   >La instancia de Vista previa, el segundo vínculo de la lista, es un entorno de prueba que duplica el entorno de producción activo. Para obtener más información, consulte [Entorno de espacio aislado de vista previa de Adobe Workfront](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).
   >
   >
   >También puede ver vínculos a entornos de simulación de pruebas en la lista. Para obtener más información, consulte [Entorno de espacio aislado de vista previa de Adobe Workfront](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

1. En la lista que se muestra, con la variable **Perfiles de producto** seleccione la pestaña , haga clic en el nombre del vínculo Perfil de producto de Workfront .

   ![](assets/prod-profile-1.png)

   Esta lista incluye todos los usuarios que ya están asignados a la instancia Producción de Workfront.

   >[!IMPORTANT]
   >
   >No realice ningún cambio en el propio perfil de producto.

1. Continúe con una de las siguientes secciones de este artículo:

   * [Crear usuarios en Workfront con Adobe Admin Console](#create-users-in-workfront-with-the-adobe-admin-console)
   * [Cree administradores de sistema en Workfront con Adobe Admin Console](#create-system-administrators-in-workfront-with-the-adobe-admin-console)

## Crear usuarios en Workfront con Adobe Admin Console {#create-users-in-workfront-with-the-adobe-admin-console}

1. Vaya al área de usuario y administrador del Admin Console, tal como se describe en [Acceda al área de usuario y administrador de la instancia de producción de Workfront](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) en este artículo.
1. Con la variable **Usuarios** ficha seleccionada encima de la lista, seleccione **Agregar usuario**.
1. En el **Agregar usuarios a este perfil de producto** , introduzca la dirección de correo electrónico o el nombre de un usuario que desea agregar y, a continuación, seleccione **Guardar**.

   El usuario se crea en Workfront con el nivel de acceso Solicitante .

   >[!IMPORTANT]
   >
   >No realice ningún cambio en el propio perfil de producto.

1. En Workfront, cambie el nivel de acceso del usuario.

   Para obtener instrucciones sobre cómo un administrador de Workfront puede cambiar el nivel de acceso del usuario, consulte [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Repita los pasos 3 y 4 para agregar más usuarios.

   >[!NOTE]
   >
   >Para los nuevos usuarios de Adobe, el Admin Console envía un correo electrónico para invitarlos a completar el proceso de registro. Todos los usuarios deben completar el proceso de registro para acceder a cualquier sistema de Adobe.
   >
   >Para los usuarios de Adobe existentes, es posible que el usuario reciba o no un correo electrónico acerca de la disponibilidad de Workfront. Se trata de una preferencia controlada por el administrador de Adobe del producto.

## Cree administradores de sistema en Workfront con Adobe Admin Console {#create-system-administrators-in-workfront-with-the-adobe-admin-console}

El nivel de acceso del administrador del sistema solo se concede en Adobe Admin Console. No puede conceder ni eliminar el acceso de administrador desde Workfront.

Debe agregar un usuario a la instancia Producción de Workfront para poder convertirlo en administrador del sistema de Workfront. Para obtener instrucciones, consulte [Crear usuarios en Workfront con Adobe Admin Console](#create-users-in-workfront-with-the-adobe-admin-console) en este artículo.

1. Vaya al área de usuario y administrador del Admin Console, tal como se describe en [Acceda al área de usuario y administrador de la instancia de producción de Workfront](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) en este artículo.
1. Seleccione el **Administradores** sobre la lista de usuarios.
1. Select **Agregar administrador**.
1. En el **Agregar administradores de perfil de producto** , introduzca las direcciones de correo electrónico o los nombres de los administradores que desea añadir y, a continuación, seleccione **Guardar**.

   ![](assets/add-admin-1.png)

   Los administradores del sistema se crean en Workfront.

   >[!IMPORTANT]
   >
   >No realice ningún cambio en el propio perfil de producto.

## Detalles adicionales sobre Adobe Admin Console:

* Los administradores del sistema de Workfront pueden desactivar un usuario de Workfront desde Workfront, pero esto no desactiva al usuario en el Admin Console.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about deactivating a user in Workfront, see </p>
  -->

* El usuario **Grupo de inicio** se determina en función del usuario que los creó. Actualmente no se puede personalizar desde el Admin Console .
* El nivel de acceso del administrador del sistema de Workfront solo se puede editar desde Adobe Admin Console.

   <!--
  DRAFTED IN FLARE:
  How is this done?
  
  -->

* La edición de un usuario que es administrador del sistema en cualquier otro nivel de acceso debe realizarse primero a través del Admin Console.

   <!--
   This is not clear
  -->

* Para eliminar el acceso de administrador del sistema de un usuario en Workfront, debe utilizar Adobe Admin Console para eliminar el usuario como administrador de perfil de producto. Esto cambia el nivel de acceso de Workfront del usuario de Administrador del sistema a Solicitante.

   >[!IMPORTANT]
   >
   >No realice ningún cambio en el propio perfil de producto.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>You can create Adobe Workfront users and system administrators with the <a href="https://adminconsole.adobe.com/" alt="Admin Console link">Adobe Admin Console</a>. The console is a central location for managing the Adobe entitlements across your organization. For more information, see the <a href="https://helpx.adobe.com/enterprise/using/admin-console.html" alt="Admin Console Overview">Admin Console Overview</a>.</p>
<p>Before using the Admin Console for Workfront, you should receive a receive an email inviting you to the console. Click in the invitation to accept it and create an account. You can also use an existing account, if already available.</p>
<h2>Create users</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Create users in WF with the Adobe admin console</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">May need to add something about oging throug WF -- check with Jonah</p>

<p>To create users in Workfront with the Admin Console:</p>
<ol>
<li value="1"> <p>From the <a href="https://adminconsole.adobe.com/">Admin Console page</a>, select the <b>Products</b> tab and then select the <b>Workfront</b> product tile.</p> </li>
<li value="2"> <p>Select the link to the Workfront instance you want to change.</p> </li>
<li value="3"> <p>Select the Product profile link. This shows a list of the currently-assigned users. If the list is very long, you can also search for users in the search field above the list.</p> </li>
<li value="4"> <p>Select the <b>Add User</b> button.</p> </li>
<li value="5"> <p>In the <b>Add users</b> box, enter the email address or name of the user you want to add. Select <b>Save</b>. The administrator is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Create system administrators</h2>
<p>To create system administrators:</p>
<ol>
<li value="1"> <p>Make product profile assignments first. To be a Workfront System Administrator, the user must be assigned the Workfront product profile and be an admin for that product profile.</p> </li>
<li value="2"> <p>From the console, select the <b>Products</b> tab and then select the <b>Admins</b> tab. </p> </li>
<li value="3"> <p>Select <b>Add Admin</b>.</p> </li>
<li value="4"> <p>In the <b>Add product profile administrators</b> box, enter the email address or name of the administrator you want to add. Select <b>Save</b>. The user is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Additional details for the Admin Console</h2>
<ul>
<li> <p>System Administrator access level is granted only on the Admin Console. You cannot grant or remove admin access from within Workfront.</p> </li>
</ul>
<ul>
<li> <p>Creating and deleting users inside Workfront is only possible through the Admin Console.</p> </li>
<li> <p>Workfront System Administrators can deactivate Workfront users from within Workfront, but this does not deactivate the user in the Admin Console.</p> </li>
<li> <p>All new users are are assigned <b>Requestor</b> access level upon creation. Also, the user <b>Home Group</b> is determined based on the user who created them. This is currently not customizable from within the Admin Console.</p> </li>
<li> <p>The Workfront System Administrator access level can only be edited from within the Adobe Admin Console.</p> </li>
<li> <p>Editing a user who is a system admin to any other access level must be done through the Admin Console first.</p> </li>
<li> <p>To remove Workfront system admin access, remove users as Product Profile Administrators. This action changes the user access level in Workfront from a system admin to a <b>Requestor</b>.</p> </li>
</ul>
</div>
-->
