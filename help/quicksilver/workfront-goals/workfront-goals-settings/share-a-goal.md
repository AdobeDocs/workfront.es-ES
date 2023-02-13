---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: Compartir un objetivo en los objetivos de Workfront
description: Cuando comparte un objetivo, concede permisos de administración a un objetivo a alguien que no lo haya creado.
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 2%

---

# Compartir un objetivo en los objetivos de Adobe Workfront

Cuando comparte un objetivo, concede permisos de administración a un objetivo a alguien que no lo haya creado.

## Requisitos de acceso

<!--drafted - replace the table below with this one when P&P releases: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>
-->

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Pro o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Información general sobre las licencias de Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>Debe adquirir una licencia adicional para los objetivos de Adobe Workfront para acceder a la funcionalidad que se describe en este artículo. </p> <p>Para obtener más información, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para utilizar los objetivos de Workfront</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Objetivos o posterior</p> <p><b>NOTA</b><p>Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Conceder acceso a los objetivos de Adobe Workfront</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> 
    <div> 
     <p>Administrar permisos para el objetivo</p> 
     <p>Para obtener información sobre cómo compartir objetivos, consulte <a href="#" class="MCXref xref selected">Compartir un objetivo en los objetivos de Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Antes de comenzar, debe tener lo siguiente:

* Plantilla de diseño que incluye el área Objetivos del menú principal.

## Consideraciones sobre los objetivos de uso compartido

* Los usuarios pueden tener los siguientes permisos para un objetivo:

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
      <td role="rowheader"><p>Vista</p></td> 
      <td>
      <p>Los usuarios tienen permisos para ver el objetivo, pero no pueden editar información para el objetivo, no pueden agregar o editar información para resultados o actividades, actualizar estado o eliminar el objetivo.</p>      
      <p>De forma predeterminada, todos los usuarios con acceso a Objetivos pueden ver todos los objetivos del sistema. Los usuarios pueden copiar el objetivo si tienen acceso de edición a Objetivos en su nivel de acceso.</p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Administrar</p></td> 
      <td> <p>Los usuarios pueden editar toda la información del objetivo, incluso para los resultados o las actividades, incluso eliminarlas.</p> 
      <p>Solo los creadores de objetivos o usuarios a los que se hayan concedido permisos de administración específicos para un objetivo pueden administrar un objetivo.</p> 
      Solo los usuarios con permisos de administración para un objetivo pueden compartir el objetivo con otros para darles permisos de administración para el objetivo. </p> </td> 
   </tr> 
   </tbody> 
   </table>

* Puede compartir los siguientes tipos de objetivos con otros:

   * Un objetivo que ha creado
   * Un objetivo creado por otra persona a la que se le han otorgado permisos para administrar.

* Si tiene permisos de administración para un objetivo, puede cambiar los permisos en el objetivo para el creador de objetivos. De forma predeterminada, tienen permisos de gestión cuando crean el objetivo, pero puede cambiar sus permisos a Vista.

## Compartir un objetivo

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) > **Objetivos** en la esquina superior derecha.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../workfront-goals-settings/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Se muestra la lista de objetivos.

1. Haga clic en el nombre de un objetivo de la lista. Se abre la página de objetivo.

1. Haga clic en el **Más icono** junto al nombre del objetivo y haga clic en **Compartir**.

   ![](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   Se muestra el cuadro Acceso a objetivo .

   ![](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. Realice una de las siguientes acciones:

   * Seleccione el **Administrar en todo el sistema** para conceder permisos de administración a todas las personas del sistema que tengan acceso de edición a Objetivos en su nivel de acceso. De forma predeterminada, esta opción no está seleccionada para todos los objetivos nuevos.
   * Comience a escribir el nombre de un usuario al que desee otorgar permisos de administración en la **Dar acceso a Administrar a** en la ventana Seleccione el nombre cuando aparezca en la lista.

      >[!TIP]
      >
      >Solo puede compartir un objetivo con otros usuarios. Los objetivos no se pueden compartir con grupos, equipos o empresas.

1. Haga clic en **Compartir**.

   El objetivo se comparte con los usuarios especificados. En el campo Acceso a administración del panel Detalles del objetivo , se muestra una etiqueta &quot;para todo el sistema&quot; o el nombre de los usuarios que tienen permisos de administración para el objetivo.

## Opciones de permiso de objetivo

En la tabla siguiente se enumeran los permisos que puede conceder al compartir un objetivo. Para obtener más información sobre el acceso que los usuarios obtienen en función de su licencia, consulte [Conceder acceso a los objetivos de Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

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
   <td> <p>Ver objetivo</p> </td> 
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
   <td>Agregar resultados o actividades para el objetivo</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Asociar un proyecto como actividad al objetivo**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Eliminar objetivo</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Eliminar resultados o actividades</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Desconectar proyectos del objetivo</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*Debe tener acceso de edición a objetivos en el nivel de acceso para poder convertir resultados y actividades en objetivos.

**Debe tener acceso a Ver proyectos y Ver permisos para los proyectos agregados o que desee agregar al objetivo para verlos.

Para obtener información sobre el nivel de acceso al proyecto, consulte [Concesión de acceso a proyectos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Para obtener información sobre los permisos del proyecto, consulte [Uso compartido de un proyecto en Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

 
