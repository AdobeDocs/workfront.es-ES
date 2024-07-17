---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Navegue hasta la sección Alineación de objetivos en Adobe Workfront Goals
description: Utilice la sección Alineación de objetivos para mostrar una vista holística de la alineación de objetivos en toda la organización en un diagrama de flujo. Las metas alineadas se muestran en las tarjetas que se interconectan en un árbol jerárquico.
author: Alina
feature: Workfront Goals
exl-id: e79ced31-4680-4af7-b083-3d615c747af8
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 1%

---

# Navegue hasta la sección Alineación de objetivos en Adobe Workfront Goals

Utilice la sección Alineación de objetivos para mostrar una vista holística de la alineación de objetivos en toda la organización en un diagrama de flujo. Las metas alineadas se muestran en las tarjetas que se interconectan en un árbol jerárquico.

Para obtener información sobre la alineación de objetivos y cómo conseguirla, consulte también los siguientes artículos:

* [Resumen de alineación de metas en Adobe Workfront Goals](../../workfront-goals/goal-alignment/goal-alignment-overview.md)
* [Alinee metas conectándolas en Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)

## Requisitos de acceso

Debe tener lo siguiente para realizar las actividades descritas en este artículo:

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
<p>Licencia actual: Solicitud o superior</p>  </td>
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

## Navegue por la sección Alineación de objetivos

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](../goal-alignment/assets/dots-main-menu-icon.png) en la esquina superior derecha de la pantalla y, a continuación, haga clic en **Metas**.
   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-alignment/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. Haga clic en **Alineación de metas** en el panel izquierdo.
1. Utilice los filtros de la esquina superior derecha del gráfico de alineación para seleccionar solo las metas que sean importantes para usted. Para obtener información acerca del uso de filtros en Workfront Goals, vea [Información sobre filtros en Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   Los objetivos que coinciden con los filtros se muestran en el gráfico de alineación de las tarjetas.

   La siguiente información se muestra en una tarjeta de objetivo:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Fechas del período de tiempo </td> 
      <td> <p>Este es el período durante el cual se abre la meta. El objetivo debe alcanzarse antes de la fecha de finalización del periodo. Workfront Goals calcula el progreso de la meta en función de la duración del periodo de la meta y la fecha actual.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Indicadores de progreso</td> 
      <td>Número de indicadores de progreso de la meta. Los indicadores de progreso pueden alinear metas, resultados o actividades. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nombre del propietario</td> 
      <td>El nombre del usuario, equipo, grupo u organización designado como Propietario del objetivo. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nombre de la meta</td> 
      <td>Nombre de la meta. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Barra de progreso de objetivo <span>y progreso</span></td> 
      <td> <p>El progreso de la meta indica cuánto de la meta se ha alcanzado actualmente. Se trata de un cálculo automático de la media del progreso de todas las metas, resultados y actividades alineados para la meta en función del tiempo transcurrido desde el inicio del periodo de tiempo de la meta. Para obtener información acerca de cómo calcular el progreso de los objetivos, vea <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Información general sobre el progreso y la condición de los objetivos en Adobe Workfront Goals</a>. </p> 
       <div> 
        <p>El progreso real de la meta en la fecha actual. Los siguientes valores y colores de progreso indican la probabilidad de que el objetivo se alcance a tiempo: </p> 
        <ul> 
         <li><span>En Target</span> (indicador verde): el objetivo se ha cumplido a tiempo y se alcanzará a tiempo.</li> 
         <li> <span>En riesgo</span> (indicador amarillo): el objetivo se retrasa y es posible que no se logre a tiempo.</li> 
         <li> <span>Con problemas</span> (indicador rojo): el objetivo corre el riesgo de no alcanzarse a tiempo. </li> 
        </ul> 
       </div> </td> 
     </tr> <!--
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">Updated on date </td> 
       <td> <p>The date when the goal was last updated</p> <p>(NOTE: drafted because I think this was removed with the alignment chart redesign - 21.1) </p> </td> 
      </tr>
     --> 
     <tr> 
      <td role="rowheader">Estado</td> 
      <td><span>Los objetivos de todos los estados se muestran en la sección Alineación de objetivos.</span> </td> 
     </tr> 
    </tbody> 
   </table>

   Las metas que se alinean con otras metas muestran el número de metas alineadas debajo de la tarjeta de metas.

   ![](assets/alignment-chart-arrow-for-aligned-goals-highlighted-350x241.png)

1. Haga clic en el icono **flecha** que apunta hacia abajo debajo de una meta para expandir y ver aún más las metas secundarias.

   ![](assets/alignment-chart-arrow-for-aligned-goals-highlighted-350x241.png)

   >[!TIP]
   >
   >Las metas que tienen metas secundarias alineadas con ellas muestran el número de metas alineadas en sus respectivas tarjetas.

1. (Condicional) Si el filtro actual excluye algunas de las metas que participan en una alineación, aparece un mensaje de advertencia para indicar que no se muestran todas las metas.

   ![](assets/parent-goal-excluded-by-filter-alignment-section-350x230.png)

1. Haga clic en **Mostrarlos** para mostrar las metas que el filtro ha eliminado actualmente.

   Observe los siguientes cambios en el gráfico de alineación:

   * Los objetivos conectados que el filtro había eliminado anteriormente ahora se muestran en el gráfico de alineación.
   * El filtro de la esquina superior derecha aparece delineado en amarillo para indicar que actualmente no se está aplicando.

     ![](assets/reapply-filter-link-and-yellow-filter-highlight-350x120.png)

     A la izquierda del nombre del filtro se muestra el vínculo Reaplicar filtro.

1. (Opcional) Haga clic en **Volver a aplicar el filtro** para volver a los resultados originales y mostrar la jerarquía de objetivos.
1. (Opcional) Pase el ratón sobre el indicador de progreso para saber dónde debe estar el progreso de la meta para el día actual.

   ![](assets/progress-mouse-over-alignment-chart-350x163.png)

   Se muestra la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Hoy</td> 
      <td>El estado de progreso siempre es actual. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>Real</span> </td> 
      <td>El progreso real (un porcentaje) de la meta en la fecha actual se calcula teniendo en cuenta todos los indicadores de progreso de la meta. Los indicadores de progreso de los objetivos se alinean con las metas, las actividades y los resultados. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Previsto</td> 
      <td> <p>El progreso esperado (un porcentaje) de la meta en la fecha actual suponiendo que logre la meta a tiempo.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en una tarjeta de objetivos para abrir la página de objetivos. Para obtener información sobre cómo editar metas existentes, consulte [Editar metas en Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md). Para obtener información acerca de cómo actualizar el progreso de las metas, consulte [Actualizar el progreso de las metas en Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).

1. Haga clic en la flecha hacia arriba de la meta del nivel actual para volver al nivel anterior en la jerarquía del gráfico.

   O

   (Opcional) Haga clic en **Salir de la jerarquía de metas** para mostrar las tarjetas de todas las metas que coincidan con el filtro actual, sin mostrar su conexión entre sí.


