---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Configurar [!DNL Adobe Workfront] para [!DNL Outlook]
description: El complemento  [!DNL Adobe Workfront] [!DNL Outlook] le permite realizar las tareas clave [!DNL Workfront] directamente desde Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: 793c8c940c8cb7ac53169edf21ddf28af2554120
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 86%

---

# Configurar [!DNL Adobe Workfront for Outlook]

<!-- Audited: 12/2023 -->

>[!IMPORTANT]
>
>[Microsoft ha deshabilitado la compatibilidad con los tokens en línea heredados de Exchange](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), que el complemento de Workfront Outlook utilizaba para la autenticación. Este cambio de Microsoft se implementó por fases y se completó el 1 de octubre de 2025.
>
>**Debido a que Microsoft ha deshabilitado estos tokens, la integración de Workfront para Microsoft Outlook ya no funciona.**

El complemento [!DNL Adobe Workfront] [!DNL Outlook] le permite realizar las siguientes tareas clave de [!DNL Workfront] directamente desde Outlook:

* Actualizar un proyecto, tarea o problema existente con información de un correo electrónico. Para obtener más información, consulte [Actualizar un objeto existente de un [!DNL Outlook] correo electrónico](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* Crear una solicitud de [!DNL Workfront] basada en un correo electrónico dentro de [!DNL Outlook]. Para obtener más información, consulte [Crear una solicitud de Adobe Workfront a partir de un [!DNL Outlook] correo electrónico](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* Añadir un correo electrónico como tarea en el área [!UICONTROL Mi trabajo]. Para obtener más información, consulte [Añadir un [!DNL Outlook] correo electrónico como tarea a su lista de trabajos](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* Responder a los comentarios mediante el complemento [!DNL Workfront] para [!DNL Outlook]. Para obtener información acerca de cómo responder a los comentarios de Workfront para [!DNL Outlook], vea [Responder a un comentario de [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* Cree tareas y problemas desde cero o a partir de correos electrónicos existentes (mediante la funcionalidad de arrastrar y soltar). Para obtener más información, consulte [Añadir un correo electrónico [!DNL Outlook] a un proyecto como tarea o problema](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

Debe añadir el complemento [!DNL Workfront] a su cuenta [!DNL Outlook] para poder usar [!DNL Workfront for Outlook].

Si no puede instalar el complemento [!DNL Workfront] con su cuenta de [!DNL Outlook], póngase en contacto con el administrador de [!DNL Workfront] para asegurarse de que los complementos de [!DNL Outlook] estén habilitados para su organización.

Para obtener información sobre cómo habilitar la integración de [!DNL Outlook] para su organización, consulte [Habilitar [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

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
   <p>Plan actual: [!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

El administrador de [!DNL Workfront] debe habilitar [!DNL Outlook for Office] con [!DNL Workfront] para poder usar esta integración.

## Requisitos del sistema

Las aplicaciones disponibles son las siguientes:

* **[!DNL Outlook]en la web:** el complemento [!DNL Workfront] está disponible cuando se usa [!DNL Outlook] desde un explorador web, ya sea en un equipo de escritorio o en un dispositivo móvil. Esta funcionalidad también está disponible al usar la aplicación web [!DNL Outlook].
* **[!DNL Outlook]Aplicación de escritorio:** El complemento [!DNL Workfront] está disponible al usar las versiones de escritorio [!DNL Windows] y [!DNL Mac] de [!DNL Outlook] incluidas en el paquete [!DNL Office].

El complemento [!DNL Workfront] de [!DNL Outlook] se admite en entornos que cumplen los siguientes requisitos:

* [Requisitos del cliente](#client-requirements-client-requirements)
* [Requisitos del servidor de correo](#mail-server-requirements-mail-server-requirements)

### Requisitos del cliente {#client-requirements}

Workfront es compatible con las siguientes versiones de [!DNL Outlook]:

* [!DNL Outlook 2013] o posterior el [!DNL Windows]
* [!DNL Outlook 2016] o posterior el [!DNL Windows]
* [!DNL Outlook] en [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] en [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] en la web

Debe estar conectado a un [!DNL Exchange Server] o [!DNL Office 365] utilizar una conexión directa.

Al configurar el cliente, el usuario debe seleccionar uno de los siguientes tipos de cuenta:

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com] Si el cliente está configurado para conectarse con POP3 o IMAP, el complemento [!DNL Workfront] no se carga.

### Requisitos del servidor de correo {#mail-server-requirements}

Los requisitos del servidor de correo se cumplen de manera predeterminada al conectarse a [!DNL Office 365] o [!DNL Outlook.com]. Sin embargo, si está conectado a una instalación On-Premise de [!DNL Exchange Server], se aplican los siguientes requisitos:

* Workfront admite todos los servidores de [!DNL Exchange On-Premise]
* [!DNL Exchange Web Services] (EWS) debe estar habilitado y expuesto a internet.
* El servidor debe tener un certificado de autenticación válido para que pueda emitir tókenes de identidad válidos. Las nuevas instalaciones de [!DNL Exchange Server] incluyen un certificado de autenticación predeterminado.

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* Para tener acceso al complemento [!DNL Workfront] desde [[!DNL Office] Store](https://store.office.com/), los servidores de acceso de cliente deben poder comunicarse con [https://store.office.com](https://store.office.com/).

Para obtener información más detallada sobre los entornos admitidos, consulte la [[!DNL Microsoft Office 365] página principal](https://products.office.com/es-es/office-365-home).

## Instalación del complemento

Puede obtener el complemento de Workfront para Outlook desde [Microsoft Store](https://appsource.microsoft.com/es-es/product/office/WA104380943?tab=Overview).

### [!DNL Workfront] para [!DNL Outlook 365] {#workfront-for-outlook-365}

1. En [!DNL Outlook 365], haga clic en el icono **[!UICONTROL Examinar complementos]** ![Examinar complementos](assets/outlook-add-in-26x26.png)en la parte superior de la interfaz de Office 365 y, a continuación, haga clic en **[!UICONTROL Administrar complementos]**.

1. En el cuadro **[!UICONTROL Search add-ins]**, busque **[!DNL Workfront]** y pulse [!UICONTROL Enter].

1. Haga clic en **[!UICONTROL Add]**.

### [!DNL Workfront] para [!DNL Outlook] en la web {#workfront-for-outlook-on-the-web}

1. Abra [!DNL Microsoft Outlook] en un explorador web.
1. Haga clic en el icono **[!UICONTROL Examinar] complementos** ![Examinar complementos](assets/outlook-add-in-web-version-20x20.png).

   Para encontrar el icono, consulte [Uso de complementos en [!DNL Outlook] en la web](https://support.microsoft.com/es-es/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) en la documentación de Microsoft.

1. Busque **[!DNL Workfront]** en el campo **[!UICONTROL Search add-ins]** y, a continuación, presione **[!UICONTROL Enter]**.

1. Cuando aparezca en la lista, haga clic en **Añadir**.

### [!DNL Workfront for Outlook] en [!UICONTROL Windows] o [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. Haga clic en **[!UICONTROL Home]** > **[!UICONTROL Store]** en la cinta de opciones.

1. Busque **[!DNL Workfront]** en el campo **[!UICONTROL Search]** y luego presione **[!UICONTROL Enter]**.

1. Haga clic en el conmutador para habilitar el **[!UICONTROL [!DNL Workfront]complemento]**.

## Inicie sesión en [!DNL Workfront] desde [!DNL Outlook].

1. En [!DNL Outlook], seleccione un mensaje de correo electrónico y luego haga clic en el icono **[!DNL Workfront]** en el encabezado del correo electrónico.
1. En la página de inicio de sesión, haga clic en **Iniciar sesión en Workfront**.
1. Siga las indicaciones para iniciar sesión en [!DNL Workfront] mediante OAuth 2.0. <!--Enhanced Authentication or your Security Assertion Markup Language (SAML) URL.-->

   <!--Before users can log in to the [!DNL Workfront] add-in using SAML, a [!DNL Workfront] administrator must first enable [!DNL Office 365] add-ins to authenticate using a SAML 2.0 solution. For more information, see the section [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) in the article [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).-->

   >[!NOTE]
   >
   >* Si se le pide que escriba el dominio de su cuenta de [!DNL Workfront], escríbalo con este formato: *yourCompany&#39;sDomain.my.workfront.com*. El dominio de su empresa suele ser el nombre de su empresa.

<!--ADDITIONAL BULLET REMOVED FROM NOTE BOX: Enhanced Authentication is not available until a Workfront administrator enables it for this integration.-->
