---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: quitar vínculo a un objeto de una columna'
description: De forma predeterminada, algunos objetos que se muestran en un vínculo de vista a la página Detalles del objeto. Por ejemplo, la columna que muestra el Nombre de un proyecto es un vínculo al proyecto; la columna que muestra el nombre de un usuario es un vínculo a la página de perfil del usuario.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Ver: quitar vínculo a un objeto de una columna

De forma predeterminada, algunos objetos que se muestran en un vínculo de vista a la página Detalles del objeto. Por ejemplo, la columna que muestra el Nombre de un proyecto es un vínculo al proyecto; la columna que muestra el nombre de un usuario es un vínculo a la página de perfil del usuario.

Puede quitar este vínculo mediante el modo de texto de las columnas que aparecen en todas las vistas.

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

## Ejemplo: Elimine el vínculo a una tarea de la columna Nombre de tarea en una vista de tareas:

1. Vaya a una lista de tareas.
1. En el **Ver** menú desplegable, haga clic en **Nueva vista** para crear una vista nueva.

   O

   Haga clic en el **Icono Editar** ![](assets/edit-icon.png)

   para editar una vista existente, seleccione la vista.

1. Haga clic en **Agregar columna** para agregar una columna nueva.

   O

   Haga clic en una columna existente con un vínculo a un objeto.

1. Haga clic en **Cambiar al modo de texto**.
1. Pase el ratón sobre el área del modo de texto y haga clic en **Haga clic para editar texto**.
1. Elimine el texto que encuentra en la sección **Modo de texto** y sustitúyalo por el siguiente código:

   <pre>nombreDePantalla=NombreDeTarea<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>valueexpression={name}</strong><br>value=Compound</pre>

   >[!TIP]
   >
   >Puede utilizar código similar para otros objetos ajustando lo siguiente:
   >
   >   
   >   
   >   * Sustituya el **campo de valor** línea del código con **valueexpression** y mantenga el mismo nombre incluido entre llaves después del signo igual.
   >   
   >   
   >
   >   
   >   
   >   * Elimine todas las líneas que empiecen por >
   >   
   >     ```>   
   >     link.
   >     ```   >   
   >   
   >     from the original text of the column. For example, eliminate all the following lines:
   >     <pre>link.linkproperty.0.name=ID</pre><pre>link.linkproperty.0.valuefield=ID</pre><pre>link.linkproperty.0.valueformat=string</pre><pre>link.lookup=link.view</pre><pre>link.value=val(objCode)</pre>
   >   
   >   
   >



1. Haga clic en **Guardar**, luego **Guardar vista**.
