---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Alinear objetivos convirtiendo resultados y actividades en objetivos
description: Puede alinear manualmente dos objetivos o puede convertir los resultados y las actividades de un objetivo existente en otro objetivo. El resultado o la actividad convertidos se convierte en el objetivo secundario del objetivo original. Para obtener información sobre la alineación manual de dos objetivos, consulte Alinear objetivos conectándolos en objetivos de Adobe Workfront.
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# Alinear objetivos convirtiendo resultados y actividades en objetivos

Puede alinear manualmente dos objetivos o puede convertir los resultados y las actividades de un objetivo existente en otro objetivo. El resultado o la actividad convertidos se convierte en el objetivo secundario del objetivo original.
Para obtener información sobre la alineación manual de dos objetivos, consulte [Alinear objetivos conectándolos en los objetivos de Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## Requisitos de acceso


<!--drafted for P&P release: 

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
   <td> <p>Editar acceso a Objetivos o posterior</p> <p><b>NOTA</b> 
   <p>Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte:</p> 
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
     <p>Para obtener información sobre cómo compartir objetivos, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartir un objetivo en los objetivos de Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Debe tener lo siguiente para poder iniciar:

* Plantilla de diseño que incluye el área Objetivos del menú principal.
* Un objetivo existente con resultados y actividades existentes.

   Para obtener información sobre la creación de objetivos, consulte [Crear objetivos en objetivos de Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Un objetivo puede tener hasta 1000 indicadores de progreso.

<!--drafted for goal redesign: At PRODUCTION: update the sentence above to remove Production/ Preview references-->

## Consideraciones al convertir resultados y actividades en objetivos

A veces, un resultado o una actividad pueden tener un alcance mayor del previsto y tendría más sentido que se convirtieran en objetivos. Puede convertir los resultados y las actividades de un objetivo existente en un nuevo objetivo. Se trata de un enfoque ascendente para alinear los objetivos.

Tenga en cuenta lo siguiente al convertir resultados y actividades en objetivos:

* El resultado o la actividad convertidos se convierte en el objetivo secundario del objetivo original y los dos objetivos se alinean.
* El objetivo recién creado se convierte en el único indicador de progreso para el objetivo original, si no hay más resultados o actividades en el objetivo original. Debe agregar resultados y actividades al objetivo secundario para poder rastrear el progreso en él.
* La conversión de un resultado o actividad en un objetivo es irreversible. Una vez convertido, el nuevo objetivo secundario no puede volver a convertirse en un resultado o actividad para el objetivo principal.

## Conversión de un resultado o actividad en un objetivo

<!--
<span class="preview">Converting results and activities differs depending on what environment you use. </span>

### Convert a result or activity to a goal in the Production environment

1. Go to a goal that has a result or an activity that you want to convert to a goal.
1. Click the name of the goal to open the **Goal Details** panel.
1. Expand the **Results** or **Activities** right-pointing arrows to see a list of results or activities for the goal. 

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name that you want to convert, then click **Convert into a Goal**.

   ![](assets/convert-to-goal-link-highlighted-350x191.png)

1. (Optional) Remove the name of the original activity or result owner from the **Goal Owner** field and replace it with another user, team, group, or your organization's name. By default, Workfront selects the owner of the result or the activity as the goal owner. 
1. Click **Convert**. The activity or result displays as an aligned goal in the Goal Details panel of the original goal and the original activity or result is removed from the original goal and transferred to the second goal. By default, the new goal has the same name as the original converted result or activity. 
1. (Optional) Click the name of the new goal to open the **Goal Details** panel and edit the name of the goal. For information about editing any information for an existing goal, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
-->

1. Vaya a un objetivo que tenga un resultado o una actividad que desee convertir en un objetivo.
1. En la página del objetivo, haga clic en **Indicadores de progreso** en el panel izquierdo.
1. Seleccione un resultado o una actividad en la lista de indicadores de progreso y, a continuación, haga clic en el botón **Convertir en objetivo** icono ![](assets/convert-to-goal-icon-unshimmed.png) en la parte superior de la lista de indicadores de progreso. Se abre el cuadro de objetivo Convertir en .

   ![](assets/convert-to-goal-box-unshimmed.png)
1. Actualice la siguiente información:
   * **Nombre del objetivo**: De forma predeterminada, el nuevo objetivo tiene el mismo nombre que el resultado o la actividad originales.
   * **Periodo**: De forma predeterminada, el período del nuevo objetivo es el trimestre actual. Puede seleccionar el **Habilitar fechas personalizadas** para definir un período de tiempo personalizado para el nuevo objetivo.
   * **Propietario del objetivo**: De forma predeterminada, el nuevo propietario del objetivo es el propietario del resultado o actividad original.
   * **Descripción**: Agregue más información sobre el nuevo objetivo.
1. Haga clic en **Guardar**

   El resultado o la actividad ahora se convierte en un objetivo secundario del objetivo original. Se incluye como objetivo en la lista de indicadores de progreso del objetivo original.



