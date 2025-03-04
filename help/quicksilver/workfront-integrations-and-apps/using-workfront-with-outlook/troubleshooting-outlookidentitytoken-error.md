---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 'Solución de problemas: error de outlookIdentityToken al usar Workfront para Outlook'
description: Si obtiene un error de outlookIdentityToken al utilizar Workfront para Outlook, debe habilitar los tokens heredados de Microsoft 365 para su organización.
author: Becky
feature: Workfront Integrations and Apps
source-git-commit: 571ed00f44322d73183323c4d4154284cd028301
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# Solución de problemas: error de outlookIdentityToken al usar Workfront para Outlook

Al utilizar Workfront para Outlook, puede ver el siguiente error:

```
Unexpected error
Unable to get the outlookIdentityToken
```

Para resolver este error, debe habilitar los tokens heredados de Microsoft 365 para su organización. Como esto debe hacerse en Microsoft 365, Workfront no puede habilitar estos tokens para su organización.

Para obtener instrucciones sobre cómo habilitar tokens heredados de Microsoft 365, consulte [Activar o desactivar tokens heredados de Exchange Online](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) en la documentación de Microsoft.

Para obtener más información sobre tokens heredados, consulte [¿Puedo volver a activar los tokens heredados de Exchange Online?](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) en la documentación de Microsoft.
