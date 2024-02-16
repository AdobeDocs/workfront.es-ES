---
title: Actualización de metadatos de SAML 2.0 en el IDP al utilizar autenticación mejorada
description: Como administrador de Adobe Workfront, puede integrar el inicio de sesión único (SSO) de Workfront con cualquier proveedor de identidad que admita el protocolo SAML (Security Assertion Markup Language) 2.0.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 55d7d8a8-0dfe-45bc-a23a-47111347e9ca
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# Actualización de metadatos de SAML 2.0 en el IDP al utilizar autenticación mejorada

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Como administrador de Adobe Workfront, puede integrar el inicio de sesión único (SSO) de Workfront con cualquier proveedor de identidad que admita el protocolo SAML (Security Assertion Markup Language) 2.0.

En las secciones siguientes se describe el proceso de integración cuando su cuenta de Workfront se ha actualizado a la experiencia de autenticación mejorada (aún no disponible para todas las organizaciones). Para obtener más información sobre la experiencia de autenticación mejorada, consulte [Introducción a la autenticación mejorada](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md).

Para obtener información sobre la configuración de SAML antes de la migración a la experiencia de autenticación mejorada, consulte [Actualización de metadatos de SAML 2.0 en el proveedor de identidad](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).


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
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Use Okta como proveedor de identidad

Okta es un ejemplo de proveedor de identidad compatible con SAML 2.0. En esta sección se describe cómo utilizar Okta como proveedor de identidad. Se requerirían pasos similares al configurar otro proveedor de identidad que admita SAML 2.0.

>[!NOTE]
>
>Los usuarios se asignan en función de su dirección de correo electrónico. Para iniciar sesión en Workfront con Okta, debe tener un usuario con la misma dirección de correo electrónico (sin distinción de mayúsculas y minúsculas) creada en su cliente de Workfront.

Complete las siguientes secciones para configurar Okta como su proveedor de identidad en Workfront.

* [Crear una aplicación de Workfront en Okta](#create-a-workfront-app-in-okta)
* [Añada la instancia de Okta como proveedor de identidad en Workfront](#add-your-okta-instance-as-an-identity-provider-in-workfront)

### Crear una aplicación de Workfront en Okta {#create-a-workfront-app-in-okta}

1. Inicie sesión en su entorno de Okta.
1. Asegúrese de que **IU clásica** está seleccionado en la esquina superior izquierda de la interfaz Okta.
1. En el menú, haga clic en **Aplicaciones** > **Aplicaciones**.

1. Clic **Agregar aplicación**, luego haga clic en **Crear nueva aplicación**.

1. En el **Cuadro de diálogo Crear una nueva integración de aplicaciones** , seleccione **SAML 2.0**, luego haga clic en **Crear**.

1. Especifique un nombre para la aplicación de Workfront y haga clic en **Siguiente**.
1. En la página Configuración de SAML que aparece, busque la información necesaria para la página Configuración de SAML:

   1. Sin salir de la pestaña del explorador donde se muestra la interfaz Okta, abra una pestaña o ventana independiente del explorador.
   1. Especifique la siguiente URL en el explorador:

      `https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata`

   1. En el archivo XML resultante, identifique los valores de **entityID** y **Ubicación**.

      ![sso-okta.png](assets/sso-okta.png)

   1. Copie el valor del **entityID** al portapapeles del sistema. No cierre esta pestaña del explorador.

1. Vuelva a la página Configuración de SAML que abrió en el paso 6.
1. Pegue el valor desde el **entityID** en el campo **URI de audiencia (ID de entidad de SP)** field.

1. En el archivo XML de la pestaña del otro explorador, copie el valor del **Ubicación** field.
1. Pegue el valor desde el **Ubicación** en el campo **Inicio de sesión único** **URL** field.

1. Desplácese hasta **Instrucciones de atributo (opcional)** sección.
1. En el **Nombre** , especifique **email**.

1. En el **Valor** , especifique **user.email**.

1. (Opcional) Añada cualquier valor avanzado.
1. Clic **Siguiente**.
1. Seleccione, **Soy cliente de Okta que agrega una aplicación interna**, luego haga clic en **Finalizar**.

### Añada la instancia de Okta como proveedor de identidad en Workfront {#add-your-okta-instance-as-an-identity-provider-in-workfront}

Este procedimiento proporciona información esencial para configurar Okta como proveedor de identidad en Workfront. Para obtener información adicional sobre otras asignaciones u opciones de configuración, consulte [Configuración de Adobe Workfront con SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

1. Descargue los metadatos del proveedor de identidad para su instancia de Okta:

   1. Inicie sesión en su entorno de Okta.
   1. Asegúrese de que **IU clásica** está seleccionado en la esquina superior izquierda de la interfaz Okta.
   1. En el menú, haga clic en **Aplicaciones** > **Aplicaciones**.

   1. Haga clic en la aplicación de Workfront que ha creado, tal como se describe en la sección, [Crear una aplicación de Workfront en Okta](#create-a-workfront-app-in-okta)
   1. En el **Iniciar sesión** pestaña, haga clic en **Metadatos del proveedor de identidad**.

      ![idp_okta_metadata.png](assets/idp-okta-metadata.png)

      Los metadatos se abren como XML en una nueva pestaña del explorador.

   1. Copie la dirección URL que se muestra en el campo URL del explorador.

1. Inicie sesión en Workfront como administrador de Workfront.
1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Sistema** > **Inicio de sesión único (SSO)**.

1. (Condicional) Si ve dos pestañas, haga clic en el **Nuevos proveedores de SSO** pestaña.

   ![sso_idp_halflife.png](assets/sso-idp-halflife-350x234.png)

   >[!IMPORTANT]
   >
   >No elimine los ajustes de configuración de SSO existentes en **Proveedor de SSO actual** hasta que su cuenta se actualice a la experiencia de autenticación mejorada y la nueva configuración de SSO funcione por completo.

1. Clic **Nuevo proveedor de SSO**.
1. Especifique un nombre, como Okta IDP, y después especifique una descripción.
1. En el **Rellenar campos a partir de metadatos del proveedor de identidad** , pegue la dirección URL que copió en el paso 1 en la sección **URL de metadatos** field.\
   También puede hacer clic en **Elegir archivo** para cargar un archivo .xml, pero le recomendamos que pegue la dirección URL.

1. En el **Asignar atributos de usuario** , en la sección **Atributo de directorio** campo, tipo **email**. (**Correo electrónico** ya se ha rellenado en **Atributo de usuario de Workfront** field.)

1. (Opcional) Habilitar **Establecer el proveedor de SSO predeterminado** para enviar usuarios no autenticados a la pantalla de inicio de sesión del proveedor de identidad en lugar de a la pantalla de inicio de sesión de Workfront para la autenticación. Se recomienda habilitar esta opción solo si todos los usuarios del sistema acceden a Workfront a través del proveedor de identidad.
1. Seleccione el **Activar** casilla de verificación Antes de hacerlo, asegúrese de que los usuarios del sistema conozcan la nueva experiencia de inicio de sesión para garantizar que no pierdan el acceso al sistema de Workfront.
1. Clic **Probar conexión**.\
   Debería ver un mensaje que le indica que la conexión se ha realizado correctamente.

1. Haga clic en **Guardar**.

## Uso de otros proveedores de identidad

Cuando utilice proveedores de identidad distintos de Okta (como Ping o Centrify), debe volver a cargar los metadatos de Workfront en su proveedor de identidad.
