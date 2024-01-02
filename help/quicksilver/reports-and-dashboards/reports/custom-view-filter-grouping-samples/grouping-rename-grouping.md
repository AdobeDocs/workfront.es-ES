---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Agrupación: editar el nombre para mostrar en una agrupación"
description: Puede cambiar el nombre de las agrupaciones en listas e informes por otro más familiar para los usuarios.
author: Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 138181de2ad8257785773a5296bc5bcfc144a801
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# Grouping: editar el nombre para mostrar en una agrupación

<!--Audited: 01/2024-->

Puede cambiar el nombre de las agrupaciones por otro más familiar para los usuarios.

Por ejemplo, cuando se aplica la agrupación Nombre de Portfolio estándar a una lista de proyectos, el nombre de la agrupación aparece como *Portfolio: Nombre:`<name of portfolio>`*.

![](assets/grouping-unedited-name-350x167.png)

Puede modificar esta agrupación mediante el modo de texto para mostrar un nombre que sea más fácil de leer.

![](assets/grouping-edited-name-350x160.png)

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
   <td>

<p>Nuevo: </p>
   <ul>
   <li> <p>Colaborador para modificar una agrupación </p></li>
   <li><p>Estándar para modificar un informe</p></li></ul>

<p> Actual:</p>
   <ul>  
   <li><p>Solicitud para modificar una agrupación </p></li>
   <li><p>Plan para modificar un informe</p></li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar una agrupación</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Editar el nombre para mostrar en una agrupación

Para cambiar el nombre para mostrar en una agrupación de proyectos:

1. Ir a una lista de proyectos.
1. Desde el **Agrupación** menú desplegable, seleccione **Nueva agrupación**.

1. Clic **Agregar agrupación** y empiece a escribir &quot;Nombre de Portfolio&quot; en **Primero por:** y, a continuación, selecciónelo cuando se muestre en la lista.

1. Clic **Cambiar a modo de texto**.
1. Realice una de las siguientes acciones:

   * Agregue el código siguiente al texto existente disponible en la **Agrupar el informe** cuadro:


     `group.0.displayname=Your Value`


     O, en este caso:

     `group.0.displayname=Portfolio`

   * Elimine todas las líneas de la interfaz de modo de texto de la agrupación que tengan la palabra &quot;name&quot; y, a continuación, añada la línea:

     `group.0.name=Your Value`

     O, en este caso:

     `group.0.name=Portfolio`

     >[!TIP]
     >
     >También puede dejar el `group.0.name=` y el `group.0.displayname=` líneas en blanco, en cuyo caso la agrupación muestra el valor por el que está agrupando.


     ![](assets/grouping-edited-name-no-name-350x162.png)

1. Clic **Listo**, entonces **Guardar agrupación**.

   El nombre predeterminado de la agrupación se modifica según la información del modo de texto.
