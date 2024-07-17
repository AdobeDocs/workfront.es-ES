---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Actualización de metadatos de SAML 2.0 en el proveedor de identidad
description: Puede actualizar los metadatos de SAML 2.0 en su proveedor de identidad.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 0%

---

# Actualización de metadatos de SAML 2.0 en el proveedor de identidad

{{important-admin-console-onboard}}

En las secciones siguientes se describe cómo actualizar los metadatos del Lenguaje de marcado de aserción de seguridad (SAML) 2.0 cuando se usan los Servicios de federación de Active Directory (ADFS) como proveedor de identidad.

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Usar ADFS como proveedor de identidad

Puede actualizar los metadatos de ADFS antes de que Adobe Workfront actualice el certificado SAML 2.0 o después. Si decide actualizar los metadatos de ADFS antes de que Workfront actualice el certificado SAML 2.0, se requieren pasos adicionales.

* [Actualice los metadatos de ADFS](#update-your-adfs-metadata)
* [Forzar la actualización de los metadatos de ADFS](#force-your-adfs-metadata-to-update)

### Actualizar los metadatos de ADFS {#update-your-adfs-metadata}

Para configurar los metadatos de ADFS para que se actualicen automáticamente, complete los pasos de esta sección.

De forma predeterminada, ADFS está configurado para comprobar automáticamente si hay actualizaciones para todos los metadatos de confianza de usuario de confianza; sin embargo, el valor predeterminado se establece en sondear solamente cada 24 horas. Puede cambiar este valor con comandos de powershell.

1. Inicie sesión en el servidor de ADFS y abra la Consola de administración de ADFS.
1. En el panel izquierdo, expanda **ADFS 2.0,** y, a continuación, expanda **Relaciones de confianza.**

1. Haga clic en la carpeta **Confianzas de usuario de confianza**.
1. Seleccione la relación de confianza de usuario autenticado que configuró anteriormente para su uso con Workfront y, a continuación, en el panel derecho, haga clic en **Actualizar a partir de metadatos de federación**.
1. (Condicional) Si esta opción está atenuada (lo que significa que la confianza de usuario autenticado se configuró previamente mediante un archivo de metadatos), complete lo siguiente.

   1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

   1. Haga clic en **Sistema** > **Inicio de sesión único (SSO)**.

   1. Haga clic en **Editar configuración.**
   1. Haga clic en **Editar configuración** y, a continuación, seleccione **SAML 2.0** en la lista desplegable **Tipo**.

   1. Copie la **URL de metadatos**, que debe ser similar a la siguiente:

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. En el servidor ADFS, haga clic con el botón secundario en la confianza de usuario autenticado que configuró anteriormente y, a continuación, haga clic en **Propiedades.**
   1. Haga clic en la ficha **Supervisión** y, a continuación, pegue la dirección URL que copió de Workfront en el campo **URL de metadatos de federación de usuario de confianza**.

   1. Marque las opciones para **Supervisar usuario autenticado** y **Actualizar automáticamente usuario autenticado**.

   1. Haga clic en **Aceptar.**
   1. Seleccione la relación de confianza de usuario autenticado que configuró anteriormente para su uso con Workfront; a continuación, en el panel derecho, haga clic en **Actualizar a partir de metadatos de federación.**

1. Haga clic en **Aceptar** para omitir el mensaje sobre algunos de los metadatos de federación que ADFS 2.0 no admite.
1. Abra **Módulos De Windows Powershell.**
1. Una vez cargados todos los módulos, ejecute el siguiente comando en powershell:

   `Get-ADFSProperties`

1. Busque el valor junto a **Intervalo de supervisión.**

   Será un número que representa el número de minutos entre encuestas. El valor predeterminado debe ser 1440 (1440 minutos = 24 horas).

1. Establezca un nuevo valor ejecutando el siguiente comando en powershell:

   `Set-ADFSProperties -MonitoringInterval 1`

   Esto cambia el intervalo de monitorización de cada 24 horas a cada minuto. Puede cambiar el 1 por otro valor mayor si desea que sondee con menos frecuencia.

1. Para comprobar que esto funciona correctamente, use el **Visor de eventos** para buscar la siguiente información en los registros ADFS2.0:

   **Id. de evento 156 y 157**

### Forzar la actualización de los metadatos de ADFS {#force-your-adfs-metadata-to-update}

Para actualizar los metadatos de ADFS, complete los pasos de la siguiente sección.

Para forzar el intercambio de metadatos entre Workfront y su proveedor SAML 2.0 al utilizar los Servicios de federación de Active Directory (ADFS):

>[!NOTE]
>
>Es posible que el departamento de TI deba realizar algunos de estos cambios.

1. Inicie sesión en el servidor ADFS y abra **Consola de administración de ADFS**.
1. En el panel izquierdo, expanda **ADFS 2.0** y, a continuación, expanda **Relaciones de confianza**.

1. Haga clic en la carpeta **Confianzas de usuario de confianza**.
1. Seleccione la relación de confianza de usuario autenticado que configuró anteriormente para su uso con Workfront y, a continuación, en el panel derecho, haga clic en **Actualizar a partir de metadatos de federación**.

   Si esta opción está atenuada y no se puede seleccionar, complete lo siguiente:

   (La opción sólo aparece atenuada cuando la confianza de usuario de confianza se configuró previamente mediante un archivo de metadatos.)

   1. En Workfront, en el área Configuración, copie la **URL de metadatos** de la pantalla de configuración de inicio de sesión único de Workfront.

      Para obtener acceso a la información de la **URL de metadatos**:

      1. Haga clic en **Configuración** cerca de la esquina superior derecha de Adobe Workfront en la barra de navegación global.
      1. Haga clic en > **Sistema** > **Inicio de sesión único (SSO)**.
      1. Haga clic en **Editar configuración.**
      1. Haga clic en **Editar configuración** y, a continuación, seleccione **SAML 2.0** en la lista desplegable **Tipo**.
      1. Copie la **URL de metadatos**, que debe ser similar a la siguiente:

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. En el servidor ADFS, haga clic con el botón secundario en la confianza de usuario autenticado que configuró anteriormente y, a continuación, haga clic en **Propiedades.**
   1. Haga clic en la ficha **Supervisión** y, a continuación, pegue la dirección URL que copió de Workfront en el campo **URL de metadatos de federación de usuario de confianza**.
   1. Marque las opciones para **Supervisar usuario autenticado** y **Actualizar automáticamente usuario autenticado**.
   1. Haga clic en **Aceptar**.
   1. Seleccione la relación de confianza de usuario autenticado que configuró anteriormente para su uso con Workfront y, a continuación, en el panel derecho, haga clic en **Actualizar a partir de metadatos de federación.**

1. Haga clic en **Aceptar** para omitir el mensaje sobre algunos de los metadatos de federación que ADFS 2.0 no admite.
1. Haga clic en **Actualizar** para completar la actualización de los metadatos de federación.

Los usuarios a los que se les permite acceder a Workfront a través de la pantalla nativa de inicio de sesión con credenciales de inicio de sesión de Workfront (esto se puede configurar desde la página de perfil de cada usuario en la sección **Acceso**) pueden iniciar sesión con su nombre de usuario y contraseña de Workfront navegando a la siguiente URL: `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`.

## Uso de otros proveedores de identidad

Cuando se utilizan proveedores de identidad distintos de ADFS (como Ping, Okta o Centrify), es necesario volver a cargar los metadatos de Workfront en el proveedor de identidad.

Para obtener más información sobre cómo obtener una nueva URL de metadatos de Workfront, consulta [Actualizar tus metadatos de ADFS](#update-your-adfs-metadata).

Para obtener información adicional acerca del uso de los Servicios de federación de Active Directory (ADFS) con SAML 2.0 en Workfront, vea [Configurar Adobe Workfront con SAML 2.0 mediante ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
