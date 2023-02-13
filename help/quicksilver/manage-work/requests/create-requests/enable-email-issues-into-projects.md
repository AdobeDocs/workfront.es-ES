---
product-area: requests
navigation-topic: create-requests
title: Permitir que los usuarios envíen un problema por correo electrónico a un proyecto de cola de solicitud
description: Permitir que los usuarios envíen un problema por correo electrónico a un proyecto de cola de solicitud
author: Alina
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: ca3c28174dca24f14a75869bdc209569d8d8d1a0
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Permitir que los usuarios envíen un problema por correo electrónico a un proyecto de cola de solicitud

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

Puede configurar un proyecto para permitir que los usuarios agreguen problemas al proyecto por correo electrónico. Puede permitir que los problemas se envíen por correo electrónico a un proyecto solo si el proyecto está designado como cola de solicitud. Para obtener más información sobre la creación de un proyecto de cola de solicitud, consulte [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>To configure the request queue, you must have Manage permissions to the project.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.<br></p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Se requieren los siguientes requisitos previos para configurar un proyecto de modo que los usuarios puedan añadir problemas al proyecto por correo electrónico.

Estas condiciones deben cumplirse antes de habilitar esta función:

* Los usuarios que envíen problemas por correo electrónico a esta cuenta deben ser usuarios activos con una licencia para Workfront.
* Los usuarios externos no pueden enviar problemas por correo electrónico a una cola de solicitudes porque no tienen acceso para crear problemas.
* Los usuarios que envíen problemas por correo electrónico a esta cuenta deben tener permisos de Agregar problema en el proyecto.
* Los correos electrónicos procedentes de la dirección de correo electrónico asociada a un usuario activo de Workfront son los únicos correos electrónicos permitidos para enviar problemas al proyecto.
* El proyecto se configura como una cola de solicitud.
* La cuenta de correo electrónico asociada al proyecto no está vinculada a una cuenta de usuario de Workfront.

## Configuración del proyecto en Workfront

>[!NOTE]
>
>Tenga en cuenta lo siguiente al habilitar la configuración de cola de correo electrónico:
>
>* Workfront permite un único correo electrónico por cola de solicitud en todos los clústeres. Si decide desactivar la cola de solicitudes, conservará la dirección de correo electrónico que ha creado siempre que siga en el cuadro Dirección de correo electrónico de entrada. Si decide dejar de utilizar el correo electrónico de admisión, debe eliminarlo del campo Correo electrónico de entrada para que pueda estar disponible para uso futuro.
>
>* Si la cola de solicitud tiene varios temas de cola o grupos de temas, Workfront seleccionará aleatoriamente el tema de cola al que se dirigirán las solicitudes enviadas por correo electrónico, lo que dificultará la gestión de las solicitudes enviadas por correo electrónico.
   >Se recomienda que el proyecto que configure para recibir solicitudes a través de correos electrónicos no tenga más de un tema en cola. Si las solicitudes enviadas están destinadas a diferentes recursos o proyectos, debe enrutarlas o moverlas manualmente después de enviarlas.


1. Vaya al proyecto que desea habilitar para recibir problemas por correo electrónico.
1. Haga clic en **Detalles de cola** en el panel izquierdo. Es posible que tenga que hacer clic en **Mostrar más** primero.
1. En el **Tipo de cola** área, seleccione **Publicar como cola de solicitud de ayuda**.

1. Desplácese hacia abajo hasta el **Configuración de cola de correo electrónico** y, a continuación, seleccione **Habilitar la admisión de solicitudes por correo electrónico**.

1. Introduzca el principio de la dirección de correo electrónico en la **Dirección de correo electrónico de entrada** en la ventana

   Debe crear una dirección de correo electrónico única. Se recomienda usar el nombre de su empresa como parte de su dirección de correo electrónico de admisión.

   >[!CAUTION]
   >
   >* Esta dirección de correo electrónico no se puede recuperar de la papelera de reciclaje si se elimina el proyecto que contiene la cola de solicitud.
   >
   >* Dado que esta dirección de correo electrónico debe ser única, es posible que no esté disponible en el futuro si se elimina.

   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in&nbsp;Workfront. Only emails created from this email address are added as issues.
   -->

1. (Opcional) Seleccione el **Reenviar todos los problemas que no se envían por correo electrónico** y, a continuación, introduzca una dirección de correo electrónico de reenvío en el cuadro siguiente.

   Esta dirección de correo electrónico recibe información sobre los correos electrónicos que no se han enviado al proyecto.

1. Haga clic en **Guardar**. Ahora, cuando los usuarios con una cuenta activa de Workfront envían un correo electrónico a esta dirección de correo electrónico, se crea un problema en el proyecto de Workfront.

   >[!NOTE]
   >
   >Los usuarios deben tener acceso para crear problemas en el proyecto para poder enviarlos por correo electrónico. Puede conceder este acceso en el cuadro de diálogo Compartir en Configuración avanzada.
   >
   >Los usuarios externos no pueden enviar problemas por correo electrónico a una cola de solicitudes porque no tienen acceso para crear problemas.

## Recibir el problema en Workfront

Cuando un usuario de Workfront envía un correo electrónico a Workfront, suceden las siguientes cosas:

* La línea Asunto del correo electrónico se convierte en el Nombre del problema.
* El cuerpo del correo electrónico se convierte en la Descripción del problema.
* Si hay algún documento adjunto al correo electrónico, esos documentos se adjuntan al problema en Workfront.
* El usuario que envía el correo electrónico se convierte en el contacto principal del nuevo problema en Workfront.
* El texto principal del correo electrónico no puede exceder los 4000 caracteres.
* Los archivos adjuntos por correo electrónico no pueden superar los 7 MB en total.
