---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Alinee metas conectándolas en Adobe Workfront Goals
description: Si usted es un colaborador individual que tiene un objetivo personal, es posible que desee alinearlo con los objetivos de su equipo para mostrar de forma eficaz el progreso de su propia meta en el contexto más amplio de la estrategia de su organización.
author: Alina
feature: Workfront Goals
exl-id: 4276f1c9-2ee9-4f74-b011-ae1e19fefe35
source-git-commit: 330ee20ad14ea7409db1c6f627ed6aa0e0c5c014
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 1%

---

# Alinee metas conectándolas en Adobe Workfront Goals

Si usted es un colaborador individual que tiene un objetivo personal, es posible que desee alinearlo con los objetivos de su equipo para mostrar de forma eficaz el progreso de su propia meta en el contexto más amplio de la estrategia de su organización.

Cuando todos los miembros de su organización tienen sus objetivos alineados con los objetivos de su organización, pueden ver claramente cómo sus contribuciones individuales y los esfuerzos de equipo ayudan a avanzar en las prioridades más grandes a nivel de empresa. Para obtener más información acerca de las prácticas recomendadas para alinear metas, consulte [Resumen de alineación de metas en Adobe Workfront Goals](../../workfront-goals/goal-alignment/goal-alignment-overview.md).

Existen dos métodos para conectar objetivos en Adobe Workfront Goals:

* Puede crear alineación entre los objetivos conectando los objetivos entre sí.

* Puede alinear manualmente dos metas o convertir los resultados y las actividades de una meta existente a otra meta. El resultado o la actividad convertidos se convierten en el objetivo secundario del objetivo original.

>[!IMPORTANT]
>
>Una meta puede tener un total de 1000 indicadores de progreso.

Este artículo describe cómo puede alinear los objetivos conectándolos entre sí. Para obtener información sobre cómo alinear metas convirtiendo resultados y actividades en metas, vea [Alinear metas convirtiendo resultados y actividades en metas](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">plan de Adobe Workfront</td>
 <td>
 <p>Cualquiera</p>

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
 <tr>
 <td role="rowheader">Permisos de objeto</td>
 <td>

<p>Ver o permisos superiores a la meta para verla</p>
  <p>Administrar permisos para el objetivo y editarlo</p>
  <p>Para obtener información acerca de cómo compartir metas, vea <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartir una meta en Workfront Goals</a>. </p>
   </td>
 </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área Objetivos en el menú principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Alinear metas conectándolas entre sí

<!--
Aligning goals by connecting them differs depending on what environment you use. 

### Align goals by connecting them in the Production environment

1. Create two goals that you want to align. For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).
1. (Optional) Activate the goals that you want to align. You can align goals that have a Draft, Active, or Inactive status. For information about activating goals, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).
1. Go to the goal that you want to align (child goal) to another goal (parent goal) and click its name to open the **Goal Details** panel.

   For example, if you want Goal 2 to influence the progress of Goal 1, you must go to Goal 2. 

1. Click **Align to another goal** in the upper-right corner of the right panel.

   ![](assets/align-to-another-goal-link-highlighted-350x128.png)

1. Start typing the name of an existing goal or the name of an owner in the **Align to another goal** field, then select it when it appears in the list. Only goals that are from the same or future periods display in the list. 
1. Click **Save**.

   The goal you started with (Goal 2) is now the child goal of the goal you aligned it with (Goal 1).   
   The aligned goals display connected in the Goal Alignment section with Goal 2 as secondary to Goal 1.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Optional) To view the goals in the Goal Alignment section, do one of the following:

   * Click the Goal Alignment section in the left panel and find the goals by applying the correct filter. For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).
   * Click the Goal List, Check-in, or Pulse sections in the left panel and find one of the goals, then click the **Alignment icon** ![](assets/align-icon.png) next to the goal name to go directly to the goal in the Goal Alignment section.

   For information about the Goal Alignment section, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md). 

1. (Optional) Add activities and results to either goal to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Optional) Remove the alignment between two goals, when you consider that no longer is relevant to your organization's overall strategy For information about removing alignment between goals, see [Remove goal alignment in Adobe Workfront Goals](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

-->
1. Cree dos metas que desee alinear. Para obtener información sobre cómo crear metas, consulte [Crear metas en Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).
1. (Opcional) Active las metas que desee alinear. Puede alinear metas que tengan un estado Borrador, Activo o Inactivo. Para obtener información sobre cómo activar metas, consulte [Activar metas en Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).
1. Vaya a la meta que desea alinear (meta secundaria) con otra meta (meta principal) y haga clic en su nombre para abrir la página de meta.

   >[!INFO]
   >
   >Por ejemplo, si desea que el Objetivo 2 influya en el progreso del Objetivo 1, debe ir al Objetivo 2.

1. Haga clic en **Detalles de la meta** en el panel izquierdo.

1. En el área **Información sobre la meta principal**, haga clic en **Agregar** en el campo **Meta principal** si no hay ninguna meta principal,

   O

   Haga clic en el nombre de la meta principal para elegir otra.

1. Empiece a escribir el nombre de una meta existente en el campo **Meta principal** y selecciónela cuando aparezca en la lista. En la lista solo se muestran las metas que son del mismo periodo o de periodos futuros.

1. Haga clic en **Guardar cambios**.

   La meta con la que comenzó (Meta 2) ahora es la meta secundaria de la meta principal con la que la alineó (Meta 1).\
   Las metas alineadas se muestran conectadas en la sección Alineación de metas con la meta 2 como secundaria a la meta 1.
La meta secundaria se muestra en la sección Indicadores de progreso de la meta principal a medida que su progreso actualiza el progreso de la meta principal.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Opcional) Para ver los objetivos en la sección Alineación de objetivos, vaya al área Objetivos de Workfront y, a continuación, haga clic en la sección **Alineación de objetivos** del panel izquierdo. Para obtener información acerca de la sección Alineación de metas, vea [Desplazarse por la sección Alineación de metas en Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).

1. (Opcional) Añada actividades y resultados a cualquiera de los objetivos para indicar su progreso. Para obtener información sobre cómo agregar actividades y resultados, consulte los siguientes artículos:

   * [Agregar actividades a metas en Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
   * [Añadir resultados a metas en Objetivos de Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Opcional) Elimine la alineación entre dos objetivos, cuando considere que ya no es relevante para la estrategia general de su organización. Para obtener información acerca de cómo quitar la alineación entre metas, vea [Quitar la alineación entre metas en Adobe Workfront Goals](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

