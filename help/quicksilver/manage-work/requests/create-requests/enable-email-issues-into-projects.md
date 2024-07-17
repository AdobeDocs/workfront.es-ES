---
product-area: requests
navigation-topic: create-requests
title: Permitir que los usuarios envíen por correo electrónico un problema a un proyecto de cola de solicitudes
description: Permitir que los usuarios envíen por correo electrónico un problema a un proyecto de cola de solicitudes
author: Alina
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: 9cda6fd41ba7fcb9b9f412a7c2b7ffd39f3fe189
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Permitir que los usuarios envíen por correo electrónico un problema a un proyecto de cola de solicitudes

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

Puede configurar un proyecto para permitir que los usuarios agreguen problemas al proyecto por correo electrónico. Puede permitir que los problemas se envíen por correo electrónico a un proyecto solo si el proyecto está designado como Cola de solicitudes. Para obtener más información acerca de cómo crear un proyecto de cola de solicitudes, vea [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
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

Se requieren los siguientes requisitos previos para configurar un proyecto de modo que los usuarios puedan agregar problemas al proyecto por correo electrónico.

Antes de habilitar esta función, deben cumplirse las siguientes condiciones:

* Los usuarios que envíen problemas por correo electrónico a esta cuenta deben ser usuarios activos con una licencia para Workfront.
* Los usuarios que envíen problemas por correo electrónico a esta cuenta deben tener permisos para agregar problemas en el proyecto.
* Los usuarios externos no pueden enviar problemas por correo electrónico a una cola de solicitudes porque no tienen acceso para crear problemas.
* Solo los correos electrónicos procedentes de una dirección de correo electrónico asociada a un usuario de Workfront activo pueden enviar problemas al proyecto. Los correos electrónicos reenviados a un correo electrónico de usuario activo de Workfront desde un correo electrónico no asociado a una cuenta de Workfront no pueden crear problemas en el proyecto, ya que la dirección de correo electrónico del remitente original debe asociarse a una cuenta de Workfront activa.
* El proyecto se configura como una cola de solicitudes.
* La cuenta de correo electrónico asociada con el proyecto no está vinculada a una cuenta de usuario de Workfront.

## Configuración del proyecto en Workfront

>[!NOTE]
>
>Tenga en cuenta lo siguiente al habilitar la configuración de la cola de correo electrónico:
>
>* Workfront permite un único mensaje de correo electrónico por cola de solicitudes en todos los clústeres. Si decide deshabilitar la cola de solicitudes, conservará la dirección de correo electrónico que creó siempre que esté en el cuadro Dirección de correo electrónico de admisión. Si decide dejar de utilizar el correo electrónico de admisión, debe eliminarlo del campo Correo electrónico de admisión para que pueda estar disponible para un uso futuro.
>
>* Si la cola de solicitudes tiene varios temas o grupos de temas en cola, Workfront seleccionará aleatoriamente el tema de la cola al que se dirigirán las solicitudes enviadas por correo electrónico, lo que dificulta la administración de las solicitudes enviadas por correo electrónico.
>Se recomienda que el proyecto configurado para recibir solicitudes por correo electrónico no tenga más de un tema en cola. Si las solicitudes enviadas están destinadas a diferentes recursos o proyectos, debe enrutarlas o moverlas manualmente, una vez enviadas.

1. Vaya al proyecto que desea habilitar para recibir problemas por correo electrónico.
1. Haga clic en **Detalles de cola** en el panel izquierdo. Es posible que primero deba hacer clic en **Mostrar más**.
1. En el área **Tipo de cola**, seleccione **Publish como Cola de solicitud de ayuda**.

1. Desplácese hacia abajo hasta el área **Configuración de la cola de correo electrónico** y, a continuación, seleccione **Habilitar la admisión de solicitudes por correo electrónico**.

1. Escriba el principio de la dirección de correo electrónico en el cuadro **Dirección de correo electrónico de admisión**.

   Debe crear una dirección de correo electrónico única. Se recomienda usar el nombre de la empresa como parte de la dirección de correo electrónico de admisión.

   >[!CAUTION]
   >
   >* Esta dirección de correo electrónico no se puede recuperar de la papelera de reciclaje si se elimina el proyecto que contiene la cola de solicitudes.
   >
   >* Debido a que esta dirección de correo electrónico debe ser única, es posible que no esté disponible en el futuro si se elimina.
   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in&nbsp;Workfront. Only emails created from this email address are added as issues.
   -->

1. (Opcional) Seleccione **Reenviar todos los problemas que no se envíen por correo electrónico** y, a continuación, escriba una dirección de correo electrónico de reenvío en el cuadro siguiente.

   Esta dirección de correo electrónico recibe información sobre los correos electrónicos que no se han enviado al proyecto.

1. Haga clic en **Guardar**. Ahora, cuando los usuarios con una cuenta de Workfront activa envían un correo electrónico a esta dirección, se crea un problema en el proyecto de Workfront.

   >[!NOTE]
   >
   >Los usuarios deben tener acceso para crear problemas en el proyecto para poder enviarlos por correo electrónico. Puede conceder este acceso en el cuadro de diálogo Compartir en Configuración avanzada.
   >
   >Los usuarios externos no pueden enviar problemas por correo electrónico a una cola de solicitudes porque no tienen acceso para crear problemas.

## Recibir el problema en Workfront

Cuando un usuario de Workfront envía un correo electrónico a Workfront, suceden los siguientes eventos:

* La línea de asunto del correo electrónico se convierte en el nombre del problema.
* El cuerpo del correo electrónico se convierte en la descripción del problema.
* Si hay algún documento adjunto al correo electrónico, ese documento se adjunta al problema en Workfront.
* El usuario que envía el correo electrónico se convierte en el contacto principal del nuevo problema en Workfront.
* El texto del cuerpo del correo electrónico no puede superar los 4000 caracteres.
* Los archivos adjuntos del correo electrónico no pueden superar los 7 MB en total.
