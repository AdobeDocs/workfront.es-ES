---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Credenciales de usuario de Adobe Workfront frente a credenciales de usuario de SAML
description: Después de la creación del usuario, puede editarlo y habilitar “Permitir solo la autenticación SAML 2.0” para que su usuario y contraseña estén controlados por el sistema SAML. Con esta opción habilitada, el usuario solo puede iniciar sesión mediante SAML.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
TQID: https://experienceleague.adobe.com/8paS2GIumamOltxTC8Gw2mBZ4bKB6TOgbly7IBPKhDw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 235
ht-degree: 90%

---

# Credenciales de usuario de Adobe Workfront frente a credenciales de usuario de SAML

Este artículo se centra específicamente en [!DNL Adobe Workfront] y SAML y no cubre otros métodos de autenticación SSO.

En una base de datos, [!DNL Workfront] almacena la dirección de correo electrónico de cada usuario como su nombre de usuario [!DNL Workfront], junto con su contraseña [!DNL Workfront]. Estas credenciales se replican en las zonas protegidas de Vista previa y Actualización personalizada.

Durante la creación del usuario, si [!DNL Workfront] detecta que SAML 2.0 está configurado, el valor predeterminado será “Permitir solo la autenticación SAML 2.0” para el usuario. Si el cuadro “Enviar un correo electrónico de invitación a esta persona” está habilitado, [!DNL Workfront] la opción “Permitir solo la autenticación SAML 2.0” se deshabilita y se oculta. Una vez habilitada la opción “Enviar un correo electrónico de invitación a esta persona”, el usuario se convierte en un usuario [!DNL Workfront] que no es de SAML.

Después de la creación del usuario, puede editarlo y habilitar **[!UICONTROL Permitir solo la autenticación SAML 2.0]** para que el sistema SAML controle el usuario y la contraseña.

Una vez hecho esto, el usuario solo puede iniciar sesión mediante SAML. Cuando los usuarios van a la dirección URL [!DNL Workfront], se les redirige automáticamente al sistema SAML y se les solicita su nombre de usuario y contraseña SAML.

Las credenciales de SAML se almacenan en un sistema SAML externo como el ADFS de Microsoft, no en Workfront.
