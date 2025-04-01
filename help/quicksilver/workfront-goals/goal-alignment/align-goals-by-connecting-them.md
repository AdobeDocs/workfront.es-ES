---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Alinear metas conectándolas en Adobe Workfront Goals
description: Si es un colaborador individual que tiene una meta personal, tal vez desee alinearla con las metas de su equipo para mostrar de forma eficaz el progreso de su propia meta en el contexto más amplio de la estrategia de su organización.
author: Alina
feature: Workfront Goals
exl-id: 4276f1c9-2ee9-4f74-b011-ae1e19fefe35
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 95%

---

# Alinear metas conectándolas en Adobe Workfront Goals

<!--Audited P&P only: 04/2025-->

Si es un colaborador individual que tiene una meta personal, tal vez desee alinearla con las metas de su equipo para mostrar de forma eficaz el progreso de su propia meta en el contexto más amplio de la estrategia de su organización.

Cuando todos los de su organización tienen sus metas alineadas con las de su organización, pueden ver claramente cómo sus aportaciones individuales y los esfuerzos de equipo ayudan a avanzar en las prioridades más amplias a nivel de la compañía. Para obtener más información sobre las prácticas recomendadas para alinear metas, consulte [Información general sobre la alineación de metas en Adobe Workfront Goals](../../workfront-goals/goal-alignment/goal-alignment-overview.md).

Existen dos métodos para conectar metas en Adobe Workfront Goals:

* Puede crear alineación entre metas conectándolas entre sí.

* Puede alinear manualmente dos metas o puede convertir los resultados y las actividades de una meta existente a otra. El resultado o actividad convertido se transforma en la meta secundaria de la meta original. 

>[!IMPORTANT]
>
>Una meta puede tener un total de 1000 indicadores de progreso.

En este artículo se describe cómo puede alinear metas conectándolas entre sí. Para obtener información sobre cómo alinear metas convirtiendo resultados y actividades en metas, consulte [Alinear metas convirtiendo resultados y actividades en metas](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Plan de Adobe Workfront*</td>
 <td> 
   <p>Para la nueva estructura de plan y licencias:
  <ul><li>Un plan Ultimate </li></ul>
   </p>
<p>Para la estructura actual de plan y licencias: 
<ul><li> Pro o superior </li>
  <li>Una licencia de Adobe Workfront Goals además de una licencia de Workfront.</li></ul></p>
   </td> 
 </tr>
 <tr>
 <td role="rowheader">Licencia de Adobe Workfront*</td>
 <td>
 <p>Nueva licencia: Contributor o superior</p>
 O
 <p>Licencia actual: Request o superior</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Producto*</td>
 <td>
  <p> Nuevo requisito de producto: Workfront</p>
  O
  <p>Requisito actual del producto: además de una licencia de Workfront, debe adquirir una licencia para Adobe Workfront Goals. </p> <p>Para obtener más información, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para usar Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Nivel de acceso</td>
 <td> <p>Editar acceso a Goals</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Permisos de objeto</td>
 <td>

<p>Permisos Ver o superiores para la meta que desea ver</p>
  <p>Permisos de administración para la meta y poder editarla</p>
  <p>Para obtener información acerca de cómo compartir metas, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartir una meta en Workfront Goals</a>. </p>
   </td>
 </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área Metas en el menú principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Alinear metas conectándolas entre sí

<!--
Aligning goals by connecting them differs depending on what environment you use. 

### Align goals by connecting them in the Production environment

1. Create two goals that you want to align. For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).
1. (Optional) Activate the goals that you want to align. You can align goals that have a Draft, Active, or Inactive status. For information about activating goals, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).
1. Go to the goal that you want to align (child goal) to another goal (parent goal) and click its name to open the **Goal Details** panel.

   For example, if you want Goal 2 to influence the progress of Goal 1, you must go to Goal 2. 

1. Click **Align to another goal** in the upper-right corner of the right panel.

   ![Align to another goal](assets/align-to-another-goal-link-highlighted-350x128.png)

1. Start typing the name of an existing goal or the name of an owner in the **Align to another goal** field, then select it when it appears in the list. Only goals that are from the same or future periods display in the list. 
1. Click **Save**.

   The goal you started with (Goal 2) is now the child goal of the goal you aligned it with (Goal 1).   
   The aligned goals display connected in the Goal Alignment section with Goal 2 as secondary to Goal 1.

   ![Aligned cards](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Optional) To view the goals in the Goal Alignment section, do one of the following:

   * Click the Goal Alignment section in the left panel and find the goals by applying the correct filter. For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).
   * Click the Goal List, Check-in, or Pulse sections in the left panel and find one of the goals, then click the **Alignment icon** ![Align icon](assets/align-icon.png) next to the goal name to go directly to the goal in the Goal Alignment section.

   For information about the Goal Alignment section, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md). 

1. (Optional) Add activities and results to either goal to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Optional) Remove the alignment between two goals, when you consider that no longer is relevant to your organization's overall strategy For information about removing alignment between goals, see [Remove goal alignment in Adobe Workfront Goals](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

-->
1. Cree dos metas que desee alinear. Para obtener información sobre cómo crear metas, consulte [Crear metas en Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).
1. (Opcional) Active las metas que desee alinear. Puede alinear metas que tengan un estado Borrador, Activo o Inactivo. Para obtener información sobre la activación de metas, consulte [Activación de metas en Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).
1. Vaya a la meta que desea alinear (meta secundaria) con otra meta (meta principal) y haga clic en su nombre para abrir la página de dicha meta.

   >[!INFO]
   >
   >Por ejemplo, si desea que la Meta 2 influya en el progreso de la Meta 1, debe ir a la Meta 2.

1. Haga clic en **Detalles de la meta** en el panel de la izquierda.

1. En el área **Información sobre la meta principal**, haga clic en **Añadir** en el campo **Meta principal** si no hay ninguna meta principal,

   O

   Haga clic en el nombre de la meta principal para elegir otra.

1. Empiece a escribir el nombre de la meta principal deseada en el campo **Meta principal** y, a continuación, selecciónela cuando aparezca en la lista. En la lista solo se muestran las metas que son del mismo periodo o de periodos futuros.

1. Haga clic en **Guardar cambios**.

   La meta con la que comenzó (Meta 2) ahora es la meta secundaria de la meta principal con la que la alineó (Meta 1).\
   Las metas alineadas se muestran conectadas en la sección Alineación de metas con la Meta 2 como secundaria de la Meta 1.
La meta secundaria se muestra en la sección Indicadores de progreso de la meta principal a medida que su progreso actualiza el progreso de la meta principal.

   ![Tarjetas alineadas](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Opcional) Para ver las metas en la sección Alineación de metas, vaya al área Metas de Workfront y, a continuación, haga clic en la sección **Alineación de metas** en el panel izquierdo. Para obtener información sobre la sección Alineación de metas, consulte [Navegar por la sección de Alineación de metas en Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).

1. (Opcional) Añada actividades y resultados a cualquiera de las metas para indicar su progreso. Para obtener información sobre cómo añadir actividades y resultados, consulte los siguientes artículos:

   * [Añadir actividades a metas en Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
   * [Añadir resultados a metas en Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Opcional) Elimine la alineación entre dos metas, cuando considere que ya no es relevante para la estrategia general de su organización. Para obtener información sobre cómo eliminar la alineación entre metas, consulte [Eliminar alineación de metas en Adobe Workfront Goals](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

