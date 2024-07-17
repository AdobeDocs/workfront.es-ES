---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Formato de dominio para llamadas a la API de Adobe Workfront
description: Busque su dominio para utilizarlo en la API de Adobe Workfront
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
source-git-commit: c2ce6776ceebe3c1d3915e3791fc84eb0245ba4d
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

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Configurar]** ![Icono de configuración](/help/_includes/assets/gear-icon-setup.png).
1. Seleccione **Sistema** y, a continuación, seleccione **Información del cliente**.

   Su dominio se muestra a la derecha de la pantalla.

   ![Dominio](assets/domain.png)

