---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Desbloquear o bloquear la configuración de las notificaciones de eventos para todos los grupos
description: Si se trata de un administrador de Adobe Workfront, puede desbloquear o volver a bloquear la capacidad de los administradores de grupos para configurar una notificación de eventos para los grupos de nivel superior que administren. La configuración de una notificación de eventos consiste en activarla o desactivarla.
author: Lisa, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: e34abb5ff1068de99eaba33dc95287164e556742
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 97%

---

# Desbloqueo o bloqueo de la configuración de notificaciones de eventos para todos los grupos

Si se trata de un administrador de Adobe Workfront, puede desbloquear o volver a bloquear la capacidad de los administradores de grupos para configurar una notificación de eventos para los grupos de nivel superior que administren. La configuración de una notificación de eventos consiste en activarla o desactivarla.

Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

Cuando un administrador configure una notificación de eventos para un grupo, la configuración afectará a los usuarios para los que ese grupo, o uno de sus subgrupos, sea su grupo de inicio. Estos usuarios verán en los perfiles de usuario las notificaciones de eventos activadas para su grupo de inicio en lugar de las notificaciones de eventos activadas en todo el sistema. Para obtener más información, consulte [Ver y configurar notificaciones de eventos para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

>[!NOTE]
>
>* Los administradores de Workfront pueden desbloquear y volver a bloquear la configuración de una notificación de eventos tanto en Adobe Workfront Classic como en la nueva experiencia de Adobe Workfront. Sin embargo, los administradores de grupo solo podrá configurar esa notificación de eventos para un grupo en la nueva experiencia de Adobe Workfront. Los administradores de grupos que utilicen Adobe Workfront Classic pueden cambiar a la nueva experiencia de Adobe Workfront para configurar las notificaciones de eventos desbloqueados para un grupo y, a continuación, volver a Adobe Workfront Classic para ver los cambios realizados.
>* Los subgrupos heredan las configuraciones de notificación de eventos de nivel de grupo de los grupos de nivel superior sobre ellos.
>

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Estándar</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Administrador del sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Desbloquear o volver a bloquear la capacidad de configurar una notificación de eventos

>[!IMPORTANT]
>
>Al volver a bloquear una notificación, todos los grupos del sistema heredarán la notificación exactamente como se establezca. Esto anulará cualquier cambio que los administradores de grupo pudieran haber realizado en sus grupos, por lo que es aconsejable consultarles en primer lugar.

{{step-1-to-setup}}

1. Haga clic en **Correo electrónico** > **Notificaciones**.

1. Asegúrese de que la pestaña **Notificaciones de eventos** esté abierta.
1. Haga clic en el icono de la derecha de la notificación para cambiarlo a la posición de bloqueo ![Bloquear icono](assets/lock-toggle-button.png) o de desbloqueo ![Desbloquear icono](assets/unlock-toggle-button.png).

   O

   Si quisiera desbloquear o bloquear varias notificaciones a la vez, selecciónelas y, a continuación, haga clic en el botón de desbloqueo del ![icono desbloquear](assets/unlock-icon-toolbar.png) o de bloqueo del ![icono bloquear](assets/lock-icon-locked-qs.png) que se muestra en la barra de herramientas situada sobre la lista.

1. Haga clic en **Guardar**.
1. (Opcional) Si desea configurar la notificación de eventos para un grupo de nivel superior en lugar de dejar esta tarea al administrador del grupo, realice una de las siguientes acciones:

   * Elimine **Notificaciones de eventos del sistema** en el cuadro de búsqueda situado encima de la lista de notificaciones, busque y seleccione el nombre del grupo de nivel superior para enumerar sus notificaciones y, a continuación, active o desactive las notificaciones desbloqueadas en la lista que se muestra.
   * Haga clic en **Grupos**, en el menú de la izquierda y, a continuación, haga clic en el nombre del grupo de nivel superior. Haga clic en **Notificaciones de eventos**, en el panel izquierdo y, a continuación, configure la notificación de eventos desbloqueados, tal y como se explica en [Ver y configurar notificaciones de eventos para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
