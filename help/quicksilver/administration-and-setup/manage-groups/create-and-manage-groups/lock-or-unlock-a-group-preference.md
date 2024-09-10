---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Bloquear o desbloquear una preferencia de proyecto, tarea o problema para subgrupos
description: Como administrador de grupo, puede configurar y, a continuación, bloquear las preferencias de un proyecto, tarea o problema si un administrador de Workfront lo ha desbloqueado en el sistema.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# Bloquear o desbloquear una preferencia de proyecto, tarea o problema para subgrupos

Como administrador de grupo, puede configurar y, a continuación, bloquear las preferencias de un proyecto, tarea o problema si un administrador de Workfront lo ha desbloqueado en el sistema.

Bloquear una preferencia de proyecto, tarea o problema que haya configurado en el nivel garantiza que todos los miembros de su grupo y de sus subgrupos utilizarán la misma configuración para esa preferencia. Aunque todavía puede volver a configurar una preferencia que bloquee para su grupo, los administradores de grupos no pueden volver a configurarla para los grupos.

Por el contrario, si se desbloquean las preferencias de un proyecto, tarea o problema, los administradores de grupos tendrán más flexibilidad para administrar el modo en que sus grupos trabajan con esos elementos. Cuando una preferencia está desbloqueada, los administradores de grupos pueden volver a configurarla para esos subgrupos.

Esto es paralelo a la capacidad que tiene un administrador de Workfront para bloquear o desbloquear una preferencia para todos los miembros del sistema.

Para obtener información sobre cómo un administrador de Workfront puede bloquear o desbloquear una preferencia para todos los grupos del sistema, consulte [Bloquear o desbloquear preferencias de proyecto para todos los grupos del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* La configuración de una preferencia desbloqueada para un grupo no afecta a esa preferencia en ningún subgrupo por debajo del grupo.
>
>  Sin embargo, cuando se crea un nuevo subgrupo, éste hereda la configuración de preferencias y el estado bloqueado o desbloqueado del grupo inmediatamente por encima.
>
>* Si mueve un grupo a un grupo que tiene una preferencia bloqueada, el grupo movido hereda esa preferencia y está bloqueado para el grupo movido.
>* Si mueve un grupo a un grupo que tiene una preferencia desbloqueada, el grupo movido no se verá afectado por esa preferencia.
>
>  Si la preferencia del grupo movido está bloqueada en el momento del movimiento, permanecerá bloqueada, pero el administrador del grupo puede desbloquearla ahora porque está desbloqueada para el grupo principal.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>O</p>
       <p>Actual: plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de grupo del grupo o administrador del sistema.</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Bloquear o desbloquear una preferencia de proyecto, tarea o problema de grupo

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos**.
1. Haga clic en el nombre del grupo en el que desea bloquear o desbloquear una preferencia de proyecto.
1. En el panel izquierdo, haga clic en **Preferencias de proyecto** o en **Preferencias de tareas y problemas**.

1. En la página que aparece, realice una de las siguientes acciones para una preferencia desbloqueada en el sistema o para un grupo por encima del suyo:

   * Si desea que los administradores de los grupos que se encuentran debajo de su grupo puedan configurar una preferencia para sus grupos, desbloquéela ![](assets/unlock-toggle-button.png).
   * Si desea que todos los grupos por debajo del suyo usen su configuración como preferencia, asegúrese de que esté bloqueado ![](assets/lock-toggle-button.png).

     >[!IMPORTANT]
     >
     >Es importante comunicarse con los administradores y usuarios de los grupos que están debajo del suyo para asegurarse de que todas las necesidades se tienen en cuenta de la forma en que configura una preferencia bloqueada. Cuando lo bloquea, la configuración para él la heredan los subgrupos a continuación. Y si la preferencia se ha desbloqueado durante cualquier período de tiempo, la configuración reemplaza las que los administradores de grupos en subgrupos inferiores puedan haber realizado.

1. Haga clic en **Guardar**.
