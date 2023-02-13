---
product-previous: workfront-goals
navigation-topic: goal-management
title: Copiar objetivos en objetivos de Adobe Workfront
description: Puede copiar objetivos en Objetivos de Adobe Workfront para crear un objetivo. Parte de la información del objetivo original se transfiere al nuevo objetivo.
author: Alina
feature: Workfront Goals
exl-id: 690a6030-ee29-4e50-869f-cd014050b364
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Copiar objetivos en objetivos de Adobe Workfront

Puede copiar objetivos en Objetivos de Adobe Workfront para crear un objetivo. Parte de la información del objetivo original se transfiere al nuevo objetivo.

## Requisitos de acceso

<!--drafted for P&P release: 

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

## Consideraciones para copiar objetivos

Debe tener acceso a Editar objetivos en el nivel de acceso para poder copiar los objetivos. Para obtener información sobre la concesión de acceso a los objetivos, consulte [Conceder acceso a los objetivos de Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

Algunas de las razones por las que puede que desee copiar un objetivo existente son:

* Al final de un período de tiempo (trimestre o año), cuando desee volver a crear el mismo objetivo para el siguiente período.
* Al final de un período de tiempo, cuando el objetivo no se puede completar y desea trabajar en él durante otro período de tiempo.
* Cuando varios integrantes del equipo tienen objetivos similares y es posible que tenga que crear uno para cada uno de ellos.

>[!TIP]
>
>Puede copiar un objetivo en cualquier estado. Para obtener información sobre los estados de objetivos, consulte [Información general sobre el estado de los objetivos en los objetivos de Adobe Workfront](../../workfront-goals/goal-management/goal-status-overview.md).

Tenga en cuenta lo siguiente al copiar objetivos:

* Toda la información sobre el objetivo también se copia al nuevo objetivo.
* Puede seleccionar para copiar los resultados de un objetivo existente. El nombre de los resultados se transfiere al nuevo objetivo, pero el progreso actual de los resultados en el objetivo existente no se copia al nuevo objetivo. Los resultados copiados se asignan al mismo propietario de forma predeterminada.

   >[!NOTE]
   >
   >Si se eliminó o desactivó el propietario original de Workfront, el nuevo resultado se asigna al usuario que ha iniciado sesión.

* No puede copiar las actividades de un objetivo cuando copia el objetivo.

## Copiar objetivos

<!--
Copying goals differs depending on what environment you use. 

To copy goals in the Production environment:

1. Go to a goal and click it to open the Goal Details panel.

   For information about accessing an individual goal, see the "Access individual goals" section in [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md).

   This opens the Goal Details panel.

1. Click the **More icon** ![](assets/more-icon.png), then click **Copy**. 

1. Update any of the following information for the copied goal:

   | Field |Description  |
   |---|---|
   | New Goal |The name of the new goal. The default is the name of the original goal.  |
   | Period |The time period during which you want to achieve the goal. Select a time period from the drop-down menu or click **Define custom dates** to indicate a custom time period. By default, the Period is always the current quarter. |
   | Owner |The owner of the goal. It can be a user, team, group, or a company. The default is the owner of the original goal.  |
   | Description |Additional information about the goal.  |

1. (Conditional) Select **Copy results** if the original goal had results added to it and you want to copy them to the new goal. This duplicates the original results to the new goal. The results of the copied goal have the same owner, names and measured values as the results of the original goal.

   >[!TIP]
   >
   >* The progress of the original result does not transfer to the copied goal. 
   >* If the original owner was deleted or deactivated from Workfront, the new result is assigned to the logged in user.

1. Click **Save**.

   The copied goal is saved with a status of Draft and displays in the Goal Details panel.

   >[!IMPORTANT]
   >
   >If you have not copied the results from the original goal, you must first associate the new goal with a progress indicator before you can activate it and start working towards achieving it. 
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
   >
   > For information about activating a goal, see [Activate goals in Adobe Workfront Goals](../goal-management/activate-goals.md). 

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

   The copied goal displays in the following sections:

   * Goal List 
   * Check-in (after it is activated)
   * Goal Alignment section (after it is activated) 
   * Pulse
(!--drafted - this was important when we could not update the goal timeframe in the past but we can do that now - not needed
1. (Optional and conditional) If you have copied a goal that was not achieved in a previous time period to continue working on it in the following time period, do the following:

   1. Go to the original goal in the Goal List, Check-in page, or Pulse section and comment on the goal, to indicate that this goal was copied to another, more current goal. For information about commenting on a goal, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md).
   1. Close the original goal, to preserve the progress in its original time period. For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   1. Update the the **Initial** value of the new Result to match the **End At** value of the previous result, so that your new goal progress will start calculating from the point you achieved in the previous period.
   
-->


1. Vaya a un objetivo y haga clic en el **Más** menú ![](assets/more-icon.png)y haga clic en **Copiar objetivo**.

   ![](assets/copy-goal-box-unshimmed.png)

1. Actualice la siguiente información para el objetivo copiado:
   * **Nombre del objetivo**: El nombre del nuevo objetivo. El nombre predeterminado para el objetivo copiado es &quot;Copia de &lt;original goal=&quot;&quot;>&quot;.
   * **Periodo**: Período de tiempo durante el cual desea alcanzar el objetivo. Seleccione un período de tiempo en el menú desplegable

      O

      Select **Habilitar fechas personalizadas** para especificar fechas personalizadas para el **Inicio** y **Fechas de finalización**. El ajuste Habilitar fechas personalizadas está deshabilitado de forma predeterminada.

      >[!TIP]
      >
      >   Al anular la selección Habilitar fechas personalizadas, se revierte al período de tiempo del objetivo original.

      * **Propietario del objetivo**: El propietario del gol. Puede ser un usuario, equipo, grupo o empresa. El valor predeterminado es el propietario del objetivo original.
      * **Descripción**: Información adicional sobre el objetivo.
      * **Copiar resultados**: Seleccione esta opción si desea transferir los resultados del objetivo actual al objetivo copiado. Esto duplica los resultados originales y los adjunta al objetivo copiado. Los resultados del objetivo copiado tienen el mismo propietario, nombres y valores medidos que los resultados del objetivo original.

         >[!NOTE]
         >
         >* El progreso del resultado original no se transfiere al objetivo copiado.
         >* Si se eliminó o desactivó el propietario original de Workfront, el nuevo resultado se asigna al usuario que ha iniciado sesión.


1. Haga clic en **Copiar objetivo**.

   Se crea un objetivo similar al original y está en estado Borrador.

   >[!NOTE]
   >
   >Si no ha copiado los resultados del objetivo original, primero debe asociar el nuevo objetivo con un indicador de progreso para poder activarlo y comenzar a trabajar para conseguirlo.
   >Para obtener información sobre la asociación de objetivos con indicadores de progreso, consulte los siguientes artículos:
   >* [Agregar resultados a objetivos en Objetivos de Adobe Workfront](../results-and-activities/add-results-to-goals.md)
   >* [Agregar actividades a objetivos en Objetivos de Adobe Workfront](../results-and-activities/add-activities-to-goals.md)
   >* [Alinear objetivos conectándolos en los objetivos de Adobe Workfront](../goal-alignment/align-goals-by-connecting-them.md)

   >
   >Para obtener información sobre la activación de objetivos, consulte [Activar objetivos](../goal-management/activate-goals.md).

