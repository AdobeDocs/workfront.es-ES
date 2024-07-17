---
title: 22.1 Solicitudes de mejoras
description: 22.1 Solicitudes de mejoras
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: be6da26d-1d80-4946-8222-cd164b2b633f
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# 22.1 Solicitudes de mejoras

Esta página describe todas las mejoras de solicitudes realizadas con la versión 22.1 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción de

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semana del 17 de enero de 2022.

Para obtener una lista de todos los cambios disponibles con la versión 22.1, consulte [Información general sobre la versión 22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Mejora de la interfaz para los usuarios que no tienen acceso para crear solicitudes

Para mejorar la experiencia de los usuarios al trabajar con solicitudes de, hemos introducido una mejora en la interfaz de que indica al usuario que ha iniciado sesión que no tiene acceso para crear solicitudes de. Con esta mejora, el botón Nueva solicitud se atenúa para los usuarios sin acceso para crear problemas. Al pasar el ratón por encima del botón atenuado, se muestra información sobre herramientas que indica que el administrador de Workfront ha restringido el acceso del usuario actual a la creación de solicitudes.

Antes de esta mejora, el botón Nueva solicitud no se mostraba en el área Solicitudes de estos usuarios. Copiar y enviar una solicitud como nueva también está restringido.

Para obtener más información sobre la creación de solicitudes, consulte [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Copiar y enviar solicitudes

Para optimizar el proceso de envío de solicitudes, hemos introducido una nueva funcionalidad que le permite copiar una solicitud existente y enviarla como una nueva solicitud. Esto resulta útil cuando envía solicitudes similares con frecuencia. En este caso, puede reutilizar una solicitud existente, realizar algunos cambios y enviarla como una solicitud nueva.

Con este cambio, los usuarios que puedan ver las solicitudes enviadas por otros también pueden copiarlas y enviarlas como nuevas. Puede evitar que esto ocurra actualizando la siguiente configuración en el proyecto de cola de solicitudes: Las personas de la misma compañía heredarán los mismos permisos para todas las solicitudes.

>[!NOTE]
>
>No puede copiar y volver a enviar problemas enviados a una cola de solicitudes sin un tema de cola antes de que se lanzara esta funcionalidad.

Para obtener más información, consulte [Copiar y enviar solicitudes](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## Se ha actualizado la experiencia del panel Resumen en la sección Enviado del área Solicitudes

>[!NOTE]
>
>Esta función se eliminó temporalmente del entorno de vista previa el 12 de noviembre de 2021. Se volverá a añadir en una fecha posterior.

Para mejorar la visibilidad y la interacción con el panel Resumen, se ha añadido una etiqueta al icono Abrir resumen en la sección Enviado del área de Solicitudes. La etiqueta ahora es dinámica y se actualiza dependiendo de si el panel está abierto o cerrado.

Al abrir el Panel de resumen sin seleccionar primero una solicitud, ahora se muestra una imagen más fácil de usar para indicar claramente al usuario que seleccione un elemento antes de abrir el panel. Para obtener más información, consulte [Localizar solicitudes enviadas](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

Con este cambio, también se ha actualizado el Panel de resumen de tareas, problemas y documentos. Para obtener información sobre el Panel de resumen, consulte [Resumen general](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).
