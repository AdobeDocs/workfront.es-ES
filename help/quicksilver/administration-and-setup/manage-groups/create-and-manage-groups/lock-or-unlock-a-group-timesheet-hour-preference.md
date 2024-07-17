---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Bloquear o desbloquear una plantilla de horas de grupo y sus preferencias horarias
description: Si es administrador de un grupo, puede configurar y bloquear una plantilla de horas y preferencias de hora para su grupo después de que un administrador de Workfront la desbloquee en el sistema.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5b36106f-d521-4cc1-9f1f-647415c282b4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 0%

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
>* La configuración de una preferencia desbloqueada para un grupo no afecta a esa preferencia en ningún subgrupo por debajo del grupo.
>
>  Sin embargo, cuando se crea un nuevo subgrupo, éste hereda la configuración de preferencias y el estado bloqueado o desbloqueado del grupo inmediatamente por encima.
>
>* Si mueve un grupo a un grupo que tiene una preferencia bloqueada, el grupo movido hereda esa preferencia y está bloqueado para el grupo movido.
>* Si mueve un grupo a un grupo que tiene una preferencia desbloqueada, el grupo movido no se verá afectado por esa preferencia.
>
>  Si la preferencia del grupo movido está bloqueada en el momento del movimiento, permanecerá bloqueada, pero el administrador del grupo puede desbloquearla ahora porque está desbloqueada para el grupo principal.
>

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> <p>Debe ser administrador de grupo del grupo o de Workfront. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> y <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Si necesita saber qué plan o tipo de licencia tiene, póngase en contacto con su administrador de Workfront.

## Bloquear o desbloquear una plantilla de horas de grupo y sus preferencias horarias

>[!TIP]
>
>Si es administrador de Workfront, puede omitir los pasos del 1 al 4 en Configuración > Plantilla de horas y Horas > Preferencias y, a continuación, buscar el nombre del grupo en el cuadro de la parte superior de la página.

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Grupos**.
1. Haga clic en el nombre del grupo en el que desee bloquear o desbloquear una plantilla de horas y una preferencia de horas.
1. En el panel izquierdo, haga clic en **Preferencias de horas y hojas de horas**.

1. En la página que aparece, realice una de las acciones siguientes:

   * Si desea que los administradores de los grupos que se encuentran debajo de su grupo puedan configurar una preferencia para sus grupos, desbloquéela ![](assets/unlock-toggle-button.png).
   * Si desea que todos los grupos por debajo del suyo usen su configuración como preferencia, asegúrese de que esté bloqueado ![](assets/lock-toggle-button.png) (este es el valor predeterminado).

     >[!IMPORTANT]
     >
     >Es importante comunicarse con los administradores y usuarios de los grupos que están debajo del suyo para asegurarse de que todas las necesidades se tienen en cuenta de la forma en que configura una preferencia bloqueada. Cuando lo bloquea, la configuración para él la heredan los subgrupos a continuación. Y si la preferencia se ha desbloqueado durante cualquier período de tiempo, la configuración reemplaza las que los administradores de grupos en subgrupos inferiores puedan haber realizado.

1. Haga clic en **Guardar**.
