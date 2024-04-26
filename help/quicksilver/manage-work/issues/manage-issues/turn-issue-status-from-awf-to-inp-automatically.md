---
product-area: projects
navigation-topic: manage-issues
title: Actualizar automáticamente los estados de los problemas de Esperando comentarios a En curso
description: Cuando el contacto principal de un problema realiza una actualización del mismo actualizando un campo (incluido un campo personalizado) o agregando un comentario, el estado del problema se actualiza automáticamente a En curso.
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: 948cd81908df3174eb985d1c65533077d3ef5d49
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Actualizar automáticamente los estados de los problemas de Esperando comentarios a En curso

Cuando el contacto principal de un problema realiza una actualización del mismo actualizando un campo (incluido un campo personalizado) o agregando un comentario, el estado del problema se actualiza automáticamente a En curso.

Para que se produzca este cambio de estado automático, es necesario lo siguiente:

* El problema debe introducirse a través de una cola de solicitudes.

  Para obtener información sobre la creación de colas de solicitudes, consulte [Crear y administrar colas de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md) sección. Para obtener información sobre la creación de solicitudes, consulte [Creación y envío de solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

* Los detalles de cola de la cola de solicitudes deben tener esta configuración:
   * **Cuando alguien realice una solicitud, conceder automáticamente** se establece en **Acceso de contribución**
   * **Cambiar estado** está seleccionado en Configuración avanzada

  ![Detalles de cola: conceder acceso de contribución y Cambiar estado está seleccionado.](assets/queuedetails-contributeaccess-changestatus.png)

  >[!IMPORTANT]
  >
  >  Al configurar una cola de solicitudes, puede definir el acceso que tienen los contactos principales a los problemas que envían.
  >
  >Cuando anule la selección de la configuración Cambiar estado al configurar la cola de solicitudes, recuerde que los administradores del sistema siempre tienen acceso para cambiar el estado de los problemas, incluso si la opción Cambiar estado no está seleccionada en la configuración de la cola de solicitudes.

  Para obtener más información sobre Detalles de cola, consulte [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* El problema debe estar en estado Esperando comentarios.
* Debe haber un estado de Esperando comentarios (AWF) disponible para los problemas en el sistema.

  Para obtener más información sobre los estados de nivel del sistema, consulte [Creación o edición de un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
