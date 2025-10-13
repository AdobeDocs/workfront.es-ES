---
product-area: projects
navigation-topic: manage-issues
title: Actualizar automáticamente los estados de los problemas de Esperando comentarios a En curso
description: Cuando el contacto principal de un problema realiza una actualización del mismo actualizando un campo (incluido un campo personalizado) o añadiendo un comentario, el estado del problema se actualiza automáticamente a En curso.
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: 393f858ba3711b367cf06ad846ea60be0d6d9034
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 80%

---

# Actualizar automáticamente los estados de los problemas de Esperando comentarios a En curso

<!--Audited: 109/2025-->

Cuando el contacto principal de un problema realiza una actualización del mismo actualizando un campo (incluido un campo personalizado) o añadiendo un comentario, el estado del problema se actualiza automáticamente a En curso.

Para que se produzca este cambio de estado automático, es necesario lo siguiente:

* El problema debe agregarse usando una cola de solicitudes.

  Para obtener información sobre cómo crear colas de solicitudes, vea la sección [Crear y administrar colas de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md).

  Para obtener información sobre cómo enviar solicitudes a una cola de solicitudes, consulte [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

* Los detalles de cola de la cola de solicitudes deben tener esta configuración:
   * **Si alguien hace una solicitud, conceder automáticamente** se establece en **Acceso de aportación**
   * **Cambiar estado** está seleccionado

  ![Los detalles de cola dan acceso de aportación y el estado de cambio está seleccionado.](assets/queuedetails-contributeaccess-changestatus.png)

  >[!IMPORTANT]
  >
  >  Al configurar una cola de solicitudes, puede definir el acceso que tienen los contactos principales a los problemas que envían.
  >
  >Cuando anule la selección de la configuración Cambiar estado al configurar la cola de solicitudes, recuerde que los administradores del sistema siempre tienen acceso para cambiar el estado de los problemas, incluso si la opción Cambiar estado no está seleccionada en la configuración de la cola de solicitudes.

  Para obtener más información sobre los detalles de cola, consulte [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* El problema debe estar en el estado Esperando comentarios.
* Debe haber un estado Esperando comentarios (AWF) disponible para los problemas en el sistema.

  Para obtener más información sobre los estados a nivel del sistema, consulte [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
