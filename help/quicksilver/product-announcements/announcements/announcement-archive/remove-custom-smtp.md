---
content-type: reference
navigation-topic: announcements
title: Eliminar SMTP personalizado como opción de correo electrónico saliente
description: Con la versión 20.3 (prevista para agosto de 2020), Adobe Workfront se está trasladando a un nuevo sistema de correo electrónico que mejorará en gran medida la fiabilidad de su envío de correo electrónico para las actualizaciones y notificaciones de Workfront. Como resultado, los clientes ya no podrán utilizar su propio servidor de correo electrónico SMTP para retransmitir su correo electrónico desde la plataforma de Workfront al destinatario deseado. Todo el correo electrónico se enviará directamente desde el servidor de correo de Workfront.
author: Luke
feature: Product Announcements
exl-id: 73abd185-81c6-43fc-b8b0-cad14d15b348
source-git-commit: 9bc394c718becbac2848c2d91ba3202483699b6f
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# Eliminar SMTP personalizado como opción de correo electrónico saliente

Con la versión 20.3 (prevista para agosto de 2020), Adobe Workfront se está trasladando a un nuevo sistema de correo electrónico que mejorará en gran medida la fiabilidad de su envío de correo electrónico para las actualizaciones y notificaciones de Workfront. Como resultado, los clientes ya no podrán utilizar su propio servidor de correo electrónico SMTP para retransmitir su correo electrónico desde la plataforma de Workfront al destinatario deseado. Todo el correo electrónico se enviará directamente desde el servidor de correo de Workfront.

Para acceder a esta función, inicie sesión como administrador del sistema y vaya a Configuración > Correo electrónico > Configuración. A continuación se muestra una captura de pantalla que destaca la función:

![](assets/email-server-settings-350x226.png)

La configuración resaltada en esta captura de pantalla cambiará automáticamente la opción para usar el servidor de correo de Workfront con la versión 20.3.

Si ha configurado un servidor de correo SMTP personalizado, **le recomendamos encarecidamente que contacte con su equipo de TI** para asegurarse de que el correo electrónico de notifications@my.workfront.com no se bloquee por la entrada de correo electrónico a su sistema. También puede hacer referencia a Configuración del cortafuegos para obtener detalles sobre las direcciones IP de las que provienen nuestro tráfico y nuestro correo electrónico.

Si tiene alguna otra pregunta o duda, póngase en contacto con el [Equipo de asistencia de Workfront](https://one.workfront.com/s/support?language=en_US).
