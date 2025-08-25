---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Administrar claves API
description: Para minimizar las vulnerabilidades de seguridad de la API, los administradores de Adobe Workfront pueden administrar las claves de API utilizadas para que las aplicaciones puedan acceder a Workfront en nombre de un usuario.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
source-git-commit: 99113ac4f2ceca6bd50f078916e33cec7f577362
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 88%

---

# Administrar claves API

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

Para minimizar las vulnerabilidades de seguridad de la API, los administradores de Adobe Workfront pueden administrar las claves de API utilizadas para que las aplicaciones puedan acceder a Workfront en nombre de un usuario.

Puede restablecer o eliminar su clave de API de administrador actual, configurar las claves de API para que caduquen y eliminar las claves de API de todos los usuarios.

Algunos ejemplos de aplicaciones que aprovechan la API de Workfront son los siguientes:

* Integraciones de documentos como Dropbox, Google Drive y Workfront DAM
* Aplicaciones móviles de Workfront

>[!IMPORTANT]
>
>Al restablecer o eliminar una clave de API, cualquier aplicación que aproveche la API de Workfront y se autentique en Workfront mediante esta clave de API debe volver a configurarse para recuperar el acceso a Workfront.

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

## Claves de API de Workfront

Cada usuario de Workfront tiene una clave de API única. Esta clave se genera por usuario cuando el usuario accede a una integración que aprovecha la API de Workfront (como la aplicación móvil de Workfront o una integración de documentos).

>[!NOTE]
>
> Las claves de API que genere en el entorno de producción se copian en el entorno de vista previa durante la actualización semanal. Las claves de API que genere en el entorno de vista previa se sobrescribirán con las claves de API del entorno de producción durante la actualización semanal.

Los administradores de Workfront también tienen una clave de API única. Cuando una aplicación utiliza una clave de API de administrador para acceder a Workfront, la aplicación tiene acceso de administrador a Workfront.

## Administración de una clave de API de administrador

Puede generar, restablecer o eliminar la clave de API de su cuenta de usuario de administrador.

>[!NOTE]
>
>También puede generar una clave de API a través de la API. Para obtener más información, consulte la sección [API de suscripción a eventos](../../../wf-api/general/event-subs-api.md) en [API de suscripción a eventos](../../../wf-api/general/event-subs-api.md).

{{step-1-to-setup}}

1. Haga clic en **Sistema >** **Información del cliente.**
1. (Condicional) Realice una de las siguientes acciones:

   Para generar una clave API: en la sección **Configuración de clave API**, haga clic en **Generar clave API**.

   O\
   Para restablecer una clave de API: en la sección **Configuración de clave API**, haga clic en **Restablecer** y, a continuación, en **Restablecer.**

   O

   Para quitar la clave de API: en la sección **Configuración de clave API**, haga clic en **Quitar** y, a continuación, en **Quitar**.

## Generación de una clave de API para usuarios no administradores—>

<!--DELETE THIS SECTION MARCH 2026-->

>[!IMPORTANT]
>
>El procedimiento descrito en esta sección se ha eliminado porque se aplicaba únicamente a las organizaciones que aún no se habían incorporado a Adobe Admin Console.
>
>Todas las organizaciones de Workfront se han incorporado a Adobe Admin Console.

<!--You can generate and manage API Keys for users in roles other than Workfront administrator.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

1. (Conditional) If your organization uses Single Sign-On (SSO) access management, temporarily disable the option requiring SSO authentication.

   {{step-1-to-setup}} 
   
   1. Expand **System**, then click **Single Sign-on (SSO)**. 
   1. In the **Type** field, select the type of SSO your organization uses.
   1. With the type selected, scroll down and clear the **Enable** checkbox. 
      ![Enable SSO](assets/sysadmin-security-sso-disable-31620-350x320.png)  
   1. Click **Save**.


1. In the address bar of a browser, enter the following API call:

   `<domain>`.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&username=**username**&password=**password**&method=PUT

   Replace `<domain>` with your Workfront domain name, and username and password with the user's Workfront credentials.

1. (Conditional) Enable the option requiring SSO authentication if you disabled it in Step 1.

   {{step-1-to-setup}}
   
   1. Expand **System**, then click **Single Sign-on (SSO)**.
   
   1. Select your SSO method in the **Type** drop down menu.
   1. Check the checkbox requiring SSO authentication.-->

## Configure cuándo caducan las claves API

Puede configurar las claves API de modo que caduquen para todos los usuarios del sistema. Cuando la clave API de un usuario caduca, el usuario debe volver a autenticarse en cualquier aplicación que utilice la API de Workfront para acceder a Workfront. Puede cambiar la frecuencia con la que caducan las claves API. También puede configurar si las claves API caducan cuando caduca la contraseña de un usuario.

{{step-1-to-setup}}

1. Haga clic en **Sistema** > **Información del cliente**.
1. En el área **Configuración de clave API**, en la lista desplegable **Después de la creación**, **Las claves API caducan en**, seleccione el periodo de tiempo en el que desea que caduquen las claves API.

   Al cambiar esta opción, el nuevo periodo de tiempo comienza a partir del momento en que realizó el cambio. Por ejemplo, si cambia esta opción de *1 mes* a *6 meses*, las claves API caducarán dentro de 6 meses a partir del momento en que realice el cambio.

   De forma predeterminada, las claves API caducan cada mes.

1. Para configurar las claves API para que caduquen cuando caduquen las contraseñas de los usuarios, habilite **Quitar clave API cuando caduque la contraseña de un usuario**.

   Esta opción no está habilitada de forma predeterminada.

   Para obtener información sobre cómo configurar las contraseñas de usuario para que caduquen, consulte [Configurar las preferencias de seguridad del sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

1. Haga clic en **Guardar**.

## Eliminar las claves API de todos los usuarios

Si le preocupa una infracción de seguridad concreta en relación con su sistema de Workfront, puede quitar las claves API simultáneamente para todos los usuarios.

>[!IMPORTANT]
>
>Al quitar las claves API de todos los usuarios, se invalidan TODAS las claves API de todos los usuarios del sistema. Esta acción hará que todas las integraciones en Workfront arrojen un error hasta que genere una nueva clave API en Workfront y actualice todas las integraciones.

{{step-1-to-setup}}

1. Expanda **Sistema** y, a continuación, haga clic en **Información del cliente**.

1. En el área **Configuración de clave API**, haga clic en **Quitar todas las claves API** y, a continuación, haga clic en **Quitar** **Todo**.

## Restricción de los inicios de sesión en la API con un certificado X.509

>[!IMPORTANT]
>
>El procedimiento descrito en esta sección se aplica solo a las organizaciones que todavía no se han incorporado a Adobe Business Platform. El inicio de sesión en Workfront a través de la API de Workfront no está disponible si su organización se ha incorporado a Adobe Business Platform.
>
>Para obtener una lista de procedimientos que difieren según si su organización se ha incorporado a Adobe Business Platform, consulte [Diferencias de administración basadas en la plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>Esto no está disponible si la instancia de Workfront de su organización está habilitada con Adobe IMS. Consulte al administrador de red o de TI si necesita más información.

Las aplicaciones de terceros pueden comunicarse con Workfront a través de la API. Para aumentar la seguridad del sitio de Workfront, puede configurar Workfront para que restrinja las solicitudes de inicio de sesión de API cargando un certificado X.509 en Workfront. Una vez habilitado, todas las solicitudes de inicio de sesión mediante la API deben incluir un certificado de cliente, además del nombre de usuario y la contraseña.

* [Obtener el certificado X.509](#obtain-the-x-509-certificate)
* [Cargar el certificado en Workfront](#upload-the-certificate-to-workfront)
* [Verificar que las llamadas de inicio de sesión de API estén restringidas](#verify-api-login-calls-are-restricted)

### Obtener el certificado X.509 {#obtain-the-x-509-certificate}

Obtenga un certificado X.509 válido de una entidad emisora de certificados de confianza (como Verisign) y guárdelo en una ubicación temporal de la estación de trabajo.

### Cargar el certificado en Workfront {#upload-the-certificate-to-workfront}

Una vez que haya obtenido el certificado X.509 de su autoridad de certificación, deberá cargarlo en Workfront.

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![Icono de configuración de engranajes](assets/gear-icon-settings.png).

1. Expanda **Sistema** y, a continuación, haga clic en **Información del cliente**.

1. En el área **Configuración de clave API**, seleccione **Requerir certificado X.509 para inicios de sesión en API**.
1. Haga clic en **Cambiar certificado**.
1. En la estación de trabajo, busque y seleccione el certificado X.509 que descargó anteriormente.
1. (Opcional) Haga clic en **Ver detalles** junto al nombre del certificado para ver los siguientes detalles sobre el certificado:

   * Nombre común del sujeto
   * Organización del sujeto
   * Unidad de organización del sujeto
   * Nombre común del emisor
   * Organización emisora
   * Unidad de organización emisora
   * Número de serie
   * Fecha de emisión
   * Fecha de caducidad

1. Haga clic en **Guardar**.

### Verificar que las llamadas de inicio de sesión de API estén restringidas {#verify-api-login-calls-are-restricted}

Antes de configurar la instancia de Workfront para que requiera un certificado X.509, realice una solicitud de API al punto final `/login` utilizando parámetros de nombre de usuario y contraseña válidos. Recibirá una respuesta 200 con un sessionID.

Después de hacer que el certificado X.509 sea un requisito a través de la página de información del cliente en su instancia de Workfront, realice otro intento de inicio de sesión. Esta vez recibirá una respuesta de error 500 con el siguiente mensaje: “Solicitud que no es de confianza. Comuníquese con el administrador del sistema y adjunte un certificado”.

Después de confirmar que el certificado X.509 es obligatorio, realice la misma solicitud de inicio de sesión con un parámetro adicional de apiCertificate establecido en el valor de su certificado. Si esta operación se ha realizado correctamente, recibirá una respuesta 200 con un sessionID válido.
