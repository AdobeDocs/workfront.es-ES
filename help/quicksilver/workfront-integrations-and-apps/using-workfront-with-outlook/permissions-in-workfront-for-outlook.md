---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Niveles de permisos para  [!DNL Workfront]  Outlook
description: El complemento  [!DNL Workfront for Outlook] requiere acceso de lectura y escritura al buzón. La integración de  [!DNL Workfront for Outlook]  requiere los permisos de nivel superior porque tiene la funcionalidad de descargar archivos adjuntos de correo electrónico del servidor de Exchange de Outlook y cargarlos en  [!DNL Workfront], cuando el usuario envía una solicitud desde un correo electrónico que tiene archivos adjuntos.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: 793c8c940c8cb7ac53169edf21ddf28af2554120
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 89%

---

# Niveles de permisos para [!DNL Workfront for Outlook]

>[!IMPORTANT]
>
>[Microsoft ha deshabilitado la compatibilidad con los tokens en línea heredados de Exchange](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), que el complemento de Workfront Outlook utilizaba para la autenticación. Este cambio de Microsoft se implementó por fases y se completó el 1 de octubre de 2025.
>
>**Debido a que Microsoft ha deshabilitado estos tokens, la integración de Workfront para Microsoft Outlook ya no funciona.**

[!DNL Workfront for Outlook] requiere el nivel más alto de permisos permitidos en complementos de [!DNL Outlook].

Para obtener más información sobre los permisos de los complementos de [!DNL Outlook], consulte [Privacidad, permisos y seguridad de los complementos [!DNL Outlook]  en la documentación de ](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security)[!DNL Microsoft].

El complemento [!DNL Workfront for Outlook] requiere acceso de lectura y escritura en el buzón (`ReadWriteMailbox`), que es el ámbito de permisos más alto.
La integración de [!DNL Workfront for Outlook] requiere los permisos de nivel superior porque tiene la funcionalidad de descargar archivos adjuntos de correo electrónico del servidor de Exchange de [!DNL Outlook] y cargarlos en [!DNL Workfront], cuando el usuario envía una solicitud desde un correo electrónico que tiene archivos adjuntos. Para que esta funcionalidad funcione, [!DNL Workfront for Outlook] usa la función `mailbox.getCallbackTokenAsync()` de la API de JavaScript del complemento [!DNL Office] para obtener el token y utilizarlo para descargar archivos adjuntos de correo electrónico del servidor de Exchange. El único permiso que permite usar esa función es `ReadWriteMailbox`. Para obtener más información, consulte [Privacidad, permisos y seguridad para complementos de Outlook](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) en la documentación de Microsoft.

El complemento [!DNL Workfront for Outlook] también requiere el permiso `ReadWriteItem` (incluido en `ReadWriteMailbox`), que se utiliza para leer el cuerpo del correo electrónico y leer o actualizar los metadatos del correo electrónico:

* Leer cuerpo del correo electrónico:

  [!DNL Workfront for Outlook] lee el cuerpo del correo electrónico cuando un usuario envía la solicitud o envía el cuerpo del correo electrónico como una actualización al objeto [!DNL Adobe Workfront].
* Leer/actualizar metadatos de correo electrónico:

  [!DNL Workfront for Outlook] actualiza los encabezados de los correos electrónicos cuando un usuario envía una solicitud desde un correo electrónico. Esto se hace para almacenar información sobre el objeto [!DNL Adobe Workfront] enviado, de modo que la próxima vez que el usuario abra el complemento para el mismo correo electrónico se muestre la información sobre las acciones anteriores con ese correo electrónico.

[!DNL Workfront for Outlook] solo tiene acceso al buzón de un usuario cuando este realiza una acción dentro del complemento. No tiene ninguna funcionalidad en segundo plano. Workfront para Outlook tiene acceso al buzón del usuario solo en el siguiente escenario:

* El usuario intenta enviar una solicitud, crear una tarea o enviar un correo electrónico como una actualización desde [!DNL Workfront for Outlook] (abriendo el complemento y seleccionando una acción)
   * [!DNL Workfront for Outlook] lee el cuerpo del correo electrónico que se rellenará en el formulario dentro del complemento.
   * [!DNL Workfront for Outlook] lee metadatos de correo electrónico para mostrar información en el complemento acerca de las acciones anteriores realizadas en el complemento con el mismo correo electrónico.
* Cuando un usuario envía una solicitud, crea una tarea o envía un correo electrónico como actualización desde [!DNL Workfront for Outlook] (haciendo clic en el botón [!UICONTROL submit] del complemento):
   * [!DNL Workfront for Outlook] lee el cuerpo del correo electrónico para enviarlo a Workfront como una descripción de solicitud o un comentario.
   * [!DNL Workfront for Outlook] actualiza los metadatos del correo electrónico para almacenar información sobre las solicitudes enviadas o el objeto actualizado.
   * [!DNL Workfront for Outlook] descarga archivos adjuntos de correo electrónico del servidor de Exchange para cargarlos en solicitudes enviadas, tareas creadas u objetos actualizados.
