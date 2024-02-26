---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Etiquetar a otros en las actualizaciones
description: Al proporcionar comentarios de actualización sobre un objeto de Adobe Workfront, todos los usuarios del proyecto pueden ver la información enviada. Sin embargo, puede haber ocasiones en que los usuarios que no están en el proyecto se beneficien de ver esta información. En lugar de incluir a esos usuarios en el proyecto, puede etiquetarlos en la actualización para compartirla con ellos. Los usuarios etiquetados reciben una notificación de evento.
author: Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: 56ab6fe79fe6e10be2ec61cb16ff48b30856dc0f
workflow-type: tm+mt
source-wordcount: '1621'
ht-degree: 0%

---

# Etiquetar a otros en las actualizaciones

{{highlighted-preview}}

<!--take new commenting and legacy commenting out when we remove the legacy commenting and the new one is the only experience-->

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  

<span class="preview">For information about the current release schedule, see [Fourth Quarter 2023 release overview](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span> 
-->

>[!IMPORTANT]
>
>Actualmente estamos rediseñando la experiencia de comentarios en Adobe Workfront.
>
>Según los objetos para los que acceda a la experiencia de comentarios, es posible que vea la siguiente funcionalidad para la sección Actualizaciones:
>* La nueva experiencia
>* La experiencia heredada
>* La nueva experiencia y la experiencia heredada
>
>Para obtener más información sobre la nueva experiencia de comentarios y su disponibilidad, consulte [Nueva experiencia de comentarios](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>La nueva experiencia de comentarios solo está disponible para la sección Actualizaciones de objetos de Workfront y no está disponible al acceder a los objetos desde las áreas siguientes:
>
> * Inicio
> * Panel de resumen en listas
> * Panel de resumen en plantillas de horas
> * Panel de resumen en el Distribuidor de cargas de trabajo
>
><span class="preview">La nueva experiencia de comentarios está disponible en el panel Resumen en las listas, las hojas de horas y el Distribuidor de cargas de trabajo en el entorno de vista previa.</span>

Puede etiquetar a los usuarios al realizar una actualización de un objeto si desea llamar su atención sobre un objeto que podrían no seguir de otra manera.

En lugar de incluir a esos usuarios en el objeto asignándolos a él o haciendo que se suscriban a él, puede etiquetarlos en la actualización para compartirla con ellos. Los usuarios etiquetados reciben una notificación sobre la actualización que introduce.

## Consideraciones sobre el etiquetado de usuarios en actualizaciones

* Los usuarios etiquetados en las actualizaciones deben habilitar una notificación personal en su perfil para que reciban la notificación por correo electrónico. Para obtener más información, consulte [Modificar sus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  Para obtener información sobre cómo agregar actualizaciones a objetos de Workfront, consulte [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* Cuando un problema se convierte en un proyecto o tarea, las actualizaciones se copian en el nuevo proyecto o tarea, pero los usuarios etiquetados no. Para continuar la conversación, debe volver a etiquetar a los participantes.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Solicitud o superior para problemas y documentos; Revisar o superior para todos los demás objetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Solicitante o superior para problemas y documentos; Revisor o superior para todos los demás objetos</p> 
   <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Ver acceso al objeto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Etiquetar a otros en las actualizaciones

El etiquetado de otros en una actualización difiere según la experiencia y el objeto que seleccione.

### Etiquete otras personas en las actualizaciones de la nueva experiencia de comentarios

Puede etiquetar a otros en las actualizaciones de la nueva experiencia de comentarios de las siguientes maneras:

* **Automáticamente**: Cuando un usuario inicia un hilo de conversación, añade un comentario o añade una respuesta, se etiquetan automáticamente y se añaden al área de Etiquetar personas o equipos del cuadro de comentarios. <!--remove the tip below when the new commenting stream is the only stream and the legacy commenting is removed-->

  >[!TIP]
  >
  >Cuando el hilo se inicia en la experiencia anterior de comentarios, los participantes del hilo no se etiquetan automáticamente.

* **Manualmente**: Cuando agrega manualmente un usuario al área de Etiquetar personas del cuadro de comentarios.

También puede quitar usuarios etiquetados por error cuando edite o responda a un comentario.

1. Comience a actualizar un elemento de trabajo como se describe en [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). Como propietario del comentario, se le etiqueta automáticamente y se le agrega al área Etiquetar personas o equipos del cuadro de comentarios.

   >[!TIP]
   >
   >El propietario del comentario no puede ver su propio nombre en el área Etiquetar personas o equipos del cuadro de comentarios.

1. En el **Etiquetar personas o equipos** , empiece a escribir el nombre del usuario o equipo que desea incluir y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   O

   Escriba el símbolo @ en la **Escribir un comentario** , empiece a escribir el nombre del usuario o equipo que desee incluir en la actualización y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   >[!TIP]
   > 
   >Para identificar al usuario correcto cuando hay usuarios con nombres similares o idénticos, observe el avatar, la función principal del usuario o su dirección de correo electrónico.
   > 
   >Los usuarios deben estar asociados con al menos una función del trabajo para verla a medida que los etiqueta en una actualización.
   > 
   >Debe tener activada la configuración Ver información de contacto en su nivel de acceso para que los usuarios vean los correos electrónicos de los usuarios. Para obtener más información, consulte [Concesión de acceso a los usuarios](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   <div class="preview">

   Ejemplo de etiquetado en el entorno de vista previa:
   ![Etiquetado de un usuario](assets/tag-others-unified-commenting-with-all-tab.png)

   </div>

   Ejemplo de etiquetado en el entorno de producción:
   ![](assets/tag-others-unified-commenting.png)

1. (Opcional) Para que la actualización sea privada, habilite **Privado para mi compañía** en la esquina inferior derecha del cuadro actualizar. Esto hace que la actualización sea visible solo para los usuarios de la compañía. El **Privado para mi compañía** Esta opción solo está disponible cuando se especifica una Compañía en el perfil de Workfront.

   >[!NOTE]
   >
   >* Esta opción solo se muestra cuando el usuario está asociado a una Empresa.
   >* Los usuarios etiquetados fuera de la empresa podrían seguir recibiendo una notificación en la aplicación o un correo electrónico, aunque no vean los comentarios privados en la pestaña Actualizaciones. Se recomienda no etiquetar a los usuarios externos en una actualización si no desea compartir la información con ellos.

1. (Opcional) Para agregar varios usuarios y equipos, repita el paso 2. <!--insure this stays accurate-->

   >[!NOTE]
   >
   >Todos los usuarios y miembros del equipo enumerados en el campo &quot;Etiquetar personas o equipos&quot; reciben una notificación en la aplicación para la actualización y pueden recibir un correo electrónico, según la configuración de su notificación por correo electrónico. Los usuarios que se etiquetan a sí mismos en un comentario o respuesta reciben una notificación por ese comentario o respuesta y pueden ver su nombre en la lista como miembro del hilo durante el resto del hilo, pero no reciben otra notificación a menos que se vuelvan a etiquetar a sí mismos. Para obtener más información, consulte [Modificar sus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) y [Configurar notificaciones de eventos para todos los usuarios del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Clic **Enviar**.\
   A los usuarios incluidos en la actualización se les concede automáticamente el permiso Ver al objeto y pueden ver y responder a las actualizaciones realizadas en el objeto.

   Los nombres de las entidades etiquetadas se muestran junto a sus avatares, con un máximo de dos entidades. Si se etiquetan más de dos entidades, se muestra el nombre de la primera, además de una serie de entidades adicionales.

   ![](assets/members-icons-expanded-unshimmed.png)

   Para obtener información sobre la funcionalidad adicional disponible al actualizar un elemento de trabajo, consulte [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Opcional) Haga clic en **Más** menú ![](assets/more-menu.png) en la esquina superior derecha del comentario y haga clic en **Editar**. Elimine cualquiera de los usuarios etiquetados y haga clic en **Enviar**. Solo puede editar un comentario 15 minutos después de haberlo introducido. Solo puede editar los comentarios que ha añadido.

   >[!TIP]
   >
   >Cuando se utiliza la experiencia de comentarios heredada para agregar comentarios y respuestas, las personas que utilizan la nueva experiencia de comentarios no pueden eliminar manualmente los propietarios de comentarios que no estén etiquetados específicamente.


### Etiquete otras en las actualizaciones en la sección Actualizaciones heredadas

Puede etiquetar usuarios manualmente en la sección Actualizaciones heredadas.

1. Comience a actualizar un elemento de trabajo como se describe en [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. En el **Notificar** , empiece a escribir el nombre del usuario o equipo que desea incluir y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   O

   Escriba el símbolo @ en la **Iniciar una nueva actualización** , empiece a escribir el nombre del usuario o equipo que desee incluir en la actualización y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   >[!TIP]
   >
   >Para identificar al usuario correcto cuando hay usuarios con nombres similares o idénticos, observe el avatar, la función principal del usuario o su dirección de correo electrónico.
   >
   >Los usuarios deben estar asociados con al menos una función del trabajo para verla a medida que los etiqueta en una actualización.
   >
   >Debe tener activada la configuración Ver información de contacto en su nivel de acceso para que los usuarios vean los correos electrónicos de los usuarios. Para obtener más información, consulte [Concesión de acceso a los usuarios](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   ![](assets/tag-users-in-update.png)

1. (Opcional) Para que la actualización sea privada, habilite **Privado para mi compañía** en la esquina inferior derecha del cuadro actualizar. Esto hace que la actualización sea visible solo para los usuarios de la compañía. El **Privado para mi compañía** Esta opción solo está disponible cuando se especifica una Compañía en el perfil de Workfront.

   >[!NOTE]
   >
   >Los usuarios etiquetados fuera de la empresa podrían seguir recibiendo una notificación en la aplicación o un correo electrónico, aunque no vean los comentarios privados en la pestaña Actualizaciones. Se recomienda no etiquetar a los usuarios externos en una actualización si no desea compartir la información con ellos.

1. (Opcional) Para agregar varios usuarios y equipos, repita el paso 2.

   >[!NOTE]
   >
   >Todos los usuarios y miembros del equipo enumerados en el campo Notificar reciben una notificación en la aplicación sobre la actualización y podrían recibir un correo electrónico, según la configuración de sus notificaciones por correo electrónico. Los usuarios que se etiquetan en un comentario o respuesta reciben una notificación para ese comentario o respuesta y pueden ver su nombre en el campo Notificar para el resto del hilo, pero no reciben otra notificación a menos que se vuelvan a etiquetar. Para obtener más información, consulte [Modificar sus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) y [Configurar notificaciones de eventos para todos los usuarios del sistema](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Clic **Actualizar**.\
   A los usuarios incluidos en la actualización se les concede automáticamente el permiso Ver al objeto y pueden ver y responder a las actualizaciones realizadas en el objeto.

   Puede ver quién ha sido etiquetado en cada respuesta en la parte superior del hilo de actualización. Estos usuarios, junto con los usuarios suscritos al objeto, reciben una notificación cada vez que se realiza una actualización o respuesta sobre el objeto.

   ![](assets/tagging-transparency-350x192.png)

   Para obtener información sobre la funcionalidad adicional disponible al actualizar un elemento de trabajo, consulte [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).



