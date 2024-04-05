---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Formato de dominio para llamadas a la API de Adobe Workfront
description: Busque su dominio para utilizarlo en la API de Adobe Workfront
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 8487f8d4b1651df268720806cfe07fa271a7b87d
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---


# Formato de dominio para llamadas a la API de Adobe Workfront

Cuando realiza una llamada de API a la API de Workfront, utiliza el dominio de su organización en la llamada. El formato de esta URL de dominio difiere según si la organización se ha incorporado al Unified Shell de Adobe.

Para saber si su organización está en el Unified Shell de Adobe, examine la dirección URL que se muestra cuando está viendo una página de Workfront.

| La URL de Workfront comienza con: | URL para llamadas API: |
|---|---|
| `<yourdomain>.my.workfront.com` | `<yourdomain>.my.workfront.com` |
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

Para localizar el dominio:

1. Haga clic en **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el botón **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda, haga clic en **[!UICONTROL Configurar]** ![Icono de configuración](/help/_includes/assets/gear-icon-setup.png).
1. Seleccionar **Sistema**, luego seleccione **Información del cliente**.

   Su dominio se muestra a la derecha de la pantalla.

   ![Dominio](assets/domain.png)