---
product-area: requests
navigation-topic: create-requests
title: Permitir que los usuarios envíen por correo electrónico un problema a un proyecto de cola de solicitudes
description: Puede configurar un proyecto para permitir que los usuarios agreguen problemas al proyecto por correo electrónico.
author: Alina, Courtney
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: 06e42fa713bc9b0c1e308feb2b84ca62dafa416c
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 90%

---

# Permitir que los usuarios envíen un problema por correo electrónico a un proyecto de cola de solicitudes

<!-- Audited: 4/2025 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

Puede configurar un proyecto para permitir que los usuarios agreguen problemas al proyecto por correo electrónico. Solo puede permitir que los problemas se envíen por correo electrónico a un proyecto si este está designado como Cola de solicitudes. Para obtener más información acerca de cómo crear un proyecto de cola de solicitudes, vea [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Nuevo: colaborador o superior</p>
   O
   <p>Actual: solicitud o superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Problemas</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Se requieren las siguientes condiciones para configurar un proyecto de modo que los usuarios puedan agregar problemas al proyecto por correo electrónico:

* Los usuarios que envíen problemas por correo electrónico a esta cuenta deben ser usuarios activos con una licencia para Workfront.
* Los usuarios que envíen problemas por correo electrónico a esta cuenta deben tener permisos para agregar problemas en el proyecto.
* Los usuarios externos no pueden enviar problemas por correo electrónico a una cola de solicitudes porque no tienen acceso para crear problemas.
* Solo se permiten correos electrónicos que provengan de una dirección de correo asociada a un usuario activo de Workfront para enviar problemas al proyecto. Los correos electrónicos que se reenvían a un correo de un usuario activo de Workfront desde una dirección de correo no asociada a una cuenta de Workfront no pueden crear problemas en el proyecto, ya que se requiere que la dirección de correo del remitente original esté asociada a una cuenta activa de Workfront.
* El proyecto está configurado como una cola de solicitudes.
* La cuenta de correo asociada al proyecto no está vinculada a una cuenta de un usuario de Workfront.

## Configurar el proyecto en Workfront

>[!NOTE]
>
>Tenga en cuenta lo siguiente al habilitar la configuración de la cola de correos electrónicos:
>
>* Workfront permite un correo electrónico único por cola de solicitudes en todos los clústeres. Si decide deshabilitar su cola de solicitudes, conservará la dirección de correo electrónico que creó siempre que aún esté en el cuadro de Dirección de correo de entrada. Si decide dejar de usar el correo de entrada, debe eliminarlo del campo de Dirección de correo de entrada para que esté disponible para uso futuro.
>
>* Si la cola de solicitudes tiene varios temas o grupos de temas, Workfront seleccionará al azar el tema de la cola al que se enviarán las solicitudes por correo electrónico, lo que dificulta la gestión de dichas solicitudes.
>Recomendamos que el proyecto que configure para recibir solicitudes por correo electrónico no tenga más de un tema de cola. Si las solicitudes enviadas están destinadas a diferentes recursos o proyectos, debe redirigirlas o moverlas manualmente una vez que se hayan enviado.

1. Vaya al proyecto que desea habilitar para recibir problemas por correo electrónico.
1. Haga clic en **Detalles de cola** en el panel izquierdo.
1. En el área **Tipo de cola**, seleccione **Publicar como cola de solicitudes de ayuda**.

1. Desplácese hacia abajo hasta el área **Configuración de la cola de correos electrónicos**, luego seleccione **Habilitar recepción de solicitudes por correo electrónico**.

1. Ingrese el inicio de la dirección de correo electrónico en el cuadro **Dirección de correo de entrada**.

   Debe crear una dirección de correo electrónico única. Recomendamos utilizar el nombre de su empresa como parte de su dirección de correo de entrada.

   >[!CAUTION]
   >
   >* Esta dirección de correo electrónico no se puede recuperar de la papelera si se elimina el proyecto que contiene la cola de solicitudes.
   >
   >* Debido a que esta dirección de correo electrónico debe ser única, es posible que no esté disponible en el futuro si se elimina.
   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in&nbsp;Workfront. Only emails created from this email address are added as issues.
   -->

1. (Opcional) Seleccione **Reenviar todos los problemas que no se puedan enviar por correo electrónico**, luego ingrese una dirección de reenvío en el cuadro de abajo.

   Esta dirección de correo electrónico recibe información sobre los correos que no se pudieron enviar al proyecto.

1. Haga clic en **Guardar**. Ahora, cuando los usuarios con una cuenta activa de Workfront envían un correo a esta dirección de correo electrónico, se crea un problema en el proyecto de Workfront.

   >[!NOTE]
   >
   >Los usuarios deben tener acceso para crear problemas en el proyecto para poder enviarlos por correo electrónico. Puede otorgar este acceso en el cuadro de diálogo Compartir, en Configuración avanzada.
   >
   >Los usuarios externos no pueden enviar problemas por correo electrónico a una cola de solicitudes porque no tienen acceso para crear problemas.

## Recibir el problema en Workfront

Cuando un usuario de Workfront envía un correo electrónico a Workfront, suceden las siguientes cosas:

* La línea de asunto del correo electrónico se convierte en el nombre del problema.
* El cuerpo del correo electrónico se convierte en la descripción del problema.
* Si hay documentos adjuntos al correo electrónico, esos documentos se adjuntan al problema en Workfront.
* El usuario que envía el correo electrónico se convierte en el compañía primaria del nuevo problema en Workfront.
* El cuerpo del correo electrónico no puede exceder los 4.000 caracteres.
* Los archivos adjuntos del correo electrónico no pueden superar los 7 MB en total.
