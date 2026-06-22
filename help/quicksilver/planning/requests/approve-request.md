---
title: Aprobar una solicitud en Adobe Workfront Planning
description: Cuando un usuario envía una solicitud a un formulario de solicitud asociado a una aprobación en Adobe Workfront Planning, los aprobadores reciben una notificación y un correo electrónico sobre la aprobación pendiente. Deben aprobar la solicitud antes de que Workfront Planning cree un objeto.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: aca9b313-3420-43f6-8f6c-dd74888bd120
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/u8dbV85NLabPjFj0-gsjPO1vz3mrmgU9yKxRBttHhtY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87effid: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 999
ht-degree: 8%

---

# Aprobar una solicitud en Adobe Workfront Planning

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Cuando un usuario envía una solicitud a un formulario de solicitud asociado a una aprobación en Adobe Workfront Planning, los aprobadores reciben una notificación y un correo electrónico sobre la aprobación pendiente. Deben aprobar la solicitud antes de que Workfront Planning cree un objeto.

En este artículo se describe cómo un administrador del espacio de trabajo puede aprobar una solicitud enviada para que Workfront Planning cree un registro.

Le recomendamos que también vea los siguientes artículos:

* [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* [Enviar solicitudes de Adobe Workfront Planning para crear registros](/help/quicksilver/planning/requests/submit-requests.md)
* [Añadir una aprobación a un formulario de solicitud](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## Consideraciones sobre la aprobación de solicitudes

* Las solicitudes enviadas se muestran en el área Solicitudes de Workfront con uno de los siguientes estados de solicitud:

   * **Revisión pendiente**: Este estado se muestra cuando ninguno de los aprobadores ha abierto el objeto de solicitud.
   * **En revisión**: El estado de **Revisión pendiente** cambia a **En revisión** cuando al menos un aprobador abre el objeto de solicitud. El estado de la solicitud permanece **en revisión** hasta que todos los aprobadores hayan aprobado la solicitud.
   * **Aprobado**: cuando un aprobador aprueba el objeto de solicitud, su estado individual pasa a ser **Aprobado**, pero el estado general del objeto de solicitud permanece **En revisión** hasta que todos los aprobadores hayan tomado sus decisiones. Cuando todos los aprobadores aprueban una solicitud, su estado pasa a ser **Aprobado**.
   * **Completada**: si todos los aprobadores aprueban el objeto de solicitud, su estado cambia a **Completada** o si la solicitud no necesita aprobación.
   * **Rechazado**: Si algún aprobador rechaza el objeto de solicitud, el estado pasa a ser **Rechazado**. No se crea ningún registro y se debe enviar una nueva solicitud para crear el registro.

* Puede mostrar la información de aprobación de un registro creado enviando un formulario de solicitud en los campos Aprobado por y Fecha de aprobación. Para obtener más información, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Paquetes de Adobe Workfront</p></td> 
   <td> 
<p>Cualquier paquete Workfront y cualquier paquete Planning</p>
O
<p>Cualquier paquete de flujo de trabajo y cualquier paquete de Planning</p>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Cualquiera</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Administrar permisos a un espacio de trabajo y tipo de registro</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aprobar una solicitud de Planning para crear un registro

Después de que los usuarios agreguen solicitudes a un formulario de solicitud de tipo de registro asociado a una aprobación, la solicitud se envía a los aprobadores.

Los aprobadores reciben las siguientes notificaciones sobre una solicitud pendiente de aprobación:

* Una notificación en la aplicación
* Una notificación por correo electrónico

Para obtener información sobre la aprobación de solicitudes de notificaciones, consulte los siguientes artículos:

* [Administrar notificaciones por correo electrónico de Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md)
* [Administrar notificaciones en la aplicación de Planificación de Adobe Workfront](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md)

>[!NOTE]
>
>La instancia de Workfront de su organización debe incorporarse a la experiencia unificada de Adobe para que los usuarios puedan recibir notificaciones por correo electrónico y en la aplicación.

Puede aprobar solicitudes para crear registros desde la propia solicitud o desde el widget Mis aprobaciones en Inicio.

### Aprobar una solicitud de Planning desde una notificación o desde el área de solicitudes

1. Abra la solicitud siguiendo uno de estos procedimientos:

   * Haga clic en **Menú principal** ![Menú principal de líneas](assets/lines-menu.png) en la esquina superior izquierda, luego haga clic en **Solicitudes** > **Usar nueva experiencia** y haga clic en la solicitud con el estado de **Revisión pendiente**.

     >[!TIP]
     >
     >* Si no tiene acceso a Workfront Planning o no tiene acceso para ver ningún espacio de trabajo, solo puede acceder a una solicitud para aprobarla mediante el correo electrónico o las notificaciones en la aplicación.
     >* No puede acceder a las solicitudes de Planning desde la experiencia de solicitud heredada.

   * Haga clic en el icono del área **Notificaciones** ![Icono del área Notificaciones en Unified Shell](assets/notifications-area-icon-unified-shell.png) en la esquina superior derecha de la pantalla y haga clic en la notificación sobre una solicitud pendiente de su aprobación para abrirla.
   * Vaya a la notificación por correo electrónico del mensaje que le notifica una solicitud pendiente de aprobación y, a continuación, haga clic en **Abrir solicitud** para abrir la solicitud.

   La página de solicitud se abre en modo de solo lectura.

   ![Página de solicitud de solo lectura en el estado de revisión](assets/read-only-reqeust-page-in-review-status.png)
1. (Opcional) Haga clic en el icono **Aprobaciones** ![Icono de aprobaciones](assets/approvals-icon.png) en la esquina superior derecha de la solicitud para ver los aprobadores.
1. Haga clic en **Revisar y aprobar**, y después elija una de las siguientes opciones:

   * **Aprobar**: Esto aprueba la solicitud. Se crea inmediatamente un registro para el tipo de registro asociado al formulario de solicitud después de que todos los aprobadores aprueben la solicitud.
   * **Rechazar**: Esto rechaza la solicitud, incluso cuando usted es el único aprobador que la rechaza. No se crea ningún registro para el tipo de registro asociado al formulario de solicitud.

   El usuario que ha enviado la solicitud recibe un correo electrónico y una notificación dentro de la aplicación cuando se aprueba o rechaza su solicitud.

   El estado de la solicitud cambia a lo siguiente, según la decisión de aprobación:

   * **Completada**: la solicitud está aprobada.
   * **Rechazada**: la solicitud es rechazada.

   La solicitud permanece en el área de **Solicitudes** de Workfront.

### Aprobar una solicitud del widget Mis aprobaciones en Inicio

{{step1-to-home}}

1. Vaya al widget **Mis aprobaciones** en **Inicio**.

   ![Widget de mis aprobaciones en Inicio](assets/my-approvals-widget-in-home.png)
1. Busque la solicitud de Planning que desea aprobar o rechazar.

1. (Opcional) Agregue un comentario haciendo clic en la flecha desplegable junto a **Aprobar** o **Rechazar**, escribiendo la nota y haciendo clic en **Agregar**.

1. Haga clic en una de las siguientes opciones:

   * **Aprobar**: Esto aprueba la solicitud. Se crea inmediatamente un registro para el tipo de registro asociado al formulario de solicitud después de que todos los aprobadores aprueben la solicitud.
   * **Rechazar**: Esto rechaza la solicitud, incluso cuando usted es el único aprobador que la rechaza. No se crea ningún registro para el tipo de registro asociado al formulario de solicitud.

   El usuario que ha enviado la solicitud recibe un correo electrónico y una notificación dentro de la aplicación cuando se aprueba o rechaza su solicitud.

   El estado de la solicitud cambia a lo siguiente, según la decisión de aprobación:

   * **Completada**: la solicitud está aprobada.
   * **Rechazada**: la solicitud es rechazada.

