---
product-previous: workfront-goals
navigation-topic: goal-management
title: Activar metas en Adobe Workfront Goals
description: Al crear una meta, Adobe Workfront Goals la guarda con el estado de Borrador. Las metas esbozadas no forman parte de la administración de metas.
author: Alina
feature: Workfront Goals
exl-id: fc556073-fe63-4f13-a313-505ca0ef1f9b
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 79%

---

# Activar metas en Adobe Workfront Goals

<!--Audited for P&P only: 4/2025-->

Al crear una meta, Adobe Workfront Goals la guarda con el estado de Borrador. Las metas esbozadas no forman parte de la administración de metas.

Para realizar un seguimiento de lo cerca que está de lograr una meta actualizando su progreso, debe activarla. Esto cambia su estado a Activo.

Para obtener información sobre cómo crear una meta, consulte [Crear metas en Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Debe activar una meta antes de poder actualizar el progreso de sus resultados y actividades.


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
  <td> <p>paquete de Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr> 
  <tr>
 <td role="rowheader">Configuraciones de nivel de acceso</td>
 <td> <p>Editar acceso a Goals</p> </td>
 </tr>
 <tr>
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
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
  <p> New product requirement: Workfront</p>
 <p>Or</p>
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
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

## Requisitos previos

Para activar una meta, es necesario que esté asociada a un indicador de progreso, como una actividad, resultado, proyecto o que esté alineada con otra meta activa.

Realice al menos una de las siguientes acciones para poder activar una meta:

* Añadir un resultado a la meta

  Para obtener más información, consulte [Añadir resultados a metas en Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* Añadir una actividad a la meta

  Para obtener más información, consulte [Añadir actividades a metas en Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

* Conectar un proyecto a la meta

  Para obtener más información, consulte [Añadir proyectos a metas en Adobe Workfront Goals](../results-and-activities/connect-projects-to-goals-overview.md).

* Alinee otra meta con la meta que desee activar

  Para obtener más información, consulte [Alinear metas conectándolas en Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## Activar metas

Puede activar las metas que ha creado o una meta para la que tenga permisos de administración.

1. Vaya a la meta que desee activar. Se abre la página de la meta.

1. Haga clic en el icono **Más** del menú ![Más](../goal-management/assets/more-icon.png) a la derecha del nombre de la meta y luego haga clic en **Activar**.

   ![Menú más expandido](assets/more-menu-on-goal-expanded-with-activate-unshimmed.png)

   El estado de la meta cambia a Activo. Ahora puede realizar un seguimiento del progreso en la meta, y esta se muestra en la sección Proteger y se tiene en cuenta en las secciones de gráficos de Workfront Goals
