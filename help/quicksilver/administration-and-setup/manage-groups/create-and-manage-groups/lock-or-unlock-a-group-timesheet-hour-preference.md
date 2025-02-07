---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Bloquear o desbloquear una hoja de horas de grupo y una preferencia de hora
description: Si es administrador de un grupo, puede configurar y bloquear una plantilla de horas y preferencias de hora para su grupo después de que un administrador de Workfront la desbloquee en el sistema.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5b36106f-d521-4cc1-9f1f-647415c282b4
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 51%

---

# Bloquear o desbloquear una plantilla de horas de grupo y sus preferencias horarias

Si es administrador de un grupo, puede configurar y bloquear una plantilla de horas y preferencias de hora para su grupo después de que un administrador de Workfront la desbloquee en el sistema.

Bloquear una preferencia de Adobe Workfront garantiza que todos los miembros del grupo y de sus subgrupos utilicen la misma configuración para esa preferencia. Aunque puede volver a configurar una preferencia que bloquee, los administradores de grupos no pueden hacerlo para los subgrupos inferiores.

Por el contrario, desbloquear una preferencia en el nivel de grupo permite a los administradores de subgrupos una mayor flexibilidad para administrar la forma en que sus grupos trabajan con esos elementos. Cuando una preferencia está desbloqueada, los administradores de grupos pueden volver a configurarla para esos subgrupos.

Esto es paralelo a la capacidad que tiene un administrador de Workfront para bloquear o desbloquear una preferencia para todos los miembros del sistema.

Para obtener información sobre cómo un administrador de Workfront puede bloquear o desbloquear una hoja de horas y las preferencias de horas para todos los grupos del sistema, consulte [Configurar las preferencias de horas y hojas de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Para obtener información sobre cómo configurar una hoja de horas y las preferencias de horas de un grupo, consulte [Configurar las preferencias de horas y hojas de horas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

<!--
Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
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

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
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

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Bloquear o desbloquear una plantilla de horas de grupo y sus preferencias horarias

>[!TIP]
>
>Si es administrador de Workfront, puede omitir los pasos del 1 al 4 desde Configuración > Plantilla de horas trabajadas y horas > Preferencias y, a continuación, buscar el nombre del grupo en el cuadro de la parte superior de la página.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos**.
1. Haga clic en el nombre del grupo en el que desee bloquear o desbloquear una plantilla de horas y una preferencia de horas.
1. En el panel izquierdo, haga clic en **Preferencias de horas y hojas de horas**.

1. En la página que aparece, realice una de las acciones siguientes:

   * Si desea que los administradores de los grupos que se encuentran debajo de su grupo puedan configurar una preferencia para sus grupos, desbloquéela ![Desbloquear opción](assets/unlock-toggle-button.png).
   * Si desea que todos los grupos por debajo del suyo usen su configuración como preferencia, asegúrese de que esté bloqueado ![Bloquear alternancia](assets/lock-toggle-button.png) (este es el valor predeterminado).

     >[!IMPORTANT]
     >
     >Es importante comunicarse con los administradores y usuarios de los grupos que están debajo del suyo para asegurarse de que todas las necesidades se tengan en cuenta todas las necesidades a la hora de configurar una preferencia bloqueada. Cuando lo bloquea, la configuración que tiene asignada es heredada por cualquier subgrupo que esté por debajo. Asimismo, si la preferencia ha estado desbloqueada durante algún tiempo, su configuración sustituye a las que pudieran haber realizado los administradores de grupo de subgrupos inferiores.

1. Haga clic en **Guardar**.
