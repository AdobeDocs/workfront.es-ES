---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ver: mostrar la relación principal-secundario en una tarea sangrando las tareas"
description: Puede mantener la distinción de relaciones principal-secundario en una lista de tareas exportada agregando una vista personalizada a la lista de tareas y asegurándose de que esta vista esté seleccionada antes de exportar la lista.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 0483230c5d8b7d33f420c6c5f09c4a5aafe37f37
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 2%

---

# Ver: muestra la relación principal-secundario en una tarea sangrando las tareas

Puede mantener la distinción de relaciones principal-secundario en una lista de tareas exportada agregando una vista personalizada a la lista de tareas y asegurándose de que esta vista esté seleccionada antes de exportar la lista.

![](assets/parent-child-indented-custom-view-350x94.png)

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

## Mostrar la relación principal-secundario en una tarea sangrando las tareas

1. Vaya al proyecto con la lista de tareas que desee exportar.
1. Haga clic en el menú desplegable **Vista** y seleccione **Nueva vista**.

1. Nombre el filtro en la esquina superior izquierda de la pantalla.
1. Haga clic en el encabezado de columna **Nombre de tarea**.

1. Seleccione **Cambiar al modo de texto** en la esquina superior derecha.
1. Haga clic en cualquier lugar del cuadro de texto para editar el texto y quitar todo el texto existente.
1. Pegue el siguiente texto:


```
   displayname=
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))
   valueformat=HTML
```

1. Haga clic en **Guardar**.
1. Pulse **Guardar vista**.
