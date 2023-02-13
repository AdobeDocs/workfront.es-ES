---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Administrar invitaciones por correo electrónico a nuevos usuarios
description: Como administrador de Adobe Workfront, puede agregar usuarios a Workfront y notificarles que se han agregado mediante invitaciones por correo electrónico.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: e13e3479-391f-4aec-b998-e9b6057f256b
source-git-commit: 9bcd792139f8f2f0198da943e5c63a2add32e856
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 1%

---

# Administrar invitaciones por correo electrónico a nuevos usuarios

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>El procedimiento descrito en esta página solo se aplica a organizaciones que aún no se han incorporado al Admin Console. Si su organización se ha incorporado a Adobe Admin Console, debe realizar esta acción a través de Adobe Admin Console.
>
>Para obtener una lista de procedimientos que difieren en función de si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en plataformas (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador de Adobe Workfront, puede agregar usuarios a Workfront y notificarles que se han agregado mediante invitaciones por correo electrónico.

La invitación por correo electrónico permite que los nuevos usuarios sigan un vínculo en el que pueden elegir una contraseña para su cuenta de Workfront. Luego pueden terminar de configurar su cuenta.

Para garantizar la seguridad de las nuevas cuentas, le recomendamos que utilice invitaciones por correo electrónico para los nuevos usuarios, de modo que puedan elegir su propia contraseña. También puede seleccionar una contraseña para un nuevo usuario al crear su cuenta. Para obtener más información sobre cómo agregar nuevos usuarios a Workfront, consulte [Agregar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Puede configurar los nuevos correos electrónicos de usuario para:

* Cualquier usuario nuevo agregado a Workfront
* Usuarios agregados a Workfront con una licencia de solicitante

Todos los usuarios nuevos ven el mismo correo electrónico cuando se envía una invitación por correo electrónico.

Para obtener información sobre la recepción de invitaciones por correo electrónico, consulte [Recibir invitaciones por correo electrónico y crear una contraseña para Adobe Workfront](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md).

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

* Al crear un nuevo usuario, seleccione la opción **Enviar un correo electrónico de invitación a esta persona** en el **Nuevo usuario** formulario. Para obtener más información sobre la creación de usuarios nuevos, consulte [Agregar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Al importar varios usuarios nuevos, seleccione la opción **Enviar correos electrónicos de invitación a estas personas** . Para obtener más información sobre la importación de varios usuarios nuevos, consulte [Importar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).
* Una vez creados los usuarios, puede generar manualmente las invitaciones a los usuarios que aún no hayan registrado su cuenta en Workfront y que no hayan establecido una contraseña de Workfront.\
   Los usuarios que tienen una cuenta creada pero aún no han registrado su cuenta se marcan como **No registrado** en Workfront.

   >[!NOTE]
   >
   >Si anula la selección de **Enviar una invitación por correo electrónico a esta persona** cuando crea el usuario, la invitación por correo electrónico no se puede generar manualmente. El reenvío manual de las invitaciones por correo electrónico solo es posible para los usuarios a los que se ha enviado la invitación por correo electrónico original cuando se creó su cuenta. Para obtener más información sobre la creación de usuarios nuevos, consulte [Agregar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Para generar manualmente invitaciones de correo electrónico para usuarios no registrados existentes:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Usuarios** ![](assets/users-icon-in-main-menu.png).
1. Seleccione el usuario que muestra la variable **No registrado** después de su nombre.

   ![](assets/unreg-user-qs-350x221.png)

1. Haga clic en el icono Más ![](assets/more-icon.png)y haga clic en **Recordar al usuario que se registre**.

   Se envía una invitación por correo electrónico al nuevo usuario con un nuevo vínculo que puede utilizar para crear su contraseña de Workfront.

   >[!NOTE]
   >
   >Si su organización se ha incorporado al Admin Console y usted agrega un usuario a través de Workfront, no tiene la opción de enviar una invitación por correo electrónico a los nuevos usuarios.
   >
   >Los nuevos usuarios de Adobe se añaden al Admin Console y el Admin Console envía un correo electrónico para invitarlos a completar el proceso de registro. Todos los usuarios deben completar el proceso de registro para acceder a cualquier sistema de Adobe.
   >
   >Para los usuarios de Adobe existentes, es posible que el usuario reciba o no un correo electrónico acerca de la disponibilidad de Workfront. Se trata de una preferencia controlada por el administrador de Adobe del producto.

## Configuración de invitaciones de correo electrónico {#configure-email-invitations}

Como administrador de Workfront, puede configurar el mensaje que incluye con las invitaciones de correo electrónico para nuevos usuarios.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En la lista de la izquierda, haga clic en **Correo electrónico** > **Invitaciones**.

1. En el **Opciones generales** , realice una de las siguientes modificaciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Desactivar vínculos de invitación después de ... días</strong> </td> 
      <td> <p>Elija el tiempo después del cual las invitaciones por correo electrónico ya no contienen un vínculo válido a Workfront. La cantidad predeterminada de días es 45.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Incluir un mensaje y/o un término de servicio</strong> </td> 
      <td> <p>Seleccione esta opción si desea modificar la invitación por correo electrónico para todos los usuarios nuevos agregados a Workfront. Esto no incluye a los usuarios con una licencia de Solicitante.</p> 
       <ul> 
        <li><strong>Mensaje</strong>: Si selecciona modificar la invitación por correo electrónico para todos los usuarios nuevos, especifique el texto que desea incluir en las invitaciones por correo electrónico como cuerpo del correo electrónico.</li> 
        <li><strong>Términos y condiciones</strong>: Si selecciona modificar la invitación por correo electrónico para todos los usuarios nuevos, especifique el texto que desea incluir en las invitaciones por correo electrónico como términos y condiciones.<br></li> 
        <li><strong>Incluir un mensaje o un término de servicio para los usuarios del servicio de asistencia</strong>: Seleccione esta opción si desea modificar la invitación por correo electrónico para todos los usuarios nuevos agregados a Workfront que tengan una licencia de Solicitante.</li> 
        <li><strong>Mensaje</strong>: Si selecciona modificar la invitación por correo electrónico para todos los usuarios nuevos con una licencia de solicitante, especifique el texto que desea incluir en las invitaciones por correo electrónico como cuerpo del correo electrónico.</li> 
        <li><strong>Términos y condiciones</strong>: Si selecciona modificar la invitación por correo electrónico para todos los usuarios nuevos con una licencia de solicitante, especifique el texto que desea incluir en las invitaciones por correo electrónico como términos y condiciones.<br></li> 
        <li> <p>En el <strong>Vista previa de invitación</strong> , puede ver una vista previa de la invitación por correo electrónico. Si ha seleccionado incluir un mensaje personalizado en la invitación del correo electrónico, en esta área se muestra el mensaje personalizado.</p> <p> <img src="assets/email-invitation-for-all-users-preview-qs-350x190.png" style="width: 350;height: 190;"> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.
