---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtrar: eliminar elementos de una lista comparando dos campos"
description: Puede filtrar elementos de una lista comparando dos de sus campos. Por ejemplo, puede mostrar sólo las tareas cuya fecha real de finalización sea mayor que la fecha planificada de finalización.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# Filtrar: elimine elementos de una lista comparando dos campos

Puede filtrar elementos de una lista comparando dos de sus campos. Por ejemplo, puede mostrar sólo las tareas cuya fecha real de finalización sea mayor que la fecha planificada de finalización.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud para modificar un filtro </p>
   <p>Plan para modificar un informe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar un filtro</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Filtrar elementos comparando dos campos

1. Ir a una lista de tareas.
1. En el menú desplegable **Filtro**, seleccione **Nuevo filtro**.

1. Haga clic en **Agregar regla de filtro** y agregue **Fecha real de finalización** >**Mayor que** > **Seleccione una fecha**.

   >[!TIP]
   >
   >Elija el modificador de filtro que desee utilizar para el campo seleccionado, si está disponible.

1. Haga clic en **Cambiar al modo de texto**.
1. En el área **Establecer reglas de filtro para su informe**, agregue el siguiente código:

   ```
   actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt
   ```

1. Haga clic en **Listo** y luego en **Guardar filtro**.
