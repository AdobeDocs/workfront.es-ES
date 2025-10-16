---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Añadir resultados a metas en Adobe Workfront Goals
description: Los resultados miden el progreso de una meta. Sin asociar resultados, actividades o metas alineadas a una meta, no puede activar la meta y no puede registrar el progreso en ella.
author: Alina
feature: Workfront Goals
exl-id: 30e22482-22e2-432d-bb73-7f9a9160aba2
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 85%

---

# Añadir resultados a metas en Adobe Workfront Goals

<!--Audited for P&P only: 10/2025-->

Los resultados miden el progreso de una meta. Sin asociar resultados, actividades o metas alineadas a una meta, no puede activar la meta y no puede registrar el progreso en ella.

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
  <td> <p>paquete de Adobe Workfront</p> </td> 
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
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Access level</p></td>
 <td> <p>Edit access to Goals</p>  </td>
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

* Una plantilla de diseño que incluya el área de Metas en el menú principal.
* Una meta existente.

  Para obtener información sobre cómo crear metas, consulte [Crear metas en Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>Una meta no puede tener más de un total de 1000 resultados, actividades, proyectos y metas alineados.

## Agregar un resultado a una meta

<!--

Adding results to goals differs depending on which environment you use.

### Add a result to a goal in the Production environment

1. Go to the goal for which you want to add a result and click the name to open the **Goal Details** panel.
1. Click **Add results**.

   ![Add result inside goal](assets/add-result-inside-goal-details-highlighted-350x145.png)

1. Start typing the result you want to achieve in the **Result** field. This is the name of the result and it displays wherever the goal displays. 
1. (Optional) If you want to set the Result Owner as someone other than yourself, click your name in the **Owner** field and start typing the name of the user that you want to assign as the owner of the result, then click it when it appears in the drop-down list.

   >[!NOTE]
   >
   >You cannot assign a team or group as a result owner.

1. In the Value drop-down menu, select the type of value that you want to measure your success by.

   ![Results value](assets/results-value-initial-target-boxes-350x49.png)

   Select from the following options:

   |Option|Value type|
   |---|---|
   | # |Number value |
   | % |Percentage value |
   |$, CN¥, DKK, KR, Mex$, R, R$, zł, £ , ¥ , &euro; , ₹, ฿, MYR, ₪  |Currency values |

   For example, if you want to increase profit to 8%, and profit is currently at 4%, you can select % as the Measured Value.

   >[!TIP]
   >
   >The result Type is always Metric and cannot be edited.

1. In the Initial field, indicate the value that the result has in the beginning, before any progress on it has been recorded. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 4 as the Starting At value. 
1. In the Target field, indicate the value that the result aims to achieve. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 8 as the Ending At value.
1. Click **Save**.

   The result is saved for the selected goal. The progress of the goal automatically updates when you update the progress of a result.

-->

1. Haga clic en el icono del menú principal ![Menú principal](assets/main-menu-icon.png) y luego en **Metas**.

1. En la **Lista de metas**, haga clic en el nombre de una meta para abrir la página de metas.
1. Haga clic en **Indicadores de progreso** en el panel de la izquierda.
1. Expanda el menú desplegable **Nuevo indicador de progreso** y luego haga clic en **Crear resultado**.

   Se abrirá el cuadro Nuevo resultado.

   ![Nuevo cuadro de resultados](assets/new-result-box-unshimmed.png)

1. Escriba un nombre para el resultado en el campo **Nombre del resultado**. Este campo es obligatorio.
1. (Opcional) Elimine su nombre del campo **Propietario del resultado** si desea asignar el resultado a otro usuario. De forma predeterminada, usted es el propietario de una actividad que crea.

   >[!NOTE]
   >
   >No se puede asignar un equipo, grupo o compañía como propietario del resultado.

1. En el área **¿Cómo quiere medir su resultado?**, especifique la siguiente información:
   * **Tipo de valor**: indica cómo desea medir el progreso en el resultado. Puede medir el progreso numéricamente, con un valor porcentual o mediante una cantidad de moneda.

     Seleccione un tipo de valor de las opciones que se muestran en la tabla siguiente:

     | Tipo de valor | Descripción |
     |---------------------------------------------------------|------------------|
     | Número | Valor numérico |
     | % | Valor porcentual |
     | CN¥,DKK,KR,Mex$, R, R$, zł, £ , ¥ , € , ₹, ฿, MYR, ₪, $ | Valores monetarios |

   * **Valor inicial**: el valor que tiene el resultado al principio, antes de que se registre cualquier progreso en él.
   * **Valor de destino**: el valor que el resultado pretende alcanzar cuando se considera completado.
1. Haga clic en **Crear resultado**.

   El resultado se muestra en la sección Indicadores de progreso de la página de metas, en la agrupación de resultados.

   Después de activar la meta, el progreso de la meta se actualiza automáticamente cuando se actualiza el progreso de un resultado. Para obtener información sobre cómo activar una meta, consulte [Activar metas en Adobe Workfront Goals](../goal-management/activate-goals.md).
