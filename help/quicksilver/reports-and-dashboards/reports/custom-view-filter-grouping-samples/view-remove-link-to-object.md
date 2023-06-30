---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ver: quitar el vínculo a un objeto de una columna"
description: De forma predeterminada, algunos objetos que se muestran en una vista se vinculan a la página Detalles del objeto. Por ejemplo, la columna que muestra el Nombre de un proyecto es un vínculo al proyecto; la columna que muestra el Nombre de un usuario es un vínculo a la página de perfil del usuario.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 5480d6b5e97c4c2e21080bb92ffe255f60ed6f60
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# Ver: Eliminar el vínculo a un objeto de una columna

De forma predeterminada, algunos objetos que se muestran en una vista se vinculan a la página Detalles del objeto. Por ejemplo, la columna que muestra el Nombre de un proyecto es un vínculo al proyecto; la columna que muestra el Nombre de un usuario es un vínculo a la página de perfil del usuario.

Puede quitar este vínculo mediante el modo de texto en columnas que se muestran en todas las vistas.

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

## Ejemplo: Quitar el vínculo a una tarea de la columna Nombre de tarea en una vista de tareas:

1. Ir a una lista de tareas.
1. Desde el **Ver** , haga clic en **Nueva vista** para crear una vista nueva.

   O

   Haga clic en **Icono Editar** ![](assets/edit-icon.png)

   para editar una vista existente, seleccione la vista.

1. Clic **Agregar columna** para añadir una nueva columna.

   O

   Haga clic en una columna existente con un vínculo a un objeto.

1. Clic **Cambiar a modo de texto**.
1. Pase el ratón sobre el área de modo de texto y haga clic en **Haga clic para editar el texto**.
1. Elimine el texto que encuentre en la **Modo de texto** y reemplácelo por el siguiente código:
   <pre>displayname=Nombre de tarea<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>valueexpression={name}</strong><br>valueformat=Compound</pre>

   >[!TIP]
   >
   >Puede utilizar un código similar para otros objetos si ajusta lo siguiente:
   >
   >* Reemplace el **valuefield** línea del código con **valueexpression** y mantenga el mismo nombre incluido entre llaves después del signo igual.
   >* Eliminar todas las líneas que comienzan con `link.` del texto original de la columna. Por ejemplo, elimine todas las líneas siguientes:
   >
   >  ```
   >  link.linkproperty.0.name=ID
   >  link.linkproperty.0.valuefield=ID
   >  link.linkproperty.0.valueformat=string
   >  link.lookup=link.view
   >  link.value=val(objCode)
   >  ```
   >

1. Clic **Guardar**, entonces **Guardar vista**.
