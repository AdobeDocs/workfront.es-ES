---
navigation-topic: notifications
title: Personalizar temas de correo electrónico para notificaciones de eventos
description: Puede personalizar la línea de asunto de los correos electrónicos activados por las notificaciones de eventos.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 2f39a091-aec2-4013-a835-0ab1c8789dc3
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 4%

---

# Personalizar temas de correo electrónico para notificaciones de eventos

Puede personalizar la línea de asunto de los correos electrónicos activados por las notificaciones de eventos:

El cambio de las líneas de asunto afecta a todos los usuarios del sistema, independientemente del nivel de acceso del destinatario. Los usuarios ven todos los objetos y campos incluidos en el asunto del correo electrónico.

Algunas notificaciones de eventos tienen varias líneas de asunto, lo que significa que esas notificaciones de eventos pueden tener varios asuntos de correo electrónico en función de su funcionalidad.

>[!IMPORTANT]
>
>Tenga cuidado al eliminar los campos predeterminados en los casos en que las líneas de asunto hagan referencia a varios objetos. A continuación se muestra la lista de notificaciones de eventos que contienen estas líneas de asunto:
>
>* Alguien me incluye en una actualización dirigida
>* Alguien incluye a mi equipo en una actualización dirigida
>* Comentario en elemento de trabajo a participantes del hilo
>* Comentario de elemento de trabajo a la persona asignada al elemento
>

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Planificador o superior, con acceso administrativo a las notificaciones de recordatorio</p> <p>Para obtener información sobre cómo otorgar acceso administrativo a un usuario del plan, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder acceso administrativo a usuarios de ciertas áreas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

+++

## Personalizar las líneas de asunto de correo electrónico para notificaciones de eventos {#customize-email-subject-lines-for-event-notifications}

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Correo electrónico** > **Notificaciones**.

1. Haga clic en la ficha **Notificaciones de eventos**.
1. Haga clic en el nombre de la notificación de eventos que desea personalizar para abrir el cuadro **Notificación de eventos**.
1. En el cuadro **Línea de asunto de correo electrónico**, cambie el texto y los campos, incluidos los campos personalizados, en el asunto del correo electrónico.

   Los nombres de los campos añadidos deben coincidir con la sintaxis en minúscula de la estructura de la base de datos. <!--For more information about how our objects and their fields are named in the Workfront database, see the [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

1. Haga clic en **Actualizar** para guardar las nuevas líneas de asunto de los mensajes de correo electrónico.

## Personalizar las líneas de asunto de los correos electrónicos con varios objetos

Algunas notificaciones de eventos tienen varias líneas de asunto, según los objetos en los que se almacenen en déclencheur.

Por ejemplo, &quot;Alguien me incluye en una actualización dirigida&quot; tiene dos líneas de asunto diferentes: la primera es para tareas, problemas, tareas de plantilla y documentos (también conocida como &quot;referenceObject&quot;) y la segunda es para objetos que permiten a los usuarios realizar comentarios, como portafolio, programa, etc. (también conocida como &quot;topReferenceObject&quot;).

![](assets/Ev-not-mult-subj-lines.png)

Si se incluye a un usuario en una conversación sobre la tarea, el problema, la tarea de plantilla o el documento, se generará un mensaje de correo electrónico con la primera línea de asunto. La línea de asunto contiene &quot;referenceObject:name&quot; y el sistema define el objeto y muestra el nombre adecuado en el campo de asunto. La línea de asunto del correo electrónico tendría un aspecto similar al siguiente: &quot;Comentario sobre la tarea 123 del proyecto ABC&quot;.

Si se añade a una conversación de proyecto, se generará un correo electrónico con el segundo asunto. En este caso, la línea de asunto contiene &quot;topReferenceObject:name&quot; y, de nuevo, Workfront identifica a qué objeto se hace referencia y devuelve ese nombre de objeto en lugar de &quot;topReferenceObject:name&quot; en el asunto. La línea de asunto del correo electrónico tendría un aspecto similar al siguiente: &quot;Comentario sobre el proyecto ABC&quot;.

Para editar las líneas de asunto del correo electrónico y agregar campos adicionales a las líneas de asunto, consulte [Personalizar las líneas de asunto del correo electrónico para las notificaciones de eventos](#customize-email-subject-lines-for-event-notifications) en este artículo.

## Personalizar las líneas de asunto de los correos electrónicos de varias acciones

Algunas notificaciones de eventos también tienen varios asuntos de correo electrónico para delinear las diferentes acciones que se realizan en los objetos.

Por ejemplo, solicitar que se agregue un documento a un problema es un evento que puede almacenar en déclencheur dos correos electrónicos diferentes: uno para cuando se agrega el documento y otro para cuando se edita.

![](assets/ev-not-mult-subj-lines-diff-actions.png)

Para editar las líneas de asunto del correo electrónico y agregar campos adicionales a las líneas de asunto, consulte [Personalizar las líneas de asunto del correo electrónico para las notificaciones de eventos](#customize-email-subject-lines-for-event-notifications) en este artículo.
