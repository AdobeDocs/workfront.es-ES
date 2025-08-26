---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Varias pestañas del explorador hacen que Workfront cierre la sesión
description: Cuando un usuario tiene varias pestañas del explorador abiertas, es posible que Workfront cierre la sesión automáticamente.
feature: Get Started with Workfront
exl-id: 1cc8bf6c-0eda-41ef-8efd-bba3a5f33b08
source-git-commit: 945fa710e98b094a37258d5c94f7b1a2eb056abb
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 30%

---

# Varias pestañas del explorador hacen que Workfront cierre la sesión

>[!IMPORTANT]
>
>Este problema solo está presente para las organizaciones que se han incorporado a Adobe IMS.

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
