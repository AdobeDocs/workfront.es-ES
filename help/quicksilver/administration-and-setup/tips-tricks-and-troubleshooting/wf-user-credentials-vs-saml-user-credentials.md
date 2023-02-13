---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Credenciales de usuario de Adobe Workfront vs. [!DNL SAML] credenciales de usuario
description: Después de la creación del usuario, puede editar el usuario y habilitar "Permitir sólo la autenticación SAML 2.0" para que su usuario y contraseña estén controlados por el sistema SAML. Con esta opción habilitada, el usuario solo puede iniciar sesión mediante SAML. Cuando vayan al [!DNL Workfront] URL, se redirigen automáticamente al sistema SAML y se les pide su nombre de usuario y contraseña de SAML.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Credenciales de usuario de Adobe Workfront frente a credenciales de usuario de SAML

Este artículo se centra específicamente en [!DNL Adobe Workfront] y SAML y no cubre otros métodos de autenticación SSO.

En una base de datos, [!DNL Workfront] almacena la dirección de correo electrónico de cada usuario como su [!DNL Workfront] nombre de usuario, junto con su [!DNL Workfront] contraseña. Estas credenciales se replican en los entornos limitados de vista previa y actualización personalizada.

Durante la creación del usuario, si [!DNL Workfront] detecta que SAML 2.0 está configurado, el valor predeterminado es &quot;Permitir autenticación SAML 2.0 solamente&quot; para el usuario. Si la casilla &quot;Enviar un correo electrónico de invitación a esta persona&quot; está activada, [!DNL Workfront] deshabilita &quot;Permitir solo autenticación SAML 2.0&quot; y oculta esta opción. Una vez habilitado &quot;Enviar un correo electrónico de invitación a esta persona&quot;, el usuario se convierte en un usuario que no es SAML [!DNL Workfront] usuario.

Tras la creación del usuario, puede editar y habilitar **[!UICONTROL Permitir solo la autenticación SAML 2.0]** para que su usuario y contraseña estén controlados por el sistema SAML.

Con esto hecho, el usuario solo puede iniciar sesión a través de SAML. Cuando vayan al [!DNL Workfront] URL, se redirigen automáticamente al sistema SAML y se les pide su nombre de usuario y contraseña de SAML.

Las credenciales de SAML se almacenan en un sistema SAML externo, como ADFS de Microsoft, no en Workfront.
