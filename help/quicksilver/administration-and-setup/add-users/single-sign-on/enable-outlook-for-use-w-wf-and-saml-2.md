---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Habilitar Outlook para usarlo con Workfront y SAML 2.0
description: Si habilita la autenticación SAML 2.0 y desea que los usuarios puedan iniciar sesión en Workfront desde Microsoft Outlook utilizando sus credenciales de SAML 2.0, debe habilitar SAML 2.0 para autenticarse en los complementos de Office.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
source-git-commit: 75fea812b4574191522af4721a013b57aa5d609f
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 68%

---

# Habilitar Outlook para usarlo con Workfront y SAML 2.0

>[!IMPORTANT]
>
>[Microsoft está deshabilitando la compatibilidad con los tokens en línea heredados de Exchange](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), que el complemento Outlook de Workfront usa actualmente para la autenticación. Este cambio de Microsoft ya ha comenzado a afectar a los clientes y seguirá implementándose por fases hasta octubre de 2025.
>
>* **Después de que Microsoft deshabilite completamente estos tokens, la integración de Workfront para Microsoft Outlook dejará de funcionar.**
>
>Como parte de este cambio, Microsoft ha tomado la decisión de cambiar la forma en que se vuelven a habilitar los tokens. Después del **30 de junio de 2025**, los administradores ya no podrán volver a habilitar los tokens, solo el soporte de Microsoft puede conceder excepciones. **El 1 de octubre de 2025, los tokens heredados se desactivarán para todos los inquilinos. No se concederán excepciones.**

Si habilita la autenticación SAML 2.0 y desea que los usuarios puedan iniciar sesión en Workfront desde Microsoft Outlook utilizando sus credenciales de SAML 2.0, debe habilitar SAML 2.0 para autenticarse en los complementos de Office.

>[!NOTE]
>
>Esto no está disponible si la instancia de Workfront de su organización utiliza un portal SSO personalizado.>
><!--
>or is enabled with Adobe IMS>
>-->
>Consulte al administrador de red o de TI si necesita más información.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Habilitar Outlook para usarlo con Workfront y SAML 2.0

{{step-1-to-setup}}

1. Haga clic en **Sistema** > **Preferencias**.

1. En la sección **Seguridad**, asegúrese de que la opción **Permitir autenticación SAML 2.0 en complementos de Office 365** está habilitada.

   Esta opción habilita la incrustación de Workfront en un elemento Iframe únicamente para los complementos de Office 365. Esto no crea una infracción de seguridad de tipo secuestro de clics, ya que no hay contenido en el que se pueda hacer clic.

   Esta opción está habilitada de forma predeterminada.

   >[!NOTE]
   >
   >Si habilita la opción **Permitir incrustación de Workfront en un iframe**, la opción **Permitir autenticación SAML 2.0 en complementos de Office 365** estará atenuada y habilitada.
   >
   >![Permitir opción de incrustación](assets/if-you-enable.png)
   >

1. Haga clic en **Guardar**.

   Los cambios que haya guardado aquí afectan a la experiencia de todos los usuarios de Workfront.
