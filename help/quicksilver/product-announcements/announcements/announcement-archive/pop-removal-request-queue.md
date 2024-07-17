---
content-type: reference
navigation-topic: announcements
title: Nuevo sistema administrado por Adobe Workfront que reemplazará el correo electrónico POP en las colas de solicitudes con 21.1
description: Estamos reemplazando la opción de correo electrónico POP para las colas de solicitud con un nuevo sistema administrado por Adobe Workfront. Todavía podrá enviar solicitudes por correo electrónico, pero en su lugar deberá configurar una nueva dirección de correo electrónico administrada por Workfront en el área de la cola de solicitudes.
author: Luke
feature: Product Announcements
exl-id: d7147641-ba36-422b-a9b2-3c2f4ab609d8
source-git-commit: f05b462ff596ccc19215ca684802a9820a98211a
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Nuevo sistema administrado por Adobe Workfront que reemplazará el correo electrónico POP en las colas de solicitudes con 21.1

Estamos reemplazando la opción de correo electrónico POP para las colas de solicitud con un nuevo sistema administrado por Adobe Workfront. Todavía podrá enviar solicitudes por correo electrónico, pero en su lugar deberá configurar una nueva dirección de correo electrónico administrada por Workfront en el área de la cola de solicitudes.

## ¿Por qué elimina la opción de correo electrónico POP?

La tecnología POP es una opción de correo electrónico poco fiable y menos segura. Además, vemos muchos problemas de clientes relacionados específicamente con el correo electrónico POP. Realizar el cambio en un sistema gestionado por Workfront resultará en una experiencia más fiable.

## ¿Qué acción debo realizar?

Debe configurar una nueva dirección de correo electrónico para cada cola de solicitudes que haya configurado con correo electrónico POP en el entorno de producción y distribuir la nueva dirección de correo electrónico según sea necesario. Para obtener más información, consulte [Permitir que los usuarios envíen un problema por correo electrónico a un proyecto de cola de solicitudes](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## ¿Cuál es el plan de transición?

A partir de la versión 21.1 de principios de febrero, tendrá 60 días para hacer la transición de los usuarios a la nueva dirección de correo electrónico *@intake.workfront.com* que cree. Durante el periodo de 60 días, el correo electrónico POP utilizado anteriormente seguirá funcionando.

## ¿Cómo puedo probar esto en la vista previa?

Para probar este cambio en la vista previa, debe habilitar los correos electrónicos en el entorno de vista previa. Para ello, siga las instrucciones de la sección Administración de correos electrónicos en vista previa en [Habilitar la entrega de correos electrónicos desde el entorno de vista previa de espacio aislado](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!IMPORTANT]
>
>Lo que configure aquí no se transferirá al entorno de producción. Tendrá que volver a pasar por este proceso después de que la funcionalidad se publique en Producción.
