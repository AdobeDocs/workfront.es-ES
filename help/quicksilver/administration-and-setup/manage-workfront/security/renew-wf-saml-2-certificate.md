---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,seguridad,certificado,Administrador,Exención,configurar,metadatos
navigation-topic: security
title: Renovación del certificado de metadatos Adobe Workfront SAML 2.0
description: Los servidores de Adobe Workfront utilizan el protocolo SAML 2.0 para la autenticación y la autorización. Una vez actualizado, el nuevo certificado sigue siendo válido durante un año. Cuando sea el momento de renovar el certificado de su proveedor de identidad, recibirá una advertencia en Workfront que le avisará de que este cambio debe producirse. Como administrador de Workfront, puede administrar este cambio en el sistema.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 206ea3ad1398849e26dea7fe77f6d7c027825b6f
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# Renovación del certificado de metadatos Adobe Workfront SAML 2.0

>[!IMPORTANT]
>
>El procedimiento descrito en esta página se aplica sólo a las organizaciones que aún no se han incorporado al Admin Console. Si su organización se ha incorporado a Adobe Admin Console, no es necesario realizar ninguna acción.
>
>Para obtener una lista de procedimientos que difieren según si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en la plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Los servidores de Adobe Workfront utilizan el protocolo SAML 2.0 para la autenticación y la autorización. Una vez actualizado, el nuevo certificado sigue siendo válido durante un año. Cuando sea el momento de renovar el certificado de su proveedor de identidad, recibirá una advertencia en Workfront que le avisará de que este cambio debe producirse. Como administrador de Workfront, puede administrar este cambio en el sistema.

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certificate before the specified date. Mismatched certificates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>Esto no está disponible si la instancia de Workfront de su organización está habilitada con Adobe IMS. Consulte al administrador de red o de TI si necesita más información.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
  <td> <p>Nuevo: estándar </p>
 <p>o</p> 
<p>Actual: plan </p> 
</td> 
 </tr>   
 <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configuración de SAML 2.0 en Workfront

Para revisar el mensaje de advertencia y confirmar la actualización de los metadatos de SAML 2.0 en su proveedor de identidad:

{{step-1-to-setup}}

1. Haga clic en **Sistema** > **Inicio de sesión único**.

1. En el menú desplegable **Tipo**, seleccione **SAML 2.0**.

1. Haga clic en **Descargar metadatos de SAML 2.0**.

   Esto descarga el certificado renovado de Workfront para SAML 2.0, que contiene los metadatos correctos para el servidor.

1. En el proveedor de identidad, copie la URL de servicio de consumidor de afirmación (ACS) actual (también conocida como URL de respuesta) en un lugar seguro.

   >[!CAUTION]
   >
   >Antes de cargar los metadatos de Workfront a su proveedor de inicio de sesión único (SSO) en el paso 6, copie la URL del servicio de atención al cliente (ACS) de aserción actual en un lugar seguro. Esta URL, también conocida como URL de respuesta, se encuentra en la página de configuración de Workfront de su proveedor de SSO.
   >
   >
   >Si la URL de ACS cambia después de cargar los metadatos de Workfront, significa que los metadatos pueden contener una URL de ACS incorrecta. Debe volver a cambiarlo al que ha copiado para evitar que se interrumpa la conexión de inicio de sesión único. El certificado actualizado seguirá siendo correcto después de hacerlo.

1. En el servidor del proveedor de identidad, actualice el nuevo certificado que descargó.
1. (Condicional) Si la URL del servicio de consumidor de afirmación (ACS) o la URL de respuesta han cambiado en su proveedor de identidad, vuelva a cambiarla a la URL que copió en el paso 5.
1. En Workfront, en la **página Inicio de sesión único (SSO)**, asegúrese de que está seleccionada esta opción: **El nuevo certificado de Workfront ya se ha cargado al proveedor de identidad**.

   >[!NOTE]
   >
   >* Esta opción solo está visible si se aplican todas las condiciones siguientes:
   >   * Su organización ya está configurada para SAML 2.0
   >   * El certificado actual está listo para caducar
   >   * El nuevo certificado está disponible
   >* Cuando se selecciona este campo, los administradores de Workfront pueden iniciar sesión en Workfront con sus credenciales de SSO o de Workfront.

1. Haga clic en **Guardar**.

   El mensaje de advertencia ya no se muestra porque ha reconocido la renovación del certificado SAML 2.0 en el servidor de su proveedor de identidad.

1. Haga clic en **Probar conexión** para probar la configuración.

   Debería ver un mensaje que confirme que la conexión se ha realizado correctamente.

Para obtener más información o ayuda con la configuración manual de los metadatos, póngase en contacto con nuestro equipo de asistencia, tal como se explica en [Póngase en contacto con la atención al cliente](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
