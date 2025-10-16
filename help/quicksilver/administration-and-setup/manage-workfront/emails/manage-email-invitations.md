---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Administrar invitaciones por correo electrónico a nuevos usuarios
description: Como administrador de Adobe Workfront, puede agregar usuarios a Workfront y notificarles que han sido agregados mediante invitaciones por correo electrónico.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: e13e3479-391f-4aec-b998-e9b6057f256b
source-git-commit: e34abb5ff1068de99eaba33dc95287164e556742
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 18%

---

# Administrar las invitaciones por correo electrónico a los nuevos usuarios

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>El procedimiento descrito en esta página se aplica solo a las organizaciones que aún no se han incorporado a Admin Console. Si su organización se ha incorporado a Adobe Admin Console, debe llevar a cabo esta acción mediante Adobe Admin Console.
>
>Para obtener una lista de procedimientos que difieren según si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en la plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador de Adobe Workfront, puede agregar usuarios a Workfront y notificarles que han sido agregados mediante invitaciones por correo electrónico.

La invitación por correo electrónico permite a los nuevos usuarios seguir un vínculo en el que pueden elegir una contraseña para su cuenta de Workfront. Luego pueden terminar de configurar su cuenta.

Para garantizar la seguridad de las nuevas cuentas, le recomendamos que utilice invitaciones por correo electrónico para los nuevos usuarios, de modo que puedan elegir su propia contraseña. También puede seleccionar una contraseña para un nuevo usuario al crear su cuenta. Para obtener más información sobre cómo agregar nuevos usuarios a Workfront, consulte [Agregar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Puede configurar los nuevos correos electrónicos de los usuarios para:

* Cualquier nuevo usuario agregado a Workfront
* Usuarios añadidos a Workfront con una licencia de solicitante

Todos los usuarios nuevos ven el mismo correo electrónico cuando se envía una invitación por correo electrónico.

Para obtener información sobre cómo recibir invitaciones por correo electrónico, consulte [Recibir invitaciones por correo electrónico y crear una contraseña para Adobe Workfront](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Estándar</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Administrador del sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Reenviar invitaciones por correo electrónico a usuarios no registrados existentes

Las invitaciones por correo electrónico se generan en los siguientes casos:

* Cuando crea un nuevo usuario y selecciona **Enviar un correo electrónico de invitación a esta persona** en el formulario **Nuevo usuario**. Para obtener más información sobre cómo crear usuarios nuevos, consulte [Añadir usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Cuando importa varios usuarios nuevos y selecciona la opción **Enviar invitación por correo electrónico a estas personas**. Para obtener más información sobre cómo importar varios usuarios nuevos, consulte [Importar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).
* Una vez creados los usuarios, puede generar manualmente las invitaciones a los usuarios que aún no hayan registrado su cuenta en Workfront y que no hayan establecido una contraseña de Workfront.\
  Los usuarios que hayan creado una cuenta pero que aún no la hayan registrado se marcarán como **No registrado** en Workfront.

  >[!NOTE]
  >
  >Si anula la selección del cuadro **Enviar una invitación por correo electrónico a esta persona** al crear el usuario, la invitación por correo electrónico no se podrá generar manualmente. El reenvío manual de las invitaciones por correo electrónico solo es posible para los usuarios a los que se les ha enviado la invitación por correo electrónico original cuando se creó su cuenta. Para obtener más información sobre cómo crear usuarios nuevos, consulte [Añadir usuarios](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Para reenviar manualmente invitaciones por correo electrónico a usuarios no registrados existentes:

{{step-1-to-users}}

1. Seleccione al usuario que muestra la etiqueta **No registrado** después de su nombre.

   ![No registrado](assets/unreg-user-qs-350x221.png)

1. Haga clic en el icono Más ![Más](assets/more-icon.png) y, a continuación, haga clic en **Recordar al usuario que se registre**.

   Se envía una invitación por correo electrónico al nuevo usuario con un nuevo vínculo que puede utilizar para crear su contraseña de Workfront.

   >[!NOTE]
   >
   >Si su organización se ha incorporado a Admin Console y agrega un usuario a través de Workfront, no tiene la opción de enviar una invitación por correo electrónico a los nuevos usuarios.
   >
   >Los nuevos usuarios de Adobe se añaden a Admin Console y Admin Console envía un correo electrónico para invitarlos a completar el proceso de registro. Todos los usuarios deben completar el proceso de registro para acceder a cualquier sistema de Adobe.
   >
   >Para los usuarios de Adobe existentes, el usuario puede recibir o no un correo electrónico sobre la disponibilidad de Workfront. Esta es una preferencia que controla el administrador de Adobe para este producto.

## Configurar invitaciones por correo electrónico {#configure-email-invitations}

Como administrador de Workfront, puede configurar el mensaje que incluye con las invitaciones por correo electrónico para nuevos usuarios.

{{step-1-to-setup}}

1. En la lista de la izquierda, haga clic en **Correo electrónico** > **Invitaciones**.

1. En la sección **Opciones generales**, realice cualquiera de las siguientes modificaciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Desactivar vínculos de invitación después de... días</strong> </td> 
      <td> <p>Elija la cantidad de tiempo después de la cual las invitaciones por correo electrónico ya no contienen un vínculo válido a Workfront. La cantidad predeterminada de días es 45.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Incluir un mensaje y/ o un término de servicio</strong> </td> 
      <td> <p>Seleccione esta opción si desea modificar la invitación por correo electrónico de todos los usuarios nuevos agregados a Workfront. Esto no incluye a los usuarios con una licencia de solicitante.</p> 
       <ul> 
        <li><strong>Mensaje</strong>: si selecciona modificar la invitación por correo electrónico para todos los usuarios nuevos, especifique el texto que desea incluir en las invitaciones por correo electrónico como cuerpo del correo electrónico.</li> 
        <li><strong>Términos y condiciones</strong>: si decide modificar la invitación por correo electrónico para todos los usuarios nuevos, especifique el texto que desea incluir en las invitaciones por correo electrónico como términos y condiciones.<br></li> 
        <li><strong>Incluir un mensaje o un término de servicio para los usuarios del servicio de asistencia</strong>: seleccione esta opción si desea modificar la invitación por correo electrónico para todos los usuarios nuevos agregados a Workfront que tengan una licencia de solicitante.</li> 
        <li><strong>Mensaje</strong>: si selecciona modificar la invitación por correo electrónico para todos los usuarios nuevos con una licencia de solicitante, especifique el texto que desea incluir en las invitaciones por correo electrónico como cuerpo del correo electrónico.</li> 
        <li><strong>Términos y condiciones</strong>: Si decide modificar la invitación por correo electrónico para todos los usuarios nuevos con una licencia de solicitante, especifique el texto que desea incluir en las invitaciones por correo electrónico como términos y condiciones.<br></li> 
        <li> <p>En la sección <strong>Vista previa de invitación</strong>, puedes ver una vista previa de tu invitación por correo electrónico. Si ha seleccionado incluir un mensaje personalizado en la invitación por correo electrónico, el mensaje personalizado se muestra en esta área.</p> <p> <img src="assets/email-invitation-for-all-users-preview-qs-350x190.png" style="width: 350;height: 190;"> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.
