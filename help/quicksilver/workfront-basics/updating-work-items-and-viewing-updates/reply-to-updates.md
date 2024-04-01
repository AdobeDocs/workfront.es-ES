---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Responder a las actualizaciones
description: Cuando alguien agrega o responde a una actualización de un objeto de trabajo, su respuesta aparece en el subproceso de comunicación de la sección Actualizaciones del objeto. Puede añadir una respuesta a una actualización o marcarla como Me gusta si tiene acceso de Vista al objeto.
author: Nolan and Alina
feature: Get Started with Workfront
role: User
topic: Collaboration
exl-id: a8271f3c-7a08-4eb3-aaff-deb250f5af73
source-git-commit: ee957e319941fe5eabb9144eed184372e5402197
workflow-type: tm+mt
source-wordcount: '1190'
ht-degree: 0%

---

# Responder a las actualizaciones

<!--remove legacy and new experience references when we remove the legacy updates in the UI - Jan 2024???-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  

<span class="preview">For information about the current release schedule, see [Fourth Quarter 2023 release overview](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span> 

-->

<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa para todos los clientes de o en Producción para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Activar o desactivar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Para obtener más información sobre la programación actual de versiones, consulte [Información general sobre la versión del segundo trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

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
><Span class="preview"> La experiencia de comentarios heredada se ha eliminado de proyectos, tareas, problemas y documentos en el entorno de vista previa. </span>
>
>La nueva experiencia de comentarios solo está disponible para la sección Actualizaciones de los objetos de Workfront y no está disponible al acceder a las actualizaciones desde las áreas siguientes:
>
> * Inicio
> * Panel de resumen en listas
> * Panel de resumen en plantillas de horas
> * Panel de resumen en el Distribuidor de cargas de trabajo
>
><span class="preview">La nueva experiencia de comentarios está disponible en el panel Resumen en listas, plantillas de horas y el Distribuidor de cargas de trabajo en el entorno de vista previa y en el entorno de producción para los clientes que han elegido el proceso de versión rápido. </span>

Cuando alguien responde a un comentario o a una actualización del sistema de un objeto de trabajo, su respuesta aparece en el subproceso de comunicación de la sección Actualizaciones del objeto.

>[!IMPORTANT]
>
>No es posible responder a las actualizaciones del sistema en la nueva experiencia de comentarios. Para obtener más información, consulte [Nueva experiencia de comentarios](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

<!--adjust the sentence before the second IMPORTANT and remove this important note when we remove legacy from the system-->

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

### Responder a un comentario al usar la nueva experiencia de comentarios

Para obtener información sobre las funciones disponibles en la nueva experiencia de comentarios y los objetos, consulte [Nueva experiencia de comentarios](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

1. Vaya al objeto al que desea agregar una respuesta.
1. Clic **Actualizaciones**, luego haga clic en **Comentarios** para el objeto y busque el comentario o la respuesta a los que desea responder

   O

   <span class="preview">Haga clic en **Todo** y haga clic en **Responder en comentarios** para abrir el comentario en la pestaña Comentarios y responder a él. No puede responder en la pestaña Todos.</span>

1. (Opcional) Para incluir texto de una actualización anterior en su respuesta, haga clic en **Más** en la esquina superior derecha del comentario al que desea responder y, a continuación, haga clic en **Cita respuesta**. El texto de la actualización anterior aparece en el área de entrada, marcado con una línea gris vertical.
1. Clic **Responder**.

   ![](assets/reply-to-update-empty-box.png)

   Puede ver los usuarios que participan activamente en la conversación en la parte inferior de la **Añadir respuesta...** y puede agregar más, o eliminar los que ya no son relevantes. Estos usuarios, junto con los usuarios suscritos al objeto, reciben una notificación cada vez que se realiza una actualización o respuesta sobre el objeto. También puede etiquetar a más usuarios para incluirlos en la respuesta.  Para etiquetar a más usuarios, consulte [Etiquetar a otros en las actualizaciones](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   >[!TIP]
   >
   >   Para agregar respuestas adicionales a una respuesta existente, puede empezar a escribir en el **Añadir respuesta...** o haga clic en **Responder** sobre el comentario original. Su respuesta se añade al final del hilo.

1. Empiece a escribir la respuesta y utilice las opciones adicionales de la barra de herramientas Texto enriquecido. Para obtener información sobre el uso de texto enriquecido u otras funciones de actualización, consulte [Actualizar trabajo](../updating-work-items-and-viewing-updates/update-work.md).

1. Clic **Enviar** para guardar la respuesta.

1. (Opcional) Haga clic en **Más** menú ![](assets/more-menu.png) en la esquina superior derecha del comentario al que desea responder para obtener más opciones y administrar la respuesta. Para obtener más información, consulte [Actualizar trabajo](../updating-work-items-and-viewing-updates/update-work.md).

### Responder a una actualización o respuesta en la sección Actualizaciones heredadas

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

## Responder a una actualización desde una notificación por correo electrónico

Según la configuración de las notificaciones por correo electrónico, podría recibir una notificación por correo electrónico cuando se realice una actualización de ciertos objetos a los que tiene acceso.

Puede responder a una actualización desde una notificación por correo electrónico de las siguientes maneras:

* Responda al correo electrónico que recibe. El correo electrónico de respuesta se agrega como respuesta de Workfront al comentario original.
* Utilice el botón Comentar dentro del correo electrónico para volver a Workfront y responder a la actualización en el área de Actualizaciones.

A continuación se muestra un ejemplo de una notificación por correo electrónico activada como resultado de una actualización realizada en la pestaña Actualizaciones de una tarea:

![email.png](assets/email-350x202.png)

Para obtener más información, consulte [Responder a notificaciones por correo electrónico](../updating-work-items-and-viewing-updates/reply-to-email-notifications.md).






