---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: Inicio de sesión único en [!DNL Workfront Proof]
description: El inicio de sesión único (SSO) permite que sus usuarios inicien sesión en  [!DNL Workfront Proof] usando el nombre de usuario y la contraseña existentes en su organización.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb1f6883-6209-4a55-b181-67af4b496ca0
TQID: https://experienceleague.adobe.com/rQkypJthOpKg1gQBH0tUjtwkbaxLn1k-lrpZj9hCQ5o
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 174
ht-degree: 97%

---

# Inicio de sesión único en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Se requiere un plan de [!UICONTROL empresa] [!DNL Workfront] para utilizar esta característica. Para obtener más información sobre los diversos planes disponibles, consulte [Planes de Workfront](https://business.adobe.com/products/workfront/pricing.html).

El inicio de sesión único (SSO) permite a sus usuarios iniciar sesión en [!DNL Workfront Proof] con el nombre de usuario y la contraseña existentes en su organización.

Para proporcionar esta capacidad, utilizamos [!DNL Security Assertion Markup Language] (SAML) 2.0, un protocolo basado en XML que le permite autorizar datos e intercambiar autenticación entre un proveedor de identidad y un servicio web.

Esto significa que se autenticará en su propio sistema de inicio de sesión, no en la página de inicio de sesión de [!DNL Workfront Proof].

Debe tener un dominio o subdominios personalizados configurados en su cuenta de revisión de [!DNL Workfront] para habilitar SAML:

<!--* Custom sub-domains are free to set up. See our [Configure a branded domain in Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/configure-branded-domain-in-wp.md) for more information.-->
* Puede obtener más información sobre los dominios totalmente personalizados en [Personalización de la marca en el sitio [!DNL Workfront Proof] : avanzado](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md).

Consulte [Configurar el inicio de sesión único para [!DNL Workfront Proof] usuarios](../../../workfront-proof/wp-acct-admin/account-settings/configure-sso-for-wp-users.md) para obtener información sobre cómo configurar el SSO en su cuenta.
