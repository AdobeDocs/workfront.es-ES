---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Niveles de permisos para [!DNL Workfront] para Outlook
description: La variable [!DNL Workfront for Outlook] requiere acceso de buzón de lectura y escritura. La variable [!DNL Workfront for Outlook] la integración requiere los permisos de nivel más alto porque tiene la funcionalidad de descargar archivos adjuntos de correo electrónico del servidor de intercambio de Outlook y cargarlos en [!DNL Workfront], cuando el usuario envía una solicitud desde un correo electrónico que tiene archivos adjuntos.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: 177bf9271dca0310653b73b9100607a82290c326
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# Niveles de permisos para [!DNL Workfront for Outlook]

[!DNL Workfront for Outlook] requiere el mayor de los cuatro niveles de permisos permitidos en [!DNL Outlook] complementos.

Para obtener más información sobre los permisos en [!DNL Outlook] complementos, consulte [Privacidad, permisos y seguridad para [!DNL Outlook] complementos](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) en el [!DNL Microsoft] documentación.

La variable [!DNL Workfront for Outlook] el complemento requiere acceso de buzón de lectura y escritura (`ReadWriteMailbox`), que es el ámbito de permiso más alto.
La variable [!DNL Workfront for Outlook] la integración requiere los permisos de nivel más alto, ya que tiene la funcionalidad de descargar archivos adjuntos de correo electrónico desde el [!DNL Outlook] intercambiar servidor y cargarlos en [!DNL Workfront], cuando el usuario envía una solicitud desde un correo electrónico que tiene archivos adjuntos. Para que esta funcionalidad funcione, [!DNL Workfront for Outlook] utiliza la función `mailbox.getCallbackTokenAsync()` from [!DNL Office] API de JavaScript de complemento para obtener el token y utilizarlo para descargar archivos adjuntos de correo electrónico del servidor de intercambio. El único permiso que permite el uso de esa función es `ReadWriteMailbox`. Para obtener más información, consulte [Privacidad, permisos y seguridad para complementos de Outlook](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) en la documentación de Microsoft.

La variable [!DNL Workfront for Outlook] también requiere `ReadWriteItem` permiso (incluido en `ReadWriteMailbox`), que se utiliza para leer el cuerpo del correo electrónico y leer/actualizar los metadatos del correo electrónico:

* Leer el cuerpo del correo electrónico:

   [!DNL Workfront for Outlook] lee el cuerpo del correo electrónico cuando un usuario envía la solicitud o envía el cuerpo del correo electrónico como una actualización a [!DNL Adobe Workfront] Objeto.
* Leer/actualizar metadatos de correo electrónico:

   [!DNL Workfront for Outlook] actualiza los encabezados de correo electrónico cuando un usuario envía una solicitud desde un correo electrónico. Esto se hace para almacenar información sobre el envío [!DNL Adobe Workfront] , de modo que la próxima vez que el usuario abra el complemento para el mismo correo electrónico se muestre la información sobre las acciones anteriores con ese correo electrónico.

[!DNL Workfront for Outlook] accede al buzón de un usuario solo cuando el usuario realiza una acción dentro del complemento. No tiene ninguna funcionalidad en segundo plano. Workfront para Outlook solo accede al buzón del usuario en el siguiente escenario:

* El usuario intenta enviar una solicitud, crear una tarea o enviar un correo electrónico como actualización desde [!DNL Workfront for Outlook] (Apertura del complemento y selección de una acción)
   * [!DNL Workfront for Outlook] lee el cuerpo del correo electrónico que se va a rellenar en el formulario dentro del complemento.
   * [!DNL Workfront for Outlook] lee los metadatos del correo electrónico para mostrar información sobre el complemento acerca de las acciones anteriores realizadas en el complemento con el mismo correo electrónico.
* Cuando un usuario envía una solicitud, crea una tarea o envía un correo electrónico como actualización desde [!DNL Workfront for Outlook] (haga clic en el botón [!UICONTROL submit] del complemento):
   * [!DNL Workfront for Outlook] lee el cuerpo del correo electrónico para enviarlo a Workfront como una descripción de solicitud o un comentario.
   * [!DNL Workfront for Outlook] actualiza los metadatos del correo electrónico para almacenar información sobre las solicitudes enviadas o el objeto actualizado.
   * [!DNL Workfront for Outlook] descarga archivos adjuntos de correo electrónico desde el servidor de intercambio para cargarlos en solicitudes enviadas, tareas creadas u objetos actualizados.
