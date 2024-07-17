---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Desbloquear o bloquear la configuración de notificaciones de eventos para todos los grupos
description: Si es administrador de Adobe Workfront, puede desbloquear o volver a bloquear la capacidad de los administradores de grupos para configurar una notificación de eventos para los grupos de nivel superior que administran. La configuración de una notificación de eventos consiste en activarla o desactivarla.
author: Lisa, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: 1c0a656f2603c5decabd2bb4e88da1b9530f9e1c
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# Desbloquear o bloquear la configuración de notificaciones de eventos para todos los grupos

Si es administrador de Adobe Workfront, puede desbloquear o volver a bloquear la capacidad de los administradores de grupos para configurar una notificación de eventos para los grupos de nivel superior que administran. La configuración de una notificación de eventos consiste en activarla o desactivarla.

Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

Cuando un administrador configura una notificación de eventos para un grupo, la configuración afecta a los usuarios para los que ese grupo, o uno de sus subgrupos, es su grupo de inicio. En sus perfiles de usuario, estos usuarios ven las notificaciones de eventos activadas para su grupo de inicio en lugar de las notificaciones de eventos activadas en todo el sistema. Para obtener más información, vea [Ver y configurar notificaciones de eventos para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

>[!NOTE]
>
>* Un administrador de Workfront puede desbloquear y volver a bloquear la configuración de una notificación de evento tanto en Adobe Workfront Classic como en la nueva experiencia de Adobe Workfront. Sin embargo, un administrador de grupo solo puede configurar esa notificación de eventos para un grupo en la nueva experiencia de Adobe Workfront. Los administradores de grupos que utilicen Adobe Workfront Classic pueden cambiar a la nueva experiencia de Adobe Workfront para configurar las notificaciones de eventos desbloqueados para un grupo y, a continuación, volver a Adobe Workfront Classic para ver los cambios en vigor.
>* Los subgrupos heredan las configuraciones de notificación de eventos de nivel de grupo de los grupos de nivel superior sobre ellos.
>

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Administrador del sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

## Desbloquear o volver a bloquear la capacidad de configurar una notificación de evento

>[!IMPORTANT]
>
>Cuando vuelve a bloquear una notificación, todos los grupos del sistema heredan la notificación exactamente como la establece. Esto anula cualquier cambio que los administradores de grupo puedan haber realizado en sus grupos, por lo que es aconsejable consultar con ellos primero.

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. Haga clic en **Correo electrónico** > **Notificaciones**.

1. Asegúrese de que la ficha **Notificaciones de eventos** esté abierta.
1. Haga clic en el icono a la derecha de la notificación para cambiarlo a la posición ![Bloquear icono](assets/lock-toggle-button.png) o ![Desbloquear icono](assets/unlock-toggle-button.png) bloqueados.

   O

   Si desea desbloquear o bloquear varias notificaciones a la vez, selecciónelas y, a continuación, haga clic en el botón Desbloquear ![icono Desbloquear](assets/unlock-icon-toolbar.png) o Bloquear ![icono Bloquear](assets/lock-icon-locked-qs.png) que aparece en la barra de herramientas sobre la lista.

1. Haga clic en **Guardar**.
1. (Opcional) Si desea configurar la notificación de eventos para un grupo de nivel superior en lugar de dejar esta tarea al administrador del grupo, puede realizar una de las siguientes acciones:

   * Elimine **Notificaciones de eventos del sistema** en el cuadro de búsqueda situado encima de la lista de notificaciones, busque y seleccione el nombre del grupo de nivel superior para enumerar sus notificaciones y, a continuación, active o desactive las notificaciones desbloqueadas en la lista que se muestra.
   * Haga clic en **Grupos** en el menú de la izquierda y, a continuación, haga clic en el nombre del grupo de nivel superior. Haga clic en **Notificaciones de eventos** en el panel izquierdo y, a continuación, configure la notificación de eventos desbloqueados, tal como se explica en [Ver y configurar notificaciones de eventos para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
