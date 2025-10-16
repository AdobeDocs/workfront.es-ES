---
title: Actualización de metadatos de SAML 2.0 en el IDP al utilizar autenticación mejorada
description: Como administrador de Adobe Workfront, puede integrar el inicio de sesión único (SSO) de Workfront con cualquier proveedor de identidad que admita el protocolo SAML (Security Assertion Markup Language) 2.0.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 55d7d8a8-0dfe-45bc-a23a-47111347e9ca
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 75fea812b4574191522af4721a013b57aa5d609f
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 98%

---

# Actualización de metadatos de SAML 2.0 en el IDP al utilizar la autenticación mejorada

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Como administrador de Adobe Workfront, puede integrar el inicio de sesión único (SSO) de Workfront con cualquier proveedor de identidad que admita el protocolo SAML (Security Assertion Markup Language) 2.0.

En las secciones siguientes se describe el proceso de integración cuando su cuenta de Workfront se ha actualizado a la experiencia de autenticación mejorada (aún no disponible para todas las organizaciones). Para obtener más información acerca de la experiencia de autenticación mejorada, consulte [Información general sobre la autenticación mejorada](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md).

Para obtener información sobre cómo configurar SAML antes de migrar a la experiencia de autenticación mejorada, consulte [Actualizar metadatos de SAML 2.0 en su proveedor de identidad](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).


## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Uso de Okta como proveedor de identidad

Okta es un ejemplo de proveedor de identidad compatible con SAML 2.0. En esta sección se describe cómo utilizar Okta como proveedor de identidad. Se requerirían pasos similares al configurar otro proveedor de identidad que admita SAML 2.0.

>[!NOTE]
>
>Los usuarios se asignan en función de su dirección de correo electrónico. Para iniciar sesión en Workfront con Okta, debe tener un usuario con la misma dirección de correo electrónico (sin distinción de mayúsculas y minúsculas) creado en su cliente de Workfront.

Complete las siguientes secciones para configurar Okta como su proveedor de identidad en Workfront.

* [Creación de una aplicación de Workfront en Okta](#create-a-workfront-app-in-okta)
* [Añadir la instancia de Okta como proveedor de identidad en Workfront](#add-your-okta-instance-as-an-identity-provider-in-workfront)

### Crear una aplicación de Workfront en Okta {#create-a-workfront-app-in-okta}

1. Inicie sesión en su entorno de Okta.
1. Asegúrese de que **IU clásica** esté seleccionada en la esquina superior izquierda de la interfaz de Okta.
1. En el menú, haga clic en **Aplicaciones** > **Aplicaciones**.

1. Haga clic en **Añadir aplicación** y, a continuación, haga clic en **Crear nueva aplicación**.

1. En el cuadro de diálogo **Crear una nueva integración de aplicación**, seleccione **SAML 2.0** y, a continuación, haga clic en **Crear**.

1. Especifique un nombre para la aplicación de Workfront y haga clic en **Siguiente**.
1. En la página Configuración de SAML que aparece, busque la información necesaria para la página Configuración de SAML:

   1. Sin salir de la pestaña del explorador donde se muestra la interfaz de Okta, abra una pestaña o ventana independiente del explorador.
   1. Especifique la siguiente URL en el explorador:

      `https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata`

   1. En el archivo XML resultante, identifique los valores de **entityID** y **Location**.

      ![sso-okta.png](assets/sso-okta.png)

   1. Copie el valor del campo **entityID** al portapapeles del sistema. No cierre esta pestaña del explorador.

1. Vuelva a la página Configuración de SAML que abrió en el paso 6.
1. Pegue el valor del campo **entityID** en el campo **URI de público (ID de entidad de SP)**.

1. En el archivo XML de la pestaña del otro explorador, copie el valor del campo **Location**.
1. Pegue el valor del campo **Location** en el campo **URL de** **inicio único de sesión**.

1. Desplácese hasta la sección **Instrucciones de atributo (opcional)**.
1. En el campo **Nombre**, especifique **email**.

1. En el campo **Valor**, especifique **user.email**.

1. (Opcional) Añada cualquier valor avanzado.
1. Haga clic en **Siguiente**.
1. Seleccione **Soy cliente de Okta y quiero añadir una aplicación interna** y luego haga clic en **Finalizar**.

### Añadir la instancia de Okta como proveedor de identidad en Workfront {#add-your-okta-instance-as-an-identity-provider-in-workfront}

Este procedimiento proporciona información esencial para configurar Okta como el proveedor de identidad en Workfront. Para obtener información adicional sobre otras asignaciones u opciones de configuración, consulte [Configuración de Adobe Workfront con SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

1. Descargue los metadatos del proveedor de identidad para su instancia de Okta:

   1. Inicie sesión en su entorno de Okta.
   1. Asegúrese de que **IU clásica** esté seleccionada en la esquina superior izquierda de la interfaz de Okta.
   1. En el menú, haga clic en **Aplicaciones** > **Aplicaciones**.

   1. Haga clic en la aplicación de Workfront que creó, tal como se describe en la sección [Crear una aplicación de Workfront en Okta](#create-a-workfront-app-in-okta)
   1. En la pestaña **Inicio de sesión**, haga clic en **Metadatos del proveedor de identidad**.

      ![idp_okta_metadata.png](assets/idp-okta-metadata.png)

      Los metadatos se abren como XML en una nueva pestaña del explorador.

   1. Copie la dirección URL que se muestra en el campo URL del explorador.

1. Inicie sesión en Workfront como administrador de Workfront.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Sistema** > **Inicio de sesión único (SSO)**.

1. (Condicional) Si ve dos pestañas, haga clic en la pestaña **Nuevos proveedores de SSO**.

   ![sso_idp_halflife.png](assets/sso-idp-halflife-350x234.png)

   >[!IMPORTANT]
   >
   >No elimine las opciones de configuración de SSO existentes en la pestaña **Proveedor de SSO actual** hasta que su cuenta se actualice a la experiencia de autenticación mejorada y la nueva configuración de SSO funcione por completo.

1. Haga clic en **Nuevo proveedor de SSO**.
1. Especifique un nombre, como Okta IDP, y después especifique una descripción.
1. En la sección **Rellenar campos a partir de los metadatos del proveedor de identidad**, pegue la dirección URL que copió en el paso 1, en el campo **URL de metadatos**.\
   También puede hacer clic en **Elegir archivo** para cargar un archivo .xml, pero le recomendamos que pegue la dirección URL.

1. En la sección **Asignar atributos de usuario**, en el campo **Atributo de directorio**, escriba **correo electrónico**. (**La dirección de correo electrónico** ya se ha rellenado en el campo **Atributo de usuario de Workfront**).

1. (Opcional) Habilite **Establecer el proveedor de SSO predeterminado** para enviar usuarios no autenticados a la pantalla de inicio de sesión del proveedor de identidad en lugar de a la pantalla de inicio de sesión de Workfront para la autenticación. Se recomienda habilitar esta opción solo si todos los usuarios de su sistema acceden a Workfront a través del proveedor de identidad.
1. Seleccione la casilla de verificación **Habilitar**. Antes de hacerlo, asegúrese de que los usuarios del sistema conozcan la nueva experiencia de inicio de sesión para garantizar que no pierden el acceso al sistema de Workfront.
1. Haga clic en **Probar conexión**.\
   Debería ver un mensaje que le indica que la conexión se ha realizado correctamente.

1. Haga clic en **Guardar**.

## Uso de otros proveedores de identidad

Si utilice proveedores de identidad distintos de Okta (como Ping o Centrify), debe volver a cargar los metadatos de Workfront en su proveedor de identidad.
