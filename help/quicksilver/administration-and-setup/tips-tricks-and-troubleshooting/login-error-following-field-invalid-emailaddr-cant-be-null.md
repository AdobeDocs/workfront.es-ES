---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Error de inicio de sesión: Los siguientes campos no son válidos: emailAddress no puede ser nulo"
description: Cuando intento iniciar sesión en [!DNL Adobe Workfront] la dirección URL de mi dominio, se me redirige al portal de inicio de sesión de SAML y después a [!DNL Workfront] con un error que indica que el campo emailAddr no puede ser nulo.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 2%

---

# Error de inicio de sesión: Los siguientes campos no son válidos: emailAddress no puede ser nulo

## Problema

Cuando intento iniciar sesión en [!DNL Adobe Workfront] con mi dirección URL (https://customerdomain.my.workfront.com), se me redirige al portal de inicio de sesión de SAML y después a [!DNL Workfront] con el siguiente error:

“Intentémoslo de nuevo. Los siguientes campos no son válidos: emailAddress no puede ser nulo&quot;.

## Causa

Este error se debe a un elemento incorrecto en el área Asignar atributos de usuario de la configuración de SAML 2.0. Para obtener más información sobre la asignación de atributos de usuario para SAML 2.0, consulte [Configuración de Adobe Workfront con SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## Solución

Actualice la asignación de atributos para la dirección de correo electrónico y haga clic en **[!UICONTROL Guardar]**.
