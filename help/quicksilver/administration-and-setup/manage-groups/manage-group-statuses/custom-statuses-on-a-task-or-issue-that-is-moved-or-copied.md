---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Estados personalizados en una tarea o problema que se ha movido o copiado
description: Cuando mueve o copia una tarea o un problema a un proyecto diferente, algunos estados de la tarea o el problema pueden actualizarse para coincidir con los estados utilizados por el grupo del proyecto de destino.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4bd9b89d-9c66-4af7-97bf-f9518ad55d7c
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# Estados personalizados de una tarea o un problema que se mueve o copia

Cuando mueve o copia una tarea o un problema a un proyecto diferente, algunos estados de la tarea o el problema pueden actualizarse para coincidir con los estados utilizados por el grupo del proyecto de destino. Esto depende de si existen estados con la misma clave en ese grupo:

* Si un estado de la tarea o del problema tiene la misma clave que un estado utilizado por el grupo del proyecto de destino, el estado de la tarea o del problema seguirá siendo el mismo.

  Si la etiqueta de estos dos estados no coincide, el estado de la tarea o el problema hereda la etiqueta del estado utilizada por el grupo del proyecto de destino.

* Si un estado de la tarea o del problema no tiene la misma clave que el estado equivalente en el grupo del proyecto de destino, el estado de la tarea o del problema cambia al estado predeterminado equivalente en el grupo del proyecto de destino.

Para obtener información acerca de las claves de estado, vea [Crear o editar un estado de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
