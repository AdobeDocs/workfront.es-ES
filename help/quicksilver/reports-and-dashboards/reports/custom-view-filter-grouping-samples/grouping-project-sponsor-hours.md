---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Agrupación: patrocinador del proyecto por horas'
description: Esta agrupación de horas organiza las horas por el patrocinador del proyecto en el que se registran. La interfaz estándar de Report Builder para las agrupaciones de horas no proporciona ninguna asignación al campo Patrocinador del proyecto. Debe utilizar la interfaz del Modo de texto para acceder a este campo.
author: Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 80%

---

# Agrupación: patrocinador del proyecto para horas

<!--Audited: 10/2024-->

Esta agrupación de horas organiza las horas por el patrocinador del proyecto en el que se registran. La interfaz estándar de Report Builder para las agrupaciones de horas no proporciona ninguna asignación al campo Patrocinador del proyecto. Debe utilizar la interfaz del Modo de texto para acceder a este campo.

![hour_report_grouped_by_sponsor.png](assets/hour-report-grouped-by-sponsor-350x39.png)

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

## Agrupar por patrocinador del proyecto para horas

Para aplicar esta agrupación:

1. Vaya a una lista de horas.
1. En el menú desplegable **Agrupación**, seleccione **Nueva agrupación**.

1. Haga clic en **Cambiar al modo de texto**.
1. Elimine el texto del área que se muestra y reemplácelo por el siguiente código:

```
   group.0.linkedname=project:sponsor:name
   group.0.name=
   group.0.valuefield=project:sponsor:name
   group.0.valueformat=HTML
   textmode=true
```

1. Haga clic en **Listo**.
1. Actualice el nombre de la agrupación y haga clic en **Guardar agrupación**.
