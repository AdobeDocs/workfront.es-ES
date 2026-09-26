---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Estados personalizados en una tarea o problema que se ha movido o copiado
description: Cuando mueve o copia una tarea o un problema a un proyecto diferente, algunos estados de la tarea o el problema pueden actualizarse para coincidir con los estados utilizados por el grupo del proyecto de destino.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4bd9b89d-9c66-4af7-97bf-f9518ad55d7c
TQID: 'https://experienceleague.adobe.com/GzG3KBfUw05edjA0DVRtODyGprG2mKVjOuUV2L5eWto'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: 254442ca-6997-5cfa-963e-f420870aea53
    internal-label: People Teams and Groups
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 94%
---
# Estados personalizados de una tarea o problema que se mueve o copia

Cuando mueve o copia una tarea o un problema a un proyecto diferente, algunos estados de la tarea o el problema pueden actualizarse para coincidir con los estados utilizados por el grupo del proyecto de destino. Esto depende de si existen estados con la misma clave en ese grupo:

* Si un estado de la tarea o del problema tiene la misma clave que un estado utilizado por el grupo del proyecto de destino, el estado de la tarea o del problema seguirá siendo el mismo.

  Si la etiqueta de estos dos estados no coincide, el estado de la tarea o el problema hereda la etiqueta del estado utilizada por el grupo del proyecto de destino.

* Si un estado de la tarea o del problema no tiene la misma clave que el estado equivalente en el grupo del proyecto de destino, el estado de la tarea o del problema cambia al estado predeterminado equivalente en el grupo del proyecto de destino.

Para obtener información acerca de las claves de estado, vea [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
