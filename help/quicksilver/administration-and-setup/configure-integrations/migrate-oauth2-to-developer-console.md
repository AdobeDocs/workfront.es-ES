---
title: Migrar de Workfront OAuth2 a Adobe Developer Console
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Se está retirando el servicio de aplicación OAuth2 personalizado heredado de Workfront. Descubra qué está cambiando, quién se ve afectado y cómo migrar sus integraciones personalizadas a Adobe Developer Console.
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
source-git-commit: db7e6a6fa0c5fc5332213c388d9b4db3a5c59f53
workflow-type: tm+mt
source-wordcount: '1473'
ht-degree: 1%

---

# Migrar de Workfront OAuth2 a Adobe Developer Console

Se está retirando el servicio de aplicaciones OAuth2 personalizado heredado de Workfront (las integraciones que configuró en **Configuración** > **Sistema** > **OAuth2**). En adelante, todas las integraciones personalizadas que se autentifiquen con Workfront deben utilizar el flujo de autenticación de Adobe Developer Console (developer.adobe.com).

Este cambio afecta a cualquier integración personalizada, script o herramienta de terceros que se autentique actualmente con un ID de cliente OAuth2 y un secreto emitidos por Workfront. No afecta a cómo inicia sesión en Workfront y no afecta a las integraciones estándar administradas por Adobe, como las integraciones empaquetadas de Microsoft Teams o Slack, que Adobe migra por separado.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Configuraciones del nivel de acceso de Adobe Workfront</td> 
   <td><p>Administrador del sistema</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Derechos de Adobe Developer Console</td> 
   <td><p>Se requieren derechos completos de administrador de organización de IMS para acceder a Adobe Developer Console for Workfront. Esto es más amplio que una función de administrador de productos de Workfront, ya que administra toda la organización de Adobe y todos los productos incluidos en ella.</p></td> 
  </tr> 
 </tbody> 
</table>

+++

## Fechas clave

| Fecha | Hito | Lo que significa para usted |
|---|---|---|
| 1 de noviembre de 2026 | Nueva creación de aplicación deshabilitada | Ya no puede crear nuevas aplicaciones OAuth2 personalizadas en Workfront. Las aplicaciones existentes siguen funcionando. |
| 1 de febrero de 2027 | Servicio heredado retirado | Las aplicaciones OAuth2 personalizadas existentes dejan de funcionar por completo. Las integraciones que no se hayan migrado a Adobe Developer Console perderán acceso a la API de Workfront en este momento. |

>[!IMPORTANT]
>
>Le recomendamos encarecidamente que planifique y complete su migración antes del 1 de noviembre de 2026, para que las integraciones sigan ejecutándose sin interrupciones y no vaya a realizar la migración con respecto al plazo del 1 de febrero de 2027.

## Organizaciones afectadas

Su organización se ve afectada por este cambio si tiene alguna integración, script o herramienta que se conecte a Workfront mediante un ID de cliente OAuth2 personalizado y un secreto emitido a través de la pantalla de configuración heredada OAuth2 de Workfront. Algunos ejemplos comunes son:

* Integraciones personalizadas que mantiene su equipo de ingeniería con la API de Workfront.
* Conectores creados por terceros o socios configurados con un ID de cliente emitido por Workfront. Le recomendamos que consulte con su proveedor si no está seguro de cómo se autentica su integración.
* Automatización interna, creación de informes o scripts de sincronización de datos que llaman directamente a la API de Workfront.

Si no sabe si su organización tiene alguno de estos elementos, el administrador de Workfront puede comprobar la lista de aplicaciones de OAuth2 en **Configuración** > **Sistema** > **OAuth2** para ver qué hay registrado actualmente. Para obtener más información, consulte [Ver y administrar aplicaciones OAuth2 personalizadas](/help/quicksilver/administration-and-setup/configure-integrations/manage-custom-oauth2-apps.md).

## Comprender los tipos de autenticación de Adobe Developer Console

Adobe Developer Console admite más de una forma de autenticarse. Puede seleccionar el tipo que coincida con el funcionamiento de la integración:

* **Autenticación de servidor a servidor**: Para una aplicación que se ejecuta en su servidor y que llama a las API de Adobe en nombre de su organización, sin que intervenga ningún usuario final. Esta es la coincidencia más cercana al patrón OAuth2 de Workfront heredado que funcionó con los ID de cliente y los secretos, y es el tipo que la mayoría de las integraciones, scripts y automatizaciones de Workfront personalizadas deben utilizar.
* **Autenticación de usuario**: En los casos en que un usuario de Adobe necesite iniciar sesión y dar su consentimiento para que su aplicación pueda ver o editar sus datos. Si la integración necesita actuar en nombre de un usuario de Workfront específico que ha iniciado sesión en lugar de en el de su organización en su conjunto, utilice este tipo en su lugar.

  Si elige Autenticación de usuario, existen tres opciones adicionales según la arquitectura de la aplicación:

  * **Aplicación web OAuth**: para aplicaciones con una interfaz de usuario de front-end y un servidor back-end. El servidor almacena de forma segura el secreto del cliente y obtiene tokens.
  * **Aplicación de una sola página de OAuth**: para aplicaciones web solo de explorador sin servidor back-end. La propia aplicación web recupera tokens.
  * **Aplicación nativa de OAuth**: para aplicaciones móviles o de escritorio que se ejecutan de forma nativa en un dispositivo y no tienen servidor back-end. La aplicación nativa obtiene tokens.

La mayoría de las organizaciones que migran una integración back-end, script o automatización del servicio heredado de OAuth2 desean la autenticación de servidor a servidor.

## Comparación de funciones: OAuth2 heredado frente a Adobe Developer Console

El servicio OAuth2 heredado de Workfront (que se encuentra en **Configuración** > **Sistema** > **Aplicaciones OAuth2**) ofrece tres tipos de aplicaciones, con un límite de 10 aplicaciones OAuth2 por instancia de Workfront. Así se comparan estos aspectos con Adobe Developer Console:

| Tipo de Workfront heredado | Método de flujo/autenticación | Developer Console equivalente | Ajuste |
|---|---|---|---|
| Aplicación de equipo a equipo (CLI, daemons, scripts back-end) | JWT con par de claves pública y privada | Autenticación de servidor a servidor | El mismo propósito de no involucrar al usuario final, pero el mecanismo cambia. El flujo heredado utiliza un par de claves pública y privada y JWT, mientras que de servidor a servidor utiliza un ID de cliente y un secreto de cliente con una concesión de credenciales de cliente de OAuth. Este no es un intercambio de credenciales desplegable. El código de autenticación de la integración debe cambiar, no solo los valores de credencial. Para obtener más información, consulte [Uso del flujo JWT para aplicaciones OAuth 2 personalizadas](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md). |
| Aplicación web (aplicaciones del lado del servidor: Go, Java, .NET, Node, PHP) | Flujo del código de autorización de OAuth 2.0 | Aplicación web de OAuth (en Autenticación de usuario) | La coincidencia 1:1 más cercana. Tiene el mismo flujo y la misma forma básica en la que un servidor back-end almacena el secreto de cliente. Para obtener más información, consulte [Flujo de código de autorización para aplicaciones OAuth 2 personalizadas](/help/quicksilver/wf-api/api/oauth-app-code-token-flow.md). |
| Aplicación web de una sola página (JS, Angular, React, Vue) | Flujo de código de autorización con PKCE, sin secreto de cliente | Aplicación de una sola página de OAuth (en Autenticación de usuario) | La coincidencia 1:1 más cercanaTiene el mismo flujo sin secreto basado en PKCE. Para obtener más información, consulte [Uso del flujo PKCE para aplicaciones de OAuth 2](/help/quicksilver/wf-api/api/oauth-app-pkce-flow.md). |
| (no hay equivalente heredado) | — | Aplicación nativa de OAuth (bajo autenticación de usuario) | Esta es una nueva capacidad. El Workfront OAuth2 heredado no tiene un tipo específico para aplicaciones nativas de escritorio o móviles. |

<!--

>[!NOTE]
>
>A few legacy capabilities don't have a confirmed equivalent yet in Adobe Developer Console, and are being validated with the Developer Console team:
>
>* Per-app controls the legacy UI offers: refresh token rotation toggle, absolute vs. inactivity refresh token expiration, custom logo, privacy policy URL, and developer contact fields.
>* Whether Developer Console enforces a cap on credentials or projects similar to the legacy 10-app-per-instance limit.
>* Whether a JWT/key pair-based option remains available anywhere in Developer Console for Machine to Machine customers, or whether all such integrations must move to the client-secret-based Server-to-Server grant.

-->

## Procedimiento de migración

### Si es administrador del sistema de Workfront

>[!NOTE]
>
>Si es administrador de productos de Workfront pero no de la organización, debe trabajar con el administrador de la organización para completar esta migración o solicitar que se le realice una.

1. Inicie sesión en [developer.adobe.com](https://developer.adobe.com) y cree un nuevo proyecto. Los proyectos son el modo en que la consola organiza las distintas integraciones o aplicaciones cliente.
1. En el proyecto, agregue una API y seleccione **Adobe Workfront**. Esta API se encuentra en la categoría Experience Cloud. Todas las API de Workfront, incluidas Planificación, Flujo de trabajo, y Revisión y aprobaciones, comparten esta sola API.
1. Seleccione la opción de autenticación **Servidor a servidor** y elija la instancia correcta si su organización de IMS tiene más de una instancia de Workfront.

   Para obtener instrucciones sobre cómo elegir un tipo de autenticación, consulte [Comprender los tipos de autenticación de Adobe Developer Console](#understand-adobe-developer-console-authentication-types) en este artículo.
1. En la página Proyecto, abra los detalles de la nueva credencial de servidor a servidor de OAuth para encontrar el ID de cliente, el secreto de cliente y la información necesaria para generar tokens de acceso.
1. Actualice la integración, el script o la herramienta para autenticarse con estas nuevas credenciales en lugar del ID de cliente OAuth2 de Workfront y el secreto.
1. Confirme el acceso en Workfront. Al crear el cliente de API, se agrega automáticamente como usuario de Workfront &quot;`techacct`&quot;. De forma predeterminada, se agrega como colaborador con acceso limitado, pero puede ajustar su nivel de acceso como lo haría para cualquier otro usuario.
1. (Opcional) Para conceder los derechos de administrador de usuarios de `techacct`, agregue el correo electrónico de la cuenta técnica como administrador del perfil de producto correspondiente en Admin Console.
1. Pruebe la integración de extremo a extremo.
1. Retire la entrada antigua de la aplicación OAuth2 en Workfront después de confirmar que la nueva conexión funciona.

Para obtener detalles paso a paso y capturas de pantalla completos, consulte [Obtener acceso](https://developer.adobe.com/workfront-apis/guides/gaining_access/) en la documentación de Developer Console de Adobe.

### Si no es administrador del sistema

Debe realizar un bucle en el administrador de organización de IMS de su organización para completar la migración, ya que la configuración de la nueva credencial en Adobe Developer Console requiere ese nivel de acceso. Si administra o mantiene una integración, pero sabe quién es el administrador de organización de IMS de su organización, póngase en contacto con uno de los siguientes enlaces:

* El equipo de su cuenta de Workfront
* Su equipo informático interno
* Su contacto de ingeniería

## Si no realiza la migración

Las integraciones que siguen utilizando el patrón secreto/ID del cliente de OAuth2 heredado después del 1 de febrero de 2027 dejan de poder autenticarse con la API de Workfront y falla cualquier flujo de trabajo, sincronización o automatización dependientes. No hay ninguna extensión planificada más allá de esta fecha, por lo que debe migrar sus integraciones mucho antes.

## Preguntas frecuentes

**¿Afecta esto a las integraciones empaquetadas que proporciona Adobe, como Slack o Microsoft Teams?**

No. Adobe migra directamente las aplicaciones globales administradas por Adobe y no requiere que usted actúe.

**¿Dejará de funcionar mi integración actual antes del 1 de febrero de 2027?**

No. Las aplicaciones OAuth2 personalizadas existentes siguen funcionando normalmente hasta el 1 de febrero de 2027. Solo se ve afectada la capacidad de crear nuevas aplicaciones OAuth2 personalizadas a partir del 1 de noviembre de 2026.

**¿Hay algún costo para migrar?**

No, no hay ningún coste adicional asociado con la autenticación a través de Adobe Developer Console.

**¿Dónde puedo obtener ayuda?**

Póngase en contacto con el equipo de su cuenta de Workfront o abra un caso de asistencia si tiene preguntas sobre su integración específica o cronología. Para ver el tutorial oficial y actualizado sobre la configuración con capturas de pantalla, consulte [Obtener acceso](https://developer.adobe.com/workfront-apis/guides/gaining_access/) en la documentación de Developer Console de Adobe.
