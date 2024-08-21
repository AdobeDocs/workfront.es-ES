---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Heredar estados de los grupos
description: Cuando se enumeran los estados disponibles para un grupo, se ve lo siguiente
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3937fd72-fa54-4777-9ec4-1f097df7a2ee
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 0%

---

# Cómo heredan los grupos los estados

Cuando se enumeran los estados disponibles para un grupo, se ve lo siguiente

* Estados personalizados creados para el grupo, como se explica en [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Estados heredados del sistema y de los niveles superiores de la jerarquía de grupo, como se explica en este artículo.

## Herencia de estados

El grupo hereda estados cuando ocurre cualquiera de las siguientes cosas:

* Usted crea el grupo.
* Un administrador bloquea un estado en un grupo de nivel superior.
* Un administrador elimina otro grupo y elige su grupo para ocupar su lugar.

En la tabla siguiente se explica cada una de estas circunstancias.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Cuando crea un grupo</td> 
   <td> <p>Al crear un grupo nuevo, se hereda automáticamente:</p> 
    <ul> 
     <li>Estados desbloqueados en el grupo un nivel por encima, si el nuevo grupo es un subgrupo.</li> 
    </ul> 
    <ul> 
     <li>Estados bloqueados en el nivel del sistema</li> 
    </ul> 
     <b>EJEMPLO:</b></span></span> 
     <p>Supongamos que un grupo llamado Marketing tiene 2 subgrupos llamados Comunicaciones de marketing y marca.</p> 
     <p>Un administrador de grupo del grupo de marketing crea un nuevo estado personalizado denominado Detección.</p> 
     <p>Más adelante, creará un nuevo subgrupo en el grupo Marketing y lo llamará Advertising.</p> 
     <p>El subgrupo hereda el estado de Detección porque lo creó después de que el otro administrador creara el estado de Detección desbloqueado.</p> 
     <p>Debido a que los subgrupos Comunicaciones de marketing y Personalización de marca ya existían debajo del grupo Marketing cuando esto ocurrió, no heredan el estado Desbloqueado.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cuando un administrador bloquea un estado en un nivel superior</td> 
   <td> <p>Cuando un administrador de Workfront bloquea un estado en el sistema, el grupo lo hereda junto con todos los demás grupos del sistema.</p> <p>Del mismo modo, cuando un administrador bloquea un estado para un grupo por encima del suyo, el grupo lo hereda junto con cualquier otro subgrupo por debajo del grupo superior.</p> <p><b>NOTA</b>: posteriormente, si un administrador desbloquea uno de estos estados en el nivel del sistema o en un grupo por encima del grupo, éste retendrá el estado que heredó anteriormente. Ahora es una versión independiente del estado y puede personalizarla solo para su grupo.</p> 
    <p><b>EJEMPLO:</b></p>
    <p>El administrador del grupo de marketing bloquea el estado de detección mencionado anteriormente para asegurarse de que los 3 subgrupos lo tengan.</p> 
    <p>Junto con su grupo de Advertising, los grupos Comunicaciones de marketing y Personalización de marca tienen el estado Descubrimiento ahora. Lo heredaron cuando estaba bloqueado en el grupo Marketing por encima de ellos.</p> 
    <p>A continuación, el administrador del grupo de marketing desbloquea el estado de detección para que los 3 subgrupos tengan su propia versión del estado de detección. Ahora usted y los administradores de los otros 2 grupos pueden personalizar el estado de Detección para satisfacer las necesidades de sus grupos.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cuando un administrador elimina un grupo</td> 
   <td> <p>Cuando un administrador elimina un grupo y elige el suyo para que ocupe su lugar en el sistema, su grupo hereda los estados personalizados del grupo eliminado si aún no existen en su grupo.</p> 
   <p><b>EJEMPLO: </b></p>
     <p>Un grupo llamado Mensajería debe fusionarse con su grupo de Advertising, por lo que un administrador de Workfront elimina el grupo Mensajería y elige a su grupo para tomar su lugar.</p> 
     <p>El grupo Mensajería tenía un estado único denominado En proceso. El grupo de Advertising ahora tiene ese estado disponible para usar.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Heredando configuraciones de estado

Cuando crea un grupo de nivel superior, hereda las siguientes configuraciones del nivel del sistema. Cuando crea un subgrupo, hereda las siguientes configuraciones del siguiente grupo superior.

* Configuraciones de estado predeterminadas

  Para obtener información sobre estos, vea [Usar estados personalizados como estados predeterminados](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

* Configuración de orden de visualización de estado

  Para obtener información sobre estos temas, consulte [Reordenar estados de grupos y de nivel de sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).

Si alguien cambia estas configuraciones después de crear su grupo, sus estados no se ven afectados.
