---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: Inicio de sesión único en  [!DNL Workfront Proof]
description: El inicio de sesión único (SSO) permite que sus usuarios inicien sesión en  [!DNL Workfront Proof] usando el nombre de usuario y la contraseña existentes en su organización.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb1f6883-6209-4a55-b181-67af4b496ca0
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# Inicio de sesión único en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], vea [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Se requiere un plan [!UICONTROL Enterprise] [!DNL Workfront] para usar esta característica. Para obtener más información sobre los diversos planes disponibles, consulte [Planes de Workfront](https://www.workfront.com/plans).

El inicio de sesión único (SSO) permite que sus usuarios inicien sesión en [!DNL Workfront Proof] con el nombre de usuario y la contraseña existentes en su organización.

Para proporcionar esta capacidad, utilizamos [!DNL Security Assertion Markup Language] (SAML) 2.0, un protocolo basado en XML que le permite autorizar datos e intercambiar autenticación entre un proveedor de identidad y un servicio web.

Esto significa que autenticará su propio sistema de inicio de sesión, no la página de inicio de sesión de [!DNL Workfront Proof].

Debe tener un dominio o subdominios personalizados configurados en su cuenta de [!DNL Workfront] Proof para habilitar SAML:

<!--* Custom sub-domains are free to set up. See our [Configure a branded domain in Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/configure-branded-domain-in-wp.md) for more information.-->
* Puede leer más sobre los dominios totalmente personalizados en [Marca el sitio [!DNL Workfront Proof] avanzado](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

Consulte [Configurar el inicio de sesión único para [!DNL Workfront Proof] usuarios](../../../workfront-proof/wp-acct-admin/account-settings/configure-sso-for-wp-users.md) para obtener información sobre cómo configurar el SSO en su cuenta.
