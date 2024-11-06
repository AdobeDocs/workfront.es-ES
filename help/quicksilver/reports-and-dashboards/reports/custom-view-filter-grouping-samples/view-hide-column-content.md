---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ver: Ocultar el contenido de una columna"
description: Es posible que desee ocultar información en la columna de una vista. Para ello, modifique el modo de texto de la columna.
author: Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Ver: ocultar el contenido de una columna

<!--Audited: 11/2024-->

Es posible que desee ocultar información en la columna de una vista. Para ello, modifique el modo de texto de la columna.

>[!NOTE]
>
>* Puede utilizar columnas ocultas para ordenar por un determinado objeto que no desee mostrar en la vista.\
>  Por ejemplo, puede ordenar por Número de tarea en una vista de tareas y ocultar la información de Número de tarea de la vista. En este caso, el objeto al que se hace referencia en la columna ayuda a ordenar la vista, pero la información de ese objeto no se muestra en la vista.
>* Cuando oculte una columna, tenga en cuenta que la información de la columna está oculta, pero la columna sigue existiendo en la vista.
>

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Nuevo:<ul><li>Colaborador para modificar una vista</li><li>Estándar para modificar un informe</li></ul></p><p>O</p>Actual:<ul><li>Solicitud para modificar una vista</li><li>Plan para modificar un informe</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar una vista</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ejemplo: Ordenar y ocultar la columna Número de tarea en una vista de tareas:

1. Ir a una lista de tareas.
1. En el menú desplegable **Vista**, haz clic en **Nueva vista**.

1. Haga clic en **Agregar columna** y empiece a escribir &quot;Número de tarea&quot; en el campo **Mostrar en esta columna**; a continuación, selecciónelo cuando se muestre en la lista.

1. Haga clic en **Cambiar al modo de texto** y luego **Editar texto**.
1. Elimine el texto que encuentre en el cuadro **Editar modo de texto** y reemplácelo por el siguiente código:

   ```
   displayname=
   linkedname=direct
   querysort=taskNumber
   sortOrder=1
   sortType=asc
   textmode=true
   value=
   valueformat=int
   width=0
   ```

   Los cambios importantes en este código que hacen que la columna esté oculta son los siguientes:

   * `displayname=`: esta línea debe estar en blanco.
   * `valuefield=`: esto ha sido reemplazado por `value`, y debe estar en blanco.
   * `width=`: según el campo, debe tener un valor de **0** o **1**.

1. Haga clic en **Listo** y luego en **Guardar vista**.
