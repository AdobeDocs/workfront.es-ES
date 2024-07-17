---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Añadir resultados a metas en Objetivos de Adobe Workfront
description: Los resultados miden el progreso de una meta. Sin asociar resultados, actividades o metas alineadas a una meta, no puede activar la meta y no puede registrar el progreso en ella.
author: Alina
feature: Workfront Goals
exl-id: 30e22482-22e2-432d-bb73-7f9a9160aba2
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 3%

---

# Añadir resultados a metas en Objetivos de Adobe Workfront

Los resultados miden el progreso de una meta. Sin asociar resultados, actividades o metas alineadas a una meta, no puede activar la meta y no puede registrar el progreso en ella.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> 
   <p>Para el nuevo plan y la estructura de licencias:
  <ul><li>Un plan definitivo </li>
  O
  <li>Licencia adicional para objetivos de Adobe Workfront para los planes Prime o Select Adobe Workfront. </li></ul> </p>
<p>Para el plan y la estructura de licencias actuales: 
<ul><li> A Pro o superior </li>
  <li>Una licencia de Adobe Workfront Goals además de una licencia de Workfront.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licencia de Adobe Workfront*</td>
 <td>
 <p>Nueva licencia: Colaborador o superior</p>
 O
 <p>Licencia actual: Solicitud o superior</p> <p>Para obtener más información, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Resumen de licencias de Adobe Workfront</a>.</p> </td>
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
 <td role="rowheader"><p>Nivel de acceso</p></td>
 <td> <p>Editar acceso a Objetivos</p>  </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permisos de objeto</td>
 <td>
  <div>
  <p>Ver o permisos superiores a la meta para verla</p>
  <p>Administrar permisos para el objetivo y editarlo</p>
  <p>Para obtener información acerca de cómo compartir metas, vea <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartir una meta en Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área Objetivos en el menú principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Requisitos previos

Debe tener lo siguiente para poder iniciar:

* Plantilla de diseño que incluye el área de Objetivos en el menú principal.
* Un objetivo existente.

  Para obtener información sobre cómo crear metas, consulte [Crear metas en Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>Una meta no puede tener más de un total de 1000 actividades, resultados, proyectos o metas alineadas.

## Agregar un resultado a una meta

<!--

Adding results to goals differs depending on which environment you use.

### Add a result to a goal in the Production environment

1. Go to the goal for which you want to add a result and click the name to open the **Goal Details** panel.
1. Click **Add results**.

   ![](assets/add-result-inside-goal-details-highlighted-350x145.png)

1. Start typing the result you want to achieve in the **Result** field. This is the name of the result and it displays wherever the goal displays. 
1. (Optional) If you want to set the Result Owner as someone other than yourself, click your name in the **Owner** field and start typing the name of the user that you want to assign as the owner of the result, then click it when it appears in the drop-down list.

   >[!NOTE]
   >
   >You cannot assign a team or group as a result owner.

1. In the Value drop-down menu, select the type of value that you want to measure your success by.

   ![](assets/results-value-initial-target-boxes-350x49.png)

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

1. Haga clic en el menú principal ![](assets/main-menu-icon.png) y luego en **Objetivos**.

1. En la **Lista de metas**, haga clic en el nombre de una meta para abrir la página de metas.
1. Haga clic en **Indicadores de progreso** en el panel izquierdo.
1. Expanda el menú desplegable **Nuevo indicador de progreso** y luego haga clic en **Crear resultado**.

   Se abrirá el cuadro Nuevo resultado.

   ![](assets/new-result-box-unshimmed.png)

1. Escriba un nombre para el resultado en el campo **Nombre del resultado**. Este campo es obligatorio.
1. (Opcional) Elimine su nombre del campo **Propietario del resultado** si desea asignar el resultado a otro usuario. De forma predeterminada, usted es el propietario de una actividad que crea.

   >[!NOTE]
   >
   >No se puede asignar un equipo, grupo o compañía como propietario del resultado.

1. En el **¿Cómo desea medir su resultado?** área, especifique la siguiente información:
   * **Tipo de valor**: esto indica cómo desea medir el progreso en el resultado. Puede medir el progreso numéricamente, con un valor porcentual o mediante una cantidad de moneda.

     Seleccione un tipo de valor de las opciones que se muestran en la tabla siguiente:

     | Tipo de valor | Descripción |
     |---------------------------------------------------------|------------------|
     | Número | Valor numérico |
     | % | Valor porcentual |
     | CN¢,DKK,KR,Mex$, R, R$, zł, £ , ¥ , € , ₹, ฿, MYR, ₪, $ | Valores monetarios |

   * **Valor inicial**: El valor que tiene el resultado al principio, antes de que se registre cualquier progreso en él.
   * **Valor de destino**: Valor que el resultado pretende alcanzar cuando se considera completado.
1. Haga clic en **Crear resultado**.

   El resultado se muestra en la sección Indicadores de progreso de la página de objetivos, en la agrupación Resultados.

   Después de activar la meta, el progreso de la meta se actualiza automáticamente cuando se actualiza el progreso de un resultado. Para obtener información sobre cómo activar una meta, consulte [Activar metas en Adobe Workfront Goals](../goal-management/activate-goals.md).
