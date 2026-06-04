---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Tener varias pestañas del explorador abiertas hace que Workfront cierre la sesión
description: Cuando un usuario tiene varias pestañas del explorador abiertas, es posible que Workfront cierre la sesión automáticamente.
feature: Get Started with Workfront
author: Becky
exl-id: 1cc8bf6c-0eda-41ef-8efd-bba3a5f33b08
TQID: https://experienceleague.adobe.com/Zof7zbTOm-w1vyBTchiXJv2QrNYbOxw9O4DYIjYQ6Ss
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 165
ht-degree: 42%

---

# Tener varias pestañas del explorador abiertas hace que Workfront cierre la sesión

## Problema

Cuando un usuario tiene varias pestañas del explorador abiertas y hace clic en una pestaña que ha estado inactiva durante un tiempo, la sesión de la pestaña ha caducado. El usuario no puede ver la página que había abierto y ve el siguiente mensaje:

```
Tab session expired
This tab session has been halted due to inactivity. Refresh the tab to continue where you left off.
```

## Motivo

Este comportamiento se debe a la Autenticación basada en directivas (PBA), una medida de seguridad configurada por su organización. Cuando una pestaña ha estado inactiva durante más tiempo del límite de tiempo establecido en la configuración de PBA de su organización, la sesión de la pestaña caduca.

## Solución

La solución depende de si ha estado activo en otra pestaña que ha iniciado sesión en Workfront.

* Si tiene una pestaña de Workfront activa abierta, vuelva a cargar la pestaña caducada. Volverá a la página que había abierto antes de que caducara.

* Si no tiene una pestaña de Workfront activa abierta, vuelva a iniciar sesión en Workfront.
