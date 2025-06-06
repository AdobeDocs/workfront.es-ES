---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Estados de grupos bloqueados y desbloqueados
description: Bloquear los estados personalizados de un grupo es una forma de asegurarse de que las personas del grupo y sus subgrupos utilicen los mismos procesos en su flujo de trabajo. Cuando el estado de un grupo está bloqueado, está disponible para todos los usuarios del grupo y de los grupos inferiores.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3463e4cb-7336-49b7-b81a-c2acef72f61d
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 91%

---

# Estados de grupo bloqueados y desbloqueados

Bloquear los estados personalizados de un grupo es una forma de asegurarse de que las personas del grupo y sus subgrupos utilicen los mismos procesos en su flujo de trabajo. Cuando el estado de un grupo está bloqueado, está disponible para todos los usuarios del grupo y de grupos inferiores. Aunque usted (o un administrador de Workfront) puede editar o eliminar un estado que bloquee, los administradores de los subgrupos siguientes no pueden hacerlo para esos grupos; pueden cambiar únicamente el orden de visualización en la lista Estado.

Por el contrario, el desbloqueo de los estados personalizados de un grupo permite a los administradores de subgrupos inferiores más flexibilidad para administrar los flujos de trabajo únicos utilizados en sus grupos. Cuando el estado de un grupo se desbloquea, los administradores de subgrupos inferiores pueden cambiar sus atributos o eliminarlos para esos subgrupos.

>[!IMPORTANT]
>
>Si bloquea un estado personalizado después de que se haya desbloqueado durante cualquier período de tiempo, la configuración del estado reemplazará a la realizada por los administradores de grupos de los subgrupos inferiores. Mientras el estado esté bloqueado, esos administradores no podrán modificar ni eliminar el estado de sus grupos.

Para obtener instrucciones sobre cómo bloquear o desbloquear un estado de grupo, consulte [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Puede utilizar los estados bloqueado y desbloqueado en un proceso de aprobación de grupo. Si crea un proceso de aprobación de grupo con un estado de grupo desbloqueado, los usuarios pueden adjuntar el proceso de aprobación a cualquier proyecto, tarea o problema asociado al grupo.

