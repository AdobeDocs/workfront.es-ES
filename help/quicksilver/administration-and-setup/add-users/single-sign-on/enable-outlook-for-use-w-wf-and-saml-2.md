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
source-git-commit: af54faae1e78d7ffbe679fd82dfb5a3abd45f5cf
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 72%

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

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

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
