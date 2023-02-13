---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Agrupación: editar el nombre para mostrar en una agrupación"
description: Puede cambiar el nombre de las agrupaciones por otro más familiar para los usuarios.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# Agrupación: editar el nombre para mostrar en una agrupación

Puede cambiar el nombre de las agrupaciones por otro más familiar para los usuarios.

Por ejemplo, al aplicar la agrupación Nombre de Portfolio estándar a una lista de proyectos, el nombre de la agrupación aparece como *Portfolio: Nombre:`<name of portfolio>`*.

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

## Edición del nombre para mostrar en una agrupación

Para cambiar el nombre para mostrar en una agrupación de proyectos:

1. Vaya a una lista de proyectos.
1. En el **Agrupación** menú desplegable, seleccione **Nuevo grupo**.

1. Haga clic en **Agregar agrupación** y empiece a escribir &quot;Nombre del Portfolio&quot; en la **Primero por:** y selecciónelo cuando aparezca en la lista.

1. Haga clic en **Cambiar al modo de texto**.
1. Se ha realizado una de las siguientes acciones:

   * Agregue el siguiente código al texto existente disponible en la sección **Agrupar su informe** cuadro:

      ```
      group.0.displayname=Your
      ```

      ```
      Value
      ```

      O, en este caso:

      ```
      group.0.displayname=Portfolio
      ```

   * Elimine todas las líneas de la interfaz de modo de texto de la agrupación que contengan la palabra &quot;nombre&quot; y, a continuación, añada la línea:

      ```
      group.0.name=Your Value
      ```

      O, en este caso:

      ```
      group.0.name=Portfolio
      ```

      También puede dejar el

      ```
      group.0.name
      ```

      línea en blanco, en cuyo caso la agrupación muestra el nombre del valor que está agrupando.

      ![](assets/grouping-edited-name-no-name-350x162.png)

1. Haga clic en **Listo**, luego **Guardar agrupación**.
