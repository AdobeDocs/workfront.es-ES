---
title: Habilitar  [!DNL Adobe Workfront]  para Outlook
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Para que los usuarios puedan empezar a usar  [!DNL Adobe Workfront]  para Outlook, primero debe habilitarlo para su sistema.
author: Lisa, Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: be523b27-191f-46ca-9a87-d512f9a15a1e
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 64%

---

# Habilitar [!DNL Adobe Workfront for Outlook]

>[!IMPORTANT]
>
>[Microsoft está deshabilitando la compatibilidad con los tokens en línea heredados de Exchange](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), que el complemento Outlook de Workfront usa actualmente para la autenticación. Este cambio de Microsoft ya ha comenzado a afectar a los clientes y seguirá implementándose por fases hasta octubre de 2025.
>
>* **Después de que Microsoft deshabilite completamente estos tokens, la integración de Workfront para Microsoft Outlook dejará de funcionar.**
>
>Como parte de este cambio, Microsoft ha tomado la decisión de cambiar la forma en que se vuelven a habilitar los tokens. Después del **30 de junio de 2025**, los administradores ya no podrán volver a habilitar los tokens, solo el soporte de Microsoft puede conceder excepciones. **El 1 de octubre de 2025, los tokens heredados se desactivarán para todos los inquilinos. No se concederán excepciones.**


Para que los usuarios puedan empezar a usar [!DNL Adobe Workfront for Outlook], primero debe habilitarlo para su sistema.

Para obtener información sobre cómo usar [!DNL Workfront for Outlook] después de haberlo habilitado, consulte [[!DNL Adobe Workfront for Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/workfront-for-outlook.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Para realizar los pasos de este artículo, debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser administrador de [!DNL Workfront]. Para obtener información sobre administradores de [!DNL Workfront], consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

+++

## Habilitar el complemento de [!DNL Workfront] [!DNL Outlook]

1. Inicie sesión en [!DNL Workfront] como administrador.

{{step-1-to-setup}}

1. Expanda **[!UICONTROL Sistema]** y, a continuación, haga clic en **[!UICONTROL Preferencias]**.

1. Asegúrese de que la opción **[!UICONTROL Permitir que las personas utilicen las aplicaciones móviles de Workfront y el [!DNL Outlook]complemento]** de [!DNL Workfront] esté seleccionada.\
   Además de permitir el uso de las aplicaciones móviles de [!DNL Workfront], esta configuración también permite el uso del complemento de [!DNL Workfront] [!DNL Outlook].

   Esta opción está habilitada de forma predeterminada.

1. Haga clic en **[!UICONTROL Guardar]**.

## Instalación del complemento de [!DNL Workfront] [!DNL Outlook]

Para obtener información sobre los requisitos del sistema para usar el complemento de [!DNL Workfront] para [!DNL Outlook], consulte [Requisitos del sistema](../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md#system-requirements-and-prerequisites) en [Configurar Adobe Workfront para  [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

Para obtener información sobre cómo instalar el complemento de [!DNL Workfront] para [!DNL Outlook], consulte [Instalación del complemento](../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md#downloading-and-installing-the-add-in) en [Configuración [!DNL Adobe Workfront for Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).
