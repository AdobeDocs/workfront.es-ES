---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Crear una [!DNL Adobe Workfront] solicitud a partir de un correo electrónico de Outlook
description: Puede crear una [!DNL Adobe Workfront] solicitud a partir de un correo electrónico en Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4ecfe632-5f2e-4dc2-8c88-6a8229887f53
source-git-commit: 793c8c940c8cb7ac53169edf21ddf28af2554120
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 88%

---

# Crear una solicitud [!DNL Adobe Workfront] a partir de un correo electrónico de [!UICONTROL Outlook]



>[!IMPORTANT]
>
>[Microsoft ha deshabilitado la compatibilidad con los tokens en línea heredados de Exchange](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), que el complemento de Workfront Outlook utilizaba para la autenticación. Este cambio de Microsoft se implementó por fases y se completó el 1 de octubre de 2025.
>
>**Debido a que Microsoft ha deshabilitado estos tokens, la integración de Workfront para Microsoft Outlook ya no funciona.**

Puede crear una solicitud [!DNL Adobe Workfront] a partir de un correo electrónico en Outlook.

Cuando crea una solicitud [!DNL Workfront] basada en un correo electrónico, el contenido del correo electrónico (incluidos el asunto y el cuerpo) se incluye en la solicitud de forma predeterminada.

>[!NOTE]
>
>No puede crear una solicitud [!DNL Workfront] desde un buzón compartido de [!UICONTROL Outlook].

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Requisitos previos

El administrador de [!DNL Workfront] debe habilitar [!DNL Outlook for Office] con [!DNL Workfront] para poder usar esta integración.

## Crear una solicitud a partir de un correo electrónico de [!DNL Outlook]

Para crear una solicitud [!DNL Workfront] a partir de [!DNL Outlook]:

1. Seleccione el correo electrónico que contiene la información que desea incluir en una solicitud [!DNL Workfront].
1. Haga clic en el icono **[!DNL Workfront]** en la esquina superior derecha del mensaje de correo electrónico para mostrar el complemento de Workfront.\
   Es posible que deba hacer clic en la flecha hacia abajo situada en la parte superior derecha del correo electrónico para acceder al icono [!DNL Workfront].

1. Haga clic en el icono **[!UICONTROL Menú]** ![o365_addin_menu2_icon.png](assets/o365-addin-menu2-icon.png) para mostrar la lista de las opciones de [!DNL Workfront] disponibles.

1. Haga clic en **[!UICONTROL Enviar solicitud]**.
1. En el campo **[!UICONTROL Seleccionar un tipo de solicitud]**, seleccione la cola de solicitudes donde desea enviar la solicitud.

1. Especifique la siguiente información:\
   Los campos disponibles pueden variar en función de cómo se haya configurado la cola de solicitudes. Para obtener una lista y una descripción completas de los campos posibles, consulte el artículo [Crear y enviar [!DNL Adobe Workfront] solicitudes](../../manage-work/requests/create-requests/create-submit-requests.md).

   * **[!UICONTROL Asunto]:** especifique un asunto para la solicitud. De forma predeterminada, se utiliza el asunto del correo electrónico.
   * **[!UICONTROL Descripción]:** especifique una descripción para la solicitud. De forma predeterminada, se utiliza el cuerpo del correo electrónico.
   * **[!UICONTROL Documentos]:** adjunte cualquier documento que desee incluir en la solicitud. Puede adjuntar documentos arrastrando y soltando o haciendo clic en **[!UICONTROL Seleccionar archivo]** y buscando y seleccionando el documento.\

     De forma predeterminada, todos los documentos adjuntos al correo electrónico se incluyen en la solicitud.

1. Haga clic en **[!UICONTROL Enviar solicitud]**.\
   La solicitud se ha enviado a [!DNL Workfront], en la cola de solicitudes especificada.

1. (Opcional) Vuelva a [!DNL Outlook] y seleccione el correo electrónico original.\
   En la parte superior del panel del complemento de [!DNL Workfront], observe la confirmación con un vínculo de que el correo electrónico se añadió a Workfront como una solicitud. El vínculo incluye la fecha en la que se convirtió.\
