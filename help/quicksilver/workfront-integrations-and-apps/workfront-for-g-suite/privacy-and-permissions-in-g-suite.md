---
product-area: workfront-integrations
keywords: google,doc,documento,hoja,diapositiva
navigation-topic: workfront-for-g-suite
title: Privacidad y permisos en Workfront para Google Workspace
description: Privacidad y permisos en Workfront para Google Workspace
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# Privacidad y permisos en Workfront para Google Workspace

Como la privacidad del cliente es importante, Adobe Workfront no almacena ni recopila datos de identificación del cliente resultantes de la autorización de terceros de una aplicación de complemento de Google. El uso de Workfront para Google Workspace y la transferencia de información recibida de las API de Google a cualquier otra aplicación se ajustarán a la [Política de datos de usuario de los servicios de API de Google](https://developers.google.com/terms/api-services-user-data-policy), incluidos los requisitos de uso limitado.

Para que el complemento Workfront para Google Workspace pueda proporcionar su valor máximo, necesitamos los siguientes permisos:

* **Vea sus mensajes de correo electrónico cuando se ejecuta el complemento**: El complemento Workfront para Google Workspace puede ahorrar a los usuarios incontables horas de trabajo duplicado al convertir correos electrónicos a nuevas tareas en Workfront y rellenar automáticamente el título y la descripción de la tarea con el asunto y el cuerpo del correo electrónico. El complemento también permite publicar los correos electrónicos en Workfront como nuevos comentarios. El complemento debe ver sus mensajes de correo electrónico cuando el complemento se esté ejecutando para proporcionar este valor.
* **Ejecutar como complemento de Gmail / no confidencial**: Se necesitan permisos para que el complemento Workfront for Google Workspace funcione en el entorno de Gmail. El complemento requiere un entorno de Gmail para funcionar, por lo que requiere el permiso `Run as a Gmail add-on / non-sensitive`.
* **Vea los metadatos de los mensajes de correo electrónico cuando se ejecuta el complemento**: Para mejorar los flujos de trabajo, el complemento Workfront for Google Workspace confirma si un correo electrónico es una notificación de Workfront e identifica el tipo de notificación de Workfront (nueva solicitud de trabajo, solicitud de aprobación, nuevo comentario, etc.). El complemento requiere el permiso `View your email message metadata when the add-on is running` para entregar este valor.
* **El complemento debe ejecutarse como un complemento de calendario/no confidencial**: el complemento de Workfront para Google Workspace se conecta al calendario para que pueda visualizar cómo afectan las tareas a las programaciones. El complemento necesita el permiso `Run as a Calendar add-on / non-sensitive` para hacerlo.
* **Conéctese a un permiso de servicio externo:** En última instancia, el complemento debe conectarse a la API de Workfront, que es la columna vertebral del valor del complemento. La API de Workfront es un servicio externo a Google, por lo que el complemento requiere que `Connect to an external service permission` funcione.

Para obtener más información sobre la dedicación de Adobe Workfront a la privacidad del cliente, consulte [Aviso de privacidad de Workfront](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

Para obtener más información, consulte [Directiva de datos de usuario de servicios de API de Google](https://developers.google.com/terms/api-services-user-data-policy).
