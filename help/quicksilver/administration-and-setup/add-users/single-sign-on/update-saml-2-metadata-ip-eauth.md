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
source-git-commit: fab7a3a1c66635b11418a216999dee84a30a50bb
workflow-type: tm+mt
source-wordcount: '938'
ht-degree: 0%

---

# Actualización de metadatos de SAML 2.0 en el IDP al utilizar autenticación mejorada

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Como administrador de Adobe Workfront, puede integrar el inicio de sesión único (SSO) de Workfront con cualquier proveedor de identidad que admita el protocolo SAML (Security Assertion Markup Language) 2.0.

En las secciones siguientes se describe el proceso de integración cuando su cuenta de Workfront se ha actualizado a la experiencia de autenticación mejorada (aún no disponible para todas las organizaciones). Para obtener más información acerca de la experiencia de autenticación mejorada, consulte [Descripción general de la autenticación mejorada](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md).

Para obtener información sobre cómo configurar SAML antes de migrar a la experiencia de autenticación mejorada, consulte [Actualizar metadatos de SAML 2.0 en su proveedor de identidad](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).


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
1. Asegúrese de que **IU clásica** esté seleccionada en la esquina superior izquierda de la interfaz de Okta.
1. En el menú, haga clic en **Aplicaciones** > **Aplicaciones**.

1. Haga clic en **Agregar aplicación** y, a continuación, haga clic en **Crear nueva aplicación**.

1. En el cuadro de diálogo **Crear una nueva integración de aplicación**, seleccione **SAML 2.0** y, a continuación, haga clic en **Crear**.

1. Especifique un nombre para la aplicación de Workfront y haga clic en **Siguiente**.
1. En la página Configuración de SAML que aparece, busque la información necesaria para la página Configuración de SAML:

   1. Sin salir de la pestaña del explorador donde se muestra la interfaz Okta, abra una pestaña o ventana independiente del explorador.
   1. Especifique la siguiente URL en el explorador:

      `https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata`

   1. En el archivo XML resultante, identifique los valores de **entityID** y **Location**.

      ![sso-okta.png](assets/sso-okta.png)

   1. Copie el valor del campo **entityID** al portapapeles del sistema. No cierre esta pestaña del explorador.

1. Vuelva a la página Configuración de SAML que abrió en el paso 6.
1. Pegue el valor del campo **entityID** en el campo **URI de audiencia (ID de entidad de SP)**.

1. En el archivo XML de la ficha del otro explorador, copie el valor del campo **Ubicación**.
1. Pegue el valor del campo **Location** en el campo **Single sign on** **URL**.

1. Desplácese hasta la sección **Instrucciones de atributo (opcional)**.
1. En el campo **Nombre**, especifique **correo electrónico**.

1. En el campo **Value**, especifique **user.email**.

1. (Opcional) Añada cualquier valor avanzado.
1. Haga clic en **Siguiente**.
1. Seleccione **Soy cliente de Okta que agrega una aplicación interna** y luego haga clic en **Finalizar**.

### Añada la instancia de Okta como proveedor de identidad en Workfront {#add-your-okta-instance-as-an-identity-provider-in-workfront}

Este procedimiento proporciona información esencial para configurar Okta como proveedor de identidad en Workfront. Para obtener información adicional sobre otras asignaciones u opciones de configuración, consulte [Configuración de Adobe Workfront con SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

1. Descargue los metadatos del proveedor de identidad para su instancia de Okta:

   1. Inicie sesión en su entorno de Okta.
   1. Asegúrese de que **IU clásica** esté seleccionada en la esquina superior izquierda de la interfaz de Okta.
   1. En el menú, haga clic en **Aplicaciones** > **Aplicaciones**.

   1. Haga clic en la aplicación Workfront que creó, tal como se describe en la sección [Crear una aplicación Workfront en Okta](#create-a-workfront-app-in-okta)
   1. En la ficha **Iniciar sesión**, haga clic en **Metadatos del proveedor de identidad**.

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
   >No elimine las opciones de configuración de SSO existentes en la ficha **Proveedor de SSO actual** hasta que su cuenta se actualice a la experiencia de autenticación mejorada y la nueva configuración de SSO funcione por completo.

1. Haga clic en **Nuevo proveedor de SSO**.
1. Especifique un nombre, como Okta IDP, y después especifique una descripción.
1. En la sección **Rellenar campos a partir de metadatos del proveedor de identidad**, pegue la dirección URL que copió en el paso 1 en el campo **URL de metadatos**.\
   También puede hacer clic en **Elegir archivo** para cargar un archivo .xml, pero le recomendamos que pegue la dirección URL.

1. En la sección **Asignar atributos de usuario**, en el campo **Atributo de directorio**, escriba **correo electrónico**. (**La dirección de correo electrónico** ya se ha rellenado en el campo **Atributo de usuario de Workfront**).

1. (Opcional) Habilite **Establecer proveedor de SSO predeterminado** para enviar usuarios no autenticados a la pantalla de inicio de sesión del proveedor de identidad en lugar de a la pantalla de inicio de sesión de Workfront para la autenticación. Se recomienda habilitar esta opción solo si todos los usuarios del sistema acceden a Workfront a través del proveedor de identidad.
1. Seleccione la casilla de verificación **Habilitar**. Antes de hacerlo, asegúrese de que los usuarios del sistema conozcan la nueva experiencia de inicio de sesión para garantizar que no pierdan el acceso al sistema de Workfront.
1. Haga clic en **Probar conexión**.\
   Debería ver un mensaje que le indica que la conexión se ha realizado correctamente.

1. Haga clic en **Guardar**.

## Uso de otros proveedores de identidad

Cuando utilice proveedores de identidad distintos de Okta (como Ping o Centrify), debe volver a cargar los metadatos de Workfront en su proveedor de identidad.
