---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Ver: calcular diferencias de fecha y hora'
description: Puede calcular la diferencia entre el siguiente - EDIT ME.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 548dd91f-02bc-43ed-8322-d0facf3488f0
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 0%

---

# Ver: calcular diferencias de fecha y hora

>[!IMPORTANT]
>
>No se puede calcular la diferencia de fecha y hora en Adobe Workfront entre dos objetos diferentes del mismo tipo. Por ejemplo, no se puede calcular la diferencia de fecha y hora entre dos fechas en dos proyectos, tareas o problemas diferentes.

Puede calcular la diferencia entre lo siguiente:

* Diferencia de fecha y hora entre dos campos de fecha en el mismo objeto
* Diferencia de fecha y hora entre el campo de un objeto y otro campo del objeto principal

>[!TIP]
>
>Estos cálculos muestran el número de días entre las dos fechas. El resultado se muestra en días. También se tiene en cuenta la marca de tiempo del campo de fecha y el número de días puede ir seguido de decimales si las marcas de tiempo no coinciden. Si la tarea se completó tarde, el número de días se muestra como un valor negativo.

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

## Calcular la diferencia de fecha y hora entre dos campos de fecha en el mismo objeto

Por ejemplo, puede calcular la diferencia entre la Fecha de Finalización Planificada y la Fecha de Finalización Real de una tarea.

![](assets/view-planned-actual-completion-dates-datediff-column-350x92.png)

1. Vaya a una lista de tareas.
1. En el **Ver** menú desplegable, haga clic en **Nueva vista**.

1. Haga clic en **Agregar columna** y empiece a escribir &quot;Fecha de finalización planeada&quot; en la **Mostrar en esta columna** a continuación, selecciónelo cuando aparezca en la lista.

1. Haga clic en **Agregar columna** y empiece a escribir &quot;Fecha de finalización real&quot; en la sección **Mostrar en esta columna** a continuación, selecciónelo cuando aparezca en la lista.

1. Haga clic en **Agregar columna** y haga clic en **Cambiar al modo de texto**.

1. Pase el ratón sobre el área del modo de texto y haga clic en **Haga clic para editar texto**.
1. Elimine el texto que encuentra en la sección **Modo de texto** y sustitúyalo por el siguiente código:

   ```
   displayname=Planned-Actual Completion Date<br>linkedname=direct<br>querysort=plannedCompletionDate<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{actualCompletionDate}),2)<br>valueformat=HTML
   ```

1. Haga clic en **Guardar**, luego **Guardar vista**.

## Calcular la diferencia de fecha y hora entre el campo de un objeto y otro campo de un objeto principal

Para obtener una lista de los objetos y sus elementos principales, consulte la sección &quot;Explicación de la interdependencia y la jerarquía de objetos&quot; en [Explicación de los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
Por ejemplo, puede calcular la diferencia entre la Fecha de Finalización Planificada de una tarea y la Fecha de Finalización Planificada de su tarea principal, o del proyecto en el que se encuentra la tarea.

![](assets/view-project-planned-task-planned-completion-dates-datediff-column-350x184.png)

1. Vaya a una lista de tareas.
1. En el **Ver** menú desplegable, haga clic en **Nueva vista**.

1. Haga clic en **Agregar columna** y empiece a escribir &quot; Fecha de finalización planeada del proyecto&quot; o &quot;Fecha de finalización principal&quot; en la **Mostrar en esta columna** a continuación, selecciónelo cuando aparezca en la lista.

1. Haga clic en **Agregar columna** y empiece a escribir &quot;Fecha de finalización planeada&quot; en la **Mostrar en esta columna** a continuación, selecciónelo cuando aparezca en la lista.

1. Haga clic en **Agregar columna** y haga clic en **Cambiar al modo de texto**.

1. Pase el ratón sobre el área del modo de texto y haga clic en **Haga clic para editar texto**.
1. Elimine el texto que encuentra en la sección **Modo de texto** y sustitúyalo por uno de los siguientes códigos:

   * Para mostrar la diferencia entre la fecha de finalización prevista del proyecto y la de la tarea:

      ```
      displayname=Project Planned Completion - Task Planned Completion (Days)<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({project}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>valueformat=HTML
      ```

   * Para mostrar la diferencia entre la Fecha de Finalización Planificada de la tarea principal y la de la tarea:

      ```
      valueexpression=ROUND(DATEDIFF({parent}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>textmode=true<br>valueformat=HTML<br>displayname=Parent Planned Completion - Planned Completion (Days)
      ```

1. Haga clic en **Guardar**, luego **Guardar vista**.
