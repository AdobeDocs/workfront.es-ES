---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Credenciales de usuario de Adobe Workfront frente a  [!DNL SAML] credenciales de usuario
description: Después de la creación del usuario, puede editarlo y habilitar "Permitir solo la autenticación SAML 2.0" para que su usuario y contraseña estén controlados por el sistema SAML. Con esta opción habilitada, el usuario solo puede iniciar sesión mediante SAML. Cuando van a la  [!DNL Workfront] URL, se les redirige automáticamente al sistema SAML y se les pide su nombre de usuario y contraseña SAML.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# Credenciales de usuario de Adobe Workfront frente a credenciales de usuario de SAML

Este artículo se centra específicamente en [!DNL Adobe Workfront] y SAML y no cubre otros métodos de autenticación SSO.

En una base de datos, [!DNL Workfront] almacena la dirección de correo electrónico de cada usuario como su nombre de usuario [!DNL Workfront], junto con su contraseña [!DNL Workfront]. Estas credenciales se replican en los entornos limitados de Vista previa y Actualización personalizada.

Durante la creación del usuario, si [!DNL Workfront] detecta que SAML 2.0 está configurado, el valor predeterminado será &quot;Permitir solo la autenticación SAML 2.0&quot; para el usuario. Si el cuadro &quot;Enviar un correo electrónico de invitación a esta persona&quot; está habilitado, [!DNL Workfront] deshabilita &quot;Permitir solo la autenticación SAML 2.0&quot; y oculta esta opción. Una vez habilitado &quot;Enviar un correo electrónico de invitación a esta persona&quot;, el usuario se convierte en un usuario [!DNL Workfront] que no es de SAML.

Después de la creación del usuario, puede editarlo y habilitar **[!UICONTROL Permitir solo la autenticación SAML 2.0]** para que el sistema SAML controle el usuario y la contraseña.

Una vez hecho esto, el usuario solo puede iniciar sesión mediante SAML. Cuando van a la dirección URL [!DNL Workfront], se les redirige automáticamente al sistema SAML y se les solicita su nombre de usuario y contraseña SAML.

Las credenciales de SAML se almacenan en un sistema SAML externo, como el ADFS de Microsoft, no en Workfront.
