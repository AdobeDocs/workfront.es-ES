---
product-previous: workfront-goals
navigation-topic: goal-management
title: Editar objetivos en objetivos de Adobe Workfront
description: Puede editar los objetivos existentes desde cualquier período de tiempo y en cualquier estado.
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 1%

---

# Editar objetivos en objetivos de Adobe Workfront

Puede editar los objetivos existentes desde cualquier período de tiempo y en cualquier estado.

## Requisitos de acceso

<!--drafted - for P&P releases: 

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
* Ha creado los objetivos que desea editar o tiene permisos de administración para ellos.

## Consideraciones sobre los objetivos de edición

* Los objetivos no se pueden editar con el estado Cerrado.
* Los objetivos se pueden editar desde cualquier período de tiempo.

   Puede editar la siguiente información para un objetivo anterior:

   * Nombre
   * Período de tiempo
   * Estado

      >[!TIP]
      >
      >Si el objetivo es Cerrado, volver a abrirlo vuelve a calcular el porcentaje de progreso completado. No se puede editar un objetivo cerrado.

   * Descripción
   * Resultados y actividades

## Editar objetivos

<!--
Editing goals differs depending on what environment you use.

### Edit goals in the Production environment

1. Go to a goal that you want to edit and click the goal name to open the **Goal Details** panel. 
1. Click the **More icon** ![](assets/more-icon.png), then click **Edit**.

   ![](assets/edit-goal-highlighted.png)

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

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png)y haga clic en **Objetivos**.\
   Se muestra una lista de objetivos.
1. Haga clic en un objetivo.\
   Se muestra la página de objetivo.

   ![](assets/goal-page-unshimmed.png)

1. Realice una de las siguientes acciones para editar la información del objetivo:
   * Haga clic en los campos que se muestran en el encabezado de objetivo para actualizarlos. No todos los campos del encabezado son editables.
   * Haga clic en el **Más icono** ![](assets/more-icon.png) a la derecha del nombre del objetivo y haga clic en **Editar**.
   * Haga clic en **Detalles del objetivo** en el panel izquierdo y haga clic en el botón **Icono Editar** ![](assets/edit-icon.png) en la esquina superior derecha, haga clic en **Editar todo**. Comience a actualizar los campos en la sección Detalles del objetivo .

      >[!IMPORTANT]
      >
      >No se pueden editar todos los campos que aparecen en las áreas mencionadas anteriormente. Workfront calcula algunos de los campos y son de solo lectura.

1. (Condicional) Según lo que haya seleccionado en el paso anterior, actualice la siguiente información sobre el objetivo:

   * Actualice la siguiente información en el encabezado de objetivo y, a continuación, pulse Intro para guardar los cambios:
      * **Nombre del objetivo**: Haga clic en el nombre del objetivo y empiece a escribir un nombre nuevo.
      * **Propietario**: Haga clic en el nombre del propietario y empiece a escribir el nombre de un usuario, equipo, grupo o empresa. A continuación, selecciónelo cuando aparezca en la lista. Solo se puede tener un propietario para un objetivo.
   * Actualice la siguiente información en el cuadro Editar objetivo y haga clic en **Guardar**:
      * **Nombre de la meta**
      * **Periodo**: Haga clic en para actualizar el período de tiempo para el objetivo\
         O\
         Select **Habilitar fechas personalizadas** para especificar fechas para el **Inicio** y **Fechas de finalización**.

         >[!TIP]
         >
         >Anular selección **Habilitar fechas personalizadas** para volver al período de tiempo original para el objetivo.

      * **Propietario de la meta**
      * **Descripción**: Agregue o actualice información sobre el objetivo.
   * Actualice o revise la información en la sección Detalles del objetivo . Para obtener más información, consulte [Actualizar objetivos en la sección Detalles del objetivo de los objetivos de Adobe Workfront](../goal-management/update-goals-in-goal-details-panel.md).

   <!-- (should you update the title here after changing it at production??? - change it to Update goals in the goal Details section)-->

1. (Opcional) Haga clic en **Indicadores de progreso** en el panel izquierdo para agregar resultados, actividades o proyectos al objetivo. Al agregar indicadores de progreso, se asegura de que se pueda rastrear el progreso del objetivo.
Para obtener más información, consulte los siguientes artículos:
   * [Agregar actividades a objetivos en Objetivos de Adobe Workfront](../results-and-activities/add-activities-to-goals.md)
   * [Agregar resultados a objetivos en Objetivos de Adobe Workfront](../results-and-activities/add-results-to-goals.md).
   * [Agregar proyectos a objetivos en Objetivos de Adobe Workfront](../results-and-activities/connect-projects-to-goals-overview.md).

</div>
