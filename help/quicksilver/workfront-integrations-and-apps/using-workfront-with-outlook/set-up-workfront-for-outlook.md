---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Configuración de [!DNL Adobe Workfront] para [!DNL Outlook]
description: El [!DNL Adobe Workfront] [!DNL Outlook] El complemento le permite realizar la clave [!DNL Workfront] tareas directamente desde Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: 4cab7bed6cb4c25d96e70ccce2ece7f6d156f435
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---

# Configuración de [!DNL Adobe Workfront for Outlook]

<!-- Audited: 12/2023 -->

El [!DNL Adobe Workfront] [!DNL Outlook] El complemento permite realizar la siguiente clave [!DNL Workfront] tareas directamente desde Outlook:

* Actualizar un proyecto, tarea o problema existente con información de un correo electrónico. Para obtener más información, consulte [Actualizar un objeto existente de un [!DNL Outlook] email](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* Crear un [!DNL Workfront] solicitud basada en un correo electrónico en [!DNL Outlook]. Para obtener más información, consulte [Crear una solicitud Adobe Workfront a partir de un [!DNL Outlook] email](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* Añada un correo electrónico como tarea en su [!UICONTROL Mi trabajo] área. Para obtener más información, consulte [Añadir un [!DNL Outlook] enviar por correo electrónico como una tarea a su lista de trabajos](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* Responder a los comentarios a través de [!DNL Workfront] complemento para [!DNL Outlook]. Para obtener información sobre cómo responder a comentarios de Workfront para [!DNL Outlook], consulte [Responder a un comentario de [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* Cree tareas y problemas desde cero o a partir de correos electrónicos existentes (mediante la funcionalidad de arrastrar y soltar ). Para obtener más información, consulte [Añadir un [!DNL Outlook] enviar por correo electrónico a un proyecto como una tarea o un problema](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

Debe agregar la variable [!DNL Workfront] complemento a su [!DNL Outlook] cuenta antes de poder usar [!DNL Workfront for Outlook].

Si no puede instalar el [!DNL Workfront] complemento con su [!DNL Outlook] cuenta, póngase en contacto con su [!DNL Workfront] administrador para garantizar que [!DNL Outlook] Los complementos de están habilitados para su organización.

Para obtener información acerca de cómo habilitar el [!DNL Outlook] integración para su organización, consulte [Activar [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td> 
   <p>Nuevo plan: [!UICONTROL Standard]</p> 
   <p>Plan actual: [!UICONTROL Trabajo], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Su [!DNL Workfront] el administrador debe habilitar [!DNL Outlook for Office] con [!DNL Workfront] antes de utilizar esta integración.

## Requisitos del sistema

Las aplicaciones disponibles son las siguientes:

* **[!DNL Outlook]en la Web:** El [!DNL Workfront] complemento está disponible al utilizar [!DNL Outlook] desde un explorador web en un dispositivo de escritorio o móvil. Esta funcionalidad también está disponible al utilizar el [!DNL Outlook] Aplicación web.
* **[!DNL Outlook]Aplicación de escritorio:** El [!DNL Workfront] está disponible cuando se utiliza el complemento [!DNL Windows] y [!DNL Mac] versiones de escritorio de [!DNL Outlook] incluido con el [!DNL Office] paquete.

El [!DNL Workfront] complemento para [!DNL Outlook] es compatible con entornos que cumplen los siguientes requisitos:

* [Requisitos del cliente](#client-requirements-client-requirements)
* [Requisitos del servidor de correo](#mail-server-requirements-mail-server-requirements)

### Requisitos del cliente {#client-requirements}

Workfront admite las siguientes versiones de [!DNL Outlook]:

* [!DNL Outlook 2013] o más tarde [!DNL Windows]
*[!DNL  Outlook 2016] o más tarde [!DNL Windows]
* [!DNL Outlook] el [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] el [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] en la web

Debe estar conectado a un [!DNL Exchange Server] o [!DNL Office 365] mediante una conexión directa.

Al configurar el cliente, el usuario debe seleccionar uno de los siguientes tipos de cuenta:

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com]palo de golf **palo de golf**&#x200B;Si el cliente está configurado para conectarse con POP3 o IMAP, la variable [!DNL Workfront] el complemento no se carga.

### Requisitos del servidor de correo {#mail-server-requirements}

Los requisitos del servidor de correo se cumplen de forma predeterminada al conectarse a [!DNL Office 365] o [!DNL Outlook.com]. Sin embargo, si está conectado a una instalación on-premise de [!DNL Exchange Server], se aplican los siguientes requisitos:

* Workfront admite todos los [!DNL Exchange On-Premise] servidores
* [!DNL Exchange Web Services] (EWS) debe estar habilitado y expuesto a Internet.
* El servidor debe tener un certificado de autenticación válido para que pueda emitir tokens de identidad válidos. Nuevas instalaciones de [!DNL Exchange Server] incluya un certificado de autenticación predeterminado.

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* Para acceder a la [!DNL Workfront] complemento de la [[!DNL Office] Almacenar](https://store.office.com/), los servidores de acceso de cliente deben poder comunicarse con  [https://store.office.com](https://store.office.com/).

Para obtener información más detallada sobre los entornos admitidos, consulte la [[!DNL Microsoft Office 365] página principal](https://products.office.com/en-us/office-365-home).

## Instalación del complemento

Puede obtener el complemento de Workfront para Outlook desde el [tienda de Microsoft](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview).

### [!DNL Workfront] para [!DNL Outlook 365] {#workfront-for-outlook-365}

1. Entrada [!DNL Outlook 365], haga clic en **[!UICONTROL Examinar complementos]** icono ![](assets/outlook-add-in-26x26.png)en la parte superior de la interfaz de Office 365, haga clic en **[!UICONTROL Administración de complementos]**.

1. En el **[!UICONTROL Buscar complementos]** cuadro, buscar **[!DNL Workfront]** a continuación pulse [!UICONTROL Entrar].

1. Clic **[!UICONTROL Añadir]**.

### [!DNL Workfront] para [!DNL Outlook] en la web {#workfront-for-outlook-on-the-web}

1. Abrir [!DNL Microsoft Outlook] en un explorador web.
1. Haga clic en **[!UICONTROL Examinar] complementos** icono ![](assets/outlook-add-in-web-version-20x20.png).

   Para localizar el icono, consulte [Uso de complementos en [!DNL Outlook] en la web](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) en la documentación de Microsoft.

1. Buscar por **[!DNL Workfront]** en el **[!UICONTROL Buscar complementos]** y luego pulse **[!UICONTROL Entrar]**.

1. Cuando aparezca en la lista, haga clic en **Añadir**.

### [!DNL Workfront for Outlook] el [!UICONTROL Windows] o [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. Clic **[!UICONTROL Inicio]** > **[!UICONTROL Almacenar]** en la cinta.

1. Buscar por **[!DNL Workfront]** en el **[!UICONTROL Buscar]** y luego pulse **[!UICONTROL Entrar]**.

1. Haga clic en el botón de alternancia para habilitar la variable **[!UICONTROL [!DNL Workfront]complemento]**.

## Iniciar sesión en [!DNL Workfront] de [!DNL Outlook]

1. Entrada [!DNL Outlook], seleccione un mensaje de correo electrónico y haga clic en **[!DNL Workfront]** en el encabezado del correo electrónico.
1. Siga las indicaciones para iniciar sesión en [!DNL Workfront] mediante la autenticación mejorada, OAuth 2.0 o su URL de lenguaje de marcado de aserción de seguridad (SAML).

   Antes de que los usuarios puedan iniciar sesión en [!DNL Workfront] complemento con SAML, a [!DNL Workfront] el administrador debe habilitar primero [!DNL Office 365] complementos para autenticarse con una solución SAML 2.0. Para obtener más información, consulte la sección [Configurar [!DNL Adobe Workfront] con SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) en el artículo [Configurar [!DNL Adobe Workfront] con SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

   >[!NOTE]
   >
   >* Cuando se le pida que introduzca el dominio de su [!DNL Workfront] , escríbalo con este formato: *yourCompany&#39;sDomain.my.workfront.com*. El dominio de su empresa suele ser el nombre de su empresa.
   >* La autenticación mejorada no está disponible hasta que [!DNL Workfront] El administrador lo habilita para esta integración.

