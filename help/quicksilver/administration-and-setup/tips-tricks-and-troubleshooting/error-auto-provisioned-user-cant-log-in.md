---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Error: el usuario aprovisionado automáticamente no puede iniciar sesión'
description: Si un usuario aprovisionado automáticamente intenta iniciar sesión por primera vez y recibe un error que indica que el sistema no le está asignando un nivel de acceso, puede deberse a que el sistema carece de niveles de acceso asociados con la licencia de solicitud.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
TQID: https://experienceleague.adobe.com/jUBGb9lqH9QL34Rw-oEhjty3l3wAf8avcLgtVe1-VSg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 200
ht-degree: 18%

---

# Error: el usuario aprovisionado automáticamente no puede iniciar sesión

Cuando un usuario aprovisionado automáticamente intenta iniciar sesión por primera vez, recibe el siguiente error:

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## Problema

El sistema no está asignando al nuevo usuario un nivel de acceso.

De forma predeterminada, el aprovisionamiento automático utiliza el tipo de licencia de solicitud. Cuando no existen niveles de acceso con una licencia de solicitud, el sistema no puede asignar al usuario un nivel de acceso.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solución

Cree un nivel de acceso básico con una licencia de solicitud:

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Niveles de acceso]**.

1. Haga clic en **[!UICONTROL Nuevo nivel de acceso]**.
1. Escriba un **[!UICONTROL Nombre]**.
1. En el menú desplegable **[!UICONTROL Tipo de licencia]**, seleccione Solicitud.
1. Haga clic en **[!UICONTROL Guardar cambios]**.

Después de crear un nivel de acceso con una licencia de solicitud, pida al usuario que inicie sesión con sus credenciales de SSO.


