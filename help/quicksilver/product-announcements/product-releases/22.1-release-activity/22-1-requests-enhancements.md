---
title: 22.1 Mejoras en las solicitudes
description: 22.1 Mejoras en las solicitudes
author: Luke
draft: Probably
feature: Product Announcements
exl-id: be6da26d-1d80-4946-8222-cd164b2b633f
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# 22.1 Mejoras en las solicitudes

En esta página se describen todas las mejoras de Solicitudes realizadas con la versión 2.1 del entorno de vista previa. Estas mejoras estarán disponibles en el entorno Producción

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semana del 17 de enero de 2022.

Para obtener una lista de todos los cambios disponibles con la versión 2.1, consulte [Resumen de la versión 2.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Mejora de la interfaz de los usuarios que no tienen acceso para crear solicitudes

Para mejorar la experiencia de los usuarios al trabajar con solicitudes, hemos introducido una mejora en la interfaz que indica al usuario que ha iniciado sesión que no tiene acceso para crear solicitudes. Con esta mejora, el botón New request está tenue para los usuarios sin acceso para crear problemas. Al pasar el ratón por encima del botón atenuado, aparece una información de objeto que explica que el administrador de Workfront restringió el acceso del usuario actual a la creación de solicitudes.

Antes de esta mejora, el botón New request no se mostraba en el área Requests de estos usuarios. También está restringida la copia y el envío de una solicitud como nueva.

Para obtener más información sobre la creación de solicitudes, consulte [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Copiar y enviar solicitudes

Para optimizar el proceso de envío de solicitudes, presentamos una nueva funcionalidad que le permite copiar una solicitud existente y enviarla como una nueva solicitud. Esto resulta útil cuando envía solicitudes similares con frecuencia. En este caso, puede reutilizar una solicitud existente, realizar algunos cambios y enviarla como una nueva solicitud.

Con este cambio, los usuarios que pueden ver solicitudes enviadas por otros también pueden copiar estas solicitudes y enviarlas como nuevas. Puede evitar que esto ocurra actualizando la siguiente configuración en el proyecto de cola de solicitudes: Las personas de la misma empresa heredarán los mismos permisos para todas las solicitudes.

>[!NOTE]
>
>No se pueden copiar y volver a enviar problemas que se enviaron a una cola de solicitudes sin un tema en cola antes de que se lanzara esta funcionalidad.

Para obtener más información, consulte [Copiar y enviar solicitudes](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## Se ha actualizado la experiencia del panel Resumen en la sección Presentadas del área Solicitudes

>[!NOTE]
>
>Esta función se eliminó temporalmente del entorno de vista previa el 12 de noviembre de 2021. Se añadirá de nuevo más adelante.

Para mejorar la visibilidad y la interacción con el panel Resumen, se ha añadido una etiqueta al icono Abrir resumen en la sección Enviado del área Solicitudes . La etiqueta es ahora dinámica y se actualiza en función de si el panel está abierto o cerrado.

Al abrir el panel Resumen sin seleccionar primero una solicitud, ahora se muestra una imagen más fácil de usar para indicar claramente al usuario que seleccione un elemento antes de abrir el panel. Para obtener más información, consulte [Localizar solicitudes enviadas](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

Con este cambio, también se ha actualizado el panel Resumen de tareas, problemas y documentos. Para obtener información sobre el panel Resumen, consulte [Resumen](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).
