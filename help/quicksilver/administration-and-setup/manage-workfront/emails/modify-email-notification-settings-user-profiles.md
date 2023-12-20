---
user-type: administrator
product-area: system-administration
keywords: modificar,correo electrónico,notificación,configuración,masiva,edición masiva,configurar,varios,usuarios
navigation-topic: emails-administration
title: Modificar la configuración de notificaciones por correo electrónico de varios usuarios
description: Este artículo proporciona información para los administradores de grupos o Workfront sobre cómo pueden actualizar las notificaciones de correo electrónico de otros usuarios.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: d98bb6b6bb8ff3bff6f367f1376948d5104887e5
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# Modificar la configuración de notificaciones por correo electrónico de varios usuarios

<!-- Audited: 12/2023 -->

Si es administrador de Adobe Workfront o tiene un nivel de acceso de Planificador que le permite editar la configuración de otros usuarios, puede definir la configuración de notificaciones para varios usuarios a la vez. Esto incluye especificar si los usuarios recibirán notificaciones cuando ocurran eventos o en un correo electrónico de resumen diario, como se describe en [Notificaciones de Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md). Para obtener información sobre el nivel de acceso necesario para editar usuarios, consulte [Concesión de acceso a los usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

También puede configurar las notificaciones por correo electrónico para un usuario a la vez, incluido su propio perfil. Para obtener más información, consulte [Modificar sus propias notificaciones por correo electrónico](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).


## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nuevo plan: Estándar </p>
 <p>o</p> 
<p>Plan actual: plan </p> 
</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan o tipo de licencia tiene, póngase en contacto con su administrador de Workfront.

## Modificar la configuración de notificaciones por correo electrónico para varios usuarios

Cuando establece la configuración de las notificaciones de forma masiva, solo puede cambiar la configuración que los usuarios seleccionados tienen en común.

Al modificar una configuración de notificación, la etiqueta **Editado** aparece para esa configuración de notificación, para hacerle saber que esa configuración de notificación se ha modificado.

Para modificar la configuración de las notificaciones por correo electrónico para varios usuarios:

{{step-1-to-users}}

1. Seleccione los usuarios y haga clic en **Editar**.
1. En el **Editar persona** que aparece, haga clic en **Notificaciones**.

1. Expanda una categoría para ver la configuración de notificaciones relacionada con esa categoría.

   Si hay al menos un usuario seleccionado y las notificaciones no coinciden con las de los demás usuarios seleccionados, la casilla de verificación de la categoría de esa notificación contiene una línea horizontal ![](assets/straight-line-instead-of-checkmark.jpg) en lugar de una marca de verificación.


1. Haga clic en cualquier notificación que desee que los usuarios reciban diaria o instantáneamente, o borre las notificaciones que desee que dejen de recibir.

   >[!NOTE]
   >
   >   Para el **Comunicación** categoría, puede seleccionar notificaciones individuales solo para envío instantáneo. Debe seleccionar todas las notificaciones que desea enviar en un compendio diario.


1. Si ha seleccionado que las notificaciones se envíen como un resumen diario, seleccione la hora del día a la que desea que se envíe el resumen en la parte superior de la **Notificaciones** de la sección **Enviar correo electrónico de resumen diario después de** menú.

   ![](assets/daily-digest-time.png)

   El compendio diario incluye eventos que cumplen los criterios de las notificaciones 24 horas antes de la hora seleccionada. Los usuarios reciben un correo electrónico de resumen diario para cada tipo de notificación.

   El resumen diario puede llegar después del tiempo seleccionado, según la cantidad de correos electrónicos en cola para su envío en el sistema. La hora indicada es la hora local según se especifica en la configuración del explorador.
