---
product-previous: workfront-goals
navigation-topic: goal-management
title: Crear metas en Adobe Workfront Goals
description: Tanto si es un CEO, un administrador o un colaborador individual, puede crear metas en Adobe Workfront Goals para alinear su trabajo con sus metas y las metas que definen la estrategia de su organización.
author: Alina
feature: Workfront Goals
exl-id: 14bf48b6-eb0c-4b00-a1a4-0d070ccc1392
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 93%

---

# Crear metas en Adobe Workfront Goals

<!--Audited for P&P only: 4/2025-->

Tanto si es un CEO, un administrador o un colaborador individual, puede crear metas en Adobe Workfront Goals para alinear su trabajo con sus metas y las metas que definen la estrategia de su organización.

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
  <p> Nuevo requisito de producto: Workfront</p>
 <p>O</p>
  <p>Requisito actual del producto: además de una licencia de Workfront, debe adquirir una licencia para Adobe Workfront Goals. </p> <p>Para obtener más información, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para usar Workfront Goals</a>. </p> </td>
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

+++

## Directrices para crear objetivos

Antes de empezar a usar Workfront Goals, le recomendamos que lea nuestras prácticas recomendadas y directrices para administrar las metas de forma eficaz. Para obtener más información acerca de las directrices para crear y administrar objetivos, consulte [Información general sobre Adobe Workfront Goals](../../workfront-goals/goal-management/wf-goals-overview.md).

## Crear metas

En este artículo se describe cómo crear un objetivo estratégico en Workfront Goals. Para obtener información sobre cómo crear un objetivo de caso empresarial, consulte [Crear objetivos de caso empresarial](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

Puede crear un objetivo estratégico de una de las siguientes maneras:

* [Crear un objetivo desde cero](#create-a-goal-from-scratch)
* [Copiar un objetivo existente](#copy-an-existing-goal)
* [Conversión de un resultado o actividad en una meta](#convert-a-result-or-activity-to-a-goal)

### Crear una meta desde cero {#create-a-goal-from-scratch}

<!--
Creating goals differs depending on what environment you use.

#### Create a goal from scratch in the Production environment 


1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) in the upper right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -)

   The Goal List displays.

1. (Conditional) Click **Goal List**, **Graphs**, **Pulse**, or **Check-in** in the left pane, then click **Add Goal** in the upper-right corner of the page. The Add Goal box displays.

   ![Add goal box](assets/add-goal-box-350x235.png)

   >[!TIP]
   >
   >You can add a goal from any section in Workfront Goals. The process for creating a goal is identical regardless of the section you choose to add the goal from.

1. Start typing what you want to achieve in the **Goal** field. This is the name of the goal and a required field. 
1. Select a time period when the goal should be executed in the **Period** drop-down menu. This is a pre-filled field. The default is the current quarter.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a **Start date** and an **End date** for your goal, if you clicked **Define custom dates**.

   >[!TIP]
   >
   >* You can create a goal with dates in any time period, including up to 2 years in the past. 
   >* When defining custom dates, they are constrained by the initial date you selected. So if you select quarter and then custom dates, you can't go beyond that quarter.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same timeframes for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your over-arching strategy.

1. (Optional) Click your name in the **Owner** field, if you want to indicate someone else as the owner of the goal. By default, you are the owner of goals you create. 
1. Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. (Optional) Enter a **Description** for the goal. This field is optional. 
1. Click **Save**.

   The status of the new goal is Draft.

   >[!IMPORTANT]
   >
   >You must associate a goal with a progress indicator to activate it and start working on it. 
   >
   >Do at least one of the following to be able to activate a goal: 
   >
   >* Add a Result
   >
   >  For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   >   
   >* Add an Activity
   >   
   >  For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 
   >   
   >* Align another goal to it
   >   
   >  For information about aligning goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

-->

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **Metas**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Se muestra la lista de metas.
1. Haga clic en **Nueva meta**.

   Se muestra el cuadro Nueva meta.

   ![Nuevo cuadro de metas](assets/new-goal-box-unshimmed.png)

1. Introduzca información en los campos siguientes:
   * **Nombre de meta**: introduzca un nombre para la meta. Este campo es obligatorio.
   * **Período**: seleccione un trimestre o año predefinido del campo desplegable **Período**

     O

     Seleccione la opción **Habilitar fechas personalizadas** y, a continuación, seleccione **Fecha de inicio** y **Fecha de finalización** para la meta.

     Los años anteriores, actuales y siguientes y sus trimestres respectivos se muestran como opciones predefinidas en el campo desplegable Período.

     El período de la meta indica el lapso de tiempo en el que espera que se complete la meta.

   * **Propietario de la meta**: empiece a escribir el nombre de un usuario, un equipo, un grupo o de su organización para indicar quién es el propietario de la meta. De forma predeterminada, se le selecciona como propietario de la meta.
   * **Descripción**: información adicional sobre la meta.
1. Haga clic en **Crear meta**.

   La nueva meta aparece en la lista de metas y tiene el estado **Borrador**.

   Debe asociar una meta con un indicador de progreso para activarla y empezar a trabajar en ella.

   Realice al menos una de las siguientes acciones para preparar una meta para su activación:
   * Añadir un resultado

     Para obtener información sobre cómo añadir resultados, consulte [Añadir resultados a metas en Adobe Workfront Goals](../results-and-activities/add-results-to-goals.md).
   * Añadir una actividad

     Para obtener información sobre cómo añadir actividades, consulte [Añadir actividades a metas en Adobe Workfront Goals](../results-and-activities/add-activities-to-goals.md).
   * Alinear otra meta a ella

     Para obtener información acerca de cómo alinear metas, consulte [Alinear metas conectándolas en Adobe Workfront Goals](../goal-alignment/align-goals-by-connecting-them.md).


### Copiar una meta existente {#copy-an-existing-goal}

Puede crear una meta copiando una existente.

Para obtener información sobre cómo copiar metas, consulte [Copiar metas en Adobe Workfront Goals](../../workfront-goals/goal-management/copy-goals.md).

### Conversión de un resultado o actividad en una meta {#convert-a-result-or-activity-to-a-goal}

Puede crear una meta convirtiendo el resultado o la actividad de una meta existente en una meta. La nueva meta se alinea con la original.

Para obtener información acerca de cómo convertir resultados y actividades en metas, consulte [Alinear metas convirtiendo resultados y actividades en metas](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

