---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: Mostrar informes programados para su envío'
description: Este filtro de informes muestra todos los informes programados para ser entregados automáticamente en Adobe Workfront. Se recomienda utilizarlo con la vista estándar.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7b937384-80c9-4bc7-94be-5573cf86b35b
source-git-commit: e8acdf8f7b3859385237e788dfda34ee62ee11d1
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 66%

---

# Filtro: mostrar informes programados para su envío

<!--Audited: 10/2024-->

Este filtro de informes muestra todos los informes programados para ser entregados automáticamente en Adobe Workfront. Se recomienda utilizarlo con la vista estándar.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> 
    <p>Nuevo:</p>
   <ul><li><p>Colaborador para modificar un filtro </p></li>
   <li><p>Estándar para modificar un informe</p></li> </ul>

<p>Actual:</p>
   <ul><li><p>Solicitud para modificar un filtro </p></li>
   <li><p>Plan para modificar un informe</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios para modificar un informe</p> <p>Acceso de edición a filtros, vistas y agrupaciones para modificar un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtro de envío de informes

Para aplicar este filtro:

1. Vaya a una lista de informes.

1. Haga clic en el menú desplegable **Filtro** y seleccione **Nuevo filtro**.

1. Haga clic en **Cambiar a modo de texto**.

1. En el área **Establecer reglas de filtro para su informe**, copie y pegue el siguiente código:

   ```
   scheduledReportID=0
   scheduledReportID_Mod=notnull
   ```

1. Haga clic en **Guardar filtro**.
