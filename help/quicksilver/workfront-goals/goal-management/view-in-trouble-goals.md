---
product-previous: workfront-goals
navigation-topic: goal-management
title: Revisar objetivos en problemas en los objetivos de Adobe Workfront
description: Los objetivos con Progreso en Problemas están en peligro de no ser alcanzados y están representados por una barra de progreso roja en los objetivos de Adobe Workfront. Debería revisar sus objetivos a menudo y comprender por qué el progreso se está retrasando.
author: Alina
feature: Workfront Goals
exl-id: df2cdc12-9102-4759-9daa-1f8ae68f110b
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# Revisar objetivos en problemas en los objetivos de Adobe Workfront

<!--
<p>(NOTE: the status of goals in "red" used to be called At Risk. Now, it is "in trouble") </p>
-->

Los objetivos con Progreso en Problemas están en peligro de no ser alcanzados y están representados por una barra roja de progreso en los objetivos de Adobe Workfront. Debería revisar sus objetivos a menudo y comprender por qué el progreso se está retrasando. Para obtener información sobre el progreso del objetivo, consulte [Resumen del progreso y la condición del objetivo en los objetivos de Adobe Workfront](../../workfront-goals/goal-management/calculate-goal-progress.md).

## Requisitos de acceso

<!--drafted for P&P release: replace the existing requirements with this:

You must have the following: 

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
   <td> <p>Editar acceso a Objetivos o posterior</p> <p><b>NOTA</b><p>Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte:</p> 
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

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Debe tener lo siguiente para poder iniciar:

* Plantilla de diseño que incluye el área Objetivos del menú principal.

## Recommendations para evitar que los objetivos alcancen el progreso de En problemas

Antes de que los objetivos alcancen un progreso de En problemas, puede monitorearlos con frecuencia y ajustar su progreso cuando alcancen un progreso de En riesgo. Los objetivos que están en riesgo corren el riesgo de tener problemas. Para obtener más información sobre el progreso del objetivo, consulte [Resumen del progreso y la condición del objetivo en los objetivos de Adobe Workfront](../../workfront-goals/goal-management/calculate-goal-progress.md)

Antes de que sus objetivos alcancen un progreso de En problemas, le recomendamos lo siguiente:

* Revise los objetivos que tienen una condición de En riesgo que a menudo se le asignan, así como los objetivos organizativos que se asignan a sus equipos, grupos o a su organización y que podrían verse afectados por el progreso de sus objetivos. Los objetivos en riesgo están en peligro de convertirse en objetivos en problemas. Los objetivos en riesgo están marcados por una barra de progreso amarilla. Utilice la lista de objetivos para ver los objetivos que le pertenecen, a sus equipos, a grupos o a su organización.


## Revisar objetivos en problemas en la lista de objetivos

Puede revisar los objetivos en cualquier sección de los Objetivos de Workfront. Para obtener información sobre las secciones Objetivos de Workfront , consulte [Información general sobre las secciones de objetivos de Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

Este artículo describe cómo revisar los objetivos en la lista de objetivos.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) > **Objetivos** en la esquina superior derecha.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Se abre el área Objetivos de Workfront y se muestra la sección Lista de objetivos de forma predeterminada.

1. (Recomendado) Ajuste los siguientes filtros para el área de lista de objetivos para revisar los objetivos en riesgo:

   * Haga clic en **Empresa**, luego **Mis equipos**, luego **Mis grupos**, luego **Personal** objetivos para poder ver los objetivos que pertenecen a su organización, sus equipos, grupos y luego sus propios objetivos.

      >[!TIP]
      >
      >En Objetivos de Adobe Workfront, el filtro Empresa muestra los objetivos para los que su organización está seleccionada como propietaria.
      >
      >
      >No puede buscar empresas que utilicen este campo. De forma predeterminada, solo está seleccionada la organización que es la propietaria de la instancia de Workfront.

   * Para cada una de las unidades organizativas seleccionadas anteriormente, haga clic en **Nuevo filtro** > **Progreso** > **En problemas** >**Aplicar.**
   * (Opcional) Seleccione el período de tiempo para el cual desee ver los objetivos.

      El indicador de la barra de progreso se muestra en rojo para cada objetivo de la lista de objetivos.

      Para obtener más información sobre los objetivos de filtrado utilizando todos los demás criterios del panel derecho, consulte [Filtrar información en objetivos de Adobe Workfront](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. Pase el ratón sobre el indicador de la barra de progreso para ver cuál es el porcentaje de progreso real y cuál es el valor esperado para el día actual.

   ![](assets/goal-progress-hover-over-detail-unshimmed.png)

1. (Opcional) Utilice los filtros para buscar objetivos que pertenezcan a un propietario específico.

   Los objetivos en problemas para los usuarios seleccionados se muestran en la lista de objetivos.

1. Haga clic en un nombre de objetivo para abrir la página de objetivo y, a continuación, haga clic en **Indicadores de progreso** en el panel izquierdo. Vea qué indicador de progreso hace que el objetivo esté detrás y actualice el progreso del indicador en línea, en la variable **Progreso real** de la lista Indicadores de progreso.

   Para obtener información sobre la actualización de resultados y actividades, consulte [Actualización del progreso del objetivo en los objetivos de Adobe Workfront](../goal-review-and-workfront-goals-sections/check-in-goals.md)

   ![](assets/actual-progress-editable-column-in-indicator-list-unshimmed.png)

   >[!NOTE]
   >
   >Solo puede actualizar los resultados y las actividades en la lista Indicadores de progreso . Debe actualizar los indicadores de progreso de los objetivos secundarios accediendo a los objetivos y actualizar las tareas de los proyectos conectados para actualizar el progreso de los proyectos.


