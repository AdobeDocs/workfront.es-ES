---
title: Actualizar los metadatos de SAML 2.0 en su IDP al utilizar la autenticación mejorada
description: Como administrador de Adobe Workfront, puede integrar el inicio de sesión único (SSO) de Workfront con cualquier proveedor de identidad que admita el protocolo Lenguaje de marcado de aserción de seguridad (SAML) 2.0.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 55d7d8a8-0dfe-45bc-a23a-47111347e9ca
source-git-commit: b6fc4775953e47a1b9d84d7537a6d9f5d35b1f2c
workflow-type: tm+mt
source-wordcount: '935'
ht-degree: 0%

---

# Actualizar los metadatos de SAML 2.0 en su IDP al utilizar la autenticación mejorada

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Como administrador de Adobe Workfront, puede integrar el inicio de sesión único (SSO) de Workfront con cualquier proveedor de identidad que admita el protocolo Lenguaje de marcado de aserción de seguridad (SAML) 2.0.

Las secciones siguientes describen el proceso de integración cuando su cuenta de Workfront se ha actualizado a la experiencia de autenticación mejorada (aún no disponible para todas las organizaciones). Para obtener más información sobre la experiencia de autenticación mejorada, consulte [Resumen de autenticación mejorada](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md).

Para obtener información sobre la configuración de SAML antes de la migración a la experiencia de autenticación mejorada, consulte [Actualización de metadatos de SAML 2.0 en su proveedor de identidad](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).


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

## Use Okta como proveedor de identidad

Okta es un ejemplo de un proveedor de identidad que admite SAML 2.0. En esta sección se describe cómo usar Okta como proveedor de identidad. Se necesitarían pasos similares al configurar otro proveedor de identidad que admita SAML 2.0.

>[!NOTE]
>
>Los usuarios se asignan en función de su dirección de correo electrónico. Para iniciar sesión en Workfront con Okta, debe tener un usuario con la misma dirección de correo electrónico (sin distinción de mayúsculas y minúsculas) creada en su cliente de Workfront.

Complete las siguientes secciones para configurar Okta como su proveedor de identidad en Workfront.

* [Creación de una aplicación de Workfront en Okta](#create-a-workfront-app-in-okta)
* [Añadir la instancia de Okta como proveedor de identidad en Workfront](#add-your-okta-instance-as-an-identity-provider-in-workfront)

### Creación de una aplicación de Workfront en Okta {#create-a-workfront-app-in-okta}

1. Inicie sesión en su entorno de Okta.
1. Asegúrese de que **IU clásica** está seleccionado en la esquina superior izquierda de la interfaz de Okta.
1. En el menú , haga clic en **Aplicaciones** > **Aplicaciones**.

1. Haga clic en **Agregar aplicación** y haga clic en **Crear nueva aplicación**.

1. En el **Cuadro de diálogo Crear una nueva integración de aplicación** , seleccione **SAML 2.0** y haga clic en **Crear**.

1. Especifique un nombre para la aplicación de Workfront y haga clic en **Siguiente**.
1. En la página Configuración de SAML que aparece, busque la información necesaria para la página Configuración de SAML:

   1. Sin salir de la pestaña del explorador donde se muestra la interfaz de Okta, abra una pestaña o ventana del explorador independiente.
   1. Especifique la siguiente URL en el explorador:

      `https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata`

   1. En el archivo XML resultante, identifique los valores de **entityID** y **Ubicación**.

      ![sso-okta.png](assets/sso-okta.png)

   1. Copie el valor de la variable **entityID** al portapapeles del sistema. No cierre esta pestaña del explorador.

1. Vuelva a la página Configuración de SAML que abrió en el paso 6.
1. Pegue el valor de la variable **entityID** en el campo **URI de audiencia (ID de entidad de SP)** campo .

1. En el archivo XML de la otra pestaña del explorador, copie el valor de la variable **Ubicación** campo .
1. Pegue el valor de la variable **Ubicación** en el campo **Inicio de sesión único** **URL** campo .

1. Desplácese hasta el **Instrucciones de atributo (opcional)** para obtener más información.
1. En el **Nombre** campo, especificar **email**.

1. En el **Valor** campo, especificar **user.email**.

1. (Opcional) Añada cualquier valor avanzado.
1. Haga clic en **Siguiente**.
1. Seleccione, **Soy un cliente de Okta que agrega una aplicación interna** y haga clic en **Finalizar**.

### Añadir la instancia de Okta como proveedor de identidad en Workfront {#add-your-okta-instance-as-an-identity-provider-in-workfront}

Este procedimiento proporciona información esencial para configurar Okta como proveedor de identidad en Workfront. Para obtener información adicional sobre otras asignaciones u opciones de configuración, consulte [Configuración de Adobe Workfront con SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

1. Descargue los metadatos del proveedor de identidad para su instancia de Okta:

   1. Inicie sesión en su entorno de Okta.
   1. Asegúrese de que **IU clásica** está seleccionado en la esquina superior izquierda de la interfaz de Okta.
   1. En el menú , haga clic en **Aplicaciones** > **Aplicaciones**.

   1. Haga clic en la aplicación de Workfront que ha creado, tal como se describe en la sección , [Creación de una aplicación de Workfront en Okta](#create-a-workfront-app-in-okta)
   1. En el **Iniciar sesión** , haga clic en **Metadatos del proveedor de identidad**.

      ![idp_okta_metadata.png](assets/idp-okta-metadata.png)

      Los metadatos se abren como XML en una nueva pestaña del explorador.

   1. Copie la dirección URL que se muestra en el campo URL del explorador .

1. Inicie sesión en Workfront como administrador de Workfront.
1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Sistema** > **Inicio de sesión único (SSO)**.

1. (Condicional) Si ve dos pestañas, haga clic en el botón **Nuevos proveedores de SSO** pestaña .

   ![sso_idp_halflife.png](assets/sso-idp-halflife-350x234.png)

   >[!IMPORTANT]
   >
   >No elimine los ajustes de configuración de SSO existentes en la sección **Proveedor de SSO actual** hasta que su cuenta se actualice a la experiencia de autenticación mejorada y la nueva configuración de SSO funcione completamente.

1. Haga clic en **Nuevo proveedor de SSO**.
1. Especifique un nombre, como IDP de Okta, y después una descripción.
1. En el **Rellenar campos de los metadatos del proveedor de identidad** , pegue la dirección URL que ha copiado en el paso 1 en la sección **Dirección URL de metadatos** campo .\
   También puede hacer clic en **Elegir archivo** para cargar un archivo .xml, pero le recomendamos que pegue la dirección URL.

1. En el **Asignar atributos de usuario** en la sección **Atributo de directorio** campo, tipo **email**. (**Dirección de correo electrónico** ya se rellena en la variable **Atributo de usuario de Workfront** ).

1. (Opcional) Active **Crear proveedor SSO predeterminado** para enviar usuarios no autenticados a la pantalla de inicio de sesión del proveedor de identidad en lugar de a la pantalla de inicio de sesión de Workfront para la autenticación. Le recomendamos que habilite esta opción solo si todos los usuarios del sistema acceden a Workfront a través del proveedor de identidad.
1. Seleccione el **Habilitar** casilla de verificación. Antes de hacerlo, asegúrese de que los usuarios del sistema estén al tanto de la nueva experiencia de inicio de sesión para asegurarse de que no pierdan acceso al sistema de Workfront.
1. Haga clic en **Probar conexión**.\
   Debería ver un mensaje que indica que la conexión se ha realizado correctamente.

1. Haga clic en **Guardar**.

## Uso de otros proveedores de identidad

Cuando utilice proveedores de identidad que no sean Okta (como Ping o Centrify), debe volver a cargar los metadatos de Workfront en su proveedor de identidad.
