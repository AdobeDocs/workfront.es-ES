---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,seguridad,certificado,administrador,exención,configurar,metadatos
navigation-topic: security
title: Renovación del certificado de metadatos de Adobe Workfront SAML 2.0
description: El procedimiento descrito en esta página solo se aplica a organizaciones que aún no se han incorporado al Admin Console. Si su organización se ha incorporado a Adobe Admin Console, debe realizar esta acción a través de Adobe Admin Console.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 3f84f6b8d6cb36fdb23ff332c4078ac1da4a8745
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Renovación del certificado de metadatos de Adobe Workfront SAML 2.0

>[!IMPORTANT]
>
>El procedimiento descrito en esta página solo se aplica a organizaciones que aún no se han incorporado al Admin Console. Si su organización se ha incorporado a Adobe Admin Console, no es necesario realizar ninguna acción.
>
>Para obtener una lista de procedimientos que difieren en función de si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en plataformas (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Los servidores de Adobe Workfront utilizan el protocolo SAML 2.0 para la autenticación y autorización. Una vez actualizado, el nuevo certificado sigue siendo válido durante un año. Cuando ha llegado el momento de renovar el certificado en su proveedor de identidad, Workfront le envía una advertencia avisándole de que este cambio debe producirse. Como administrador de Workfront, puede administrar este cambio en el sistema.

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certiﬁcate before the speciﬁed date. Mismatched certiﬁcates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>Esto no está disponible si la instancia de Workfront de su organización está habilitada con Adobe IMS. Si necesita más información, consulte con su administrador de red o TI.

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

## Configuración de SAML 2.0 en Workfront

Para revisar el mensaje de advertencia y confirmar la actualización de los metadatos de SAML 2.0 en su proveedor de identidad:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Sistema** > **Inicio de sesión único**.

1. En el **Tipo** menú desplegable, seleccione **SAML 2.0**.

1. Haga clic en **Descargar metadatos de SAML 2.0**.

   Esto descarga el certificado Workfront renovado para SAML 2.0, que contiene los metadatos correctos para el servidor.

   >[!CAUTION]
   >
   >Antes de cargar los metadatos de Workfront en su proveedor de inicio de sesión único (SSO) en el paso 5, copie la URL actual de Servicio al consumidor de aserciones (ACS) en un lugar seguro. Esta URL, también conocida como URL de respuesta, se encuentra en la página de configuración de Workfront de su proveedor de SSO.
   >
   >
   >Si la URL de ACS cambia después de cargar los metadatos de Workfront, significa que los metadatos pueden contener una URL de ACS incorrecta. Debe volver a cambiarlo por el que copió para evitar romper la conexión de inicio de sesión único. El certificado actualizado seguirá siendo correcto después de hacerlo.

1. Vaya al servidor del proveedor de identidad y actualice el nuevo certificado que descargó.
1. En Workfront, en la **Página Inicio de sesión único (SSO)**, asegúrese de que esta opción está seleccionada: **El nuevo certificado de Workfront ya se ha cargado en el proveedor de identidad**.

   Cuando se selecciona este campo, los administradores de Workfront pueden iniciar sesión en Workfront con sus credenciales de SSO o sus credenciales de Workfront.

1. Haga clic en **Guardar**.

   El mensaje de advertencia ya no aparece porque ha reconocido la renovación del certificado SAML 2.0 en el servidor de su proveedor de identidad.

1. Haga clic en **Probar conexión** para probar la configuración.

   Debería ver un mensaje que confirma que la conexión se ha realizado correctamente.

Para obtener más información o para obtener ayuda con la configuración manual de los metadatos, póngase en contacto con nuestro equipo de asistencia, tal como se explica en [Contactar con el servicio de atención al cliente](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
