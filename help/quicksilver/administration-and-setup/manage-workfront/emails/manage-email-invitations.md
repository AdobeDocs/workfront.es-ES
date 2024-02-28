---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Administrar invitaciones por correo electrónico a nuevos usuarios
description: Como administrador de Adobe Workfront, puede agregar usuarios a Workfront y notificarles que han sido agregados mediante invitaciones por correo electrónico.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: e13e3479-391f-4aec-b998-e9b6057f256b
source-git-commit: 1c0a656f2603c5decabd2bb4e88da1b9530f9e1c
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 0%

---

# Administrar invitaciones por correo electrónico a nuevos usuarios

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>El procedimiento descrito en esta página se aplica sólo a las organizaciones que aún no se han incorporado al Admin Console. Si su organización se ha incorporado a Adobe Admin Console, debe realizar esta acción a través de Adobe Admin Console.
>
>Para obtener una lista de procedimientos que difieren en función de si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en la plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador de Adobe Workfront, puede agregar usuarios a Workfront y notificarles que han sido agregados mediante invitaciones por correo electrónico.

La invitación por correo electrónico permite a los nuevos usuarios seguir un vínculo en el que pueden elegir una contraseña para su cuenta de Workfront. Luego pueden terminar de configurar su cuenta.

Para garantizar la seguridad de las nuevas cuentas, le recomendamos que utilice invitaciones por correo electrónico para los nuevos usuarios, de modo que puedan elegir su propia contraseña. También puede seleccionar una contraseña para un nuevo usuario al crear su cuenta. Para obtener más información sobre cómo agregar nuevos usuarios a Workfront, consulte [Adición de usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Puede configurar los nuevos correos electrónicos de los usuarios para:

* Cualquier nuevo usuario agregado a Workfront
* Usuarios añadidos a Workfront con una licencia de solicitante

Todos los usuarios nuevos ven el mismo correo electrónico cuando se envía una invitación por correo electrónico.

Para obtener información sobre la recepción de invitaciones por correo electrónico, consulte [Reciba invitaciones por correo electrónico y cree una contraseña para Adobe Workfront](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

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
   <td> <p>Administrador del sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

## Generar invitaciones por correo electrónico {#generate-email-invitations}

Las invitaciones por correo electrónico se generan en los siguientes casos:

* Cuando crea un nuevo usuario y selecciona la variable **Enviar invitación por correo electrónico a esta persona.** en el **Nuevo usuario** formulario. Para obtener más información sobre la creación de usuarios nuevos, consulte [Adición de usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Cuando se importan varios usuarios nuevos y se selecciona la variable **Enviar invitación por correo electrónico a estas personas.** opción. Para obtener más información sobre cómo importar varios usuarios nuevos, consulte [Importar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).
* Una vez creados los usuarios, puede generar manualmente las invitaciones a los usuarios que aún no hayan registrado su cuenta en Workfront y que no hayan establecido una contraseña de Workfront.\
  Los usuarios que tienen una cuenta creada pero que aún no han registrado su cuenta se marcan como **No registrado** en Workfront.

  >[!NOTE]
  >
  >Si anula la selección de **Enviar una invitación por correo electrónico a esta persona** casilla al crear el usuario, la invitación por correo electrónico no se puede generar manualmente. El reenvío manual de las invitaciones por correo electrónico solo es posible para los usuarios a los que se les ha enviado la invitación por correo electrónico original cuando se creó su cuenta. Para obtener más información sobre la creación de usuarios nuevos, consulte [Adición de usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Para generar manualmente invitaciones por correo electrónico a usuarios no registrados existentes:

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Usuarios** ![](assets/users-icon-in-main-menu.png).
1. Seleccione el usuario que muestra la variable **No registrado** después del nombre.

   ![](assets/unreg-user-qs-350x221.png)

1. Haga clic en el icono Más ![](assets/more-icon.png), luego haga clic en **Recordar al usuario registrarse**.

   Se envía una invitación por correo electrónico al nuevo usuario con un nuevo vínculo que puede utilizar para crear su contraseña de Workfront.

   >[!NOTE]
   >
   >Si su organización se ha incorporado al Admin Console y agrega un usuario a través de Workfront, no tiene la opción de enviar una invitación por correo electrónico a los nuevos usuarios.
   >
   >Los nuevos usuarios de Adobe se añaden al Admin Console Admin Console y este envía un correo electrónico para invitarlos a completar el proceso de registro. Todos los usuarios deben completar el proceso de registro para acceder a cualquier sistema de Adobe.
   >
   >Para los usuarios de Adobe existentes, el usuario puede recibir o no un correo electrónico sobre la disponibilidad de Workfront. Es una preferencia controlada por el administrador de Adobe para el producto.

## Configurar invitaciones por correo electrónico {#configure-email-invitations}

Como administrador de Workfront, puede configurar el mensaje que incluye con las invitaciones por correo electrónico para nuevos usuarios.

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. En la lista de la izquierda, haga clic en **Correo electrónico** > **Invitaciones**.

1. En el **Opciones generales** , realice cualquiera de las siguientes modificaciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Desactivar vínculos de invitación después de ... días</strong> </td> 
      <td> <p>Elija la cantidad de tiempo después de la cual las invitaciones por correo electrónico ya no contienen un vínculo válido a Workfront. La cantidad predeterminada de días es 45.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Incluir un mensaje y/o un término de servicio</strong> </td> 
      <td> <p>Seleccione esta opción si desea modificar la invitación por correo electrónico de todos los usuarios nuevos agregados a Workfront. Esto no incluye a los usuarios con una licencia de solicitante.</p> 
       <ul> 
        <li><strong>Mensaje</strong>: si selecciona modificar la invitación por correo electrónico para todos los usuarios nuevos, especifique el texto que desea incluir en las invitaciones por correo electrónico como cuerpo del correo electrónico.</li> 
        <li><strong>Términos y condiciones</strong>: si selecciona modificar la invitación por correo electrónico para todos los usuarios nuevos, especifique el texto que desea incluir en las invitaciones por correo electrónico como términos y condiciones.<br></li> 
        <li><strong>Incluir un mensaje o un término de servicio para los usuarios del servicio de asistencia</strong>: seleccione esta opción si desea modificar la invitación por correo electrónico de todos los usuarios nuevos añadidos a Workfront que tengan una licencia de solicitante.</li> 
        <li><strong>Mensaje</strong>: si selecciona modificar la invitación por correo electrónico para todos los usuarios nuevos con una licencia de solicitante, especifique el texto que desea incluir en las invitaciones por correo electrónico como cuerpo del correo electrónico.</li> 
        <li><strong>Términos y condiciones</strong>: si selecciona modificar la invitación por correo electrónico para todos los usuarios nuevos con una licencia de solicitante, especifique el texto que desea incluir en las invitaciones por correo electrónico como términos y condiciones.<br></li> 
        <li> <p>En el <strong>Previsualización de invitación</strong> , puede ver una previsualización de su invitación por correo electrónico. Si ha seleccionado incluir un mensaje personalizado en la invitación por correo electrónico, el mensaje personalizado se muestra en esta área.</p> <p> <img src="assets/email-invitation-for-all-users-preview-qs-350x190.png" style="width: 350;height: 190;"> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.
