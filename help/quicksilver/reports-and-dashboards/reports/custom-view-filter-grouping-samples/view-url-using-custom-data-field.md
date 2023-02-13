---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: URL externa con campo de datos personalizado'
description: Puede mostrar un vínculo a una URL personalizada interna utilizando un campo personalizado calculado denominado "URL personalizada" en una vista de tareas.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 0%

---

# Ver: URL externa con campo de datos personalizado

Puede mostrar un vínculo a una dirección URL personalizada interna mediante una **Campo personalizado calculado** se denomina &quot;URL personalizada&quot; en una **Vista de tareas**.

Esto le ayuda a vincular rápidamente desde ciertos objetos con vistas a ciertas áreas de la aplicación directamente desde los informes.

Al crear un campo personalizado calculado, primero debe crear el campo y, a continuación, crear la vista.

Las secciones siguientes son un ejemplo de campo personalizado calculado para tareas. El campo personalizado se denomina URL personalizada. La vista personalizada muestra el valor del campo, así como el valor de **URL** para tareas.

Con los mismos pasos, puede crear campos personalizados y vistas personalizadas calculadas similares para todos los objetos del sistema que tengan un formulario personalizado.

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

## Crear el campo personalizado &quot;URL personalizada&quot;

Para obtener información sobre la creación de un campo personalizado calculado, consulte el artículo [Agregar datos calculados a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Si tiene acceso para crear un formulario personalizado, puede crear un campo personalizado calculado para tareas llamadas &quot;URL personalizada&quot;. Este campo se vincula directamente al **Información general** dentro de la subficha **Detalles de la tarea** pestaña .

1. Cree un campo personalizado calculado.
1. En el campo Calculation , introduzca el siguiente código:

   CONCAT(&#39;&#39;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,ID&quot;/overview&#39;)

1. Reemplazar &quot;`<domain>`&quot; con su nombre de dominio real, sin los corchetes.

   El

   ```
   /overview
   ```

   de esta dirección URL dirige el vínculo a la **Información general** en el panel izquierdo de la tarea.

1. Después de crear el **Campo personalizado calculado**, adjunte el **Formulario personalizado** con este campo a varias tareas de Adobe Workfront que desea mostrar en la nueva vista.

## Cree la vista que muestra los campos &quot;URL personalizada&quot; y &quot;URL&quot; de la tarea

La tarea **Ver** en el ejemplo siguiente se muestra la variable **Campo personalizado calculado** denominada &quot;URL personalizada&quot; como vínculo directo al **Información general** subficha dentro de la tarea **Detalles** , así como la **URL** de la tarea.

![](assets/task-view-with-custom-url-field-quicksilver-350x70.png)

Para personalizar esta vista:

1. Vaya a una lista de tareas.
1. Expanda el **Ver** en la parte superior de la lista de tareas.
1. Haga clic en **Personalizar vista**.
1. Elimine todas las columnas de la vista, excepto la primera columna.
1. Haga clic en el encabezado de la primera columna.
1. Haga clic en **Cambiar al modo de texto** en la esquina superior derecha de la interfaz.
1. Haga clic en **Haga clic para editar texto**.
1. Pegue el modo de texto siguiente en una columna.\
   En este ejemplo, la columna &quot;column.1.&quot; muestra el valor en el campo &quot;URL personalizada&quot; como un vínculo en el **Información general**. &quot;Columna.2.&quot; muestra el valor almacenado en la variable **Campo URL** de la tarea.
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.value.format= int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield= objCode<br>column.0.link.value.format= val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.name=name.abbr<br>column.0.querysort=name<br>column.0.abreviview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=Custom URL<br>column.1.link.isnewwindow=true<br>column.1.link.url=customDataLabelsAsString(URL personalizada)<br>column.1.linkedname=direct<br>column.1.listsort=customDataLabelsAsString(URL personalizada)<br>column.1.name=Custom URL<br>column.1.querysort=URL<br>column.1.abreviview=false<br>column.1.stretch=0<br>column.1.valuefield=Custom URL<br>column.1.valueformat=customDataLabelsAsString<br>column.1.width=150<br>column.2.descriptionkey=url<br>column.2.linkedname=direct<br>column.2.listsort=string(URL)<br>column.2.namekey=url.abbr<br>column.2.querysort=URL<br>column.2.abreviview=false<br>column.2.stretch=0<br>column.2.valuefield=URL<br>column.2.valueformat=HTML<br>column.2.width=150</pre>

1. Haga clic en **Guardar vista**.
