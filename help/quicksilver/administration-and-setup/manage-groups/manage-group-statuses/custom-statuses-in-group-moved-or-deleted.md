---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Estados personalizados en un grupo que se mueve o elimina
description: Este artículo explica qué sucede con los estados personalizados de grupo cuando se mueve o elimina un grupo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 83885d86-eb00-46cc-93e9-e3364b6125e8
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# Estados personalizados en un grupo que se mueve o elimina

Este artículo explica qué sucede con los estados personalizados de grupo cuando se mueve o elimina un grupo.

## Estados personalizados en un grupo que se mueve

Tenga en cuenta los siguientes escenarios que describen lo que sucede con los estados personalizados de grupo cuando se mueve un grupo a una nueva ubicación debajo de otro grupo.

Para obtener información acerca de cómo mover un grupo, vea [Mover un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Cuando mueve un grupo a otro grupo </td> 
   <td> <p>Todos los estados del grupo movido permanecen con él. No se añaden a los estados del nuevo grupo principal del grupo.</p> <p>Sin embargo, el grupo movido hereda los estados bloqueados del grupo o grupos que ahora se encuentran más arriba en su jerarquía. Y, a partir de ahora, si un administrador bloquea un estado superior en la jerarquía, el grupo movido hereda ese estado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cuando un estado en ambos grupos tiene la misma clave pero atributos diferentes</td> 
   <td> <p>Supongamos que dos subgrupos diferentes heredan el mismo estado desbloqueado de un grupo principal. A continuación, los administradores de grupo de los 2 grupos personalizan el estado de sus grupos de diferentes maneras.</p> <p>Posteriormente, uno de los dos grupos se mueve debajo del otro. Ahora ambos tienen un estado con la misma clave, pero tiene atributos diferentes en los dos grupos.</p> <p>En este caso, se da una de las siguientes condiciones:</p> 
    <ul> 
     <li>Si el estado del nuevo grupo padre es desbloqueado, el estado del grupo movido conserva sus atributos, no afectados por el movimiento.</li> 
     <li>Si el estado del nuevo grupo padre está bloqueado, los atributos del estado del grupo padre sustituirán a los del estado del grupo movido.</li> 
    </ul> <p>Para obtener información acerca de las claves de estado, vea <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Crear o editar un estado</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Cuando un grupo movido tiene estados heredados de su grupo principal anterior </td> 
   <td> <p>Todos los estados personalizados heredados del grupo principal anterior vienen con el grupo movido y se convierten en sus propios estados personalizados. Ya no están conectados con el grupo principal anterior.</p> 
    <ul> 
     <li>Si el grupo principal anterior edita un estado personalizado bloqueado después del movimiento, los cambios no afectan al estado del subgrupo movido.</li> 
     <li>Si el grupo principal anterior bloquea un estado personalizado que estaba desbloqueado cuando el grupo se movió, el estado del subgrupo movido no estará bloqueado.</li> 
     <li>El grupo movido ahora puede desbloquear los estados que estaban bloqueados cuando los heredó del grupo principal anterior.</li> 
    </ul> 
     <p><b>EJEMPLO:</b><p> 
     <p>Olivia, la administradora del grupo de marketing, crea dos estados para el grupo. Nombra un First Review, con la clave ABC, y lo cierra. Nombra la otra revisión final, con la clave XYZ, y no la bloquea.</p> 
     <p>También crea un subgrupo en el grupo Marketing llamado Marketing de productos. En el momento en que se crea, hereda automáticamente First Review y Final Review del grupo de marketing.</p> 
     <p>Más adelante, Olivia mueve el subgrupo Marketing de productos al grupo Producto. Tanto la Primera revisión como la Revisión final van con el grupo Marketing de productos a su nueva ubicación dentro del grupo Productos.</p> 
     <p>Aunque la primera revisión estaba bloqueada antes del traslado, el administrador del grupo de marketing de productos puede editarla ahora porque ya no es un estado heredado controlado por el grupo principal del que procede.</p> 
     <p>La revisión final está desbloqueada y se puede editar como siempre.</p> 
     <p>Para el grupo Marketing, Olivia cambia los colores de Primera revisión y Revisión final y les cambia el nombre de Primera revisión-Editada y Revisión final-Editada. También bloquea Final Review-Edited. Mientras tanto, en el grupo Marketing de productos, los colores y nombres de los estados Primera revisión y Revisión final no cambian.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Estados personalizados en un grupo que se elimina

Al eliminar un grupo o subgrupo, la información asociada a él, incluidos sus estados personalizados, se reasigna a otro grupo o subgrupo. Los estados del grupo eliminado se añaden a los del grupo de destino.

Si uno de los estados del grupo eliminado también estaba siendo utilizado por el grupo de destino (el estado en ambos grupos tiene la misma clave) y el grupo de destino personalizó el estado de diferentes maneras, la configuración de la versión del grupo de destino anula la configuración de la versión del grupo movido.

>[!INFO]
>
>**EJEMPLO:**
>
>El administrador del grupo A cambia el nombre de un estado de nivel de sistema desbloqueado para su grupo. El administrador de un grupo B también cambia el nombre de ese estado para su grupo. Aunque el estado tiene nombres diferentes en los dos grupos, tiene la misma clave.
>
>Posteriormente, el Grupo A se elimina y toda su información se reasigna al Grupo B.
>
>* El nombre de la versión del Grupo B del estado anula el nombre de la versión del Grupo A.
>* Si alguien del Grupo A aplicó el estado a un objeto antes de que se eliminara ese grupo, el nombre del estado del objeto se actualiza al nombre del estado utilizado por el Grupo B.
>
>Para obtener información acerca de la clave de un estado, vea la tabla de este artículo en [Crear o editar un estado personalizado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md#create) [Crear o editar un estado para un grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md#create).
>
>Para obtener información acerca de cómo eliminar un grupo, vea [Eliminar un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).
