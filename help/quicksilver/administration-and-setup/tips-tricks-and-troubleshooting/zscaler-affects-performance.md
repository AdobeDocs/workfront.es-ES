---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: La configuración de ZScaler puede reducir el rendimiento
description: Después de la creación del usuario, puede editarlo y habilitar "Permitir solo la autenticación SAML 2.0" para que su usuario y contraseña estén controlados por el sistema SAML. Con esta opción habilitada, el usuario solo puede iniciar sesión mediante SAML.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 2752a9e2-44fe-49b5-a7ab-4021d91ed37b
source-git-commit: f66b219e9fd203f108844ad397bcfa848b8f1134
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Workfront: La configuración de ZScaler puede reducir el rendimiento

>[!NOTE]
>
>Este es un problema con ZScaler y Workfront no lo solucionará.

El servicio web de ZScaler usa `http/1.1` de forma predeterminada, lo que puede reducir el rendimiento en Workfront.

Para comprobar y resolver este problema, configure el software ZScaler para que use `http/2`. Esto no se puede configurar en Workfront.

Puede encontrar información sobre `http/2` en la documentación de ZScaler.
