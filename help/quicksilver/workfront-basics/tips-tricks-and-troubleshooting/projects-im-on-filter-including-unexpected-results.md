---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Filtro Proyectos en los que participo, incluidos resultados inesperados
description: Lea este artículo para solucionar los problemas del filtro Proyectos en los que participo, incluidos los resultados inesperados.
feature: Get Started with Workfront
author: Nolan
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 1%

---

# El filtro Proyectos en los que estoy incluye resultados inesperados

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
   <td role="rowheader"><strong>Licencia de Adobe [!DNL Workfront]</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>[!UICONTROL Administrador del sistema]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problema

El filtro [!UICONTROL **Proyectos en los que participo**] incluye resultados que no esperaría, ya que no estoy asignado o asociado con esos proyectos.

## Solución

El filtro [!UICONTROL **Proyectos en los que participo**] incluye proyectos que contienen al usuario en cualquiera de sus campos [!UICONTROL **Detalles del proyecto**], incluidos los campos que se pueden perder fácilmente o que se rellenan automáticamente, como [!UICONTROL **Ingresado por**] o [!UICONTROL **Identificador de patrocinador**]. Para eliminar los resultados no deseados, existen dos soluciones posibles:

1. Compruebe [!UICONTROL **Detalles del proyecto**] para cada proyecto inesperado incluido por el filtro y quite el nombre de todos los campos.

   O

1. Intente usar un filtro similar, como [!UICONTROL **Proyectos de mi propiedad**], que solo incluye los proyectos que se le hayan asignado específicamente.

Para obtener más información sobre el uso de filtros en [!DNL Workfront], vea [Información general sobre filtros](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
