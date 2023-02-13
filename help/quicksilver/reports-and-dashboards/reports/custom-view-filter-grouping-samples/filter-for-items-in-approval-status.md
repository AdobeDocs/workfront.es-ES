---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: mostrar solo los elementos en un estado de aprobación'
description: Solo se pueden mostrar elementos con un estado determinado que se encuentre en Pendiente de aprobación. Esto funciona igual para cualquier otro objeto con un estado de aprobación.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 1%

---

# Filtro: mostrar solo los elementos en un estado de aprobación

Solo se pueden mostrar elementos con un estado determinado que se encuentre en Pendiente de aprobación. Esto funciona igual para cualquier otro objeto con un estado de aprobación.

Puede colocar los siguientes objetos en un estado de aprobación:

* Tareas
* Problemas
* Proyectos

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

## Mostrar solo los elementos en estado de aprobación

1. Vaya al filtro que desea personalizar para una lista de proyectos, por ejemplo.
1. Haga clic en **Agregar una regla de filtro** para el **Estado** del objeto de la lista.\
   Por ejemplo, en un informe de proyecto, agregue **Situación de la planificación**, si solo desea mostrar proyectos que estén en estado de **Planificación: pendiente de aprobación**.

1. Haga clic en **Cambiar al modo de texto**.
1. Modifique el

   ```
   status
   ```

   línea añadiendo **:A** a la clave de 3 letras del estado:
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Haga clic en **Listo**, luego **Guardar filtro**.

   La lista muestra solo los proyectos que están en estado Planning - Pending Approval.
