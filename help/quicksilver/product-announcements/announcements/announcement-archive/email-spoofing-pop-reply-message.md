---
content-type: reference
navigation-topic: announcements
title: Eliminación de suplantación de correo electrónico y respuesta POP
description: Estamos realizando dos cambios en la forma en que Adobe Workfront envía y recibe correos electrónicos con la versión 20.3 (prevista para agosto de 2020).
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
TQID: 'https://experienceleague.adobe.com/eOFRSbJicMbYHqq74-O9VW0c73RDQmAC-OIkLX-FKFw'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 85%
---
# Suplantación de correo electrónico y respuesta POP

Estamos realizando dos cambios en la forma en que Adobe Workfront envía y recibe correos electrónicos con la versión 20.3 (prevista para agosto de 2020).

## Correo electrónico saliente de Workfront

En un esfuerzo por aumentar el envío correcto de correos electrónicos, eliminaremos la suplantación de correos electrónicos, lo que a menudo se etiqueta como correo no deseado (consulte Suplantación de correo electrónico). Todo el correo electrónico de Workfront se enviará desde `notifications@my.workfront.com`, incluidas las alertas automatizadas y la comunicación de usuario a usuario. Un ejemplo de correo electrónico de Joan Harris tendrá este aspecto en el área De del correo electrónico:

![Ejemplo de correo electrónico](assets/noreply.png)

*Le recomendamos encarecidamente que se ponga en contacto con su equipo de TI* para asegurarse de que el correo electrónico de `notifications@my.workfront.com` no se bloqueará para el correo electrónico entrante a su sistema. También puede remitirse a [Configurar la lista de permitidos del cortafuegos](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) para obtener detalles sobre las direcciones IP de las que provienen nuestro tráfico y correo electrónico.

## Respuestas por correo electrónico a las notificaciones (respuesta POP)

Algunas notificaciones por correo electrónico permiten a los usuarios responder por correo electrónico y hacer que la respuesta se copie en Workfront como una respuesta a un comentario en el sistema de Workfront. Tradicionalmente, las personas con la función de administrador del sistema de Workfront han podido elegir entre proporcionar su propio servidor de correo electrónico POP para recibir esas respuestas o utilizar el sistema de respuesta integrado de Workfront. La opción de servidor de correo electrónico POP personalizado se elimina con la versión 20.3. Todas las cuentas configuradas para utilizar un servidor personalizado pasarán a utilizar automáticamente el sistema nativo de respuesta de correo electrónico de Workfront. No se requiere ninguna acción por parte de los administradores del sistema u otros usuarios de Workfront.

No se producirán cambios en los correos electrónicos procedentes directamente del sistema de Workfront Proof. Seguirá recibiendo esos correos electrónicos como lo ha hecho en el pasado.

Si tiene otras preguntas o inquietudes, comuníquese con el [Equipo de soporte de Workfront](https://experienceleague.adobe.com/?support-tab=home&lang=es#support).
