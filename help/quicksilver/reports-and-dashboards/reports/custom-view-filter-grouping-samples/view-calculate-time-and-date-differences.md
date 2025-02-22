---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: Calcular Diferencias de Fecha y Hora'
description: Aprenda a calcular las diferencias de fecha y hora.
author: Nolan
feature: Reports and Dashboards
exl-id: 548dd91f-02bc-43ed-8322-d0facf3488f0
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 91%

---

# Vista: calcular diferencias de fecha y hora

<!-- Audited: 11/2024 -->

>[!IMPORTANT]
>
>No se puede calcular la diferencia de fecha y hora en Adobe Workfront entre dos objetos diferentes del mismo tipo. Por ejemplo, no se puede calcular la diferencia de fecha y hora entre dos fechas en dos proyectos, tareas o problemas diferentes.

Puede calcular la diferencia entre lo siguiente:

* Diferencia de fecha y hora entre dos campos de fecha en el mismo objeto
* Diferencia de fecha y hora entre un campo de un objeto y otro campo del objeto principal

>[!TIP]
>
>Estos cálculos muestran el número de días entre las dos fechas. El resultado se muestra en días. La marca de tiempo del campo de fecha también se tiene en cuenta, y el número de días puede ir seguido de decimales si las marcas de tiempo no coinciden. Si la tarea se completó tarde, el número de días se muestra como un valor negativo.

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
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Nuevo: </p><ul><li><p>Colaborador para modificar una vista </p></li><li>
   <p>Estándar para modificar un informe</p></li></ul><p>O</p><p>Actual:</p><ul><li><p>Solicitud para modificar una vista </p></li><li>
   <p>Plan para modificar un informe</p> </li><ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios para modificar un informe</p> <p>Edición del acceso a Filtros, Vistas y Agrupaciones para modificar una vista</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Calcule la diferencia de hora y fecha entre dos campos de fecha en el mismo objeto

Por ejemplo, puede calcular la diferencia entre la fecha planificada de finalización y la fecha real de finalización de una tarea.

![Ver diferencia de fechas](assets/view-planned-actual-completion-dates-datediff-column-new.png)

1. Vaya a una lista de tareas.
1. En el menú desplegable **Vista**, haga clic en **Nueva vista**.

1. Haga clic en **Añadir columna** y empiece a escribir &quot;Fecha planificada de finalización&quot; en el campo **Mostrar en esta columna**; a continuación, selecciónela cuando se muestre en la lista.

1. Haga clic en **Añadir columna** y empiece a escribir &quot;Fecha real de finalización&quot; en el campo **Mostrar en esta columna**; a continuación, selecciónelo cuando se muestre en la lista.

1. Haga clic en **Añadir columna** y, a continuación, haga clic en **Cambiar al modo de texto**.

1. Pase el puntero por encima del área de modo de texto y haga clic en **Haga clic para editar el texto**.
1. Elimine el texto que encuentre en el cuadro **Modo de texto** y reemplácelo por el siguiente código:

   ```
    displayname=Planned-Actual Completion Date
    linkedname=direct
    querysort=plannedCompletionDate
    textmode=true
    valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{actualCompletionDate}),2)
    valueformat=HTML
   ```

1. Haga clic en **Guardar** y luego en **Guardar vista**.

## Calcular la diferencia de fecha y hora entre el campo de un objeto y otro campo de un objeto principal

Para obtener una lista de objetos y sus elementos principales, consulte la sección &quot;Explicación de la interdependencia y la jerarquía de objetos&quot; en [Explicación de los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
Por ejemplo, puede calcular la diferencia entre la fecha planificada de finalización de una tarea y la fecha planificada de finalización de su tarea principal o del proyecto en el que se encuentra la tarea.

![Ver diferencia de fecha planificada de finalización](assets/view-project-planned-task-planned-completion-dates-datediff-column-new.png)

1. Vaya a una lista de tareas.
1. En el menú desplegable **Vista**, haga clic en **Nueva vista**.

1. Haga clic en **Añadir columna** y empiece a escribir &quot;Fecha planificada de finalización del proyecto&quot; o &quot;Fecha de finalización principal&quot; en el campo **Mostrar en esta columna** y, a continuación, selecciónelo cuando se muestre en la lista.

1. Haga clic en **Añadir columna** y empiece a escribir &quot;Fecha planificada de finalización&quot; en el campo **Mostrar en esta columna**; a continuación, selecciónela cuando se muestre en la lista.

1. Haga clic en **Agregar columna** y, a continuación, haga clic en **Cambiar al modo de texto** > **Editar modo de texto**.
1. Quite el texto que encuentre en el cuadro **Editar modo de texto** y reemplácelo por uno de los códigos siguientes:

   * Para mostrar la diferencia entre la fecha planificada de finalización del proyecto y la de la tarea:

     ```
      displayname=Project Planned Completion - Task Planned Completion (Days)
      textmode=true
      valueexpression=ROUND(DATEDIFF({project}.{plannedCompletionDate},{plannedCompletionDate}),2)
      valueformat=HTML
     ```

   * Para mostrar la diferencia entre la fecha planificada de finalización de la tarea principal y la de la tarea:

     ```
      valueexpression=ROUND(DATEDIFF({parent}.{plannedCompletionDate},{plannedCompletionDate}),2)
      textmode=true<br>valueformat=HTML
      displayname=Parent Planned Completion - Planned Completion (Days)
     ```

1. Haga clic en **Listo** y luego en **Guardar vista**.
