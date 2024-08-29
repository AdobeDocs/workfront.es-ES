---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: Compartir una meta en Workfront Goals
description: Cuando comparte una meta, otorga permisos de administración a una meta a alguien que no la ha creado.
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '788'
ht-degree: 4%

---

# Compartir una meta en Adobe Workfront Goals

Cuando comparte una meta, otorga permisos de administración a una meta a alguien que no la ha creado.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> 
   <p>Para el nuevo plan y la estructura de licencias:
  <ul><li>Un plan definitivo </li></ul>
   </p>
<p>Para el plan y la estructura de licencias actuales: 
<ul><li> A Pro o superior </li>
  <li>Una licencia de Adobe Workfront Goals además de una licencia de Workfront.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licencia de Adobe Workfront*</td>
 <td>
 <p>Nueva licencia: Colaborador o superior</p>
 O
 <p>Licencia actual: Solicitud o superior</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Producto*</td>
 <td>
 <p> Nuevo requisito de producto, uno de los siguientes: </p>
<ul>
<li>Un plan Select or Prime Adobe Workfront y una licencia adicional de Adobe Workfront Goals.</li>
<li>Un plan Ultimate Workfront que incluye Workfront Goals de forma predeterminada. </li></ul>
 <p>O</p>
 <p>Requisito de producto actual: un plan de Workfront y una licencia adicional para los objetivos de Adobe Workfront. </p> <p>Para obtener más información, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para usar Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Nivel de acceso</td>
 <td> <p>Editar acceso a Objetivos</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permisos de objeto</td>
 <td>
  <div>
  <p>Ver o permisos superiores a la meta para verla</p>
  <p>Administrar permisos para el objetivo y editarlo</p>
  <p>Para obtener información acerca de cómo compartir metas, vea <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartir una meta en Workfront Goals</a>. </p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área Objetivos en el menú principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Consideraciones acerca de compartir objetivos

* Los usuarios pueden tener los siguientes permisos para una meta:

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Permisos de objetivo</b></p></td> 
      <td>
      <p><b>Descripción</b></p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Ver</p></td> 
      <td>
      <p>Los usuarios tienen permisos para ver la meta, pero no pueden editar información para la meta, no pueden añadir ni editar información para resultados o actividades, actualizar el estado o eliminar la meta.</p>      
      <p>De forma predeterminada, todos los usuarios con acceso a las metas pueden ver todas las metas en el sistema. Los usuarios pueden copiar la meta si tienen acceso de edición a las metas en su nivel de acceso.</p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Administrar</p></td> 
      <td> <p>Los usuarios pueden editar toda la información de la meta, incluidos los resultados, o las actividades, incluso eliminarlos.</p> 
      <p>Solo los creadores de objetivos o los usuarios a los que se les conceda específicamente permisos de Administración de una meta pueden administrar una meta.</p> 
      Solo los usuarios con permisos de Administración de una meta pueden compartir la meta con otros para darles permisos de Administración de la meta. </p> </td> 
   </tr> 
   </tbody> 
   </table>

* Puede compartir los siguientes tipos de objetivos con otros usuarios:

   * Una meta que ha creado
   * Una meta creada por otra persona para la que se le han concedido permisos de administración.

* Si tiene permisos de Administración para una meta, puede cambiar los permisos de la meta para el creador de la meta. De forma predeterminada, tienen permisos de Administración cuando crean el objetivo, pero puede cambiar sus permisos a Vista.

## Compartir una meta

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) > **Metas** en la esquina superior derecha.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../workfront-goals-settings/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Se muestra la Lista de metas.

1. Haga clic en el nombre de una meta en la lista. Se abre la página de la meta.

1. Haga clic en el **icono Más** junto al nombre de la meta y, a continuación, haga clic en **Compartir**.

   ![](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   Se muestra el cuadro Acceso a metas.

   ![](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. Realice una de las siguientes acciones:

   * Seleccione la configuración **Administrar en todo el sistema** para dar permisos de Administración a todos los usuarios del sistema que tengan acceso de Edición a las Metas en su nivel de acceso. De forma predeterminada, esta opción no está seleccionada para todas las metas nuevas.
   * Empiece a escribir el nombre de un usuario al que desee conceder permisos de administración en el cuadro **Dar acceso de administración a**. Seleccione el nombre cuando aparezca en la lista.

     >[!TIP]
     >
     >Solo puede compartir un objetivo con otros usuarios. No puede compartir objetivos con grupos, equipos o su compañía.

1. Haga clic en **Compartir**.

   El objetivo se comparte con los usuarios especificados. Una etiqueta &quot;en todo el sistema&quot; o el nombre de los usuarios que tienen permisos de Administración para la meta se muestran en el campo Acceso a Administrar del panel Detalles de la meta.

## Opciones de permiso de objetivo

En la tabla siguiente se enumeran los permisos que puede conceder al compartir un objetivo. Para obtener más información sobre el acceso que obtienen los usuarios según su licencia, consulte [Conceder acceso a Adobe Workfront Goals](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p><strong>Acciones</strong> </p> </th> 
   <th> <p><strong>Administrar</strong> </p> </th> 
   <th> <p><strong>Vista</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Ver meta</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ver resultados o actividades</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Copiar meta* </td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Convertir resultados o actividades en otros objetivos*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Ver proyectos agregados como actividades** </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Editar meta</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar resultados o actividades</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Añadir resultados o actividades para la meta</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Asocie un proyecto como una actividad a la meta**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Eliminar meta</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Eliminar resultados o actividades</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Desconectar proyectos de la meta</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*Debe tener acceso de edición a las Metas en su nivel de acceso para poder convertir resultados y actividades en metas.

**Debe tener acceso a Ver proyectos y permiso de visualización en los proyectos agregados o que desee agregar al objetivo para verlos.

Para obtener información acerca del nivel de acceso al proyecto, vea [Conceder acceso a proyectos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Para obtener información acerca de los permisos del proyecto, vea [Compartir un proyecto en Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

 
