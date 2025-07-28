---
product-area: workfront-integrations
keywords: google,doc,documento,hoja,diapositiva
navigation-topic: workfront-for-g-suite
title: Privacidad y permisos en Workfront para Google Workspace
description: Privacidad y permisos en Workfront para Google Workspace
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 76%

---

# Privacidad y permisos en Workfront para Google Workspace

>[!IMPORTANT]
>
>Para ofrecer integraciones más estables y escalables, estamos adoptando un enfoque de integración moderno y flexible mediante la automatización e integración (Fusion) de Workfront. Como parte de este proceso de transición, la siguiente funcionalidad de Workfront para Google Workspace no estará disponible después del **28 de febrero de 2026**:
>
>* Acceso a la funcionalidad de Google Workspace desde Workfront
>
>* Visualización y administración de tareas de Workfront desde Gmail o el panel de sitio Calendario de Google
>
>Recomendamos utilizar la automatización e integración de Workfront para las necesidades de integración de su organización con Google Workspace.
>
>Para obtener una descripción general de la automatización e integración de Workfront, consulte [Información general de Adobe Workfront Fusion](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obtener información sobre las capacidades específicas de los módulos de integración y automatización de Workfront para Google Workspace, consulte [Módulos de Gmail](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) y [Módulos de Google Calendar](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

Puesto que la privacidad del cliente es importante, Adobe Workfront no almacena ni recopila datos de identificación del cliente que son producto de la autorización de terceros de una aplicación de complemento de Google. El uso de Workfront para Google Workspace y la transferencia de información recibida de las API de Google a cualquier otra aplicación se ajustarán a la [Política de datos de usuario de servicios de API de Google](https://developers.google.com/terms/api-services-user-data-policy), incluidos los requisitos de uso limitado.

Para que el complemento de Workfront para Google Workspace pueda ofrecer su valor máximo, necesitamos los siguientes permisos:

* **Ver tus mensajes de correo electrónico cuando se ejecute el complemento**: el complemento de Workfront para Google Workspace puede ahorrar a los usuarios incontables horas de trabajo duplicado al convertir correos electrónicos a nuevas tareas en Workfront y rellenar automáticamente el título y la descripción de la tarea con el asunto y el cuerpo del correo electrónico. Este complemento también permite publicar los correos electrónicos en Workfront como comentarios nuevos. El complemento debe ver sus mensajes de correo electrónico cuando el complemento se esté ejecutando a fin de proporcionar este valor.
* **Ejecutar como complemento de Gmail / no confidencial**: se necesitan permisos para que el complemento de Workfront para Google Workspace funcione en el entorno de Gmail. El complemento requiere un entorno de Gmail para funcionar, por lo que requiere el permiso `Run as a Gmail add-on / non-sensitive`.
* **Ver los metadatos de los mensajes de correo electrónico cuando se ejecuta el complemento**: para mejorar los flujos de trabajo, el complemento de Workfront para Google Workspace confirma si un correo electrónico es una notificación de Workfront e identifica el tipo de notificación de Workfront (nueva solicitud de trabajo, solicitud de aprobación, nuevo comentario, etc.). El complemento requiere el permiso `View your email message metadata when the add-on is running` para ofrecer este valor.
* **El complemento debe ejecutarse como un complemento de calendario/no confidencial**: el complemento de Workfront para Google Workspace se conecta al calendario para que usted pueda visualizar cómo las tareas afectan a las programaciones. El complemento necesita el permiso `Run as a Calendar add-on / non-sensitive` para hacerlo.
* **Permiso para conectarse a un servicio externo:** en última instancia, el complemento debe conectarse a la API de Workfront, que es el eje central del valor del complemento. La API de Workfront es un servicio externo a Google, por lo que el complemento requiere el permiso `Connect to an external service permission` para funcionar.

Para obtener más información sobre la dedicación de Adobe Workfront a la privacidad del cliente, consulte [Aviso de privacidad de Workfront](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

Para obtener más información, consulte la [Política de datos de usuario de servicios de API de Google](https://developers.google.com/terms/api-services-user-data-policy).
