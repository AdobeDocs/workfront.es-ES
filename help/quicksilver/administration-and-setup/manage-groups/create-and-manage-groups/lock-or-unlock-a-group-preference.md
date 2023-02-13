---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Bloquear o desbloquear un proyecto, tarea o preferencia de problemas para subgrupos
description: Como administrador de grupo, puede configurar y luego bloquear un proyecto, tarea o preferencia de problema si un administrador de Workfront lo ha desbloqueado a nivel de sistema.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Bloquear o desbloquear un proyecto, tarea o preferencia de problemas para subgrupos

Como administrador de grupo, puede configurar y luego bloquear un proyecto, tarea o preferencia de problema si un administrador de Workfront lo ha desbloqueado a nivel de sistema.

Bloquear un proyecto, tarea o preferencia de problema que haya configurado en el nivel garantiza que todos los miembros del grupo y de sus subgrupos usen la misma configuración para esa preferencia. Aunque aún puede volver a configurar una preferencia que bloquee para su grupo, los administradores de grupos no podrán volver a configurarla para grupos.

Por el contrario, al desbloquear un proyecto, una tarea o una preferencia de problemas, los administradores de grupos pueden disponer de más flexibilidad para administrar la forma en que sus grupos trabajan con esos elementos. Cuando se desbloquea una preferencia, los administradores del grupo pueden volver a configurarla para esos subgrupos.

Esto es paralelo a la capacidad que tiene un administrador de Workfront de bloquear o desbloquear una preferencia para todos los miembros del sistema.

Para obtener información sobre cómo un administrador de Workfront puede bloquear o desbloquear una preferencia para todos los grupos del sistema, consulte [Bloquear o desbloquear las preferencias del proyecto para todos los grupos del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* La configuración de una preferencia desbloqueada para un grupo no afecta a esa preferencia para ningún subgrupo debajo del grupo.
>
>  Sin embargo, cuando se crea un nuevo subgrupo, hereda la configuración de preferencias y el estado bloqueado o desbloqueado del grupo inmediatamente por encima.
>
>* Si mueve un grupo debajo de un grupo que tiene una preferencia bloqueada, el grupo movido heredará esa preferencia y se bloqueará para el grupo movido.
>* Si mueve un grupo debajo de un grupo que tiene una preferencia desbloqueada, el grupo movido no se verá afectado por esa preferencia.
>
>  Si la preferencia del grupo movido está bloqueada en el momento del movimiento, permanece bloqueada, pero el administrador del grupo puede desbloquearla ahora porque está desbloqueada para el grupo principal.

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Debe ser administrador de grupo del grupo o administrador de Workfront. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> y <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con el administrador de Workfront.

## Bloquear o desbloquear un proyecto, una tarea o una preferencia de problema de grupo

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Grupos**.
1. Haga clic en el nombre del grupo en el que desea bloquear o desbloquear una preferencia de proyecto.
1. En el panel izquierdo, haga clic en **Preferencias de proyecto** o **Preferencias de Tareas y problemas**.

1. En la página que aparece, realice una de las siguientes acciones con una preferencia desbloqueada a nivel de sistema o con un grupo por encima de su grupo:

   * Si desea que los administradores de los grupos situados debajo del grupo puedan configurar una preferencia para sus grupos, desbloquéela ![](assets/unlock-toggle-button.png).
   * Si desea que todos los grupos debajo de la suya utilicen la configuración para una preferencia, asegúrese de que esté bloqueada ![](assets/lock-toggle-button.png).

      >[!IMPORTANT]
      >
      >Es importante comunicarse con los administradores y usuarios de los grupos situados debajo del suyo para asegurarse de que todas las necesidades se tienen en cuenta de la forma en que configura una preferencia bloqueada. Cuando la bloquea, la configuración para ella la heredan los subgrupos siguientes. Y si la preferencia se ha desbloqueado por cualquier periodo de tiempo, la configuración sustituye a los que agrupan administradores en subgrupos inferiores que puedan haber hecho.

1. Haga clic en **Guardar**.
