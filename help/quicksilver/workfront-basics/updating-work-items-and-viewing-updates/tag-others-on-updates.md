---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Etiquetar otros en actualizaciones
description: Al proporcionar comentarios de actualización en un objeto de Adobe Workfront, todos los usuarios del proyecto pueden ver la información enviada. Sin embargo, es posible que a veces los usuarios que no están en el proyecto se beneficien de ver esta información. En lugar de incluir a esos usuarios en el proyecto, puede etiquetarlos en la actualización para compartirlos con ellos. Los usuarios etiquetados reciben una notificación de evento.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 607e0523cf97fdf26b650dc441e52b4ae4528af4
workflow-type: tm+mt
source-wordcount: '1456'
ht-degree: 0%

---

# Etiquetar otros en actualizaciones

<!--take "Beta" references out when we remove the beta-->


<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.-->

>[!NOTE]
>
>Actualmente estamos rediseñando la experiencia de comentarios en Adobe Workfront.
>Para obtener más información sobre la nueva experiencia de actualización, consulte [Nueva experiencia de comentarios](../updating-work-items-and-viewing-updates/unified-commenting-experience.md).
>
>Puede acceder al nuevo diseño para los siguientes objetos:
> * Problemas, al activar el comentario Beta.
   >
   >     Esta funcionalidad solo está disponible para la sección Actualizaciones de los problemas y no está disponible para las siguientes áreas:
   >
   >     * Página de inicio
   >     * Panel Resumen en listas
   >     * Panel Resumen en hojas de horas
>
> * Metas

   >
   >   La nueva experiencia de comentarios es la predeterminada para los objetivos. Debe tener una licencia adicional para acceder a los objetivos de Workfront. Para obtener más información, consulte [Requisitos para utilizar los objetivos de Workfront](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   >
   >    Para obtener información sobre cómo comentar objetivos, consulte [Administrar comentarios de objetivo en objetivos de Adobe Workfront](../../workfront-goals/goal-management/manage-goal-comments.md).



Puede etiquetar a los usuarios al realizar una actualización de un objeto si desea llamar su atención sobre un objeto que de otra manera no seguirían.
En lugar de incluir a esos usuarios en el objeto asignándolos o haciendo que se suscriban a él, puede etiquetarlos en la actualización para compartirlos con ellos. Los usuarios etiquetados reciben una notificación sobre la actualización que introduzca.

>[!NOTE]
>
>Se debe activar una notificación de evento para que un usuario reciba la notificación por correo electrónico. Los administradores pueden activar notificaciones para todo el sistema o para un grupo de nivel superior. Un usuario también puede habilitar y deshabilitar notificaciones de eventos individuales en su propio perfil de usuario. Para obtener más información, consulte lo siguiente:
>
>* [Configurar notificaciones de eventos para todos los miembros del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
>* [Ver y configurar notificaciones de eventos para un grupo](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)
>* [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).
>


Para obtener información sobre cómo agregar actualizaciones a objetos de Workfront, consulte [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>Cuando un problema se convierte en un proyecto o tarea, las actualizaciones se copian en el nuevo proyecto o tarea, pero los usuarios etiquetados no. Para continuar con la conversación, debe etiquetar a los participantes de nuevo.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan de Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Solicitar o superior problemas y documentos; Revisar o superior para todos los demás objetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Solicitante o superior para problemas y documentos; Revisor o superior para todos los demás objetos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Ver acceso al objeto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Etiquetar otros en actualizaciones

El etiquetado de otros en una actualización difiere según la experiencia y el objeto que seleccione.

### Etiquete a otros en las actualizaciones de la sección Actualizaciones actuales

1. Comience a actualizar un elemento de trabajo, tal como se describe en [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. En el **Notificar** , empiece a escribir el nombre del usuario o equipo que desea incluir y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   O

   Escriba el símbolo @ en la variable **Iniciar una nueva actualización** , empiece a escribir el nombre del usuario o equipo que desea incluir en la actualización y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   >[!TIP]
   >
   >Para identificar el usuario correcto cuando hay usuarios con nombres similares o idénticos, fíjese en el avatar, la función principal del usuario o su dirección de correo electrónico. Los usuarios deben estar asociados con al menos una función de trabajo para verla al etiquetarlos en una actualización.

   ![](assets/tag-users-in-update.png)

1. (Opcional) Para que la actualización sea privada, active **Privado para mi empresa** en la esquina inferior derecha del cuadro de actualización. Esto hace que la actualización sea visible solo para los usuarios de su empresa. La variable **Privado para mi empresa** solo está disponible cuando se especifica una empresa en el perfil de Workfront.

   >[!NOTE]
   >
   >Los usuarios etiquetados fuera de la empresa aún podían recibir una notificación o un correo electrónico en la aplicación, aunque no vieran los comentarios privados en la pestaña Actualizaciones . Se recomienda no etiquetar a los usuarios externos en una actualización si no desea compartir la información con ellos.

1. (Opcional) Para agregar varios usuarios y equipos, repita el paso 2.

   >[!NOTE]
   >
   >Todos los usuarios y miembros del equipo que aparecen en el campo Notificar reciben una notificación en la aplicación para la actualización y podrían recibir un correo electrónico, en función de la configuración de sus ajustes de notificación por correo electrónico. Los usuarios que se etiquetan en un comentario o respuesta reciben una notificación para ese comentario o respuesta y pueden ver su nombre en el campo Notificar durante el resto del subproceso, pero no reciben otra notificación a menos que se etiqueten de nuevo. Para obtener más información, consulte [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) y [Configurar notificaciones de eventos para todos los miembros del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Haga clic en **Actualizar**.\
   A los usuarios incluidos en la actualización se les concede automáticamente el permiso Ver al objeto y pueden ver y responder a las actualizaciones realizadas en el objeto.

   Puede ver quién ha sido etiquetado en cada respuesta en la parte superior del subproceso de actualización. Estos usuarios, junto con los usuarios suscritos al objeto, reciben una notificación cada vez que se realiza una actualización o una respuesta en el objeto.

   ![](assets/tagging-transparency-350x192.png)

   Para obtener información sobre la funcionalidad adicional disponible al actualizar un elemento de trabajo, consulte [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

### Etiquete a otros en actualizaciones en la experiencia de comentarios en la versión beta

Puede etiquetar a otros en actualizaciones en la experiencia beta de comentarios. También puede eliminar usuarios etiquetados por error al editar un comentario.

1. Comience a actualizar un elemento de trabajo, tal como se describe en [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. En el **Etiquetar personas o equipos** , empiece a escribir el nombre del usuario o equipo que desea incluir y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   O

   Escriba el símbolo @ en la variable **Escribir un comentario** , empiece a escribir el nombre del usuario o equipo que desea incluir en la actualización y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   >[!TIP]
   >
   >Para identificar el usuario correcto cuando hay usuarios con nombres similares o idénticos, fíjese en el avatar, la función principal del usuario o su dirección de correo electrónico. Los usuarios deben estar asociados con al menos una función de trabajo para verla al etiquetarlos en una actualización.

   ![](assets/tag-others-unified-commenting.png)

1. (Opcional) Para que la actualización sea privada, active **Privado para mi empresa** en la esquina inferior derecha del cuadro de actualización. Esto hace que la actualización sea visible solo para los usuarios de su empresa. La variable **Privado para mi empresa** solo está disponible cuando se especifica una empresa en el perfil de Workfront.

   >[!NOTE]
   >
   >* Esta opción solo se muestra cuando el usuario está asociado con una empresa.
   >* Los usuarios etiquetados fuera de la empresa aún podían recibir una notificación o un correo electrónico en la aplicación, aunque no vieran los comentarios privados en la pestaña Actualizaciones . Se recomienda no etiquetar a los usuarios externos en una actualización si no desea compartir la información con ellos.


1. (Opcional) Para agregar varios usuarios y equipos, repita el paso 2. <!--insure this stays accurate-->

   >[!NOTE]
   >
   >Todos los usuarios y miembros del equipo que aparecen en el campo &quot;Etiquetar personas o equipos&quot; reciben una notificación en la aplicación para la actualización y podrían recibir un correo electrónico, en función de la configuración de sus ajustes de notificación por correo electrónico. Los usuarios que se etiquetan en un comentario o respuesta reciben una notificación para ese comentario o respuesta y pueden ver su nombre en la lista como miembro del subproceso para el resto del subproceso, pero no reciben otra notificación a menos que se etiqueten de nuevo. Para obtener más información, consulte [Activar o desactivar sus propias notificaciones de eventos](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) y [Configurar notificaciones de eventos para todos los miembros del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Haga clic en **Submit**.\
   A los usuarios incluidos en la actualización se les concede automáticamente el permiso Ver al objeto y pueden ver y responder a las actualizaciones realizadas en el objeto.

   Puede ver quién ha sido etiquetado en cada respuesta bajo el texto de la actualización, en el área Miembros. Estos usuarios, junto con los usuarios suscritos al objeto, reciben una notificación cada vez que se realiza una actualización o una respuesta en el objeto.
1. (Opcional) Haga clic en el número de **Miembros** incluido en la actualización para mostrar una lista de entidades con las que se comparte la actualización introducida.

   ![](assets/members-icons-expanded-unshimmed.png)

   Para obtener información sobre la funcionalidad adicional disponible al actualizar un elemento de trabajo, consulte [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Opcional) Haga clic en el **Más** menú ![](assets/more-menu.png) a la derecha del icono &quot;Me gusta&quot; y, a continuación, haga clic en **Editar**. Elimine cualquiera de los usuarios etiquetados y haga clic en **Submit**. Puede editar un comentario solo en los 15 minutos siguientes a su introducción. Solo puede editar los comentarios que ha agregado.