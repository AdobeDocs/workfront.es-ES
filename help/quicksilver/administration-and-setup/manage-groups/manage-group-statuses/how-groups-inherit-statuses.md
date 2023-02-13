---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Cómo heredan los estados los grupos
description: Cuando enumera los estados disponibles para un grupo, verá lo siguiente
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3937fd72-fa54-4777-9ec4-1f097df7a2ee
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# Cómo heredan los estados los grupos

Cuando enumera los estados disponibles para un grupo, verá lo siguiente

* Estados personalizados creados para el grupo, tal como se explica en [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Estados heredados del sistema y de una jerarquía superior en la jerarquía de grupos, como se explica en este artículo.

## Heredación de estados

El grupo hereda los estados cuando sucede cualquiera de las siguientes cosas:

* El grupo se crea.
* Un administrador bloquea un estado en un grupo de nivel superior.
* Un administrador elimina otro grupo y elige que lo sustituya.

En la tabla siguiente se explica cada una de estas circunstancias.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Al crear un grupo</td> 
   <td> <p>Cuando crea un nuevo grupo, hereda automáticamente:</p> 
    <ul> 
     <li>Estados desbloqueados en el grupo un nivel hacia arriba, si el nuevo grupo es un subgrupo.</li> 
    </ul> 
    <ul> 
     <li>Estados bloqueados a nivel del sistema .</li> 
    </ul> 
     <b>EJEMPLO:</b></span></span> 
     <p>Supongamos que un grupo llamado Marketing tiene 2 subgrupos llamados Marketing Communications y Branding.</p> 
     <p>Un administrador de grupo del grupo Marketing crea un nuevo estado personalizado llamado Discovery.</p> 
     <p>Posteriormente, se crea un nuevo subgrupo en el grupo Marketing y se lo llama Publicidad.</p> 
     <p>El subgrupo hereda el estado de Discovery porque creó el grupo después de que el otro administrador creara el estado de Discovery desbloqueado.</p> 
     <p>Debido a que los subgrupos Marketing Communications y Branding ya existían debajo del grupo Marketing cuando esto ocurrió, no heredan el estado de Discovery desbloqueado.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cuando un administrador bloquea un estado en un nivel superior</td> 
   <td> <p>Cuando un administrador de Workfront bloquea un estado a nivel de sistema, el grupo lo hereda junto con todos los demás grupos del sistema.</p> <p>Del mismo modo, cuando un administrador bloquea el estado de un grupo por encima del grupo, el grupo lo hereda junto con cualquier otro subgrupo por debajo del grupo superior.</p> <p><b>NOTA</b>: Posteriormente, si un administrador desbloquea uno de estos estados en el sistema o en un grupo por encima del grupo, el grupo conserva el estado que heredó anteriormente. Ahora es una versión independiente del estado y puede personalizarla solo para su grupo.</p> 
    <p><b>EJEMPLO:</b></p>
    <p>El administrador del grupo de marketing bloquea el estado de detección mencionado anteriormente para asegurarse de que lo tienen los 3 subgrupos.</p> 
    <p>Junto con su grupo Publicidad, los grupos Comunicaciones de marketing y Marcas ahora tienen el estado Discovery. La heredaron cuando estaba bloqueada en el grupo Marketing por encima de ellas.</p> 
    <p>A continuación, el administrador del grupo de marketing desbloquea el estado de detección para que los 3 subgrupos tengan su propia versión del estado de detección. Ahora usted y los administradores de los otros 2 grupos pueden personalizar el estado de Discovery para satisfacer las necesidades de sus grupos.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cuando un administrador elimina un grupo</td> 
   <td> <p>Cuando un administrador elimina un grupo y elige que el suyo ocupe su lugar en el sistema, el grupo hereda los estados personalizados del grupo eliminado si no existen en el grupo.</p> 
   <p><b>EJEMPLO: </b></p>
     <p>Un grupo llamado Mensajería debe fusionarse con el grupo Publicidad, por lo que un administrador de Workfront elimina el grupo Mensajería y elige a su grupo para ocupar su lugar.</p> 
     <p>El grupo Mensajería tenía un estado único llamado In Process. El grupo Publicidad ahora tiene ese estado disponible para su uso.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Heredar configuraciones de estado

Cuando crea un grupo de nivel superior, hereda las siguientes configuraciones del nivel del sistema. Cuando crea un subgrupo, hereda las siguientes configuraciones del siguiente grupo superior.

* Configuraciones de estado predeterminadas

   Para obtener más información, consulte [Usar estados personalizados como estados predeterminados](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

* Configuraciones del orden de visualización del estado

   Para obtener más información, consulte [Reordenar los estados del sistema y del grupo](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).

Si alguien cambia estas configuraciones después de crear el grupo, sus estados no se verán afectados.
