---
content-type: reference
navigation-topic: announcements
title: Suplantación de correo electrónico y eliminación de la respuesta POP
description: Con la versión 20.3 (prevista para agosto de 2020), estamos realizando dos cambios en la forma en que Adobe Workfront envía y recibe correos electrónicos.
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Falsificación de correo electrónico y respuesta POP

Con la versión 20.3 (prevista para agosto de 2020), estamos realizando dos cambios en la forma en que Adobe Workfront envía y recibe correos electrónicos.

## Correo electrónico de salida de Workfront

En un esfuerzo por aumentar el envío correcto de correos electrónicos, eliminaremos la suplantación de correos electrónicos, que a menudo se etiqueta como correo no deseado (consulte Suplantación de correos electrónicos). Todo el correo electrónico de Workfront se enviará desde notifications@my.workfront.com, incluidas tanto las alertas automatizadas como la comunicación del usuario con el usuario. Un ejemplo de correo electrónico de Joan Harris se verá así en el área de origen de su correo electrónico:

![](assets/noreply.png)

*Le recomendamos encarecidamente que contacte con su equipo de TI* para asegurarse de que el correo electrónico de notifications@my.workfront.com no se bloquee por la entrada de correo electrónico a su sistema. También puede hacer referencia a [Configurar la lista de permitidos del cortafuegos](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) para obtener más información sobre las direcciones IP de las que provienen nuestro tráfico y nuestro correo electrónico.

## Respuestas de correo electrónico entrante a notificaciones (POP Reply)

Algunas notificaciones por correo electrónico permiten a los usuarios responder por correo electrónico y hacer que la respuesta se copie en Workfront como respuesta de comentario en el sistema de Workfront. Tradicionalmente, los administradores de sistemas de Workfront han podido elegir entre suministrar su propio servidor de correo electrónico POP para recibir esas respuestas o utilizar el sistema de respuesta integrado de Workfront. La opción del servidor de correo electrónico POP personalizado se está eliminando con la versión 20.3. Todas las cuentas configuradas para utilizar un servidor personalizado se transitarán automáticamente para utilizar el sistema de respuesta de correo electrónico nativo de Workfront. No se requiere ninguna acción para los administradores del sistema u otros usuarios de Workfront.

No habrá cambios en los correos electrónicos que provengan directamente del sistema de prueba de Workfront. Seguirá recibiendo esos correos electrónicos como lo ha hecho en el pasado.

Si tiene cualquier otra pregunta o duda, póngase en contacto con el [Equipo de asistencia de Workfront](https://one.workfront.com/s/support?language=en_US).
