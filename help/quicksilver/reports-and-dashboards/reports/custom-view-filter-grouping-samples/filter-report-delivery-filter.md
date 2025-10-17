---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: Mostrar informes programados para su envío'
description: Este filtro de informes muestra todos los informes programados para ser entregados automáticamente en Adobe Workfront. Se recomienda utilizarlo con la vista estándar.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: 7b937384-80c9-4bc7-94be-5573cf86b35b
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 57%

---

# Filtro: mostrar informes programados para su envío

<!--Audited: 10/2024-->

Este filtro de informes muestra todos los informes programados para ser entregados automáticamente en Adobe Workfront. Se recomienda utilizarlo con la vista estándar.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o solicitud para modificar un filtro </p>
   <p>Estándar o Plan para modificar un informe</p>
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

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
