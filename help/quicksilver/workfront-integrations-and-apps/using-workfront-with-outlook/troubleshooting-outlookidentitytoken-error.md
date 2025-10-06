---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 'Solución de problemas: error de outlookIdentityToken al usar Workfront para Outlook'
description: Si obtiene un error de outlookIdentityToken al utilizar Workfront para Outlook, debe habilitar los tokens heredados de Microsoft 365 para su organización.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4a911760-e3fe-4e77-b7aa-b08f9ea59d6a
source-git-commit: 793c8c940c8cb7ac53169edf21ddf28af2554120
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 43%

---

# Solución de problemas: error de outlookIdentityToken al usar Workfront para Outlook

>[!IMPORTANT]
>
>[Microsoft ha deshabilitado la compatibilidad con los tokens en línea heredados de Exchange](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), que el complemento de Workfront Outlook utilizaba para la autenticación. Este cambio de Microsoft se implementó por fases y se completó el 1 de octubre de 2025.
>
>**Debido a que Microsoft ha deshabilitado estos tokens, la integración de Workfront para Microsoft Outlook ya no funciona.**

Al utilizar Workfront para Outlook, puede ver el siguiente error:

```
Unexpected error
Unable to get the outlookIdentityToken
```

Para resolver este error, debe habilitar los tókenes heredados de Microsoft 365 para su organización. Como esto debe hacerse en Microsoft 365, Workfront no puede habilitar estos tókenes para su organización.

Para obtener instrucciones sobre cómo habilitar los tókenes heredados de Microsoft 365, consulte [Activar o desactivar los tokens heredados de Exchange Online](https://learn.microsoft.com/es-es/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) en la documentación de Microsoft.

Para obtener más información sobre los tókenes heredados, consulte [¿Puedo volver a activar los tókenes heredados de Exchange Online?](https://learn.microsoft.com/es-es/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) en la documentación de Microsoft.
