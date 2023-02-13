---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Habilitar Outlook para su uso con Workfront y SAML 2.0
description: Si habilita la autenticación SAML 2.0 y desea que los usuarios puedan iniciar sesión en Workfront desde Microsoft Outlook con sus credenciales de SAML 2.0, debe habilitar SAML 2.0 para que se autentique en los complementos de Office.
author: Caroline, Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 1%

---

# Habilitar Outlook para su uso con Workfront y SAML 2.0

Si habilita la autenticación SAML 2.0 y desea que los usuarios puedan iniciar sesión en Workfront desde Microsoft Outlook con sus credenciales de SAML 2.0, debe habilitar SAML 2.0 para que se autentique en los complementos de Office.

>[!NOTE]
>
>Esto no está disponible si la instancia de Workfront de su organización utiliza un portal SSO personalizado.>
><!--
>or is enabled with Adobe IMS>
>-->
>Si necesita más información, consulte con su administrador de red o TI.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Habilitar Outlook para su uso con Workfront y SAML 2.0

1. Haga clic en **Configuración** cerca de la esquina superior derecha de Adobe Workfront en la barra de navegación global.
1. Haga clic en **Sistema** > **Preferencias**.

1. En el **Seguridad** , asegúrese de que **Permitir la autenticación SAML 2.0 en los complementos de Office 365** está activada.

   Esta opción permite incrustar Workfront en un iframe solo para complementos de Office 365. Esto no abre una infracción de secuestro de clics, ya que no hay contenido en el que se pueda hacer clic.

   Esta opción está activada de forma predeterminada.

   >[!NOTE]
   >
   >Si activa la opción **Permitir la incrustación de Workfront en un iframe**, la opción **Permitir la autenticación SAML 2.0 en los complementos de Office 365** está atenuado y habilitado.
   >
   >![](assets/if-you-enable.png)

1. Haga clic en **Guardar**.

   Los cambios que guardó aquí afectan a la experiencia de todos los usuarios de Workfront.
