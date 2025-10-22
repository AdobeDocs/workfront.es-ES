---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Formato de dominio para llamadas a la API de Adobe Workfront
description: Busque su dominio para utilizarlo en la API de Adobe Workfront
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
source-git-commit: b9547764abd4f1f61d93da6bc66d9e6776954f4d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 95%

---

# Formato de dominio para llamadas a la API de Adobe Workfront

Cuando realiza una llamada de API a la API de Workfront, utiliza el dominio de su organización en la llamada. El formato de esta URL de dominio difiere según si la organización se ha incorporado al Unified Shell de Adobe.

Para saber si su organización está en el Unified Shell de Adobe, examine la dirección URL que se muestra cuando está viendo una página de Workfront.

| La URL de Workfront comienza con: | URL para llamadas API: |
|---|---|
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


Para localizar el dominio:

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Configurar]** ![Icono de configuración](/help/_includes/assets/gear-icon-setup.png).
1. Seleccione **Sistema** y, a continuación, seleccione **Información del cliente**.

   Su dominio se muestra a la derecha de la pantalla.

   ![Dominio](assets/domain.png)

