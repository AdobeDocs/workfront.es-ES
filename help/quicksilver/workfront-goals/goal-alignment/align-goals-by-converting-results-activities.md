---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Alinear metas convirtiendo resultados y actividades en metas
description: Puede alinear manualmente dos metas o convertir los resultados y las actividades de una meta existente en otra meta. El resultado o actividad convertido se transforma en la meta secundaria de la meta original. Para obtener información sobre cómo alinear manualmente dos metas, consulte Alinear metas conectándolas en Adobe Workfront Goals.
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 81%

---

# Alinear metas convirtiendo resultados y actividades en metas

<!--Audited P&P only: 4/2025-->

Puede alinear manualmente dos metas o convertir los resultados y las actividades de una meta existente en otra meta. El resultado o actividad convertido se transforma en la meta secundaria de la meta original. 
Para obtener información acerca de cómo alinear manualmente dos metas, consulte [Alinear metas conectándolas en Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## Requisitos de acceso

>[!NOTE]
>
>Su empresa puede optar por seguir utilizando los objetivos de Adobe Workfront si compró este paquete anteriormente. Debe hablar con el representante de su cuenta para obtener más detalles.
>
>Adobe Workfront Goals ya no se puede adquirir.

+++Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<td> <p>paquete de Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>Licencia de Adobe Workfront</p> </td> 
   <td> <p>Colaborador o superior</p> 
     <p>Solicitante o superior</p> </td> 
  </tr>

<td><p>Configuraciones de nivel de acceso</p> </td> 
   <td> <p>Editar acceso a Goals</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permisos de objeto </p> </td> 
   <td> <p>Administración de permisos para una meta</p>  </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores del sistema, se les debe asignar una plantilla de diseño que incluya el área Objetivos en el menú principal. </p>  
</td>
  </tr>
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso a la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   Or
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

Debe tener lo siguiente para poder comenzar:

* Una meta existente con resultados y actividades existentes.

  Para obtener información sobre cómo crear metas, consulte [Crear metas en Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Una meta puede tener hasta 1 000 indicadores de progreso.

<!--drafted for goal redesign: At PRODUCTION: update the sentence above to remove Production/ Preview references-->

## Consideraciones al convertir resultados y actividades en metas

A veces, un resultado o una actividad pueden tener un ámbito más amplio de lo previsto y sería más lógico que se convirtieran en metas. Puede convertir los resultados y las actividades de una meta existente en una nueva meta. Se trata de un enfoque ascendente para alinear las metas.

Tenga en cuenta lo siguiente al convertir resultados y actividades en metas:

* El resultado o la actividad convertidos pasan a ser la meta secundaria de la original y las dos se alinean.
* La meta recién creada se convierte en el único indicador de progreso para la original, si no hay más resultados o actividades en ella. Debe agregar resultados y actividades a la meta secundaria para poder rastrear el progreso en ella.
* La conversión de un resultado o actividad en una meta es irreversible. Una vez convertida, la nueva meta secundaria no puede volver a convertirse en un resultado o actividad para la principal.

## Conversión de un resultado o actividad en una meta

<!--
<span class="preview">Converting results and activities differs depending on what environment you use. </span>

### Convert a result or activity to a goal in the Production environment

1. Go to a goal that has a result or an activity that you want to convert to a goal.
1. Click the name of the goal to open the **Goal Details** panel.
1. Expand the **Results** or **Activities** right-pointing arrows to see a list of results or activities for the goal. 

1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the result or activity name that you want to convert, then click **Convert into a Goal**.

   ![Convert to goal](assets/convert-to-goal-link-highlighted-350x191.png)

1. (Optional) Remove the name of the original activity or result owner from the **Goal Owner** field and replace it with another user, team, group, or your organization's name. By default, Workfront selects the owner of the result or the activity as the goal owner. 
1. Click **Convert**. The activity or result displays as an aligned goal in the Goal Details panel of the original goal and the original activity or result is removed from the original goal and transferred to the second goal. By default, the new goal has the same name as the original converted result or activity. 
1. (Optional) Click the name of the new goal to open the **Goal Details** panel and edit the name of the goal. For information about editing any information for an existing goal, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
-->

1. Vaya a una meta que tenga un resultado o a una actividad que desee convertir en una meta.
1. En la página de la meta, haga clic en **Indicadores de progreso** en el panel izquierdo.
1. Seleccione un resultado o una actividad en la lista de indicadores de progreso y, a continuación, haga clic en el icono **Convertir en meta** ![Convertir en meta](assets/convert-to-goal-icon-unshimmed.png) en la parte superior de la lista de indicadores de progreso. Se abre el cuadro Convertir en meta.

   ![Convertir en cuadro de metas](assets/convert-to-goal-box-unshimmed.png)
1. Actualice la siguiente información:
   * **Nombre de la meta**: de forma predeterminada, la nueva meta tiene el mismo nombre que el resultado o actividad original.
   * **Período**: de manera predeterminada, el período de la nueva meta es el trimestre actual. Puede seleccionar la configuración **Habilitar fechas personalizadas** para definir un período de tiempo personalizado para la nueva meta.
   * **Propietario de la meta**: de forma predeterminada, el nuevo propietario de la meta es el propietario de la actividad o el resultado original.
   * **Descripción**: añade más información sobre la nueva meta.
1. Haga clic en **Guardar**

   El resultado o la actividad se convierte ahora en una meta secundaria de la meta original. Se enumera como una meta en la lista Indicadores de progreso de la meta original.



