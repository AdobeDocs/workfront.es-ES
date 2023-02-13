---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Filtro: eliminar elementos de una lista comparando dos campos'
description: Puede filtrar elementos de una lista comparando dos de sus campos. Por ejemplo, puede mostrar solo las tareas en las que la Fecha de finalización real de la tarea sea buena a la Fecha de finalización planeada.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Filtro: eliminar elementos de una lista comparando dos campos

Puede filtrar elementos de una lista comparando dos de sus campos. Por ejemplo, puede mostrar solo las tareas en las que la Fecha de finalización real de la tarea sea buena a la Fecha de finalización planeada.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y grupos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Filtrado de elementos comparando dos campos

1. Vaya a una lista de tareas.
1. En el **Filtro** menú desplegable, seleccione **Nuevo filtro**.

1. Haga clic en **Agregar regla de filtro** y agregue **Fecha de finalización real** >**Bueno que** > **Seleccionar una fecha**.

   >[!TIP]
   >
   >Elija el modificador de filtro que desee utilizar para el campo seleccionado, si está disponible.

1. Haga clic en **Cambiar al modo de texto**.
1. En el **Definir reglas de filtro para el informe** , añada el siguiente código:

   ```
   actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt
   ```

1. Haga clic en **Listo**, luego **Guardar filtro**.
