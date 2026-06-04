---
user-type: administrator
product-area: system-administration
keywords: modificar, correo electrónico, notificación, configuración, por lote, edición por lote, configurar, varios, usuarios
navigation-topic: emails-administration
title: Modificar la configuración de notificaciones por correo electrónico de varios usuarios
description: Este artículo proporciona información para los administradores de grupos o de Workfront sobre cómo pueden actualizar las notificaciones de correo electrónico de otros usuarios.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YboJ-FC-3HsfZpI4bRi7PENzjoN-Y9gIIsElbJBUw0A
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 449
ht-degree: 88%

---

# Modificar la configuración de notificaciones por correo electrónico de varios usuarios

<!-- Audited: 12/2023 -->

Si es administrador de Adobe Workfront o tiene un nivel de acceso de Planificador que le permite editar la configuración de otros usuarios, puede definir la configuración de notificaciones para varios usuarios a la vez. Esto incluye especificar si los usuarios recibirán notificaciones cuando ocurran eventos o en un correo electrónico de resumen diario, tal como se describe en [notificaciones de Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md). Para obtener más información sobre el nivel de acceso necesario para editar usuarios, consulte [Conceder acceso a usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

También puede configurar las notificaciones por correo electrónico para un usuario, incluido su propio perfil. Para obtener más información, consulte [Modificar sus propias notificaciones por correo electrónico](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).


## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
    <p>Estándar</p>
    <p>Plan</p>
   </td>
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modificar la configuración de notificaciones por correo electrónico para varios usuarios

Cuando establece la configuración de las notificaciones por lote, únicamente puede cambiar la configuración que los usuarios seleccionados tienen en común.

Cuando modifica una configuración de notificación, aparece la etiqueta **Editada** para esa configuración de notificación para informarle de que esa configuración de notificación se ha modificado.

Para modificar la configuración de las notificaciones por correo electrónico para varios usuarios:

{{step-1-to-users}}

1. Seleccione los usuarios y haga clic en **Editar**.
1. En el cuadro **Editar persona** que aparece, haga clic en **Notificaciones**.

1. Expanda una categoría para ver la configuración de notificaciones relacionada con esa categoría.

   Si hay al menos un usuario seleccionado en el que las notificaciones no coinciden con las notificaciones de los demás usuarios seleccionados, la casilla de verificación de categoría de esa notificación contiene una línea horizontal ![Línea en lugar de marca de verificación](assets/straight-line-instead-of-checkmark.jpg).


1. Haga clic en cualquier notificación que desee que los usuarios reciban diaria o instantáneamente, o borre las notificaciones que desea que dejen de recibir.

   >[!NOTE]
   >
   >   Para la categoría **Comunicación**, puede seleccionar notificaciones individuales únicamente para envío instantáneo. Debe seleccionar todas las notificaciones que desea enviar en un resumen diario.


1. Si seleccionó que las notificaciones se enviaran como un resumen diario, seleccione la hora del día a la que desea que se envíe el resumen en la parte superior de la sección **Notificaciones** en el menú **Resumen diario de correo electrónico después de**.

   ![Tiempo de resumen diario](assets/daily-digest-time.png)

   El resumen diario incluye eventos que cumplen los criterios de las notificaciones 24 horas antes de la hora seleccionada. Los usuarios reciben un correo electrónico de resumen diario para cada tipo de notificación.

   El resumen diario puede llegar después del tiempo seleccionado, según la cantidad de correos electrónicos en cola para su envío en el sistema. La hora indicada es la hora local según se especifica en la configuración del explorador.
