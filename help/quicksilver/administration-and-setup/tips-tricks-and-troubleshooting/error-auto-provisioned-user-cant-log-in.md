---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Error: El usuario aprovisionado automáticamente no puede iniciar sesión"
description: Si un usuario aprovisionado automáticamente intenta iniciar sesión por primera vez y recibe un error que indica que el sistema no les asigna un nivel de acceso, esto puede deberse a que el sistema carece de niveles de acceso asociados a la licencia de Solicitud. El aprovisionamiento automático utiliza el tipo de licencia Solicitud , por lo que puede solucionar este problema creando un nivel de acceso asociado a una licencia Solicitud .
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Error: El usuario aprovisionado automáticamente no puede iniciar sesión

Cuando un usuario aprovisionado automáticamente intenta iniciar sesión por primera vez, recibe el siguiente error:

## Problema

El sistema no asigna al nuevo usuario un nivel de acceso.

De forma predeterminada, el aprovisionamiento automático utiliza el tipo de licencia Solicitud . Cuando no existe ningún nivel de acceso con una licencia de Solicitud, el sistema no puede asignar al usuario un nivel de acceso.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser [!DNL Workfront] administrador. Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solución

Cree un nivel de acceso básico con una licencia de solicitud:

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Niveles de acceso]**.

1. Haga clic en **[!UICONTROL Nuevo nivel de acceso]**.
1. Escriba un **[!UICONTROL Nombre]**.
1. En el **[!UICONTROL Tipo de licencia]** menú desplegable, seleccione Solicitud.
1. Haga clic en **[!UICONTROL Guardar cambios]**.

Después de crear un nivel de acceso con una licencia de solicitud, haga que el usuario inicie sesión con sus credenciales de SSO.
