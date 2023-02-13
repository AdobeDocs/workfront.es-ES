---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Estados personalizados en un grupo que se mueve o elimina
description: En este artículo se explica qué sucede con el grupo de estados personalizados al mover o eliminar un grupo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 83885d86-eb00-46cc-93e9-e3364b6125e8
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---

# Estados personalizados en un grupo que se mueve o elimina

En este artículo se explica qué sucede con el grupo de estados personalizados al mover o eliminar un grupo.

## Estados personalizados en un grupo que se mueve

Considere los siguientes escenarios que describen lo que sucede con el grupo de estados personalizados cuando mueve un grupo a una nueva ubicación bajo otro grupo.

Para obtener información sobre cómo mover un grupo, consulte [Mover un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Cuando mueve un grupo debajo de otro grupo </td> 
   <td> <p>Todos los estados del grupo movido permanecen con él. No se agregan a los estados del nuevo grupo principal del grupo.</p> <p>Sin embargo, el grupo movido hereda cualquier estado bloqueado en el grupo o grupos que ahora sean superiores en su jerarquía. Y, a partir de ahora, si un administrador bloquea un estado superior en la jerarquía, el grupo movido hereda ese estado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cuando un estado en ambos grupos tiene la misma clave pero atributos diferentes</td> 
   <td> <p>Supongamos que dos subgrupos diferentes heredan el mismo estado desbloqueado de un grupo principal. Los administradores de grupos de los 2 grupos personalizan el estado de sus grupos de diferentes maneras.</p> <p>Posteriormente, uno de los dos grupos se mueve debajo del otro. Ahora, ambos tienen un estado con la misma clave, pero tienen atributos diferentes en los dos grupos.</p> <p>En este caso, uno de los siguientes es true:</p> 
    <ul> 
     <li>Si el estado del nuevo grupo principal está desbloqueado, el estado del grupo movido conserva sus atributos, sin que ello afecte al movimiento.</li> 
     <li>Si el estado del nuevo grupo principal está bloqueado, los atributos del estado en el grupo principal anulan los del estado en el grupo movido.</li> 
    </ul> <p>Para obtener información sobre las claves de estado, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Crear o editar un estado</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Cuando un grupo movido tiene estados heredados de su grupo principal anterior </td> 
   <td> <p>Todos los estados personalizados heredados del grupo principal anterior vienen con el grupo movido y se convierten en sus propios estados personalizados. Ya no están conectadas con el grupo principal anterior.</p> 
    <ul> 
     <li>Si el grupo principal anterior edita un estado personalizado bloqueado después del movimiento, los cambios no afectan al estado del subgrupo movido.</li> 
     <li>Si el grupo principal anterior bloquea un estado personalizado que se desbloqueó cuando se movió el grupo, el estado del subgrupo movido no se bloquea.</li> 
     <li>El grupo movido ahora puede desbloquear estados que estaban bloqueados cuando los heredó del grupo principal anterior.</li> 
    </ul> 
     <p><b>EJEMPLO:</b><p> 
     <p>Olivia, el administrador del grupo para el grupo Marketing, crea dos estados para el grupo. Nombra a una First Review, con la clave ABC, y la bloquea. Nombra al otro Final Review, con la clave XYZ, y no lo bloquea.</p> 
     <p>También crea un subgrupo en el grupo Marketing llamado Marketing de productos. En el momento en que se crea, hereda automáticamente la primera revisión y la última revisión del grupo de marketing.</p> 
     <p>Posteriormente, Olivia mueve el subgrupo Marketing de productos dentro del grupo Producto. Tanto la primera revisión como la última revisión van con el grupo Marketing de productos a su nueva ubicación en el grupo Producto .</p> 
     <p>Aunque la primera revisión estaba bloqueada antes del movimiento, el administrador del grupo de marketing de productos puede editarla ahora porque ya no es un estado heredado controlado por el grupo principal del que provino.</p> 
     <p>La revisión final está desbloqueada y es editable, como siempre lo estaba.</p> 
     <p>Para el grupo de marketing, Olivia cambia los colores de la primera revisión y la última revisión y cambia su nombre a Primera revisión, editada y última revisión. También bloquea la última revisión editada. Mientras tanto, en el grupo Marketing de productos, los colores y nombres de los estados Primera revisión y Última revisión no cambian.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Estados personalizados en un grupo que se elimina

Al eliminar un grupo o subgrupo, se reasigna la información asociada a él, incluidos sus estados personalizados, a otro grupo o subgrupo. Los estados del grupo eliminado se añaden a los del grupo de destino.

Si el grupo de destino también estaba utilizando uno de los estados del grupo eliminado (el estado de ambos grupos tiene la misma clave) y el grupo de destino personalizó el estado de diferentes maneras, la configuración de la versión del grupo de destino anula la configuración de la versión del grupo movido.

>[!INFO]
>
>**EJEMPLO:**
>
>El administrador del grupo A cambia el nombre de un estado de nivel de sistema desbloqueado para su grupo. El administrador de grupo de un grupo B también cambia el nombre de ese estado para su grupo. Aunque el estado tiene nombres diferentes en los dos grupos, tiene la misma clave.
>
>Posteriormente, se elimina el Grupo A y toda su información se reasigna al Grupo B.
>
>* El nombre de la versión del grupo B del estado anula el nombre de la versión del grupo A.
>* Si alguien del Grupo A aplicó el estado a un objeto antes de que se eliminara ese grupo, el nombre del estado del objeto se actualiza al nombre del estado utilizado por el Grupo B.
>
>Para obtener información sobre la clave de un estado, consulte la tabla de este artículo en [Crear o editar un estado personalizado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md#create) [Crear o editar un estado para un grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md#create).
>
>Para obtener información sobre cómo eliminar un grupo, consulte [Eliminar un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).
