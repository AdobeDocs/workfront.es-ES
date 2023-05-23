---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ver: ocultar el contenido de una columna"
description: Es posible que desee ocultar información en la columna de una vista. Para ello, modifique el modo de texto de la columna.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Ver: ocultar el contenido de una columna

Es posible que desee ocultar información en la columna de una vista. Para ello, modifique el modo de texto de la columna.

>[!TIP]
>
>* Puede utilizar columnas ocultas para ordenar por un determinado objeto que no desee mostrar en la vista.\
   >  Por ejemplo, puede ordenar por Número de tarea en una vista de tareas y ocultar la información de Número de tarea de la vista. En este caso, el objeto al que se hace referencia en la columna ayuda a ordenar la vista, pero la información de ese objeto no se muestra en la vista.
>* Cuando oculte una columna, tenga en cuenta que la información de la columna está oculta, pero la columna sigue existiendo en la vista.
>


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

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Ejemplo: Ordenar y ocultar la columna Número de tarea en una vista de tareas:

1. Ir a una lista de tareas.
1. Desde el **Ver** , haga clic en **Nueva vista**.

1. Clic **Agregar columna** y empiece a escribir &quot;Número de tarea&quot; en la **Mostrar en esta columna** a continuación, selecciónelo cuando se muestre en la lista.

1. Clic **Cambiar a modo de texto**.
1. Pase el ratón sobre el área de modo de texto y haga clic en **Haga clic para editar el texto**.
1. Elimine el texto que encuentre en la **Modo de texto** y reemplácelo por el siguiente código:

   <pre><strong>displayname=</strong>linkedname=direct<br>querysort=taskNumber<br>sortOrder=1<br>sortType=asc<br>textmode=true<br><strong>value=</strong>valueformat=int<br><strong>width=0</strong></pre>Los cambios importantes en este código que hacen que la columna esté oculta son los siguientes:

   ```
   displayname
   ```

   esta línea debe estar en blanco.

   ```
   valuefield
   ```

   Esto se ha reemplazado por *valor*, y debe estar en blanco.

   ```
   width
   ```

   : Según el campo, debe tener un valor de *0* o *1*.

1. Clic **Guardar**, entonces **Guardar vista**.
