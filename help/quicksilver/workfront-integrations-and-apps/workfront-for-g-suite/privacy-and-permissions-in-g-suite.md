---
product-area: workfront-integrations
keywords: google,doc,documento,hoja,diapositiva
navigation-topic: workfront-for-g-suite
title: Privacidad y permisos en Workfront para G Suite
description: Privacidad y permisos en Workfront para G Suite
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: 90d088846e72f1632274043c8d8ca7807ff05b4a
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# Privacidad y permisos en Workfront para G Suite

Como la privacidad del cliente es importante, Adobe Workfront no almacena ni recopila ningún dato de identificación del cliente que resulte de la autorización de terceros de una aplicación de complemento de Google. Workfront para G Suite cumple con la Política de datos de usuario de los servicios de Google API, incluidos los requisitos de uso limitado.

Se necesitan los siguientes permisos para que el complemento Workfront for G Suite pueda proporcionar su máximo valor:

* **Ver los mensajes de correo electrónico cuando se está ejecutando el complemento**: El complemento Workfront para G Suite puede ahorrar a los usuarios innumerables horas de trabajo duplicado al convertir correos electrónicos a nuevas tareas en Workfront y rellenar automáticamente el título y la descripción de la tarea con el asunto y el cuerpo del correo electrónico. El complemento también permite publicar sus correos electrónicos en Workfront como comentarios nuevos. El complemento debe ver los mensajes de correo electrónico cuando el complemento se esté ejecutando para proporcionar este valor.
* **Ejecutar como un complemento de Gmail/no sensible**: Se necesitan permisos para que el complemento Workfront for G Suite funcione en el entorno de Gmail. El complemento requiere un entorno de Gmail para funcionar, por lo que requiere la variable `Run as a Gmail add-on / non-sensitive` permiso.
* **Ver los metadatos del mensaje de correo electrónico cuando se está ejecutando el complemento**: Para mejorar los flujos de trabajo, el complemento Workfront for G Suite confirma si un correo electrónico es una notificación de Workfront e identifica el tipo de notificación de Workfront (nueva solicitud de trabajo, solicitud de aprobación, nuevo comentario, etc.). El complemento requiere la variable `View your email message metadata when the add-on is running` permiso para entregar este valor.
* **El complemento debe ejecutarse como un complemento de calendario o no ser sensible**: El complemento de Workfront para G Suite se conecta al calendario para que pueda visualizar cómo afectan las tareas a las programaciones. El complemento necesita la variable `Run as a Calendar add-on / non-sensitive` permiso para ello.
* **Conéctese a un permiso de servicio externo:** En última instancia, el complemento debe conectarse a la API de Workfront, que es la columna vertebral del valor del complemento. La API de Workfront es un servicio externo a Google, por lo que el complemento requiere la variable `Connect to an external service permission` para que el complemento funcione.

Para obtener más información sobre la dedicación de Adobe Workfront a la privacidad del cliente, consulte [Aviso de privacidad de Workfront](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

Para obtener más información, consulte [Política de datos de usuario de los servicios de API de Google](https://developers.google.com/terms/api-services-user-data-policy).
