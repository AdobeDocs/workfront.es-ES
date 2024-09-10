---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Eliminar un estado de grupo
description: Como administrador de grupo, puede suprimir un estado de un grupo que administre si no está configurado como un estado obligatorio o bloqueado en el sistema o para un grupo superior en la jerarquía.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: bfce0325-fe6e-459f-96ca-9a5c94c61ed3
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---

# Eliminar un estado de grupo

Como administrador de grupo, puede suprimir un estado de un grupo que administre si no está configurado como un estado obligatorio o bloqueado en el sistema o para un grupo superior en la jerarquía.

Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

>[!NOTE]
>
>No puede eliminar lo siguiente:
>
>* Los estados integrados Planificación, Actual y Finalizado. Puede actualizar sus nombres, editar sus colores y bloquearlos o desbloquearlos, pero no se pueden eliminar.
>* Estados que están en un estado de aprobación pendiente para al menos un objeto asociado con el grupo o uno de sus subgrupos.

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

## Eliminar un estado de grupo

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos**.
1. Haga clic en el nombre del grupo de nivel superior.
1. En el panel izquierdo, haga clic en **Estados**.
1. En la lista de estados que se muestra, pase el ratón sobre el estado que quiera eliminar y luego haga clic en **Eliminar** cuando aparezca en el extremo derecho.

   ![](assets/hover-click-delete.jpg)

1. En el cuadro que aparece, seleccione un estado para designar un estado de reemplazo para los objetos (proyectos, tareas, problemas y procesos de aprobación) que estaban utilizando el estado que está eliminando.

   Solo están disponibles los estados que equivalen al estado que está eliminando. Por ejemplo, si elimina un estado que es igual a Actual, solo verá los estados que son iguales a Actual.

   Además, los estados que se muestran dependen de si el estado que está eliminando está desbloqueado o bloqueado:

   * **Si está desbloqueado**: los estados bloqueado y desbloqueado no oculto están disponibles.

     Junto con los estados creados para el subgrupo, se incluyen los estados heredados de los grupos de nivel superior y de nivel del sistema.

   * **Si está bloqueado**: Una de las siguientes opciones es verdadera:

      * Si hay otros estados bloqueados y no ocultos, solo están disponibles esos estados.
      * Si no hay ningún estado bloqueado no oculto, el estado predeterminado de Workfront estará disponible, aunque esté oculto o desbloqueado.

        Para obtener información acerca de los estados de Workfront predeterminados, vea [Obtener acceso a la lista de estados de proyectos del sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md), [Obtener acceso a la lista de estados de tareas del sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md) y la información acerca de los 4 estados de problemas requeridos en [Obtener acceso a la lista de estados de problemas del sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md).

1. Haga clic en **Eliminar estado**.

   Si el estado eliminado era el estado predeterminado para ese tipo en el grupo, el estado de reemplazo ocupa su lugar.

   Si el estado eliminado se estableció como el estado predeterminado del proyecto en las preferencias del proyecto, la preferencia ahora se establece como el estado de reemplazo.

## Cuando se elimina un grupo

Cuando se elimina un grupo y se reemplaza por otro, los estados únicos que tenía el grupo eliminado se agregan a los estados del grupo de reemplazo. Para obtener más información, vea [Estados personalizados en un grupo que se ha movido o eliminado](../../../administration-and-setup/manage-groups/manage-group-statuses/custom-statuses-in-group-moved-or-deleted.md).
