---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtrar: eliminar elementos de una lista comparando dos campos'
description: Puede filtrar elementos de una lista comparando dos de sus campos. Por ejemplo, puede mostrar solo las tareas cuya fecha real de finalización sea mayor que la fecha planificada de finalización.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 77%

---

# Filtrar: eliminar elementos de una lista comparando dos campos

<!--Audited: 10/2024-->

Puede filtrar elementos de una lista comparando dos de sus campos. Por ejemplo, puede mostrar solo las tareas cuya fecha real de finalización sea mayor que la fecha planificada de finalización.

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

## Filtrar elementos comparando dos campos

1. Vaya a una lista de tareas.
1. En el menú desplegable **Filtro**, seleccione **Nuevo filtro**.

1. Agregue un filtro para **Fecha de finalización de la tarea:Actual** > **Más que** > **Seleccione una fecha**.

   >[!TIP]
   >
   >Elija el modificador de filtro que desee utilizar para el campo seleccionado, si está disponible.

1. Haga clic en **Modo de texto**.
1. En el área mostrada, añada el siguiente código:

   ```
   actualCompletionDate=FIELD:plannedCompletionDate
   actualCompletionDate_Mod=gt
   ```

1. Haga clic en **Aplicar** > **Guardar como nuevo**.
