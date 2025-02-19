---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Vista: URL externa con campo de datos personalizados'
description: Puede mostrar un vínculo a una URL personalizada interna utilizando un campo personalizado calculado denominado “URL personalizada” en una vista de tareas.
author: Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 6a1152bb86a856d60585db7d6ffd43a59a212a72
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 84%

---

# “Vista: URL externa que usa el campo de datos personalizados”

<!--Audited: 11/2024-->

Puede mostrar un vínculo a una URL personalizada interna usando un **Campo personalizado calculado** denominado “URL personalizada” en una **Vista de tareas**.

Esto le ayuda a vincular rápidamente desde ciertos objetos de una vista hasta determinadas áreas de la aplicación directamente desde los informes.

Al crear un campo personalizado calculado, primero debe crear el campo y, a continuación, crear la vista.

Las siguientes secciones son un ejemplo de un campo personalizado calculado para tareas. El campo personalizado se denomina URL personalizada. La vista personalizada muestra el valor del campo, así como el campo **URL** para las tareas.

Con los mismos pasos, puede crear campos personalizados calculados y vistas personalizadas similares para todos los objetos del sistema que tengan un formulario personalizado.

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
   <td> <p> Actual: 
   <ul>
   <li>Solicitud para modificar una vista</li> 
   <li>Plan para modificar un informe</li>
   </ul>
     </p>
     <p> Nuevo: 
   <ul>
   <li>Colaborador para modificar una vista</li> 
   <li>Estándar para modificar un informe</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios para modificar un informe</p> <p>Edición del acceso a Filtros, Vistas y Agrupaciones para modificar una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creación del campo personalizado calculado “URL personalizada”

Para obtener información acerca de cómo crear un campo personalizado calculado, consulte [Añadir campos calculados a un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Si tiene acceso para crear un formulario personalizado, puede crear un campo personalizado calculado para las tareas denominadas “URL personalizada”. Este campo se vincula directamente a la subpestaña **Información general** en la pestaña **Detalles de la tarea**.

1. Cree un campo personalizado calculado.
1. En el campo Cálculo, introduzca el siguiente código:

   CONCAT(&#39;&#39;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,ID,&quot;/overview&#39;&#39;)

1. Reemplace &quot;`<domain>`&quot; por su nombre de dominio real, sin los corchetes. La parte `/overview` de esta dirección URL dirige el vínculo a la sección **Información general** en el panel izquierdo de la tarea.

1. Después de crear su **Campo personalizado calculado**, adjunte el **Formulario personalizado** con este campo a varias tareas de Adobe Workfront que desee mostrar en la nueva vista.

## Crear la vista que muestra los campos “URL personalizada” y “URL” de la tarea

La tarea **Vista** del ejemplo siguiente muestra el **Campo personalizado calculado** denominado “URL personalizada” como un vínculo directo a la subpestaña **Información general** dentro de la pestaña **Detalles** de la tarea, así como el campo **URL** de la tarea.

(assets/task-view-with-custom-url-field-quicksilver-350x70.png)

Para personalizar esta vista:

1. Vaya a una lista de tareas.
1. Expanda la lista desplegable **Vista** en la parte superior de la lista de tareas.
1. Pulse **Guardar vista**.
1. Quite todas las columnas dentro de la vista, excepto la primera.
1. Haga clic en el encabezado de la primera columna.
1. Haga clic en **Cambiar al modo de texto** > **Editar modo de texto**.
1. Elimine el texto del cuadro **Editar modo de texto** y reemplácelo por el siguiente código:


   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat= int
   column.0.link.lookup=link.view
   column.0.link.valuefield= objCode
   column.0.link.valueformat= val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.description=Custom URL
   column.1.link.isnewwindow=true
   column.1.link.url=customDataLabelsAsString(Custom URL)
   column.1.linkedname=direct
   column.1.listsort=customDataLabelsAsString(Custom URL)
   column.1.name=Custom URL
   column.1.querysort=URL
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=Custom URL
   column.1.valueformat=customDataLabelsAsString
   column.1.width=150
   column.2.descriptionkey=url
   column.2.linkedname=direct
   column.2.listsort=string(URL)
   column.2.namekey=url.abbr
   column.2.querysort=URL
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=URL
   column.2.valueformat=HTML
   column.2.width=150
   ```

   En este ejemplo, &#39;column.1.&#39;  Las líneas muestran el valor del campo &quot;URL personalizada&quot; como un vínculo a la sección **Información general** de la tarea; &quot;columna.2.&quot; muestra el valor almacenado en el **campo URL** de la tarea.

1. Haga clic en **Listo** > **Guardar vista**.
