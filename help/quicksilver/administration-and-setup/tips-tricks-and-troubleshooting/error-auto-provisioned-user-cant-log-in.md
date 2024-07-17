---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Error: el usuario aprovisionado automáticamente no puede iniciar sesión"
description: Si un usuario aprovisionado automáticamente intenta iniciar sesión por primera vez y recibe un error que indica que el sistema no le está asignando un nivel de acceso, puede deberse a que el sistema carece de niveles de acceso asociados con la licencia de solicitud. El aprovisionamiento automático utiliza el tipo de licencia de solicitud, por lo que puede solucionar este problema creando un nivel de acceso asociado a una licencia de solicitud.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: 477f65efb09e8566dd0af88adfbe88135d6c6ae9
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# Error: el usuario aprovisionado automáticamente no puede iniciar sesión

Cuando un usuario aprovisionado automáticamente intenta iniciar sesión por primera vez, recibe el siguiente error:

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## Problema

El sistema no está asignando al nuevo usuario un nivel de acceso.

De forma predeterminada, el aprovisionamiento automático utiliza el tipo de licencia de solicitud. Cuando no existen niveles de acceso con una licencia de solicitud, el sistema no puede asignar al usuario un nivel de acceso.

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
   <td> <p>Debe ser administrador de [!DNL Workfront]. Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo completo a un usuario</a>.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solución

Cree un nivel de acceso básico con una licencia de solicitud:

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Niveles de acceso]**.

1. Haga clic en **[!UICONTROL Nuevo nivel de acceso]**.
1. Escriba un **[!UICONTROL Nombre]**.
1. En el menú desplegable **[!UICONTROL Tipo de licencia]**, seleccione Solicitud.
1. Haga clic en **[!UICONTROL Guardar cambios]**.

Después de crear un nivel de acceso con una licencia de solicitud, pida al usuario que inicie sesión con sus credenciales de SSO.


