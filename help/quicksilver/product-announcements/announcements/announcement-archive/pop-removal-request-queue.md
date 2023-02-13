---
content-type: reference
navigation-topic: announcements
title: Nuevo sistema administrado por Adobe Workfront para reemplazar el correo electrónico POP para colas de solicitud con 21.1
description: Estamos reemplazando la opción de correo electrónico POP para colas de solicitud con un nuevo sistema administrado por Adobe Workfront. Aún podrá enviar solicitudes por correo electrónico, pero tendrá que configurar una nueva dirección de correo electrónico administrada por Workfront en el área Cola de solicitudes .
author: Luke
feature: Product Announcements
exl-id: d7147641-ba36-422b-a9b2-3c2f4ab609d8
source-git-commit: f05b462ff596ccc19215ca684802a9820a98211a
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Nuevo sistema administrado por Adobe Workfront para reemplazar el correo electrónico POP para colas de solicitud con 21.1

Estamos reemplazando la opción de correo electrónico POP para colas de solicitud con un nuevo sistema administrado por Adobe Workfront. Aún podrá enviar solicitudes por correo electrónico, pero tendrá que configurar una nueva dirección de correo electrónico administrada por Workfront en el área Cola de solicitudes .

## ¿Por qué se elimina la opción de correo electrónico POP?

La tecnología POP es una opción de correo electrónico poco fiable y menos segura. Además, vemos muchos problemas de clientes relacionados específicamente con el correo electrónico POP. Si realiza el cambio en un sistema administrado por Workfront, obtendrá una experiencia más fiable.

## ¿Qué acción debo realizar?

Debe configurar una nueva dirección de correo electrónico para cada cola de solicitud que haya configurado con el correo electrónico POP en su entorno de producción y distribuir la nueva dirección de correo electrónico según sea necesario. Para obtener más información, consulte [Permitir que los usuarios envíen un problema por correo electrónico a un proyecto de cola de solicitud](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## ¿Cuál es el plan de transición?

A partir de la versión 21.1 a principios de febrero, tendrá 60 días para la transición de los usuarios al nuevo *@take.workfront.com* dirección de correo electrónico que cree. Durante el periodo de 60 días, el correo electrónico POP utilizado anteriormente seguirá funcionando.

## ¿Cómo puedo probar esto en Vista previa?

Para probar este cambio en la vista previa, debe habilitar los correos electrónicos en el entorno de vista previa. Para ello, siga las instrucciones de la sección Administración de correos electrónicos en vista previa en [Habilitar el envío de correos electrónicos desde el entorno de Preview Sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!IMPORTANT]
>
>Lo que haya establecido aquí no se transferirá a su entorno de producción. Después de publicar la funcionalidad en Producción, tendrá que volver a pasar por este proceso.
