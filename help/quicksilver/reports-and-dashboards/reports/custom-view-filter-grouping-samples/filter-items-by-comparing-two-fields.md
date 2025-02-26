---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtrar: eliminar elementos de una lista comparando dos campos'
description: Puede filtrar elementos de una lista comparando dos de sus campos. Por ejemplo, puede mostrar solo las tareas cuya fecha real de finalización sea mayor que la fecha planificada de finalización.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: e8acdf8f7b3859385237e788dfda34ee62ee11d1
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 83%

---

# Filtrar: eliminar elementos de una lista comparando dos campos

<!--Audited: 10/2024-->

Puede filtrar elementos de una lista comparando dos de sus campos. Por ejemplo, puede mostrar solo las tareas cuya fecha real de finalización sea mayor que la fecha planificada de finalización.

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

## Filtrar elementos comparando dos campos

1. Vaya a una lista de tareas.
1. En el menú desplegable **Filtro**, seleccione **Nuevo filtro**.

1. Agregar un filtro para **Tarea: Fecha real de finalización** > **Mayor que** > **Seleccione una fecha**.

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
