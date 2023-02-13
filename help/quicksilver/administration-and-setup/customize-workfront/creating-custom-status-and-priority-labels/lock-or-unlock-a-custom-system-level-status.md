---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Estados de nivel de sistema bloqueados y desbloqueados
description: Bloquear estados personalizados es una forma de garantizar que las personas de toda la organización utilicen los mismos procesos en su flujo de trabajo. Cuando un estado está bloqueado, está disponible para todos los usuarios del sistema. Aunque puede editarlo o eliminarlo, los administradores de grupos no pueden hacerlo para sus grupos. Por el contrario, el desbloqueo de estados personalizados permite a los administradores de grupos una mayor flexibilidad para administrar los flujos de trabajo únicos utilizados en sus grupos. Pueden cambiar los atributos de un estado desbloqueado o eliminarlos para sus grupos.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0e58a1d6-5e0c-4445-a5ac-400dfd4c4948
source-git-commit: c70a10a920d32ad00a2e833b331c92a598902d21
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Estados de nivel de sistema bloqueados y desbloqueados

Bloquear estados personalizados es una forma de garantizar que las personas de toda la organización utilicen los mismos procesos en su flujo de trabajo. Cuando un estado está bloqueado, está disponible para todos los usuarios del sistema. Aunque puede editar o eliminar un estado que bloquee, los administradores de grupos no pueden hacerlo para sus grupos; solo pueden cambiar su orden de visualización en la lista Estado.

Por el contrario, el desbloqueo de estados personalizados permite a los administradores de grupos una mayor flexibilidad para administrar los flujos de trabajo únicos utilizados en sus grupos. Cuando un estado está desbloqueado, los administradores de grupos pueden cambiar sus atributos o eliminarlos para sus grupos.

>[!IMPORTANT]
>
>Si bloquea un estado personalizado después de desbloquearlo durante cualquier período de tiempo, la configuración del estado para todo el sistema reemplazará a las realizadas por los administradores del grupo. Mientras el estado está bloqueado, los administradores del grupo no pueden modificar ni eliminar el estado de sus grupos.

Para obtener instrucciones sobre cómo bloquear o desbloquear un estado de sistema, consulte [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Estados desbloqueados en procesos de aprobación

Puede utilizar los estados bloqueado y desbloqueado en un proceso de aprobación del sistema. Si crea un proceso de aprobación del sistema con un estado del sistema desbloqueado, los usuarios de todo el sistema pueden adjuntar el proceso de aprobación a cualquier proyecto, tarea o problema del sistema.

Los mensajes de advertencia aparecen en los siguientes casos para ayudarle a usted y a los usuarios a comprender los resultados de los siguientes escenarios:

* Un administrador desbloquea un estado de nivel de sistema que se utiliza en un proceso de aprobación. Un mensaje advierte de que puede eliminar el estado desbloqueado de sus grupos, lo que impediría que los miembros del grupo usen correctamente ese proceso de aprobación para los objetos asignados a su grupo.

* Un usuario comienza a editar un proceso de aprobación que utiliza un estado desbloqueado. Un mensaje alerta al usuario sobre el estado de desbloqueo para que pueda evaluar si sería buena idea volver a bloquearlo o reemplazarlo.

* Un proceso de aprobación a nivel de sistema con un estado desbloqueado se adjunta en un objeto y el estado se eliminó para el grupo asignado al objeto. Cuando un miembro del grupo va a la sección Approvals del objeto, un mensaje explica que el proceso de aprobación no se puede iniciar para el objeto.

Puede utilizar los estados bloqueado y desbloqueado en un proceso de aprobación de grupo. Si crea un proceso de aprobación de grupo con un estado de grupo desbloqueado, los usuarios pueden adjuntar el proceso de aprobación a cualquier proyecto, tarea o problema asociado al grupo.