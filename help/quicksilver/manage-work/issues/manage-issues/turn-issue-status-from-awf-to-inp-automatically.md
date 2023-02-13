---
product-area: projects
navigation-topic: manage-issues
title: Actualizar automáticamente los estados de los problemas de la sección Esperando comentarios a en curso
description: Cuando el Contacto principal de un problema actualiza el problema actualizando un campo (incluido un campo personalizado) o añadiendo un comentario, el estado del problema se actualiza automáticamente a In Progress .
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# Actualizar automáticamente los estados de los problemas de la sección Esperando comentarios a en curso

Cuando el Contacto principal de un problema actualiza el problema actualizando un campo (incluido un campo personalizado) o añadiendo un comentario, el estado del problema se actualiza automáticamente a In Progress .

Para que se produzca este cambio de estado automático, se requiere lo siguiente:

* El problema debe introducirse a través de una cola de solicitudes.

   Para obtener información sobre la creación de colas de solicitud, consulte la [Crear y administrar colas de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md) para obtener más información. Para obtener información sobre la creación de solicitudes, consulte [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

* Los detalles de cola de la cola de solicitud deben tener esta configuración:
   * **Cuando alguien realiza una solicitud, concede automáticamente** está configurado como **Acceso a Contribute**
   * **Cambiar estado** está seleccionado en Configuración avanzada

   ![Los Detalles de Cola dan a Contribute Acceso y Estado de Cambio está seleccionado.](assets/queuedetails-contributeaccess-changestatus.png)

   Para obtener más información sobre los detalles de la cola, consulte [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* El problema debe estar en estado Esperando comentarios .
* Debe haber un estado Comentarios pendientes (AWF) disponible para los problemas a nivel del sistema.

   Para obtener más información sobre los estados de nivel de sistema, consulte [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
