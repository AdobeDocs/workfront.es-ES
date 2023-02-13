---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Eliminar un estado de grupo
description: Como administrador de grupos, puede eliminar un estado de un grupo que administra si no está configurado como estado obligatorio o bloqueado en el nivel del sistema o para un grupo superior en la jerarquía.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: bfce0325-fe6e-459f-96ca-9a5c94c61ed3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# Eliminar un estado de grupo

Como administrador de grupos, puede eliminar un estado de un grupo que administra si no está configurado como estado obligatorio o bloqueado en el nivel del sistema o para un grupo superior en la jerarquía.

Si hay algún grupo por encima del grupo que administra, sus administradores también pueden hacerlo por su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

>[!NOTE]
>
>No puede eliminar lo siguiente:
>
>* Los estados integrados son Planning, Current y Complete. Puede actualizar sus nombres, editar sus colores y bloquearlos o desbloquearlos, pero no se pueden eliminar.
>* Estados que están en estado de aprobación pendiente para al menos un objeto asociado al grupo o a uno de sus subgrupos.


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

## Eliminar un estado de grupo

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Grupos**.
1. Haga clic en el nombre del grupo de nivel superior.
1. En el panel izquierdo, haga clic en **Estados**.
1. En la lista de estados que se muestran, pase el ratón sobre el estado que desee eliminar y haga clic en **Eliminar** cuando parezca a la derecha.

   ![](assets/hover-click-delete.jpg)

1. En el cuadro que aparece, seleccione un estado para designar un estado de reemplazo para los objetos (proyectos, tareas, problemas y procesos de aprobación) que estaban utilizando el estado que está eliminando.

   Solo están disponibles los estados que coinciden con el estado que está eliminando. Por ejemplo, si está eliminando un estado que es igual a Actual, solo puede ver estados que sean iguales a Actual.

   Además, los estados que se muestran dependen de si el estado que elimine está desbloqueado o bloqueado:

   * **Si está desbloqueado**: Los estados sin bloquear y sin bloquear están disponibles.

      Junto con los estados creados para el subgrupo, se incluyen los estados heredados de los grupos de nivel superior y de nivel del sistema.

   * **Si está bloqueado**: Uno de los siguientes es true:

      * Si hay otros estados bloqueados y no ocultos, solo están disponibles.
      * Si no hay ningún estado bloqueado no oculto, el estado predeterminado de Workfront está disponible, aunque esté oculto o desbloqueado.

         Para obtener información sobre los estados predeterminados de Workfront, consulte [Acceso a la lista de estados de proyectos del sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md), [Acceso a la lista de estados de tareas del sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)y la información sobre los 4 estados de problema requeridos en [Acceda a la lista de estados de problemas del sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md).

1. Haga clic en **Eliminar estado**.

   Si el estado eliminado era el estado predeterminado para ese tipo en el grupo, el estado de reemplazo ocupará su lugar.

   Si el estado eliminado se estableció como el estado predeterminado del proyecto en las preferencias del proyecto, la preferencia se establece ahora en el estado de reemplazo.

## Cuando se elimina un grupo

Cuando se elimina un grupo y se reemplaza por otro grupo, cualquier estado único que tuviera el grupo eliminado se agrega a los estados del grupo de reemplazo. Para obtener más información, consulte [Estados personalizados en un grupo que se mueve o elimina](../../../administration-and-setup/manage-groups/manage-group-statuses/custom-statuses-in-group-moved-or-deleted.md).
