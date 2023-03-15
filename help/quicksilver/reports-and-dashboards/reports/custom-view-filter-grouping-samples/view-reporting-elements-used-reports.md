---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Ver: elementos de informes utilizados en los informes'
description: Esta vista muestra la vista, el filtro y la agrupación utilizados para crear cada informe en Adobe Workfront cuando se utiliza en una lista de informes.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 67f86523-e136-4768-af93-586a107b106f
source-git-commit: ''
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Ver: elementos de informes utilizados en informes

Esta vista muestra la vista, el filtro y la agrupación utilizados para crear cada informe en Adobe Workfront cuando se utiliza en una lista de informes.

Puede ver el

```
valuefields
```

o

```
valueexpressions
```

se utiliza en cada elemento del informe.

![report_with_elements_definitions.png](assets/report-with-elements-definitions-350x130.png)

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

## Ver los elementos de informes utilizados en los informes

1. Vaya a una lista de informes.
1. En el **Ver** menú desplegable, seleccione **Nueva vista**.

1. En el **Vista previa de columna** , elimine todas las columnas excepto una.
1. Haga clic en el encabezado de la columna restante y, a continuación, haga clic en **Cambiar al modo de texto**.
1. Pase el cursor sobre el área del modo de texto y haga clic en **Haga clic para editar texto**.
1. Elimine el texto que encuentra en la sección **Modo de texto** y sustitúyalo por el siguiente código:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.value.format=string<br>column.0.link.lookup=link.run<br>column.0.link.value=val(objCode)<br>column.0.listsort=string(name)<br>column.0.name=name.abbr<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=200<br>column.1.descriptionkey=objecttype<br>column.1.listsort=nested(view).string(uiObjCode)<br>column.1.namekey=objecttype.abbr<br>column.1.querysort=uiObjCode<br>column.1.valueField=uiObjCode<br>column.1.valueformat=objCodeMessage<br>column.1.width=80<br>column.2.descriptionkey=enteredby<br>column.2.listsort=nested(enteredBy).string(lastName)<br>column.2.namekey=enteredby.abbr<br>column.2.querysort=enteredBy:lastName<br>column.2.valuefield=enteredBy:name<br>column.2.valueformat=HTML<br>column.2.width=130<br>column.3.displayname=Filter definition<br>column.3.textmode=true<br>column.3.valuefield=filter:definition<br>column.3.valueformat=HTML<br>column.4.displayname=View definition<br>column.4.textmode=true<br>column.4.valuefield=view:definition<br>column.4.valueformat=HTML<br>column.5.displayname=Grouping definition<br>column.5.textmode=true<br>column.5.valuefield=groupBy:definition<br>column.5.valueformat=HTML<br></pre>

1. Haga clic en **Guardar vista**.
