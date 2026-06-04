---
title: Mejoras de las solicitudes en la versión 22.1
description: Mejoras de las solicitudes en la versión 22.1
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: be6da26d-1d80-4946-8222-cd164b2b633f
TQID: https://experienceleague.adobe.com/AmKIQPLxnJW4nPNdIEUlnMvUlxMbh4jquWpFYz0k6qY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 456
ht-degree: 100%

---

# Mejoras de las solicitudes en la versión 22.1

Esta página describe todas las mejoras de solicitudes realizadas con la versión 22.1 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semana del 17 de enero de 2022.

Para obtener una lista de todos los cambios disponibles con la versión 22.1, consulte [Información general sobre la versión 22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Mejora de la interfaz para los usuarios que no tienen acceso de creación de solicitudes

Para mejorar la experiencia de los usuarios al trabajar con solicitudes, hemos introducido una mejora en la interfaz que indica al usuario que ha iniciado sesión que no tiene acceso de creación de solicitudes. Con esta mejora, el botón Nueva solicitud se atenúa para los usuarios sin acceso de creación de problemas. Al pasar el puntero por encima del botón atenuado, se muestra una ayuda contextual que indica que la persona con la función de administrador de Workfront ha restringido el acceso del usuario actual a la creación de solicitudes.

Antes de esta mejora, el botón Nueva solicitud no se mostraba en el área Solicitudes de estos usuarios. También se ha restringido la copia y el envío de una solicitud como nueva.

Para obtener más información sobre la creación de solicitudes, consulte [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Copiar y enviar solicitudes

Para optimizar el proceso de envío de solicitudes, hemos introducido una nueva funcionalidad que permite copiar una solicitud existente y enviarla como una nueva. Esto resulta útil cuando se envían solicitudes similares con frecuencia. En este caso, puede reutilizar una solicitud existente, realizar algunos cambios y enviarla como una nueva.

Con este cambio, los usuarios que puedan ver las solicitudes enviadas por otros también pueden copiarlas y enviarlas como nuevas. Para evitar que ocurra, actualice la siguiente opción de configuración en el proyecto de cola de solicitudes: las personas de la misma compañía heredarán los mismos permisos en todas las solicitudes.

>[!NOTE]
>
>No puede copiar y volver a enviar los problemas que se hayan enviado a una cola de solicitudes sin un tema de cola antes de que se lanzara esta funcionalidad.

Para obtener más información, consulte [Copiar y enviar solicitudes](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## Experiencia actualizada de panel Resumen en la sección Enviadas del área Solicitudes

>[!NOTE]
>
>Esta función se eliminó temporalmente del entorno de vista previa el 12 de noviembre de 2021. Se volverá a añadir en una fecha posterior.

Para mejorar la visibilidad y la interacción con el panel Resumen, se ha añadido una etiqueta al icono Abrir resumen en la sección Enviadas del área Solicitudes. La etiqueta ahora es dinámica y se actualiza dependiendo de si el panel está abierto o cerrado.

Al abrir el panel Resumen sin seleccionar primero una solicitud, ahora se muestra una imagen más fácil de usar para indicar claramente al usuario que seleccione un elemento antes de abrir el panel. Para obtener más información, consulte [Localizar solicitudes enviadas](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

Con este cambio, también se ha actualizado el panel Resumen de tareas, problemas y documentos. Para obtener información sobre el panel Resumen, consulte [Información general sobre el resumen](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).
