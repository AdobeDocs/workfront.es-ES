---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Proyectos en los que estoy activado, incluidos resultados inesperados
description: Lea este artículo para solucionar los problemas del filtro Proyectos en los que estoy incluido, incluyendo resultados inesperados.
feature: Get Started with Workfront
author: Nolan
source-git-commit: 5a4c98f9ce6bb7eb936a0b24b634d2545a0f13ee
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 1%

---

# El filtro Proyectos en los que estoy activo incluye resultados inesperados

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] licencia</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>[!UICONTROL System administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problema

La variable [!UICONTROL **Proyectos en los que estoy**] incluye resultados que no esperaría, ya que no estoy asignado ni asociado a esos proyectos.

## Solución

La variable [!UICONTROL **Proyectos en los que estoy**] filtro incluye proyectos que contienen al usuario en cualquiera de sus [!UICONTROL **Detalles del proyecto**] campos, incluidos campos fácilmente omitidos o rellenados automáticamente, como [!UICONTROL **Introducido por**] o [!UICONTROL **ID del patrocinador**]. Para eliminar los resultados no deseados, hay dos soluciones posibles:

1. Marque la [!UICONTROL **Detalles del proyecto**] para cada proyecto inesperado incluido en el filtro y elimine su nombre de todos los campos.

O

1. Intente usar un filtro similar, como [!UICONTROL **Proyectos de los que soy propietario**], que solo incluye proyectos que se le hayan asignado específicamente.

Para obtener más información sobre el uso de filtros en [!DNL Workfront], consulte [Información general de filtros en [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)