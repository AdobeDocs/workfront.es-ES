---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Administrar claves de API
description: Para minimizar las vulnerabilidades de seguridad de la API, los administradores de Adobe Workfront pueden administrar las claves de API utilizadas para permitir que las aplicaciones accedan a Workfront en nombre de un usuario.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1374'
ht-degree: 2%

---

# Administrar claves de API

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

Para minimizar las vulnerabilidades de seguridad de la API, los administradores de Adobe Workfront pueden administrar las claves de API utilizadas para permitir que las aplicaciones accedan a Workfront en nombre de un usuario.

Puede restablecer o eliminar la clave de API del administrador actual, configurar las claves de API para que caduquen y eliminar las claves de API para todos los usuarios.

Algunos ejemplos de aplicaciones que aprovechan la API de Workfront son:

* Integraciones de documentos como Dropbox, Google Drive y Workfront DAM
* Aplicaciones móviles de Workfront

>[!IMPORTANT]
>
>Al restablecer o eliminar una clave de API, cualquier aplicación que aproveche la API de Workfront y se autentique en Workfront mediante esta clave de API debe volver a configurarse para recuperar el acceso a Workfront.

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

## Claves de API de Workfront

Cada usuario de Workfront tiene una clave de API única. Esta clave se genera por usuario cada vez que el usuario accede a una integración que aprovecha la API de Workfront (como la aplicación móvil de Workfront o la integración de documentos).

>[!NOTE]
>
> Las claves de API que genera en el entorno de producción se copian en el entorno de vista previa durante la actualización semanal. Las claves de API que genere en el entorno de vista previa se sobrescribirán con las claves de API de producción durante la actualización semanal.

Los administradores de Workfront también tienen una clave de API única. Cuando una aplicación utiliza una clave de API de administrador para acceder a Workfront, la aplicación tiene acceso de administrador a Workfront.

## Administrar una clave de API de administrador

Puede generar, restablecer o eliminar la clave de API de su cuenta de usuario administrador.

>[!NOTE]
>
>También puede generar una clave de API a través de la API. Para obtener más información, consulte la [API de suscripción de evento](../../../wf-api/general/event-subs-api.md) en [API de suscripción de evento](../../../wf-api/general/event-subs-api.md).

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Sistema >** **Información del cliente.**
1. (Condicional) Realice una de las siguientes acciones:

   Para generar una clave de API: En el **Configuración de clave de API** , haga clic en **Generar clave de API**.

   O\
   Para restablecer una clave de API: En el **Configuración de clave de API** , haga clic en **Restablecer**, luego **Restablecer.**

   O

   Para eliminar la clave de API: En el **Configuración de clave de API** , haga clic en **Eliminar**, luego **Eliminar**.

## Generar una clave de API para usuarios no administradores

Puede generar y administrar claves de API para usuarios en funciones que no sean el administrador de Workfront.

>[!NOTE]
>
>Esto no está disponible si la instancia de Workfront de su organización está habilitada con Adobe IMS. Si necesita más información, consulte con su administrador de red o TI.

1. (Condicional) Si su organización utiliza la administración de acceso del inicio de sesión único (SSO), desactive temporalmente la opción que requiere autenticación SSO.

   1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

   1. Expandir **Sistema** y haga clic en **Inicio de sesión único (SSO)**.\
      ![](assets/sysadmin-security-sso-disable-31620-350x320.png)

   1. Desactive la casilla que requiere autenticación SSO.

      Por ejemplo, si su organización utiliza SAML 2.0, deshabilite **Permitir solo la autenticación SAML 2.0**.

1. En la barra de direcciones de un explorador, introduzca la siguiente llamada de API:

   `<domain>`**.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&amp;username=**username**&amp;password=**password**&amp;method=PUT

   Reemplazar `<domain>` con el nombre de dominio de Workfront, el nombre de usuario y la contraseña con las credenciales de Workfront del usuario.

1. (Condicional) Active la opción que requiere autenticación SSO si la ha deshabilitado en el paso 1.

   1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

   1. Expandir **Sistema** y haga clic en **Inicio de sesión único (SSO)**.

   1. Seleccione su método SSO en la **Tipo** menú desplegable.
   1. Marque la casilla que requiere autenticación SSO.

## Configurar cuándo caducan las claves de API

Puede configurar las claves de API para que caduquen para todos los usuarios del sistema. Cuando caduca la clave de API de un usuario, este debe volver a autenticarse en cualquier aplicación que utilice la API de Workfront para acceder a Workfront. Puede cambiar la frecuencia con la que caducan las claves de API. También puede configurar si las claves de API caducan cuando caduca la contraseña de un usuario.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Sistema** > **Información del cliente**.
1. En el **Configuración de clave de API** , en el **Después de la creación**, **Las claves de API caducan en** en la lista desplegable, seleccione el intervalo de tiempo en el que desea que caduquen las claves de API.

   Al cambiar esta opción, el nuevo intervalo de tiempo comienza a partir del momento en que se realizó el cambio. Por ejemplo, si cambia esta opción de *1 mes* a *6 meses*, las claves de API caducan a los 6 meses del momento en que realiza el cambio.

   De forma predeterminada, las claves de API caducan cada mes.

1. Para configurar las claves de API para que caduquen cuando caduquen las contraseñas de los usuarios, seleccione **Eliminar la clave de API cuando caduque la contraseña de un usuario**.

   De forma predeterminada, esta opción no está seleccionada.

   Para obtener información sobre cómo configurar las contraseñas de los usuarios para que caduquen, consulte [Configuración de las preferencias de seguridad del sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

1. Haga clic en **Guardar**.

## Eliminación de las claves de API para todos los usuarios

Si le preocupa una infracción de seguridad específica en relación con su sistema Workfront, puede eliminar las claves de API de forma simultánea para todos los usuarios.

>[!IMPORTANT]
>
>Al eliminar las claves de API para todos los usuarios, se invalidan TODAS las claves de API para todos los usuarios del sistema. Esta acción hará que todas las integraciones en Workfront fallen hasta que genere una nueva clave de API en Workfront y actualice todas las integraciones.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Expandir **Sistema** y haga clic en **Información del cliente.**

1. En el **Configuración de clave de API** área, haga clic en **Eliminar todas las claves de API** y haga clic en **Eliminar** **Todo**.

## Restricción de los inicios de sesión de API con un certificado X.509

>[!IMPORTANT]
>
>El procedimiento descrito en esta sección se aplica únicamente a las organizaciones que aún no se han incorporado a la plataforma empresarial de Adobe. El inicio de sesión en Workfront a través de la API de Workfront no está disponible si su organización se ha incorporado a la plataforma empresarial de Adobe.
>
>Para obtener una lista de procedimientos que difieren en función de si su organización ha sido incorporada a la plataforma empresarial de Adobe, consulte [Diferencias de administración basadas en plataformas (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Las aplicaciones de terceros pueden comunicarse con Workfront a través de la API. Para aumentar la seguridad del sitio de Workfront, puede configurar Workfront para que restrinja las solicitudes de inicio de sesión de API cargando un certificado X.509 a Workfront. Una vez activada, todas las solicitudes de inicio de sesión a través de la API deben incluir un certificado de cliente, además del nombre de usuario y la contraseña.

>[!NOTE]
>
>Esto no está disponible si la instancia de Workfront de su organización está habilitada con Adobe IMS. Si necesita más información, consulte con su administrador de red o TI.

* [Obtener el certificado X.509](#obtain-the-x-509-certificate)
* [Cargar el certificado a Workfront](#upload-the-certificate-to-workfront)
* [Verifique que las llamadas de inicio de sesión de API estén restringidas](#verify-api-login-calls-are-restricted)

### Obtener el certificado X.509 {#obtain-the-x-509-certificate}

Obtenga un certificado X.509 válido de una entidad emisora de certificados de confianza (como Verisign) y colóquelo en una ubicación temporal de su estación de trabajo.

### Cargar el certificado a Workfront {#upload-the-certificate-to-workfront}

Una vez que haya obtenido el certificado X.509 de su autoridad certificadora, debe cargarlo en Workfront.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Expandir **Sistema** y haga clic en **Información del cliente**.

1. En el **Configuración de clave de API** área, seleccione **Habilitar certificado X.509**.
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

### Verifique que las llamadas de inicio de sesión de API estén restringidas {#verify-api-login-calls-are-restricted}

Antes de configurar la instancia de Workfront para que requiera un certificado X.509, realice una solicitud de API a la función `/login` usando parámetros de nombre de usuario y contraseña válidos. Recibirá una respuesta de 200 que contiene un sessionID.

Después de hacer que el certificado X.509 sea un requisito a través de la página de información del cliente en su instancia de Workfront, realice otro intento de inicio de sesión. Esta vez recibirá una respuesta de error 500 con el siguiente mensaje: &quot;Solicitud no confiable. Póngase en contacto con el administrador del sistema y adjunte el certificado&quot;.

Después de confirmar que el certificado X.509 es obligatorio, realice la misma solicitud de inicio de sesión con un parámetro adicional para apiCertificate establecido en el valor del certificado. Si esta operación se realizó correctamente, recibirá una respuesta de 200 que contiene un sessionID válido.
