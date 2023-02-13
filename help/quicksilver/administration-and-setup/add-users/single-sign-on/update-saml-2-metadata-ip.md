---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Actualización de metadatos de SAML 2.0 en su proveedor de identidad
description: Puede actualizar los metadatos de SAML 2.0 en su proveedor de identidad.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: 96f1d50024605328713ca2019f3b726e27dc569c
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 0%

---

# Actualización de metadatos de SAML 2.0 en su proveedor de identidad

{{important-admin-console-onboard}}

Las siguientes secciones describen cómo actualizar los metadatos de Lenguaje de marcado de aserción de seguridad (SAML) 2.0 al usar los Servicios de federación de Active Directory (ADFS) como proveedor de identidad.

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

## Usar ADFS como proveedor de identidad

Puede actualizar los metadatos de ADFS antes de que Adobe Workfront actualice el certificado SAML 2.0 o posterior. Si decide actualizar los metadatos de ADFS antes de que Workfront actualice el certificado SAML 2.0, se requieren pasos adicionales.

* [Actualización de los metadatos de ADFS](#update-your-adfs-metadata)
* [Forzar la actualización de los metadatos de ADFS](#force-your-adfs-metadata-to-update)

### Actualización de los metadatos de ADFS {#update-your-adfs-metadata}

Para configurar los metadatos de ADFS para que se actualicen automáticamente, complete los pasos de esta sección.

De forma predeterminada, ADFS está configurado para comprobar automáticamente si hay actualizaciones en todos sus metadatos de confianza de la parte de confianza; sin embargo, el valor predeterminado se establece en encuesta solo cada 24 horas. Puede cambiar este valor con comandos powershell.

1. Inicie sesión en el servidor ADFS y abra la Consola de administración de ADFS.
1. En el panel izquierdo, expanda **ADFS 2.0,** a continuación, expanda **Relaciones de confianza.**

1. Haga clic en el **Confiar en las confianzas del partido** carpeta.
1. Seleccione la confianza de la parte que confía que ha configurado anteriormente para su uso con Workfront y, a continuación, en el panel derecho, haga clic en **Actualización desde metadatos de federación**.
1. (Condicional) Si esta opción está atenuada (lo que significa que la confianza de la parte que confía se configuró anteriormente mediante un archivo de metadatos), complete lo siguiente.

   1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

   1. Haga clic en **Sistema** > **Inicio de sesión único (SSO)**.

   1. Haga clic en **Editar configuración.**
   1. Haga clic en **Editar configuración** y, a continuación, seleccione **SAML 2.0** en el **Tipo** lista desplegable.

   1. Copie el **Dirección URL de metadatos**, que debería ser similar a lo siguiente:

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. En el servidor ADFS, haga clic con el botón derecho en la confianza de la parte de confianza que configuró anteriormente y, a continuación, haga clic en **Propiedades.**
   1. Haga clic en el **Monitorización** , pegue la dirección URL que ha copiado de Workfront en la **URL de metadatos de federación de la parte que confía** campo .

   1. Consulte las opciones para **Supervisar a la parte que confía** y **Actualizar automáticamente la parte de confianza**.

   1. Haga clic en **OK.**
   1. Seleccione la confianza de la parte que confía que configuró anteriormente para su uso con Workfront; a continuación, en el panel derecho, haga clic en **Actualización desde metadatos de federación.**

1. Haga clic en **OK** para ignorar el mensaje acerca de que parte del contenido de los metadatos de federación no es compatible con ADFS 2.0.
1. Apertura **Módulos PowerShell de Windows.**
1. Después de cargar todos los módulos, ejecute el siguiente comando en powershell:

   `Get-ADFSProperties`

1. Busque el valor situado junto a **Intervalo de monitorización.**

   Será un número que representa el número de minutos entre las encuestas. El valor predeterminado debe ser 1440 (1440 minutos = 24 horas).

1. Establezca un nuevo valor ejecutando el siguiente comando en powershell:

   `Set-ADFSProperties -MonitoringInterval 1`

   Esto cambia el intervalo de monitorización de cada 24 horas a cada minuto. Puede cambiar el valor 1 por otro mayor si desea que sondee con menos frecuencia.

1. Para comprobar que esto funciona correctamente, utilice la variable **Visor de eventos** para buscar la siguiente información en los registros ADFS2.0:

   **ID de evento 156 y 157**

### Forzar la actualización de los metadatos de ADFS {#force-your-adfs-metadata-to-update}

Para actualizar los metadatos de ADFS, complete los pasos de la siguiente sección.

Para forzar el intercambio de metadatos entre Workfront y su proveedor SAML 2.0 al utilizar los Servicios de federación de Active Directory (ADFS):

>[!NOTE]
>
>Es posible que el departamento de TI deba realizar algunos de estos cambios.

1. Inicie sesión en el servidor ADFS y abra la **Consola de administración de ADFS**.
1. En el panel izquierdo, expanda **ADFS 2.0** y, a continuación, expanda **Relaciones de confianza**.

1. Haga clic en el **Confiar en las confianzas del partido** carpeta.
1. Seleccione la confianza de la parte que confía que ha configurado anteriormente para su uso con Workfront y, a continuación, en el panel derecho, haga clic en **Actualización desde metadatos de federación**.

   Si esta opción está atenuada y no se puede seleccionar, complete lo siguiente:

   (La opción solo se verá atenuada cuando la confianza de la parte que confía se haya configurado anteriormente mediante un archivo de metadatos).

   1. En Workfront, en el área Configuración, copie la **Dirección URL de metadatos** desde la pantalla de configuración del inicio de sesión único de Workfront.

      Para acceder a la información de la variable **Dirección URL de metadatos**:

      1. Haga clic en **Configuración** cerca de la esquina superior derecha de Adobe Workfront en la barra de navegación global.
      1. Haga clic en > **Sistema** > **Inicio de sesión único (SSO)**.
      1. Haga clic en **Editar configuración.**
      1. Haga clic en **Editar configuración** y, a continuación, seleccione **SAML 2.0** en el **Tipo** lista desplegable.
      1. Copie el **Dirección URL de metadatos**, que debería ser similar a lo siguiente:

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`
   1. En el servidor ADFS, haga clic con el botón derecho en la confianza de la parte de confianza que configuró anteriormente y, a continuación, haga clic en **Propiedades.**
   1. Haga clic en el **Monitorización** , pegue la dirección URL que ha copiado de Workfront en la **URL de metadatos de federación de la parte que confía** campo .
   1. Consulte las opciones para **Supervisar a la parte que confía** y **Actualizar automáticamente la parte de confianza**.
   1. Haga clic en **OK**.
   1. Seleccione la confianza de la parte que confía que ha configurado anteriormente para su uso con Workfront y, a continuación, en el panel derecho, haga clic en **Actualización desde metadatos de federación.**


1. Haga clic en **OK** para ignorar el mensaje acerca de que parte del contenido de los metadatos de federación no es compatible con ADFS 2.0.
1. Haga clic en **Actualizar** para completar la actualización de los metadatos de federación.

Usuarios a los que se permite acceder a Workfront a través de la pantalla de inicio de sesión nativa mediante las credenciales de inicio de sesión de Workfront (esto se puede configurar desde la página de perfil de cada usuario en la **Acceso** ) puede iniciar sesión con su nombre de usuario y contraseña de Workfront navegando a la siguiente URL: `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`.

## Uso de otros proveedores de identidad

Al utilizar proveedores de identidad que no sean ADFS (como Ping, Okta o Centrify), debe volver a cargar los metadatos de Workfront en su proveedor de identidad.

Para obtener más información sobre cómo obtener una nueva URL de metadatos de Workfront, consulte [Actualización de los metadatos de ADFS](#update-your-adfs-metadata).

Para obtener información adicional sobre el uso de los Servicios de federación de Active Directory (ADFS) con SAML 2.0 en Workfront, consulte [Configuración de Adobe Workfront con SAML 2.0 mediante ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
