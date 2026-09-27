---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: La configuración de ZScaler puede reducir el rendimiento
description: Después de la creación del usuario, puede editarlo y habilitar “Permitir solo la autenticación SAML 2.0” para que su usuario y contraseña estén controlados por el sistema SAML. Con esta opción habilitada, el usuario solo puede iniciar sesión mediante SAML.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 2752a9e2-44fe-49b5-a7ab-4021d91ed37b
TQID: 'https://experienceleague.adobe.com/-3-p8fzXIiV-gnjIjhRzBmLfspAEEVAuD2lpmcsVjLA'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 70%
---
# Workfront: la configuración de ZScaler puede reducir el rendimiento

>[!NOTE]
>
>Es un problema de ZScaler y Workfront no lo solucionará.

El servicio web de ZScaler usa `http/1.1` de forma predeterminada, lo que puede reducir el rendimiento en Workfront.

Para comprobar y resolver este problema, configure el software ZScaler para que use `http/2`. Esto no se puede configurar en Workfront.

Puede encontrar información sobre `http/2` en la documentación de ZScaler.
