---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Mensaje de error al ejecutar un informe: "Actualmente no ha iniciado sesión".'
description: Obtenga información acerca del mensaje de error “Actualmente no ha iniciado sesión”.
author: Courtney
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Vg-z-oXY25if70i5l2GBZad4iBj6hNRhu9LHE-6kCU8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 215
ht-degree: 94%

---

# Mensaje de error al ejecutar un informe: “Actualmente no ha iniciado sesión”.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
     <p>Estándar</p>
     <p>Trabajo o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de Edición a informes, paneles de control y calendarios</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Problema

Al ejecutar un informe o mostrarlo en un panel de control, se devuelve el siguiente error:\
*Intentémoslo de nuevo. Aún no ha iniciado sesión.*

No se muestran resultados en el informe.

## Causa

El informe está configurado actualmente para ejecutarse como un usuario desactivado.

## Solución

Debe tener permisos de administración en el informe para poder cambiar la configuración del informe.\
Para ajustar el informe y ver los resultados:

1. Vaya al informe.
1. Haga clic en **Acciones de informe** > **Editar** > **Configuración de informe**.

1. Especifique el nombre de un usuario activo en el campo **Ejecutar este informe con los derechos de acceso de:**.\
   O\
   Deje el campo **Ejecutar este informe con los derechos de acceso de:** en blanco.

1. Haga clic en **Aceptar**.
1. Haga clic en **Guardar + Cerrar**.\
   El error no debería aparecer de nuevo al ejecutar este informe.
