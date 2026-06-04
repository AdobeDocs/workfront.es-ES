---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Error de inicio de sesión: Los siguientes campos no son válidos: emailAddress no puede ser nulo'
description: Cuando intento iniciar sesión en [!DNL Adobe Workfront] la dirección URL de mi dominio, se me redirige al portal de inicio de sesión de SAML y después a [!DNL Workfront] con un error que indica que el campo emailAddr no puede ser nulo.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
TQID: https://experienceleague.adobe.com/MfWVOYcQAVjlbxwiqVaPwipyq5ulv0toajH-2tX7c9k
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 146
ht-degree: 4%

---

# Error de inicio de sesión: Los siguientes campos no son válidos: emailAddress no puede ser nulo

## Problema

Cuando intento iniciar sesión en [!DNL Adobe Workfront] con mi dirección URL (https://customerdomain.my.workfront.com), se me redirige al portal de inicio de sesión de SAML y después a [!DNL Workfront] con el siguiente error:

“Intentémoslo de nuevo. Los siguientes campos no son válidos: emailAddress no puede ser nulo&quot;.

## Causa

Este error se debe a un elemento incorrecto en el área Asignar atributos de usuario de la configuración de SAML 2.0. Para obtener más información sobre la asignación de atributos de usuario para SAML 2.0, consulte [Configuración de Adobe Workfront con SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## Solución

Actualice la asignación de atributos para la dirección de correo electrónico y haga clic en **[!UICONTROL Guardar]**.
