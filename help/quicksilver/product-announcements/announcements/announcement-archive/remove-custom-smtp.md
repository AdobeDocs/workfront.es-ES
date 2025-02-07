---
content-type: reference
navigation-topic: announcements
title: Quitar servidor SMTP personalizado como opción de correo electrónico saliente
description: Con la versión 20.3 (prevista para agosto de 2020), Adobe Workfront pasa a un nuevo sistema de correo electrónico que mejorará en gran medida la fiabilidad del envío de correos electrónicos para las actualizaciones y notificaciones de Workfront. Como resultado, los clientes ya no podrán utilizar su propio servidor SMTP de correo electrónico para retransmitir su correo electrónico desde la plataforma de Workfront al destinatario deseado. Todo el correo electrónico se enviará directamente desde el servidor de correo de Workfront.
author: Luke
feature: Product Announcements
exl-id: 73abd185-81c6-43fc-b8b0-cad14d15b348
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 98%

---

# Quitar servidor SMTP personalizado como opción de correo electrónico saliente

Con la versión 20.3 (prevista para agosto de 2020), Adobe Workfront pasa a un nuevo sistema de correo electrónico que mejorará en gran medida la fiabilidad del envío de correos electrónicos para las actualizaciones y notificaciones de Workfront. Como resultado, los clientes ya no podrán utilizar su propio servidor SMTP de correo electrónico para retransmitir su correo electrónico desde la plataforma de Workfront al destinatario deseado. Todo el correo electrónico se enviará directamente desde el servidor de correo de Workfront.

Para acceder a esta función, inicie sesión como administrador del sistema y vaya a Configuración > Correo electrónico > Configuración. A continuación se muestra una captura de pantalla con esta función resaltada:

![Configuración del servidor de correo electrónico](assets/email-server-settings-350x226.png)

La opción resaltada en esta captura de pantalla cambiará automáticamente para utilizar la opción Servidor de correo de Workfront con la versión 20.3.

Si tiene configurado un servidor SMTP de correo electrónico personalizado, **le recomendamos encarecidamente que se ponga en contacto con su equipo de TI** para asegurarse de que los correos electrónicos de notifications@my.workfront.com no son bloqueados al entrar en su sistema. También puede consultar Configurar el cortafuegos para obtener más información sobre las direcciones IP de las que proceden nuestro tráfico y correo electrónico.

Si tiene alguna pregunta o inquietud, contacte con el [Equipo de Soporte de Workfront](https://experienceleague.adobe.com/es?support-tab=home#support).
