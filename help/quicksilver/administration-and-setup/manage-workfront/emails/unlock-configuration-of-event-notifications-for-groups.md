---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Desbloquear o bloquear la configuración de las notificaciones de eventos para todos los grupos
description: Si es administrador de Adobe Workfront, puede desbloquear o volver a bloquear la capacidad de los administradores de grupos para configurar una notificación de evento para los grupos de nivel superior que administran. La configuración de una notificación de evento consiste en activarla o desactivarla.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# Desbloquear o bloquear la configuración de las notificaciones de eventos para todos los grupos

Si es administrador de Adobe Workfront, puede desbloquear o volver a bloquear la capacidad de los administradores de grupos para configurar una notificación de evento para los grupos de nivel superior que administran. La configuración de una notificación de evento consiste en activarla o desactivarla.

Si hay algún grupo por encima del grupo que administra, sus administradores también pueden hacerlo por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

Cuando un administrador configura una notificación de evento para un grupo, la configuración afecta a los usuarios para los que dicho grupo, o uno de sus subgrupos, sea su grupo de inicio. En sus perfiles de usuario, estos usuarios ven las notificaciones de eventos activadas para su grupo principal en lugar de las notificaciones de eventos activadas en todo el sistema. Para obtener más información, consulte [Ver y configurar notificaciones de eventos para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

>[!NOTE]
>
>* Un administrador de Workfront puede desbloquear y volver a bloquear la configuración para una notificación de evento tanto en Adobe Workfront Classic como en la nueva experiencia de Adobe Workfront. Sin embargo, un administrador de grupo puede configurar esa notificación de evento para un grupo solo en la nueva experiencia de Adobe Workfront. Los administradores de grupos que utilizan Adobe Workfront Classic pueden cambiar a la nueva experiencia de Adobe Workfront para configurar las notificaciones de eventos desbloqueados para un grupo y, a continuación, volver a Adobe Workfront Classic para ver los cambios en vigor.
>* Los subgrupos heredan las configuraciones de notificación de eventos de nivel de grupo de los grupos de nivel superior por encima de ellos.
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
>Cuando vuelve a bloquear una notificación, todos los grupos del sistema heredan la notificación exactamente como la configuró. Esto anula los cambios que los administradores de grupos puedan haber realizado para sus grupos, por lo que es aconsejable consultarlos primero.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Correo electrónico** > **Notificaciones**.

1. Asegúrese de que la variable **Notificaciones de eventos** está abierta.
1. Haga clic en el icono a la derecha de la notificación para cambiarla a la ![](assets/lock-toggle-button.png) o bloqueado ![](assets/unlock-toggle-button.png) posición.

   O

   Si desea desbloquear o bloquear varias notificaciones a la vez, selecciónelas y haga clic en el botón Desbloquear ![](assets/unlock-icon-toolbar.png) o Bloquear ![](assets/lock-icon-locked-qs.png) que se muestra en la barra de herramientas situada encima de la lista.

1. Haga clic en **Guardar**.
1. (Opcional) Si desea configurar la notificación de evento para un grupo de nivel superior en lugar de dejar esta tarea al administrador del grupo, puede realizar una de las siguientes acciones:

   * Eliminar **Notificaciones de eventos del sistema** en el cuadro de búsqueda situado encima de la lista de notificaciones, busque y seleccione el nombre del grupo de nivel superior para enumerar sus notificaciones y, a continuación, active o desactive las notificaciones desbloqueadas en la lista que se muestra.
   * Haga clic en **Grupos** en el menú de la izquierda, haga clic en el nombre del grupo de nivel superior. Haga clic en **Notificaciones de eventos** en el panel izquierdo, configure la notificación de evento desbloqueado como se explica en [Ver y configurar notificaciones de eventos para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
