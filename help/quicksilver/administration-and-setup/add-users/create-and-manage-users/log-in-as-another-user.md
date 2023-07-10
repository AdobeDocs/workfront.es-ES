---
title: Iniciar sesión como otro usuario
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Como administrador de Adobe Workfront, a veces es posible que deba acceder a Workfront en nombre de otro usuario.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: 82f42d81970c7572f43519423ec3a8c0889aaff4
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 1%

---

# Iniciar sesión como otro usuario


<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible para todos los usuarios en el entorno de vista previa.</span>
<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

>[!IMPORTANT]
>
>El procedimiento descrito en esta página se aplica solo a las organizaciones que aún no se han incorporado a Adobe Admin Console. Si su organización se ha incorporado a Adobe Admin Console, esta acción no está disponible.
>
>Para obtener una lista de procedimientos que difieren en función de si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en la plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador de Adobe Workfront, a veces es posible que deba acceder a Workfront en nombre de otro usuario.

O bien, como administrador de grupo, es posible que deba acceder a Workfront en nombre de un usuario que sea miembro de un grupo que administre.

Por ejemplo, si una tarea no puede progresar hasta que un usuario de vacaciones realice una determinada acción, puede iniciar sesión como ese usuario y realizar la acción en su lugar.

<!--
<note type="note">
Some users, such as executives, need to be able to control which administrators can log in to their accounts, and for how long. Working with your organization, Workfront configures settings that allow this control for these users. When a Workfront administrator or group administrator (associated with one of the user's groups) tries to log in as one of these users, an on-screen message prompts the administrator to contact the user for access. From the user profile area, the user can then grant access to the administrator and specify an expiration time for it. For more information on how the user does this, see
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md#access" class="MCXref xref">Access</a> in
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configure My Settings</a>.
<span class="PinkDraftNote">[Add a note about this being only for the Enterprise package if they decide to do it that way]</span>
</note>
-->

>[!NOTE]
>
>Dado que una integración de documentos puede conectarse a archivos personales privados, los administradores no pueden acceder a las integraciones de documentos mientras estén conectados como otro usuario.
>
>Para obtener más información sobre las integraciones de documentos, consulte [Configurar integraciones de documentos](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)

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
   <td> <p>Con el nivel de acceso de administrador del sistema, puede iniciar sesión como cualquier persona. Para obtener información sobre este nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>. </p> <p>Con un nivel de acceso de Planificador, puede iniciar sesión como un usuario con un nivel de licencia inferior si la variable <b>Usuarios</b> La configuración del nivel de acceso se configura en <b>Editar</b> acceso, con <b>Crear</b> y al menos uno de los dos <b>Administrador de usuarios</b> opciones activadas en <b>Ajuste la configuración</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
   <p><b>NOTA</b>: de estas dos opciones, si el usuario <b>Administrador (usuarios de grupo)</b> está habilitada, debe ser administrador de un grupo del que sea miembro el usuario.</p> 
   <p>Para obtener más información sobre <b>Usuarios</b> configuración en un nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concesión de acceso a los usuarios</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Iniciar sesión y realizar acciones como otro usuario

1. Inicie sesión en Workfront como administrador de Workfront o de un grupo.

   >[!NOTE]
   >
   >* Si es administrador de un grupo, solo podrá iniciar sesión como usuarios en los grupos que administre. Además, el permiso Administración de usuarios (usuarios de grupo) debe estar habilitado en su nivel de acceso:
   >   
   >  ![](assets/group-admin-user.png)
   >   
   >  Esta configuración está deshabilitada de forma predeterminada. Para obtener más información, consulte [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   >   
   >* No puede restablecer la contraseña de un administrador de Workfront.

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Iniciar sesión como**.

1. En el **Usuarios** en el cuadro **Iniciar sesión como** , empiece a escribir el nombre del usuario y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   El usuario debe tener un nivel de acceso definido en Workfront. No puede iniciar sesión en el sistema de Workfront como un usuario que no tiene derechos para iniciar sesión.

   >[!NOTE]
   >
   >Los administradores de grupos solo pueden iniciar sesión como los usuarios que son miembros de los grupos que administran. No pueden iniciar sesión como administradores de Workfront.

1. Clic **Iniciar sesión.**

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Might come in a future story:</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">click an Access period and then click Request to ask the user for access to log as him or her for the specified period of time. Continue these steps after the user grants access. Specify somewhere here that this is only for the Enterprise package if they decide on that</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Or </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a prompt appears indicating that the user has restricted access to their account, contact the user to request access.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The user can then can grant you "Log in as" access in their user profile. They can also specify an expiration date and time for the access period. </p>
   -->

   <!--
   This triggers an email to let you know that you have access to log in as the user, depending on how your event notifications are enabled. For more information, see <a href="../../../workfront-basics/using-notifications/event-notifications.md" class="MCXref xref">Event notifications</a>.
   </div>
   -->

   Cuando inicia sesión como otro usuario, aparece una notificación en la parte superior de la pantalla para indicarlo.

1. Después de haber realizado las acciones necesarias como usuario, haga clic en **Cerrar sesión.**

## Seguimiento y auditoría de la actividad mientras un administrador ha iniciado sesión como otro usuario

Workfront proporciona mecanismos para el seguimiento y la auditoría de la actividad que tiene lugar mientras el administrador ha iniciado sesión como otro usuario.

Cuando inicia sesión como otro usuario, la fecha del último inicio de sesión se modifica para ese usuario hasta la fecha en que el administrador del sistema o del grupo inicia sesión como ese usuario.

* [Ver indicadores en elementos](#view-indicators-on-items)
* [Ver información de auditoría](#view-audit-information)

### Ver indicadores en elementos {#view-indicators-on-items}

Cuando inicia sesión en Workfront como otro usuario y realiza una acción, Workfront indica claramente que cualquier acción que realice la realizará usted en nombre del usuario con el que ha iniciado sesión.

Por ejemplo, si comenta un elemento mientras está conectado como otro usuario, una instrucción indica que usted hizo el comentario en nombre del usuario.

>[!NOTE]
>
><span class="preview">Al utilizar la nueva experiencia de comentarios, el comentario se agrega como el usuario que ha iniciado sesión como otro usuario y no hay indicación de que esté agregando un comentario en nombre de otra persona.
>
>Por ejemplo, si un administrador de Workfront inicia sesión como otro usuario, el usuario asociado con el comentario es el administrador de Workfront. Para obtener más información, consulte [Nueva experiencia de comentarios](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). </span>


### Ver información de auditoría {#view-audit-information}

1. Inicie sesión en Workfront como administrador de Workfront o de grupo.
1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. Clic **Iniciar sesión como,** luego haga clic en **Acceder al registro** pestaña.

   Cada vez que un administrador de sistemas o de grupos inicia sesión en Workfront como otro usuario, el evento se registra en la pista de auditoría. Además, todas las acciones auditables que se realizan mientras el administrador inicia sesión como otro usuario se registran en la pista de auditoría.

1. (Opcional) Puede filtrar los resultados que se muestran en la pista de auditoría de las siguientes maneras:

   * Por usuario que ha iniciado sesión
   * Por usuario que ha iniciado sesión como
   * Por fecha
