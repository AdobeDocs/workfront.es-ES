---
product-previous: workfront-goals
navigation-topic: goal-management
title: Editar metas en Adobe Workfront Goals
description: Puede editar las metas existentes de cualquier periodo de tiempo y en cualquier estado.
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 14%

---

# Editar metas en Adobe Workfront Goals

<!--Audited for P&P only: 10/2025-->

Puede editar las metas existentes de cualquier periodo de tiempo y en cualquier estado.

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

{{step1-to-goals}}

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
