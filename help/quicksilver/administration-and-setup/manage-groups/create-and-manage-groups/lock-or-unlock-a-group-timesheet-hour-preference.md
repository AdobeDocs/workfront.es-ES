---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Bloquear o desbloquear un grupo de preferencias de horas y horas
description: Si es administrador de grupos, puede configurar y luego bloquear un parte de horas y una preferencia de hora para su grupo después de que un administrador de Workfront lo desbloquee a nivel de sistema.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5b36106f-d521-4cc1-9f1f-647415c282b4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# Bloquear o desbloquear un grupo de preferencias de horas y horas

Si es administrador de grupos, puede configurar y luego bloquear un parte de horas y una preferencia de hora para su grupo después de que un administrador de Workfront lo desbloquee a nivel de sistema.

Bloquear una preferencia de Adobe Workfront garantiza que todos los miembros del grupo y de sus subgrupos usen la misma configuración para esa preferencia. Aunque aún puede volver a configurar una preferencia que bloquee, los administradores de grupos no pueden hacerlo para subgrupos inferiores.

Por el contrario, desbloquear una preferencia en el nivel de grupo permite a los administradores de subgrupos una mayor flexibilidad para administrar la forma en que sus grupos trabajan con esos elementos. Cuando se desbloquea una preferencia, los administradores del grupo pueden volver a configurarla para esos subgrupos.

Esto es paralelo a la capacidad que tiene un administrador de Workfront de bloquear o desbloquear una preferencia para todos los miembros del sistema.

Para obtener información sobre cómo un administrador de Workfront puede bloquear o desbloquear un parte de horas y una preferencia de horas para todos los grupos del sistema, consulte [Configuración de las preferencias de horas y horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Para obtener información sobre la configuración de un parte de horas y las preferencias de hora para un grupo, consulte [Configuración de las preferencias de horas y horas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

<!--
Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
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

## Bloquear o desbloquear un grupo de preferencias de horas y horas

>[!TIP]
>
>Si es administrador de Workfront, puede evitar los pasos del 1 al 4 accediendo a Configuración > Horario y horas > Preferencias y buscando el nombre del grupo en el cuadro de la parte superior de la página.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Grupos**.
1. Haga clic en el nombre del grupo en el que desea bloquear o desbloquear una preferencia de horas y hojas de horas.
1. En el panel izquierdo, haga clic en **Preferencias de horas y hojas de horas**.

1. En la página que aparece, realice una de las acciones siguientes:

   * Si desea que los administradores de los grupos situados debajo del grupo puedan configurar una preferencia para sus grupos, desbloquéela ![](assets/unlock-toggle-button.png).
   * Si desea que todos los grupos debajo de la suya utilicen la configuración para una preferencia, asegúrese de que esté bloqueada ![](assets/lock-toggle-button.png) (este es el valor predeterminado).

      >[!IMPORTANT]
      >
      >Es importante comunicarse con los administradores y usuarios de los grupos situados debajo del suyo para asegurarse de que todas las necesidades se tienen en cuenta de la forma en que configura una preferencia bloqueada. Cuando la bloquea, la configuración para ella la heredan los subgrupos siguientes. Y si la preferencia se ha desbloqueado por cualquier periodo de tiempo, la configuración sustituye a los que agrupan administradores en subgrupos inferiores que puedan haber hecho.

1. Haga clic en **Guardar**.
