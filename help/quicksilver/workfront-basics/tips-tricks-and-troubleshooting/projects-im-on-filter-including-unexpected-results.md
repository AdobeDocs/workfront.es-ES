---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Filtro Proyectos en los que participo, incluidos resultados inesperados
description: Lea este artículo para solucionar los problemas del filtro Proyectos en los que participo, incluidos los resultados inesperados.
feature: Get Started with Workfront
author: Alina
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
TQID: https://experienceleague.adobe.com/xE5RW947MUFg5d2X6ikKhHSftQDUMxDJlC05un0oDH0
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
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 180
ht-degree: 26%

---

# El filtro proyectos en los que estoy incluye resultados inesperados

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table>
  <tr>
   <td>Paquete de Adobe Workfront
   </td>
   <td>Cualquiera</td>
  </tr>
  <tr>
   <td>Licencias de Adobe Workfront
   </td>
   <td><p>Estándar</p>
   <p>Plan</p>
   </td>
  </tr>
   <tr>
   <td>Configuraciones de nivel de acceso
   </td>
   <td>Debe ser administrador de [!DNL Workfront].
   </td>
  </tr>
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Problema

El filtro [!UICONTROL **Proyectos en los que participo**] incluye resultados que no esperaría, ya que no estoy asignado o asociado con esos proyectos.

## Solución

El filtro [!UICONTROL **Proyectos en los que participo**] incluye proyectos que contienen al usuario en cualquiera de sus campos [!UICONTROL **Detalles del proyecto**], incluidos los campos que se pueden perder fácilmente o que se rellenan automáticamente, como [!UICONTROL **Ingresado por**] o [!UICONTROL **Identificador de patrocinador**]. Para eliminar los resultados no deseados, existen dos soluciones posibles:

1. Compruebe [!UICONTROL **Detalles del proyecto**] para cada proyecto inesperado incluido por el filtro y quite el nombre de todos los campos.

   O

1. Intente usar un filtro similar, como [!UICONTROL **Proyectos de mi propiedad**], que solo incluye los proyectos que se le hayan asignado específicamente.

Para obtener más información sobre el uso de filtros en [!DNL Workfront], vea [Información general sobre filtros](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
