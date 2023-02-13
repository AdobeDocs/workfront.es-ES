---
content-type: tips-tricks-troubleshooting
product-previous: mobile
navigation-topic: tips-tricks-and-troubleshooting-mobile-apps
title: '"Mensaje de error en la variable [!DNL Adobe Workfront] Aplicación móvil: "Su cuenta no está habilitada para API".'
description: '"Mensaje de error en la variable [!DNL Adobe Workfront] Aplicación móvil: "Su cuenta no está habilitada para API".'
author: Lisa
feature: Get Started with Workfront
exl-id: 120e56f4-9fd5-4c41-890e-981937714db0
source-git-commit: fdef22d9685d349a6f9492dec98475493ee9c048
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 2%

---

# Mensaje de error en la variable [!DNL Adobe Workfront] Aplicación móvil: &quot;[!UICONTROL Su cuenta no está habilitada para API.]&quot;

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
   <td role="rowheader"><strong>Adobe [!DNL Workfront] licencia</strong></td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>[!UICONTROL System administrator] </p> </td> 
  </tr> 
 </tbody> 
</table>

## Problema

Cuando intente iniciar sesión en la [!DNL Adobe Workfront] aplicación móvil, recibe el siguiente error: *[!UICONTROL Su cuenta no está habilitada para API. Informe a su administrador del sistema y le permitirán configurarlo. Perdón por eso.]*

## Causa

Su [!DNL Workfront] el administrador no ha habilitado su [!DNL Workfront] entorno al que se va a acceder desde un dispositivo móvil.

## Solución

1. Inicie sesión en el [!DNL Workfront] aplicación web como [!DNL Workfront] Administrador.
1. Vaya a la **[!UICONTROL Configuración]** .
1. Expanda el **[!UICONTROL Sistema]** a continuación, haga clic en **[!UICONTROL Preferencias]**.

1. En el **[!UICONTROL Seguridad]** seleccione **[!UICONTROL Dejar que las personas usen [!DNL Workfront]las aplicaciones móviles de y el [!DNL Workfront Outlook] Complemento]** para activarla.

1. Haga clic en **[!UICONTROL Guardar]**.\
   Ahora, todos los usuarios del sistema pueden acceder a [!DNL Workfront] desde sus aplicaciones móviles y desde [!DNL Outlook].
