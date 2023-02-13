---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Avisos automáticos frente a notificaciones de recordatorio
description: Este artículo describe las diferencias entre los recordatorios automáticos y las notificaciones de recordatorio, y proporciona escenarios para cada uno. Para obtener más información sobre todo [!DNL Adobe Workfront] notificaciones, consulte Adobe [!DNL Workfront] notificaciones.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 26c6fa2c-5c3a-4f53-bd7e-e49a623ff60d
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# Avisos automáticos frente a notificaciones de recordatorio

Este artículo describe las diferencias entre los recordatorios automáticos y las notificaciones de recordatorio, y proporciona escenarios para cada uno. Para obtener más información sobre todo [!DNL Adobe Workfront] notificaciones, consulte [[!DNL Adobe Workfront] notificaciones](../../workfront-basics/using-notifications/wf-notifications.md).

## Avisos automáticos

Las siguientes características son específicas de los recordatorios automáticos:

* Solo se puede activar y editar mediante un [!DNL Workfront] administrador
* Se activan en todas las tareas y problemas cuando vencen, se retrasan o se acercan a la fecha de finalización planificada
* Solo se puede enviar al usuario asignado, al administrador del usuario asignado o al administrador del administrador inmediato.
* No puede tener una plantilla de correo electrónico adjunta.

Escenario: Si desea que se activen recordatorios en todas las tareas y problemas del sistema, configure la configuración automática del recordatorio. Para obtener más información, consulte [Configurar recordatorios automáticos](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

## Notificaciones de recordatorio

Las siguientes características son específicas de las notificaciones de recordatorio:

* Pueden crearlo un administrador o cualquier usuario con una licencia del plan y acceso administrativo a las notificaciones de recordatorio
* Solo se puede asociar manualmente a un objeto
* Solo se puede notificar con respecto al objeto adjunto
* Se puede enviar a varias partes interesadas del objeto, como propietario, creador, aprobador o usuario asignado
* Puede utilizar el correo electrónico predeterminado o una plantilla de correo electrónico personalizada adjunta

Escenario: Si desea crear recordatorios para proyectos, partes de horas o desea personalizar recordatorios para tareas y problemas, configure las notificaciones de recordatorio. Para obtener más información, consulte [Configuración de notificaciones de recordatorio](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).
