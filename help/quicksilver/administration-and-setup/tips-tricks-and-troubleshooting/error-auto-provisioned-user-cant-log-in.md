---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Error: el usuario aprovisionado automáticamente no puede iniciar sesión"
description: Si un usuario aprovisionado automáticamente intenta iniciar sesión por primera vez y recibe un error que indica que el sistema no le está asignando un nivel de acceso, puede deberse a que el sistema carece de niveles de acceso asociados con la licencia de solicitud.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 2%

---

# Error: el usuario aprovisionado automáticamente no puede iniciar sesión

Cuando un usuario aprovisionado automáticamente intenta iniciar sesión por primera vez, recibe el siguiente error:

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## Problema

El sistema no está asignando al nuevo usuario un nivel de acceso.

De forma predeterminada, el aprovisionamiento automático utiliza el tipo de licencia de solicitud. Cuando no existen niveles de acceso con una licencia de solicitud, el sistema no puede asignar al usuario un nivel de acceso.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td>
   <p>Nuevo: estándar</p>
   <p>o</p>
   <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de [!DNL Workfront]. </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solución

Cree un nivel de acceso básico con una licencia de solicitud:

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Niveles de acceso]**.

1. Haga clic en **[!UICONTROL Nuevo nivel de acceso]**.
1. Escriba un **[!UICONTROL Nombre]**.
1. En el menú desplegable **[!UICONTROL Tipo de licencia]**, seleccione Solicitud.
1. Haga clic en **[!UICONTROL Guardar cambios]**.

Después de crear un nivel de acceso con una licencia de solicitud, pida al usuario que inicie sesión con sus credenciales de SSO.


