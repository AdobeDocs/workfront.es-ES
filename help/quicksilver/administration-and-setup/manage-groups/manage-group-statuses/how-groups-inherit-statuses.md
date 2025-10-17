---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Heredar estados de los grupos
description: Cuando se enumeran los estados disponibles para un grupo, se ve lo siguiente
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3937fd72-fa54-4777-9ec4-1f097df7a2ee
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 99%

---

# Estados heredados de los grupos

Cuando se enumeran los estados disponibles para un grupo, se ve lo siguiente

* Estados personalizados creados para el grupo, según se explica en [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Estados heredados del sistema y de los niveles superiores de la jerarquía de grupo, tal como se explica en este artículo.

## Estados heredados

Su grupo hereda estados cuando se produce algunas de las situaciones siguientes:

* Usted crea el grupo.
* Un administrador bloquea un estado en un grupo de nivel superior.
* Un administrador elimina otro grupo y elige el suyo para sustituirlo.

En la tabla siguiente se explica cada una de estas circunstancias.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Al crear un grupo</td> 
   <td> <p>Al crear un grupo nuevo, este hereda automáticamente lo siguiente:</p> 
    <ul> 
     <li>Estados desbloqueados de un grupo de un nivel superior, si el nuevo grupo es un subgrupo.</li> 
    </ul> 
    <ul> 
     <li>Estados bloqueados a nivel del sistema.</li> 
    </ul> 
     <b>EJEMPLO:</b></span></span> 
     <p>Supongamos que un grupo denominado Marketing tiene 2 subgrupos, Comunicaciones de marketing y Personalización de marca.</p> 
     <p>El administrador de grupos de marketing crea un nuevo estado personalizado denominado Descubrimiento.</p> 
     <p>Más adelante, crea un nuevo subgrupo en el grupo Marketing y lo llama Publicidad.</p> 
     <p>El subgrupo hereda el estado de Descubrimiento porque lo creó después de que el otro administrador creara el estado de Descubrimiento desbloqueado.</p> 
     <p>Debido a que los subgrupos Comunicaciones de marketing y Personalización de marca ya existían debajo del grupo Marketing cuando esto ocurrió, no heredan el estado Descubrimiento.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cuando un administrador bloquea un estado en un nivel superior</td> 
   <td> <p>Cuando un administrador de Workfront bloquea un estado en el sistema, el grupo lo hereda junto con todos los demás grupos del sistema.</p> <p>Del mismo modo, cuando un administrador bloquea un estado para un grupo por encima del suyo, el grupo lo hereda junto con cualquier otro subgrupo por debajo del grupo superior.</p> <p><b>NOTA</b>: Posteriormente, si un administrador desbloquea uno de estos estados en el nivel del sistema o en un grupo por encima del grupo, este retendrá el estado que heredó anteriormente. Ahora es una versión independiente del estado y puede personalizarla solo para su grupo.</p> 
    <p><b>EJEMPLO:</b></p>
    <p>El administrador de grupos de marketing bloquea el estado de Descubrimiento mencionado anteriormente para asegurarse de que los tres subgrupos lo tengan.</p> 
    <p>Junto con su grupo de Publicidad, los grupos Comunicaciones de marketing y Personalización de marca tienen el estado Descubrimiento ahora. Lo heredaron cuando estaba bloqueado en el grupo Marketing por encima de ellos.</p> 
    <p>A continuación, el administrador del grupo de marketing desbloquea el estado de detección para que los tres subgrupos tengan su propia versión del estado de Descubrimiento. Ahora usted y los administradores de los otros dos grupos pueden personalizar el estado de Detección para satisfacer las necesidades de sus grupos.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cuando un administrador elimina un grupo</td> 
   <td> <p>Cuando un administrador elimina un grupo y elige el suyo para que ocupe su lugar en el sistema, su grupo hereda los estados personalizados del grupo eliminado si aún no existen en su grupo.</p> 
   <p><b>EJEMPLO: </b></p>
     <p>Un grupo llamado Mensajería debe combinarse con su grupo de Publicidad, por lo que un administrador de Workfront elimina el grupo Mensajería y elige a su grupo para tomar su lugar.</p> 
     <p>El grupo Mensajería tenía un estado único denominado En proceso. El grupo de Publicidad ahora tiene ese estado disponible para usarlo.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Herencia de configuraciones de estado

Cuando crea un grupo de nivel superior, hereda las siguientes configuraciones del nivel del sistema. Cuando crea un subgrupo, hereda las siguientes configuraciones del siguiente grupo superior.

* Configuraciones de estado predeterminadas

  Para obtener información sobre estos estados, vea [Usar estados personalizados como estados predeterminados](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

* Configuraciones de orden/visualización de estado

  Para obtener información sobre estos temas, consulte [Reordenar estados de grupo y de nivel del sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).

Si alguien cambia estas configuraciones después de crear su grupo, sus estados no se ven afectados.
