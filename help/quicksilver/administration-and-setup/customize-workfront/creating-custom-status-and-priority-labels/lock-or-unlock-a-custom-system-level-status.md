---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Estados bloqueados y desbloqueados en el nivel del sistema
description: Bloquear los estados personalizados es una forma de asegurarse de que las personas de la organización utilicen los mismos procesos en su flujo de trabajo. Cuando el estado está bloqueado, está disponible para todos los usuarios del sistema. Aunque puede editarlo o eliminarlo, los administradores de grupos no pueden hacerlo para sus grupos. Por el contrario, el desbloqueo de los estados personalizados permite a los administradores de grupos más flexibilidad para administrar los flujos de trabajo únicos utilizados en sus grupos. Pueden cambiar los atributos de un estado desbloqueado o eliminarlo para sus grupos.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0e58a1d6-5e0c-4445-a5ac-400dfd4c4948
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 98%

---

# Estados de nivel del sistema bloqueados y desbloqueados

Bloquear los estados personalizados es una forma de asegurarse de que las personas de la organización utilicen los mismos procesos en su flujo de trabajo. Cuando el estado está bloqueado, está disponible para todos los usuarios del sistema. Aunque puede editar o eliminar un estado que bloquee, los administradores de grupos no pueden hacerlo para sus grupos; pueden cambiar únicamente el orden de visualización en la lista Estado.

Por el contrario, el desbloqueo de los estados personalizados permite a los administradores de grupos más flexibilidad para administrar los flujos de trabajo únicos utilizados en sus grupos. Cuando un estado se desbloquea, los administradores de grupos pueden cambiar sus atributos o eliminarlos para sus grupos.

>[!IMPORTANT]
>
>Si bloquea un estado personalizado después de que se haya desbloqueado durante cualquier período de tiempo, la configuración del estado en todo el sistema reemplazará a la realizada por los administradores de grupos. Mientras el estado esté bloqueado, los administradores de grupos no podrán modificar ni eliminar el estado de sus grupos.

Para obtener instrucciones sobre cómo bloquear o desbloquear un estado de nivel de sistema, consulte [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Estados desbloqueados en procesos de aprobación

Puede utilizar los estados bloqueado y desbloqueado en un proceso de aprobación de sistema. Si crea un proceso de aprobación de sistema con un estado de sistema desbloqueado, los usuarios de todo el sistema pueden adjuntar el proceso de aprobación a cualquier proyecto, tarea o problema del sistema.

Los mensajes de advertencia se muestran en los siguientes casos para ayudarle a usted y a los usuarios a asegurarse de que comprenden los resultados de los mismos:

* Un administrador desbloquea un estado de nivel de sistema que se utiliza en un proceso de aprobación. Un mensaje advierte que podrían eliminar el estado desbloqueado de sus grupos, lo que impediría que los miembros del grupo usaran correctamente ese proceso de aprobación para los objetos asignados a su grupo.
* Un usuario comienza a editar un proceso de aprobación que utiliza un estado desbloqueado. Un mensaje alerta al usuario sobre el estado desbloqueado para que pueda evaluar si sería una buena idea volver a bloquearlo o reemplazarlo.
* Un proceso de aprobación de nivel de sistema con un estado desbloqueado está adjunto a un objeto y se eliminó el estado del grupo asignado al objeto. Cuando un miembro del grupo va a la sección Aprobaciones del objeto, un mensaje explica que no se puede iniciar el proceso de aprobación del objeto.

Puede utilizar los estados bloqueado y desbloqueado en un proceso de aprobación de grupo. Si crea un proceso de aprobación de grupo con un estado de grupo desbloqueado, los usuarios pueden adjuntar el proceso de aprobación a cualquier proyecto, tarea o problema asociado al grupo.
