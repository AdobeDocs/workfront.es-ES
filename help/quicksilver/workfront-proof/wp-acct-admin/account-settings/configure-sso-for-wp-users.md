---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: 'Configurar el inicio de sesión único para los usuarios de  [!DNL Workfront Proof] '
description: Si tiene el plan Select o Premium, puede proporcionar la capacidad de inicio de sesión único (SSO), que le permite usar el nombre de usuario y la contraseña existentes de su organización para acceder a su cuenta de  [!DNL Workfront Proof] .
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 52ac1919-1821-424f-89f8-72865b236e4e
source-git-commit: 74a877145b55ccc14b4d5aefd1889919a39e1f20
workflow-type: tm+mt
source-wordcount: '1225'
ht-degree: 100%

---

# Configurar el inicio de sesión único para los usuarios de [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Si tiene el plan Select o Premium, puede proporcionar la capacidad de inicio de sesión único (SSO), que le permite usar el nombre de usuario y la contraseña existentes de su organización para acceder a su cuenta de [!DNL Workfront Proof].

Esto significa que se autenticará con su propio sistema de inicio de sesión, no con la página de inicio de sesión de [!DNL Workfront Proof].

>[!NOTE]
>
>Debe tener un subdominio o dominio personalizado configurado en su cuenta de [!DNL Workfront Proof] para habilitar SAML. Los subdominios personalizados se pueden configurar gratuitamente. Consulte [Personalización de marca](https://support.workfront.com/hc/en-us/sections/115000921208-Branding) para obtener más información. Puede leer más sobre los dominios totalmente personalizados en [Personalizar la marca del sitio de  [!DNL Workfront Proof]  - configuración avanzada](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

## Habilitación del SSO en [!DNL Workfront Proof]

La funcionalidad de inicio de sesión único se puede habilitar en la pestaña [!UICONTROL Inicio de sesión único] de [!UICONTROL Configuración de la cuenta] y se aplicará a todos los usuarios de la cuenta de [!DNL Workfront Proof]. Consulte [Configuración de la cuenta](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) para obtener más información.

## ID de entidad

Como proveedor de servicio, hemos publicado nuestro ID de entidad aquí:

[https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq](https://yoursubdomain.proofhq.com/saml/module.php/saml/sp/metadata.php/phq) (en que “yoursubdomain” es el subdominio de la cuenta)

[!DNL Workfront Proof] requiere la dirección de correo electrónico del usuario como identificador único, que se puede transferir como uno de los atributos siguientes:

* urn:mace:dir:attribute-def:emailAddress
* http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress
* http://schemas.xmlsoap.org/claims/EmailAddress
* urn:oid:0.9.2342.19200300.100.1.3
* http://axschema.org/contact/email
* openid.sreg.email
* mail
* email
* emailAddress

Para configurar el SSO:

1. Abra la pestaña **[!UICONTROL Inicio de sesión único]** (1).
1. Introduzca la **URL de SSO** (2).
Es el vínculo al servidor SSO (por ejemplo, **https://sso.mycompany.com/opensso**).

1. Introduzca la **URL de inicio de sesión** (3).
Es la URL que se invocará para redirigir a los usuarios al proveedor de identidad.

   No se trata de una URL real que se introduzca en el explorador, sino de un punto final que procesará la información que le enviemos para presentar la pantalla de inicio de sesión.

1. Introduzca la **URL de cierre de sesión** (4).
Es la URL a la que volverá tras cerrar la sesión, por ejemplo

   **https://www.yourcompany.com/services/logout.asp**

1. Introduzca la **huella digital del certificado** (5).
1. Es la huella digital SHA1 del certificado SAML proporcionado por su proveedor de identidad SAML.
1. Asegúrese de incluir la información de clave estableciéndola en el proveedor de identidad.
1. Cambie **SSO** a **[!UICONTROL Habilitado]** (6).
Una vez habilitado el SSO, usted y todos los usuarios de su cuenta iniciarán sesión mediante su propio mecanismo de autenticación. Esto significa que cuando los usuarios accedan a la pantalla de inicio de sesión de su cuenta de [!DNL Workfront Proof] (por ejemplo, **yourcompany.proofhq.com/login**), se les indicará la ventana de transferencia a su propia página de inicio de sesión de autenticación.

1. (Opcional) Habilite **Aprovisionar usuarios automáticamente** (7).
Una vez habilitada esta opción, se crearán automáticamente cuentas de usuario para las personas que no tengan sus propios perfiles de [!DNL Workfront Proof], pero accederán a su cuenta de [!DNL Workfront Proof] mediante sus credenciales de inicio de sesión único. Esto solo se llevará a cabo cuando aún no se haya alcanzado el límite de usuarios en su cuenta.

1. Los nuevos usuarios aprovisionados tendrán los permisos del perfil Admimistrador asignados de forma predeterminada. Si necesita más información, consulte [Perfiles de permisos de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

![Enable_SSO_SAML_2.0.png](assets/enable-sso-saml-2.0-350x236.png)

## Habilitación de SSO para cuentas satélite

Cuando tenga cuentas satélite conectadas a su cuenta central, puede administrarlas desde el nivel de cuenta central.

El inicio de sesión único es una características de Select y Premium, por lo que el inicio de sesión único solo se puede habilitar en satélites que tengan planes Select y Premium.

1. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la cuenta]** (1).

1. Haga clic en la cuenta satélite en el menú desplegable (2).
1. Abra la pestaña **[!UICONTROL Inicio de sesión único]** (3).
1. Comience a editar la configuración de SSO (4).
1. ![Enabling_SSO_-_Satellite_Account.png](assets/enabling-sso---satellite-account-350x266.png)
Aquí tiene dos métodos (5) de configuración:

1. **Heredado:** SSO con la configuración tomada de su cuenta central.
Si un usuario accede a [!DNL Workfront Proof] a través de la **página de inicio de sesión predeterminada** ([https://www.proofhq.com/login](https://www.proofhq.com/login)), habrá **dos niveles de autorización**: en primer lugar, se pide al usuario que inicie sesión con los datos de acceso de [!DNL Workfront Proof] (correo electrónico y contraseña); a continuación, se transfiere al usuario a través de una ventana de SSO a la página de inicio de sesión de SSO.
Por lo tanto, con el servicio SSO habilitado, recomendamos iniciar sesión a través de su propio subdominio/dominio de [!DNL Workfront Proof].

   >[!NOTE]
   >
   >En este momento, cuando el inicio de sesión único está habilitado en su cuenta de [!DNL Workfront Proof], no podrá iniciar sesión en la aplicación de iPhone con esas credenciales.

   1. **Manual** (predeterminado): SSO con una configuración diferente (por ejemplo, apuntando a otro proveedor de identidad).

      >[!NOTE]
      >
      >Si la cuenta satélite hereda la configuración de SSO de la cuenta central, la pantalla de inicio de sesión será la de la cuenta central. Cuando el usuario de la cuenta satélite introduce sus datos de inicio de sesión de SSO en esta página, se le redirige a la cuenta satélite.

      ![Enabling_SSO_-_Satellite_Account_2.png](assets/enabling-sso---satellite-account-2-350x224.png)

   1. Haga clic en **[!UICONTROL Guardar]** (6).

## Configuración de SSO heredada de una cuenta central

Cuando elija heredar la configuración de su cuenta central, verá que todos los campos se rellenan ahora con los datos de su cuenta central (7) y que el inicio de sesión único se habilita o deshabilita automáticamente (8) como en su cuenta principal. Además, ya no hay vínculos de edición en los campos, ya que toda la configuración de SSO de la cuenta satélite ahora se establece y administra desde la cuenta central.

![Satellite_Account_-_Inherited_SSO.png](assets/satellite-account---inherited-sso-350x99.png)

En su cuenta central (9), el campo [!UICONTROL Uso de SSO] muestra que esta configuración la utilizan las cuentas satélite (10).\
![Hub_Account_-_Inherited_SSO.png](assets/hub-account---inherited-sso-350x275.png)

## SSO configurado manualmente

Si se ha elegido la configuración de SSO manual para una cuenta satélite (1), debe introducir manualmente los datos del inicio de sesión único.

1. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la cuenta]** (1).

1. Abra la pestaña **[!UICONTROL Inicio de sesión único]**.
1. Haga clic en **[!UICONTROL Editar],** rellene el campo y, a continuación, haga clic en **[!UICONTROL Guardar]** (2).

1. En la fila **[!UICONTROL SSO]**, haga clic en **[!UICONTROL Habilitado]** (3).

![Satellite_Account_-_Manual_SSO.png](assets/satellite-account---manual-sso-350x280.png)

## Inicio de sesión de SSO

1. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la cuenta]** (1).

1. Abra la pestaña **[!UICONTROL Inicio de sesión único]**.
1. Asegúrese de que el dominio o subdominio de [!DNL Workfront Proof] (1) esté configurado y de que los usuarios accedan a su cuenta de [!DNL Workfront Proof] a través de este dominio o subdominio personalizado.
   ![SAML_Subdomain.png](assets/saml-subdomain-350x150.png)
Con el inicio de sesión único habilitado, la dirección URL de inicio de sesión de subdominio (por ejemplo, yourcompany.proofhq.com/login) muestra una pantalla de transferencia (2) que le lleva directamente a la página de inicio de sesión de SSO.
   ![SSO_login_page.png](assets/sso-login-page-350x164.png)

1. Si un usuario accede a [!DNL Workfront Proof] a través de la **página de inicio de sesión predeterminada** ([https://www.proofhq.com/login](https://www.proofhq.com/login)), habrá **dos niveles de autorización**. Primero se le pide al usuario que inicie sesión usando los datos de acceso de [!DNL Workfront Proof] (correo electrónico y contraseña). A continuación, el usuario se transfiere a través de una ventana de SSO (2) a la página de inicio de sesión de SSO.\
   Por lo tanto, con el servicio SSO habilitado, recomendamos iniciar sesión a través de su propio subdominio/dominio [!DNL Workfront Proof].

1. En este momento, cuando el inicio de sesión único está habilitado en su cuenta de Workfront Proof, no podrá iniciar sesión en la aplicación de iPhone con esas credenciales.

## Acerca de la adición de un nuevo usuario

Cuando la funcionalidad Inicio de sesión único está habilitada en su cuenta de [!DNL Workfront Proof], los nuevos usuarios no recibirán ningún correo electrónico de confirmación, ya que sus cuentas se activarán automáticamente y estarán listas para usar.

Desde la página de inicio de sesión de [!DNL Workfront Proof], después de hacer clic en el botón [!UICONTROL Iniciar sesión], se redirige a los usuarios a la página de inicio de sesión de SSO y se les pide que escriban sus credenciales de inicio de sesión único.

>[!IMPORTANT]
>
>Los usuarios se identifican mediante una dirección de correo electrónico durante el proceso de autenticación, lo que significa que la cuenta de correo electrónico utilizada para su inicio de sesión de SSO debe ser la dirección de correo electrónico del usuario registrado en su cuenta.

## Servicios de federación de Active Directory (ADFS)

Los Servicios de federación de Active Directory (ADFS) son un componente de software de [!DNL Microsoft] que se puede instalar en sistemas operativos Windows Server para proporcionar a los usuarios con acceso de inicio de sesión único a los sistemas y aplicaciones ubicados en los límites de la organización. Para obtener más información, consulte &quot;Servicios de federación de Active Directory&quot; en el sitio web de Microsoft Developer Network.

El sistema [!DNL Workfront Proof] es compatible con SAML 2.0 y solo es compatible con AD FS versión 2.0 o superior.

Consulte [Inicio de sesión único en  [!DNL Workfront Proof]: configuración de AD FS](../../../workfront-proof/wp-acct-admin/account-settings/sso-in-wp-adfs-configuration.md) para obtener instrucciones detalladas.
