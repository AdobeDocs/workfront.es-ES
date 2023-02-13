---
user-type: administrator
product-area: system-administration
keywords: modificar,correo electrónico,notificación,configuración,edición masiva,configurar,varios,usuarios
navigation-topic: emails-administration
title: Modificación de la configuración de las notificaciones por correo electrónico en los perfiles de los usuarios
description: Si es administrador de Adobe Workfront o tiene un nivel de acceso de Planificador que le permite editar la configuración de otros usuarios, puede configurar la configuración de notificación para varios usuarios al mismo tiempo. Esto incluye especificar si los usuarios reciben notificaciones cuando se producen eventos o en un compendio diario de correo electrónico, tal como se describe en las notificaciones de Adobe Workfront. Para obtener información sobre el nivel de acceso necesario para editar usuarios, consulte Concesión de acceso a usuarios.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---

# Modificación de la configuración de las notificaciones por correo electrónico en los perfiles de los usuarios

Si es administrador de Adobe Workfront o tiene un nivel de acceso de Planificador que le permite editar la configuración de otros usuarios, puede configurar la configuración de notificación para varios usuarios al mismo tiempo. Esto incluye especificar si los usuarios reciben notificaciones cuando se producen eventos o en un resumen diario de correo electrónico, tal como se describe en [Notificaciones de Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md). Para obtener información sobre el nivel de acceso necesario para editar usuarios, consulte [Conceder acceso a los usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Cuando configura la configuración de notificaciones de forma masiva, solo puede cambiar la configuración que tienen en común los usuarios seleccionados.

También puede configurar las notificaciones por correo electrónico para un usuario a la vez. Para obtener más información, consulte [Activar o desactivar sus propias notificaciones de eventos](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan o tipo de licencia tiene, póngase en contacto con el administrador de Workfront.

## Modificación de la configuración de notificación por correo electrónico de varios usuarios de forma masiva

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Usuarios** ![](assets/users-icon-in-main-menu.png). Seleccione los usuarios y haga clic en **Editar**.
1. En el **Editar persona** que aparece, haga clic en **Notificaciones**.

1. Expanda una categoría para ver la configuración de notificación relacionada con esa categoría.

   Si hay al menos un usuario seleccionado en el que las notificaciones no coinciden con las notificaciones de los demás usuarios seleccionados, la casilla de verificación de la categoría para esa notificación contiene una línea horizontal ![](assets/straight-line-instead-of-checkmark.jpg) en lugar de una marca de verificación.

1. Haga clic en las notificaciones que desee que reciban los usuarios diariamente o al instante, o borre las que desee que dejen de recibir.

   Para la variable **Comunicación** , puede seleccionar notificaciones individuales solo para envío instantáneo. Debe seleccionar todas las notificaciones que desea enviar en un compendio diario.

   Al modificar una configuración de notificación, la etiqueta **Editado** para esa configuración de notificación, para informarle de que se ha modificado dicha configuración de notificación.

1. Si ha seleccionado que las notificaciones se envíen como un compendio diario, seleccione la hora del día en la que desea que se envíe el compendio en la parte superior del **Notificaciones** en la sección **Enviar un resumen diario por correo electrónico después de** para abrir el Navegador.

   Después de seleccionar una hora de envío, la variable **Enviar un resumen diario por correo electrónico después de** se muestra con un marco naranja para indicar que se ha editado la hora de la entrega.

   El compendio diario incluye eventos que cumplen los criterios de las notificaciones 24 horas antes de la hora seleccionada. Los usuarios reciben un correo electrónico de resumen diario por cada tipo de notificación.

   El compendio diario puede llegar después del tiempo seleccionado, dependiendo de cuántos correos electrónicos se hayan puesto en cola para su envío en el sistema. La hora que aparece es la hora local, tal como se especifica en la configuración del explorador.
