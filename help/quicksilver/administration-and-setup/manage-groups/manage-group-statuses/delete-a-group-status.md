---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Eliminar un estado de grupo
description: Como administrador de grupos, puede eliminar un estado de un grupo que administre si no está configurado como un estado obligatorio o bloqueado en el sistema o para un grupo superior en la jerarquía.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: bfce0325-fe6e-459f-96ca-9a5c94c61ed3
source-git-commit: 1554c067afcc548c7f7abd03dbc3a49404e3c89c
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 96%

---

# Eliminar un estado de grupo

Como administrador de grupos, puede eliminar un estado de un grupo que administre si no está configurado como un estado obligatorio o bloqueado en el sistema o para un grupo superior en la jerarquía.

Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

>[!NOTE]
>
>No puede eliminar lo siguiente:
>
>* Los estados integrados Planificados, Actuales, Completados. Puede actualizar sus nombres, editar sus colores y bloquearlos o desbloquearlos, pero no puede eliminarlos.
>* Estados que están en un estado pendiente de aprobación para al menos un objeto asociado con el grupo o uno de sus subgrupos.

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

## Eliminar un estado de grupo

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Grupos**.
1. Haga clic en el nombre del grupo de nivel superior.
1. En el panel izquierdo, haga clic en **Estados**.
1. En la lista de estados que se muestra, pase el puntero por encima del estado que quiera eliminar y luego haga clic en **Eliminar** cuando aparezca en el extremo derecho.

   ![Eliminar](assets/hover-click-delete.jpg)

1. En el cuadro que aparece, seleccione un estado para designar un estado de sustitución para los objetos (proyectos, tareas, problemas y procesos de aprobación) que estaban utilizando el estado que está eliminando.

   Solo están disponibles los estados que equivalen al estado que está eliminando. Por ejemplo, si elimina un estado que es igual a Actual, solo verá los estados que son iguales a Actual.

   Además, los estados que se muestran dependen de si el estado que está eliminando está desbloqueado o bloqueado:

   * **Si está desbloqueado**: los estados bloqueados y desbloqueados no ocultos están disponibles.

     Junto con los estados creados para el subgrupo, se incluyen los estados heredados de los grupos de nivel superior y de nivel del sistema.

   * **Si está bloqueado**: una de las siguientes opciones es verdadera:

      * Si hay otros estados bloqueados y no ocultos, solo están disponibles esos estados.
      * Si no hay ningún estado bloqueado no oculto, el estado predeterminado de Workfront estará disponible, aunque esté oculto o desbloqueado.

        Para obtener información sobre los estados predeterminados de Workfront, consulte [Obtener acceso a la lista de estados de proyectos del sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md), [Obtener acceso a la lista de estados de tareas del sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md) y la información acerca de los cuatro estados de problemas requeridos en [Obtener acceso a la lista de estados de problemas del sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md).

1. Haga clic en **Eliminar estado**.

   Si el estado eliminado era el estado predeterminado para ese tipo en el grupo, el estado de sustitución ocupa su lugar.

   Si el estado eliminado se estableció como el estado predeterminado del proyecto en las preferencias del proyecto, la preferencia ahora se establece como el estado de sustitución.

## Cuando se elimina un grupo

Cuando se elimina un grupo y se sustituye por otro, los estados únicos que tenía el grupo eliminado se añaden a los estados del grupo de sustitución. Para obtener más información, consulte [Estados personalizados en un grupo que se ha movido o eliminado](../../../administration-and-setup/manage-groups/manage-group-statuses/custom-statuses-in-group-moved-or-deleted.md).
