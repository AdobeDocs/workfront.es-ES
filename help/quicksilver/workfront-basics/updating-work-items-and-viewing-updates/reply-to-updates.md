---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Responder a las actualizaciones
description: Cuando alguien agrega o responde a una actualización de un objeto de trabajo, su respuesta aparece en el subproceso de comunicación de la sección Actualizaciones del objeto. Puede añadir una respuesta a una actualización o marcarla como Me gusta si tiene acceso de Vista al objeto.
author: Lisa and Alina
feature: Get Started with Workfront
role: User
topic: Collaboration
exl-id: a8271f3c-7a08-4eb3-aaff-deb250f5af73
source-git-commit: d93d42322d62ff5eb927ca13febcb763cbec3f13
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 0%

---

# Responder a las actualizaciones

<!--take "Beta" references out when we remove the beta and change "current" to "legacy" after October 26-->

<!--after August 17: 
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/enable-fast-release-process.html?lang=en ). </span>  
<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md). </span>-->

<!--replace the note below with this at August 17: 
>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>Depending on what environment and what objects you access the commenting experience from, you might see different functionality in the Updates section. 
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>The new commenting experience is available only for the Updates section, and it is not available for the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets

-->

>[!NOTE]
>
>Actualmente estamos rediseñando la experiencia de comentarios en Adobe Workfront.
>
>Para obtener más información sobre la nueva experiencia de comentarios, consulte [Nueva experiencia de comentarios](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>Puede acceder a la nueva experiencia para los siguientes objetos:
> * Problemas, proyectos, tareas y documentos.
>
>     Esta opción está disponible al habilitar la experiencia de comentarios beta.
>
>     Esta funcionalidad solo está disponible para la sección Actualizaciones y no para las áreas siguientes:
>
>     * Página de inicio
>     * Panel de resumen en listas
>     * Panel de resumen en plantillas de horas
>
> * Metas, tarjetas en el área Tableros
>
>   La nueva experiencia de comentar es la única experiencia para los goles y las cartas. Debe tener una licencia adicional para acceder a los objetivos de Workfront. Para obtener más información, consulte [Requisitos para utilizar Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
>
>     Puede agregar y ver actualizaciones a las tarjetas en el área de Tableros al habilitar las secciones Comentarios y Actividad del sistema en una tarjeta. Para obtener más información, consulte [Añadir una tarjeta ad hoc a un tablero](../../agile/get-started-with-boards/add-card-to-board.md).


Cuando alguien responde a un comentario o a una actualización del sistema de un objeto de trabajo, su respuesta aparece en el subproceso de comunicación de la sección Actualizaciones del objeto.

>[!IMPORTANT]
>
>No es posible responder a las actualizaciones del sistema en la nueva experiencia de comentarios. Para obtener más información, consulte [Nueva experiencia de comentarios](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).


## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>Solicitante o superior para problemas y documentos; Revisor o superior para todos los demás objetos</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Ver acceso al objeto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Responder a una actualización o una respuesta en Workfront

Puede responder a un comentario en el hilo de un objeto que pueda ver, o puede iniciar sesión como Workfront o administrador de grupo y responder a un comentario en nombre de otro usuario. Para obtener más información, consulte [Iniciar sesión como otro usuario](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

Responder a un comentario o una respuesta depende de la experiencia y del objeto que seleccione.

### Responder a una actualización o respuesta en la sección Actualizaciones actuales

1. Vaya al objeto al que desea agregar una respuesta.
1. En el **Actualizaciones** para el objeto, busque la actualización o respuesta a la que desee responder.

1. (Opcional) Para ver una imagen en la actualización existente, realice una de las siguientes acciones:

   * Haga clic en **Previsualizar** icono ![](assets/previewimageicon-31x31.png) en la miniatura de la imagen para abrir la imagen a tamaño completo en una nueva pestaña del explorador.
   * Haga clic en **Descargar** icono ![](assets/downloadimageicon.png) en la miniatura para descargar la imagen.

1. Clic **Responder** en la actualización, escriba una respuesta en el cuadro que aparece.

   Puede ver los usuarios que participan activamente en la conversación o que están etiquetados en cada respuesta en la parte superior de ese hilo de actualización. Estos usuarios, junto con los usuarios suscritos al objeto, reciben una notificación cada vez que se realiza una actualización o respuesta sobre el objeto. También puede etiquetar a más usuarios para incluirlos en la respuesta.  Para etiquetar a más usuarios, consulte [Etiquetar a otros en las actualizaciones](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   ![](assets/tagging-transparency-350x192.png)

1. (Opcional) Para incluir texto de una actualización anterior en su respuesta, haga clic en **Más** situado junto a la actualización o respuesta que desee citar y, a continuación, haga clic en **Citar respuesta**. El texto de la actualización anterior aparece en el área de entrada, marcado con una línea gris vertical.
1. (Opcional) Use formato, emojis, incluya vínculos o imágenes como se explica en la sección &quot;Usar texto enriquecido en una actualización de Workfront&quot; del artículo [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. Clic **Responder** para guardar la respuesta.

### Responder a un comentario al usar la nueva experiencia de comentarios

Para obtener información sobre las funciones disponibles en la nueva experiencia de comentarios y los objetos, consulte [Nueva experiencia de comentarios](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

1. Vaya al objeto al que desea agregar una respuesta.
1. Clic **Actualizaciones**, luego haga clic en **Comentarios** para el objeto y busque el comentario o la respuesta a los que desea responder.
1. (Opcional) Para incluir texto de una actualización anterior en su respuesta, haga clic en **Más** junto a la actualización o respuesta que desee citar <!--(replace placing of the More menu - August 17) <span class="preview">in the upper-right corner of the comment you want to reply to</span>-->, luego haga clic en **Cita respuesta**. El texto de la actualización anterior aparece en el área de entrada, marcado con una línea gris vertical.
1. Clic **Responder**.

   Puede ver los usuarios que participan activamente en la conversación en la parte inferior de la **Nuevo comentario** y puede agregar más, o eliminar los que ya no son relevantes. Estos usuarios, junto con los usuarios suscritos al objeto, reciben una notificación cada vez que se realiza una actualización o respuesta sobre el objeto. También puede etiquetar a más usuarios para incluirlos en la respuesta.  Para etiquetar a más usuarios, consulte [Etiquetar a otros en las actualizaciones](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

1. Empiece a escribir la respuesta y utilice las opciones adicionales de la barra de herramientas Texto enriquecido. Para obtener información sobre el uso de texto enriquecido u otras funciones de actualización, consulte [Actualizar trabajo](../updating-work-items-and-viewing-updates/update-work.md).

1. Clic **Enviar** para guardar la respuesta.

1. (Opcional) Haga clic en **Más** menú ![](assets/more-menu.png) junto a la actualización <!--(replace placing of the More menu - August 17) <span class="preview">in the upper-right corner of the comment you want to reply to</span>--> para ver más opciones para administrar la respuesta. Para obtener más información, consulte [Actualizar trabajo](../updating-work-items-and-viewing-updates/update-work.md).


## Responder a una actualización desde una notificación por correo electrónico

Según la configuración de las notificaciones por correo electrónico, podría recibir una notificación por correo electrónico cuando se realice una actualización de ciertos objetos a los que tiene acceso.

Puede responder a una actualización desde una notificación por correo electrónico de las siguientes maneras:

* Responda al correo electrónico que recibe. El correo electrónico de respuesta se agrega como respuesta de Workfront al comentario original.
* Utilice el botón Comentar dentro del correo electrónico para volver a Workfront y responder a la actualización en el área de Actualizaciones.

A continuación se muestra un ejemplo de una notificación por correo electrónico activada como resultado de una actualización realizada en la pestaña Actualizaciones de una tarea:

![email.png](assets/email-350x202.png)

Para obtener más información, consulte [Responder a notificaciones por correo electrónico](../updating-work-items-and-viewing-updates/reply-to-email-notifications.md).






