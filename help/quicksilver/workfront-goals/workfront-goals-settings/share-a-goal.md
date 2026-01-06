---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: Compartir una meta en Workfront Goals
description: Cuando se comparte una meta, se otorgan permisos de administración a una meta a alguien que no la creó.
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 91%

---

# Compartir metas en Adobe Workfront Goals

Cuando se comparte una meta, se otorgan permisos de administración a una meta a alguien que no la creó.

## Requisitos de acceso

>[!NOTE]
>
>Su empresa puede optar por seguir utilizando los objetivos de Adobe Workfront si compró este paquete anteriormente. Debe hablar con el representante de su cuenta para obtener más detalles.
>
>Adobe Workfront Goals ya no se puede adquirir.

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Paquete de Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licencia de Adobe Workfront</td>
 <td>
 <p>Colaborador o superior</p>
<p>Solicitud o superior</p></td>
 </tr>
  <tr>
 <td role="rowheader">Configuración de nivel de acceso</td>
 <td> <p>Editar acceso a Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permisos de objeto</td>
 <td>
  <div>
  <p>Permisos Ver o superiores para la meta que desea ver</p>
  <p>Permisos de administración para la meta y poder editarla</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores del sistema, se les debe asignar una plantilla de diseño que incluya el área Objetivos en el menú principal. </p>  
</td>
  </tr>
</tbody>
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
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
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Consideraciones acerca del uso compartido de metas

* Los usuarios pueden tener los siguientes permisos para una meta:

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Permisos de la meta</b></p></td> 
      <td>
      <p><b>Descripción</b></p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Ver</p></td> 
      <td>
      <p>Los usuarios tienen permiso para ver la meta, pero no pueden editar su información, ni añadir o editar información de resultados o actividades, actualizar el estado o eliminar la meta.</p>      
      <p>De forma predeterminada, todos los usuarios que tengan acceso a las metas podrán ver todas las metas del sistema. Los usuarios podrán copiar la meta en caso de tener acceso de edición a las metas en su nivel de acceso.</p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Administrar</p></td> 
      <td> <p>Los usuarios podrán editar toda la información de la meta, incluyendo los resultados o las actividades, incluyendo la eliminación.</p> 
      <p>Solo los creadores de metas o los usuarios a los que se les concedan específicamente permisos de administración de una meta podrán administrar una meta.</p> 
      Solo los usuarios con permisos de administración de una meta podrán compartir la meta con otros para darles permisos de administración de la misma. </p> </td> 
   </tr> 
   </tbody> 
   </table>

* Es posible compartir los siguientes tipos de metas con otros usuarios:

   * Una meta que creó
   * Una meta creada por otra persona para la que se le concedieron permisos de administración.

* Si se tienen permisos de administración de una meta, es posible cambiarlos para el creador de la meta. De forma predeterminada, se tienen permisos de administración cuando se crea la meta, pero es posible cambiarlos a Vista.

## Compartir una meta

{{step1-to-goals}}

Se muestra la lista de metas.

1. Haga clic en el nombre de una meta de la lista. Se abre la página de la meta.

1. Haga clic en el **icono Más** que hay junto al nombre de la meta y, a continuación, haga clic en **Compartir**.

   ![Menú Más](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   Se muestra la casilla de acceso a la meta.

   ![Acceso a la meta](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. Realice una de las siguientes acciones:

   * Seleccione la configuración **Administrar todo el sistema** para otorgar permisos de administración a todos los usuarios del sistema que tengan acceso de edición a la metas a través de sus niveles de acceso. De forma predeterminada, esta opción no está seleccionada para todas las metas nuevas.
   * Comience a escribir el nombre de un usuario al que quiera proporcionar permisos de Administración en la casilla **Otorgar acceso de administración a**. Seleccione el nombre cuando aparezca en la lista.

     >[!TIP]
     >
     >Solo es posible compartir una meta con otros usuarios. No es posible compartir metas con grupos, equipos o compañías. 

1. Haga clic en **Compartir**.

   La meta se comparte con los usuarios especificados. Una etiqueta “para todo el sistema” o los nombres de los usuarios que tienen permisos de administración para la meta se muestran en el campo Acceso a la administración en el panel Detalles de la meta.

## Opciones de permisos de metas

En la tabla siguiente se enumeran los permisos que se pueden conceder al compartir metas. Para obtener más información sobre el acceso que obtienen los usuarios según su licencia, consulte [Conceder acceso a Adobe Workfront Goals](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

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
   <td>Convertir resultados o actividades en otras metas*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Ver proyectos añadidos como actividades** </td> 
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
   <td> </td> 
  </tr> 
  <tr> 
   <td>Añadir resultados o actividades para la meta</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Asociar un proyecto como una actividad a la meta**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Eliminar meta</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Eliminar resultados o actividades</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Desconectar proyectos de la meta</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*Es necesario tener acceso de edición a las metas en su nivel de acceso para poder convertir resultados y actividades en metas.

**Es necesario tener acceso de visualización de proyectos y permisos de visualización en los proyectos añadidos o que quiera añadir a la meta para verlos.

Para obtener información acerca del nivel de acceso de proyectos, consulte [Conceder acceso a proyectos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Para obtener información acerca de los permisos de proyectos, consulte [Uso compartido de proyectos en Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).


