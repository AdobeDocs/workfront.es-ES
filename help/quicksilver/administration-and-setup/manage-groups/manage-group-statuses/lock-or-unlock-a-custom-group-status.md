---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Estados de grupo bloqueados y desbloqueados
description: Bloquear los estados personalizados de un grupo es una forma de garantizar que las personas del grupo y sus subgrupos usen los mismos procesos en su flujo de trabajo. Cuando un estado de grupo está bloqueado, está disponible para todos los usuarios del grupo y de los grupos inferiores. Aunque usted (o un administrador de Workfront) puede editar o eliminar un estado que bloquee, los administradores de los subgrupos siguientes no pueden hacerlo para esos grupos. Por el contrario, el desbloqueo de los estados personalizados de un grupo permite a los administradores de subgrupos inferiores disponer de más flexibilidad para administrar sus flujos de trabajo. Pueden cambiar los atributos de un estado desbloqueado o eliminarlos para sus grupos.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3463e4cb-7336-49b7-b81a-c2acef72f61d
source-git-commit: d67de32fcbe4706cf8a1fc6f5bb8ec9d08b07119
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# Estados de grupo bloqueados y desbloqueados

Bloquear los estados personalizados de un grupo es una forma de garantizar que las personas del grupo y sus subgrupos usen los mismos procesos en su flujo de trabajo. Cuando un estado de grupo está bloqueado, está disponible para todos los usuarios del grupo y de los grupos inferiores. Aunque usted (o un administrador de Workfront) puede editar o eliminar un estado que bloquee, los administradores de los subgrupos siguientes no pueden hacerlo para esos grupos; solo pueden cambiar su orden de visualización en la lista Estado.

Por el contrario, el desbloqueo de los estados personalizados de un grupo permite a los administradores de subgrupos inferiores disponer de más flexibilidad para administrar los flujos de trabajo únicos utilizados en sus grupos. Cuando se desbloquea un estado de grupo, los administradores de subgrupos inferiores pueden cambiar sus atributos o eliminarlos para esos subgrupos.

>[!IMPORTANT]
>
>Si bloquea un estado personalizado después de desbloquearlo durante cualquier período de tiempo, la configuración del estado sustituirá a las realizadas por los administradores de grupos en subgrupos inferiores. Mientras el estado está bloqueado, esos administradores no pueden modificar ni eliminar el estado de sus grupos.

Para obtener instrucciones sobre cómo bloquear o desbloquear un estado de grupo, consulte [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Puede utilizar los estados bloqueado y desbloqueado en un proceso de aprobación de grupo. Si crea un proceso de aprobación de grupo con un estado de grupo desbloqueado, los usuarios pueden adjuntar el proceso de aprobación a cualquier proyecto, tarea o problema asociado al grupo.

