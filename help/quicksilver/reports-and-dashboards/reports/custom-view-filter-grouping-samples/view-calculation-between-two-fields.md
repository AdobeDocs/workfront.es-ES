---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Vista: muestra el resultado de un cálculo entre dos campos de una columna"
description: Puede utilizar el modo de texto en una columna para mostrar un cálculo entre dos campos.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# Vista: muestra el resultado de un cálculo entre dos campos de una columna

Puede utilizar el modo de texto en una columna para mostrar un cálculo entre dos campos.

Por ejemplo, si desea averiguar la cantidad de días de semana que transcurrieron entre dos fechas, puede utilizar la sintaxis del modo de texto y expresiones de datos para calcular esta diferencia.\
Por ejemplo, puede calcular la diferencia de días de semana entre la fecha planificada de finalización y la fecha real de finalización de una tarea y mostrar el resultado en una columna.

Puede utilizar otras dos fechas en este cálculo (inicio real, finalización real, inicio proyectado, finalización proyectada, etc.).\
Para obtener más información sobre las expresiones de datos calculados, vea [Información general sobre expresiones de datos calculados](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

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
   <td> <p>Solicitud para modificar una vista </p>
   <p>Plan para modificar un informe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar una vista</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Mostrar el resultado de un cálculo entre dos campos en una columna

Para agregar esta columna a una vista de tareas:

1. Ir a una lista de tareas.
1. En el menú desplegable **Vista**, haz clic en **Nueva vista**.

1. Haga clic en **Agregar columna** y, a continuación, **Cambiar al modo de texto**.

1. Pase el ratón sobre el área de modo de texto y haga clic **Haga clic para editar el texto**.
1. Elimine el texto que encuentre en el cuadro **Modo de texto** y reemplácelo por el siguiente código:
   <pre>displayname=Diferencia de día de semana<br>textmode=true<br>valueexpression=WEEKDAYDIFF({plannedCompletionDate},{actualCompletionDate})<br>valueformat=HTML</pre>

1. (Opcional) Para agregar los valores mostrados en la vista en una agrupación, siga los pasos descritos en [Agrupación: muestre el resultado de agregar varios valores calculados en una agrupación](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. Haz clic en **Guardar** y luego en **Guardar vista**.
