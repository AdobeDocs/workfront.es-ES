---
content-type: tips-tricks-troubleshooting
product-previous: mobile
navigation-topic: tips-tricks-and-troubleshooting-mobile-apps
title: Mensaje de error en la aplicación móvil  [!DNL Adobe Workfront] Tu cuenta no tiene habilitada la API.'
description: Mensaje de error en la aplicación móvil  [!DNL Adobe Workfront] Tu cuenta no tiene habilitada la API.'
author: Lisa
feature: Get Started with Workfront
exl-id: 120e56f4-9fd5-4c41-890e-981937714db0
source-git-commit: d11066d9aa76077bfaaa2d44f2e29c983dafa96f
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 68%

---

# Mensaje de error en la aplicación móvil [!DNL Adobe Workfront]: “[!UICONTROL Su cuenta no tiene habilitada la API]”.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p> Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe [!DNL Workfront]</strong></td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>[!UICONTROL System administrator] </p> </td> 
  </tr> 
 </tbody> 
</table>

## Problema

Al intentar iniciar sesión en la aplicación móvil [!DNL Adobe Workfront], recibe el siguiente error: *[!UICONTROL Su cuenta no tiene habilitada la API. Informe al administrador del sistema y le ayudará a configurarla. Lo sentimos mucho.]*

## Causa

El administrador de [!DNL Workfront] no ha habilitado el acceso al entorno de [!DNL Workfront] desde un dispositivo móvil.

## Solución

1. Inicie sesión en la aplicación web [!DNL Workfront] como administrador de [!DNL Workfront].
1. Vaya al área **[!UICONTROL Setup]**.
1. Expanda el menú **[!UICONTROL System]** y, a continuación, haga clic en **[!UICONTROL Preferences]**.

1. En la sección **[!UICONTROL Seguridad]**, seleccione la opción **[!UICONTROL Permitir que los usuarios usen las aplicaciones móviles[!DNL Workfront] de]** para habilitarla.

1. Haga clic en **[!UICONTROL Guardar]**.\
   Ahora todos los usuarios del sistema pueden acceder a [!DNL Workfront] desde sus aplicaciones móviles.
