---
product-previous: workfront-goals
navigation-topic: goal-management
title: Editar metas en Adobe Workfront Goals
description: Puede editar las metas existentes de cualquier periodo de tiempo y en cualquier estado.
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 32%

---

# Editar metas en Adobe Workfront Goals

Puede editar las metas existentes de cualquier periodo de tiempo y en cualquier estado.

## Requisitos de acceso

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
 <p>Licencia actual: Request o superior</p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Información general sobre las licencias de Adobe Workfront</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Producto*</td>
 <td>
 <p> Nuevo requisito de producto, uno de los siguientes: </p>
<ul>
<li>Un plan Select or Prime Adobe Workfront y una licencia adicional de Adobe Workfront Goals.</li>
<li>Un plan Ultimate Workfront que incluye Workfront Goals de forma predeterminada. </li></ul>
 <p>O</p>
 <p>Requisito de producto actual: un plan de Workfront y una licencia adicional para Adobe Workfront Goals. </p> <p>Para obtener más información, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para usar Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Nivel de acceso</td>
 <td> <p>Editar acceso a Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permisos de objeto</td>
 <td>
  <div>
  <p>Permisos Ver o superiores para la meta que desea ver</p>
  <p>Permisos de administración para la meta y poder editarla</p>
  <p>Para obtener información acerca de cómo compartir metas, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartir una meta en Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área Metas en el menú principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Consideraciones sobre la edición de objetivos

* No puede editar metas con el estado Cerrado.
* Puede editar metas desde cualquier periodo de tiempo.

  Puede editar la siguiente información para un objetivo anterior:

   * Nombre
   * Período de tiempo
   * Estado

     >[!TIP]
     >
     >Si el objetivo está Cerrado, al volver a abrirlo se vuelve a calcular el Porcentaje de progreso completado. No puede editar un objetivo cerrado.

   * Descripción
   * Resultados y actividades

## Editar metas

<!--
Editing goals differs depending on what environment you use.

### Edit goals in the Production environment

1. Go to a goal that you want to edit and click the goal name to open the **Goal Details** panel. 
1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Edit**.

   ![Edit goal](assets/edit-goal-highlighted.png)

1. Update the name of the goal in the **Goal** field. 
1. Select a time period when the goal should be completed.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a start and an end date for your goal, if you clicked **Define custom dates**.

   
   <p>(NOTE: these fields don't yet have a name) </p>
   

   >[!CAUTION]
   >
   >You cannot create a goal with custom dates in the past.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same time frames for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your larger organization-wide strategy.

1. Click the **Owner** field and select a new owner for the goal, if you want to indicate someone else as the owner of the goal. 
1. (Conditional) Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. Update the **Description** of the goal, then click **Save**.

-->

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) y luego haga clic en **Metas**.\
   Se muestra una lista de objetivos.
1. Haga clic en una meta.\
   Se muestra la página de objetivo.

   ![Página de metas](assets/goal-page-unshimmed.png)

1. Realice una de las siguientes acciones para editar la información del objetivo:
   * Haga clic en los campos que se muestran en el encabezado de la meta para actualizarlos. No todos los campos del encabezado son editables.
   * Haga clic en el **icono Más** ![icono Más](assets/more-icon.png) a la derecha del nombre de la meta y, a continuación, haga clic en **Editar**.
   * Haga clic en **Detalles de la meta** en el panel izquierdo, haga clic en el **icono Editar** ![Icono Editar](assets/edit-icon.png) en la esquina superior derecha y, a continuación, haga clic en **Editar todo**. Comience a actualizar los campos en la sección Detalles del objetivo.

     >[!IMPORTANT]
     >
     >No se pueden editar todos los campos que se muestran en las áreas mencionadas anteriormente. Workfront calcula algunos de los campos y son de solo lectura.

1. (Condicional) Según lo que haya seleccionado en el paso anterior, actualice la siguiente información sobre el objetivo:

   * Actualice la siguiente información en el encabezado de objetivo y, a continuación, pulse Intro para guardar los cambios:
      * **Nombre de la meta**: haga clic en el nombre de la meta y empiece a escribir un nombre nuevo.
      * **Propietario**: haga clic en el nombre del propietario, empiece a escribir el nombre de un usuario, equipo, grupo o empresa y, a continuación, selecciónelo cuando se muestre en la lista. Solo puede tener un propietario para un objetivo.
   * Actualice la siguiente información en el cuadro Editar meta y, a continuación, haga clic en **Guardar**:
      * **Nombre de meta**
      * **Periodo**: Haga clic para actualizar el periodo de tiempo de la meta\
        O\
        Seleccione **Habilitar fechas personalizadas** para especificar fechas para las **fechas de inicio** y de finalización **de la meta**.

        >[!TIP]
        >
        >Anule la selección de **Habilitar fechas personalizadas** para volver al período de tiempo original de la meta.

      * **Propietario de la meta**
      * **Descripción**: agrega o actualiza información sobre la meta.
   * Actualice o revise la información en la sección Detalles del objetivo. Para obtener más información, consulte [Actualizar metas en la sección Detalles de las metas en Adobe Workfront Goals](../goal-management/update-goals-in-goal-details-panel.md).

   <!-- (should you update the title here after changing it at production??? - change it to Update goals in the goal Details section)-->

1. (Opcional) Haga clic en **Indicadores de progreso** en el panel izquierdo para agregar resultados, actividades o proyectos a la meta. Al agregar indicadores de progreso, se asegura de poder rastrear el progreso de la meta.
Para obtener más información, consulte los siguientes artículos:
   * [Añadir actividades a metas en Adobe Workfront Goals](../results-and-activities/add-activities-to-goals.md)
   * [Agregar resultados a metas en Adobe Workfront Goals](../results-and-activities/add-results-to-goals.md).
   * [Agregar proyectos a metas en Adobe Workfront Goals](../results-and-activities/connect-projects-to-goals-overview.md).

</div>
