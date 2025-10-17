---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Bloquear o desbloquear una preferencia de proyecto, tarea o problema para subgrupos
description: Como administrador de grupo, puede configurar y, a continuación, bloquear las preferencias de un proyecto, tarea o problema si un administrador de Workfront lo ha desbloqueado en el sistema.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 87%

---

# Bloquear o desbloquear una preferencia de proyecto, tarea o problema para subgrupos

Como administrador de grupo, puede configurar y, a continuación, bloquear las preferencias de un proyecto, tarea o problema si un administrador de Workfront lo ha desbloqueado en el sistema.

Al bloquear una preferencia de proyecto, tarea o problema que haya configurado en el nivel, se asegura de que todos los miembros de su grupo y de sus subgrupos utilizarán la misma configuración para esa preferencia. Aunque puede volver a configurar una preferencia que haya bloqueado para su grupo, los administradores de grupos no pueden volver a configurarla para los grupos.

Por el contrario, si se desbloquean las preferencias de un proyecto, tarea o problema, los administradores de grupos tendrán más flexibilidad para administrar el modo en que sus grupos trabajan con esos elementos. Cuando una preferencia está desbloqueada, los administradores de grupos pueden volver a configurarla para esos subgrupos.

Esto es paralelo a la capacidad que tiene un administrador de Workfront para bloquear o desbloquear una preferencia para todos los miembros del sistema.

Para obtener información sobre cómo un administrador de Workfront puede bloquear o desbloquear una preferencia para todos los grupos del sistema, consulte [Bloquear o desbloquear las preferencias de proyecto de todos los grupos del sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* La configuración de una preferencia desbloqueada para un grupo no afecta a dicha preferencia en ningún subgrupo por debajo del grupo.
>
>  Sin embargo, cuando se crea un nuevo subgrupo, este hereda la configuración de preferencias y el estado bloqueado o desbloqueado del grupo inmediatamente superior.
>
>* Si mueve un grupo bajo un grupo que tiene una preferencia bloqueada, el grupo trasladado hereda esa preferencia y queda bloqueado para el grupo movido.
>* Si mueve un grupo bajo un grupo que tiene una preferencia desbloqueada, el grupo trasladado no se verá afectado por esa preferencia.
>
>  Si la preferencia del grupo trasladado está bloqueada en el momento del traslado, permanecerá bloqueada, pero el administrador del grupo puede desbloquearla ahora porque está desbloqueada para el grupo principal.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de grupo del grupo o administrador del sistema.</td>
  </tr>
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Bloquear o desbloquear una preferencia de proyecto, tarea o problema de grupo

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos**.
1. Haga clic en el nombre del grupo en el que desea bloquear o desbloquear una preferencia de proyecto.
1. En el panel izquierdo, haga clic en **Preferencias del proyecto** o en **Preferencias de tareas y problemas**.

1. En la página que aparece, realice una de las siguientes acciones para una preferencia desbloqueada en el sistema o para un grupo por encima del suyo:

   * Si desea que los administradores de los grupos que se encuentran debajo de su grupo puedan configurar una preferencia para sus grupos, desbloquéela ![Desbloquear opción](assets/unlock-toggle-button.png).
   * Si desea que todos los grupos por debajo del suyo usen su configuración como preferencia, asegúrese de que esté bloqueado ![Bloquear alternancia](assets/lock-toggle-button.png).

     >[!IMPORTANT]
     >
     >Es importante comunicarse con los administradores y usuarios de los grupos que están debajo del suyo para asegurarse de que todas las necesidades se tengan en cuenta todas las necesidades a la hora de configurar una preferencia bloqueada. Cuando lo bloquea, la configuración que tiene asignada es heredada por cualquier subgrupo que esté por debajo. Asimismo, si la preferencia ha estado desbloqueada durante algún tiempo, su configuración sustituye a las que pudieran haber realizado los administradores de grupo de subgrupos inferiores.

1. Haga clic en **Guardar**.
