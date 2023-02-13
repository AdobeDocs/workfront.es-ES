---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: Inicio de sesión único [!DNL Workfront Proof]
description: Inicio de sesión único (SSO) permite a los usuarios iniciar sesión [!DNL Workfront Proof] uso del nombre de usuario y la contraseña existentes de su organización.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb1f6883-6209-4a55-b181-67af4b496ca0
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# Inicio de sesión único [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

Un [!UICONTROL Empresa] [!DNL Workfront] Se requiere un plan para utilizar esta función. Para obtener más información sobre los distintos planes disponibles, consulte [Planes de Workfront](https://www.workfront.com/plans).

Inicio de sesión único (SSO) permite a los usuarios iniciar sesión [!DNL Workfront Proof] uso del nombre de usuario y la contraseña existentes de su organización.

Para proporcionar esta capacidad, utilizamos [!DNL Security Assertion Markup Language] (SAML) 2.0, un protocolo basado en XML que permite autorizar datos e intercambiar autenticación entre un proveedor de identidad y un servicio web.

Esto significa que se autenticará contra su propio sistema de inicio de sesión, no contra [!DNL Workfront Proof]de inicio de sesión de .

Debe tener configurados subdominios o dominios personalizados en su [!DNL Workfront] Cuenta de prueba para habilitar SAML:

<!--* Custom sub-domains are free to set up. See our [Configure a branded domain in Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/configure-branded-domain-in-wp.md) for more information.-->
* Puede obtener más información sobre los dominios totalmente personalizados en  [Marca la variable [!DNL Workfront Proof] sitio: avanzado](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

Consulte [Configuración del inicio de sesión único para [!DNL Workfront Proof] usuarios](../../../workfront-proof/wp-acct-admin/account-settings/configure-sso-for-wp-users.md) para obtener información sobre la configuración de SSO en su cuenta.
