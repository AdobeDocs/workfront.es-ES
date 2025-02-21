---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Resolución de conflictos de iniciativas en el Planificador de escenarios
description: Cuando las iniciativas entran en conflicto entre sí, compiten por los mismos recursos. Los recursos que tiene disponibles para un escenario no son suficientes para cubrir todos los recursos requeridos por todas las iniciativas del escenario.
author: Alina
feature: Workfront Scenario Planner
exl-id: d3a3e177-bece-4e03-89d7-9cee6127bc55
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '2220'
ht-degree: 93%

---

# Resolver conflictos de iniciativas en [!DNL Scenario Planner]

Cuando las iniciativas entran en conflicto entre sí, compiten por los mismos recursos. Los recursos que tiene disponibles para un escenario no son suficientes para cubrir todos los recursos requeridos por todas las iniciativas del escenario.

Esto puede ocurrir en cualquiera de los siguientes casos:

* El número de funciones necesarias para la iniciativa es mayor que el número de funciones presupuestadas para el plan.
* Los costes de la iniciativa son mayores que el importe del presupuesto disponible para el plan.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>Nuevo: Ultimate </p></li>
   <p>El Scenario Planner no está disponible para los nuevos planes Workfront Select o Workfront Prime. </p>
   <li><p>Actual: [!UICONTROL Business] o superior</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licencia*</p> </td> 
   <td> <p>Nuevo: Light o superior</p> 
   <p>Actual: [!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td>Producto* </td> 
   <td> <ul><li><p>Para los nuevos planes de Workfront:</p><p> Adobe Workfront</li></p>
   <li><p>Para los planes actuales de Workfront: </p>
   <p>Adobe Workfront</p> <p>Planificador de escenarios de Adobe Workfront</p></li></ul>

<p>Para obtener más información, consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acceso necesario para utilizar [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Nivel de acceso </td> 
   <td> <p>Acceso de [!UICONTROL Edit] al [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Permisos de objeto </p> </td> 
   <td> <p>Permisos de [!UICONTROL Manage] para un plan</p> <p>Para obtener información sobre cómo solicitar acceso adicional a un plan, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acceso a un plan en [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso a la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Información general sobre la resolución de conflictos

* Un conflicto también se entiende como una sobreasignación de las funciones o el presupuesto de un escenario.
* Cuando [!DNL Workfront] detecta un conflicto, la barra correspondiente al mes en conflicto durante la duración de la iniciativa se muestra en rojo. Esto puede ocurrir en cualquiera de los siguientes casos:

   * El número de funciones necesarias mensualmente para una iniciativa es mayor que el número de funciones presupuestadas para el plan después de que todas las iniciativas anteriores hayan utilizado los recursos presupuestados para el plan.
   * Los costes mensuales de la iniciativa son mayores que el presupuesto disponible para el plan después de que todas las iniciativas anteriores hayan utilizado el presupuesto del plan para cubrir sus costes.

>[!TIP]
>
>De manera predeterminada, [!DNL Scenario Planner] supone que ha presupuestado 0 funciones y 0 $ o el equivalente de 0 $ en la moneda del sistema para un escenario, a menos que especifique lo contrario. El número de funciones indica el número de ETC completas (equivalentes a jornada completa) u horas presupuestadas para la función.
>
>Para todos los cálculos del planificador de escenarios, Workfront utiliza el siguiente valor: 1 FTE = 8 horas.
>
>Para obtener información sobre cómo actualizar las funciones disponibles para un plan y un presupuesto, consulte [Crear y editar planes en el  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

* Para resolver un conflicto, siga uno de estos procedimientos:

   * Añadir automáticamente los recursos necesarios que faltan de las iniciativas en el escenario. Este artículo describe cómo resolver conflictos mediante esta opción.
   * Ajuste los recursos de función y presupuesto para el escenario editando el plan. Para obtener más información, consulte [Crear y editar planes en el  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Resolución de conflictos entre iniciativas

1. Vaya a un plan para el que desee resolver conflictos.

   Para obtener información sobre cómo crear planes, consulte [Crear y editar planes en el  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   Para obtener información sobre cómo crear iniciativas, consulte [Crear y editar iniciativas en el  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. (Opcional) En el menú desplegable **[!DNL Initial scenario]**, seleccione el escenario que desea revisar.

   >[!TIP]
   >
   >Un plan puede tener varios escenarios. Al observar los conflictos del plan, [!DNL Workfront] se refiere a los recursos disponibles actualmente en el escenario seleccionado y a los necesarios en las iniciativas de ese escenario. Para obtener información sobre los escenarios, consulte [Crear y comparar escenarios de plan en el  [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. Asegúrese de que **[!UICONTROL Mostrar conflictos]** esté habilitada. Está habilitada de forma predeterminada.

   ![Mostrar alternancia de escenarios](assets/show-scenarios-toggle-on.png)

   La primera iniciativa en conflicto muestra los meses que tienen conflictos en rojo y aparece un icono de advertencia junto al nombre de la iniciativa.

   El fondo de todas las iniciativas que comienzan con la primera en conflicto se muestra en rojo en el gráfico del plan.

   Cuando una iniciativa muestra un conflicto, significa que el número de función para al menos una función específica, los costes incurridos o ambos exceden el número de funciones o el presupuesto definido para el plan para un mes específico.

   ![Iniciativas en plan con conflicto](assets/initiatives-on-plan-with-conflicts-350x126.png)

1. Realice una de las siguientes acciones para obtener más información sobre los conflictos que podrían existir:

   * Pase el puntero por encima del icono de advertencia situado junto al nombre de la iniciativa para saber si tiene una función o un presupuesto en conflicto.

     ![Conflicto en el rol del presupuesto](assets/budget-job-role-conflict-tooltip-on-warning-icon-350x109.png)

     Dependiendo de si ha asignado demasiadas funciones o ha sobrestimado los costes de su iniciativa, podría ver una de las siguientes opciones al pasar el puntero por encima del icono de advertencia:

      * Mostrar detalles de los conflictos de las funciones del puesto
      * Mostrar detalles de los conflictos del presupuesto
      * Mostrar detalles de los conflictos de las funciones y del presupuesto

   * Cuando visualice el plan por mes, pase el puntero por encima de un mes en la cronología del plan para ver los recursos necesarios para ese mes y si los conflictos del mes están relacionados con las personas o los costes.

     ![Detalles de conflictos en la escala de tiempo mensual](assets/details-of-conflicts-on-monthly-plan-timeline-pop-up-350x178.png)

     Revise la siguiente información mensual en el nivel de plan:

      * Número de funciones disponibles, requeridas y sobreasignadas del mes para todas las iniciativas planificadas para ese mes
      * Los costes disponibles, requeridos y sobreasignados del mes para todas las iniciativas planificadas para ese mes

        >[!TIP]
        >
        >Los costes [!UICONTROL Disponibles] son el presupuesto del escenario para ese mes.

   * Pase el puntero por encima de la barra roja de una iniciativa de un mes para mostrar el cuadro de información adicional sobre el conflicto que se produce ese mes.

     ![Detalles de conflictos en la cronología de la iniciativa](assets/details-of-conflicts-on-initiative-timeline-pop-up-350x113.png)

     Revise los campos siguientes del cuadro de información adicional en el nivel de la iniciativa:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Mes en el que se produce el conflicto</td> 
        <td>Se muestra en el título del cuadro de información adicional.</td> 
       </tr> 
       <tr> 
        <td role="rowheader">El nombre de la iniciativa</td> 
        <td>Se muestra en el título del cuadro de información adicional.</td> 
       </tr> 
       <tr> 
        <td role="rowheader">[!UICONTROL Job Roles]</td> 
        <td> <p>Las funciones asociadas con esta iniciativa que están sobreasignadas para el mes seleccionado. Las siguientes columnas muestran información sobre cada función necesaria para el mes seleccionado y que entra en conflicto con el número de funciones disponibles para ese mes:</p> 
         <ul> 
          <li> <p><strong>[!UICONTROL Available]</strong>: el número de cada función disponible en el escenario para el mes seleccionado.</p> </li> 
          <li> <p><strong>[!UICONTROL Required]</strong>: el número de cada función requerida para la iniciativa en el mes seleccionado.</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[!UICONTROL Overallocated]:</strong> la diferencia entre el número requerido en la iniciativa y el número disponible en el escenario. </p> </li> 
         </ul> <p>Sugerencia: a veces, el número de funciones [!UICONTROL Available] coincide o es mayor que el número de funciones [!UICONTROL Required], pero el [!DNL Scenario Planner] sigue mostrando una sobreasignación. Esto significa que hay iniciativas de mayor clasificación que ya utilizaron las funciones disponibles en el plan para el mismo mes. </p> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Costes</td> 
        <td> <p>Los costes de la iniciativa para el mes seleccionado. Las siguientes columnas muestran información sobre los costes necesarios y el presupuesto disponible del mes seleccionado:</p> 
         <ul> 
          <li> <p><strong>[!UICONTROL Available]</strong>: el presupuesto disponible del plan para el mes seleccionado.</p> </li> 
          <li> <p><strong>[!UICONTROL Required]</strong>: los costes asociados con esta iniciativa para el mes seleccionado.</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[!UICONTROL Overallocated]:</strong> la diferencia entre los costes de la iniciativa y el presupuesto disponible en el plan. </p> </li> 
         </ul> <p>Sugerencia: a veces, los costes [!UICONTROL Available] coinciden o son superiores al coste [!UICONTROL Required] de la iniciativa para el mes seleccionado y el [!DNL Scenario Planner] sigue mostrando una sobreasignación de coste. Esto significa que hay iniciativas de mayor clasificación que ya utilizan el presupuesto disponible en el plan para el mismo mes. </p> </td> 
       </tr> 
      </tbody> 
     </table>

1. Realice una de las siguientes acciones para abrir el panel de detalles de la iniciativa y ver más información sobre dónde se producen los conflictos y resolverlos:

   * Haga clic en el icono de advertencia que está junto al nombre de la iniciativa.
   * Haga clic en la barra de una iniciativa.
   * Haga clic en el icono **[!UICONTROL Más]** ![Más icono](assets/more-icon.png) a la derecha del nombre de la iniciativa y, a continuación, haga clic en **[!UICONTROL Editar]**.

     El panel de detalles de la iniciativa aparece a la derecha.

     Cuando no hay suficientes personas o presupuesto disponibles para su iniciativa, aparece un icono de advertencia rojo junto a las siguientes secciones:

   * [!UICONTROL Funciones requeridas]
   * [!UICONTROL Costes]

1. (Condicional) Para las iniciativas que tienen conflictos de funciones, vaya a la sección **[!UICONTROL Funciones requeridas]** para ver todas las funciones requeridas para su iniciativa. Identifique qué funciones pueden estar sobreasignadas. Revise el número de jornadas completas u horas necesarias para cada función en cada mes de la iniciativa. El cuadro con el número de jornadas completas o de horas de los meses que están sobreasignados se muestra con el contorno en color rojo.

   ![Funciones sobreasignadas](assets/details-panel-overallocated-roles-350x275.png)

1. (Opcional) Haga clic en la flecha que apunta hacia la derecha junto a los meses en la cronología de la iniciativa para ver qué meses adicionales muestran conflictos de funciones.

   ![Error derecho dentro del cuadro de detalles](assets/right-arrow-initiative-months-inside-details-box-highlighted-350x145.png)

1. (Opcional) Haga clic en **[!UICONTROL Mostrar detalles]** en la función que muestra un conflicto para ver dónde aparecen los conflictos y para resaltar los meses en conflicto en el área de gráfico del plan. Se muestra información adicional para cada función.

   Se muestran los campos siguientes para cada función:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Available]</td> 
      <td> <p>El número de funciones disponibles en el plan para cada mes. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Previously allocated]</td> 
      <td>El número de funciones ya asignadas del presupuesto del plan a iniciativas de mayor clasificación para un mes específico. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Overallocated]</td> 
      <td> <p>La diferencia entre el número de funciones requeridas en la iniciativa y el número disponible en el plan después de que las iniciativas de mayor clasificación también hayan utilizado algunas de las funciones. Workfront calcula el número de funciones [!UICONTROL Overallocated] mediante la siguiente fórmula:</p> <p><code>Overallocated roles = (Roles Previously Allocated to higher initiatives + Required roles for current initiative) - Monthly available roles from the plan</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >En el gráfico del plan, los meses en los que se asignan las funciones muestran el nombre y el número de funciones necesarias para cada iniciativa donde hacen falta. Debe seleccionar la vista [!UICONTROL Mes] para ver el nombre de las funciones

   ![Funciones en conflicto](assets/conflicting-job-role-months-on-plan-after-clicking-show-details-350x158.png)

1. Realice una de las siguientes acciones para resolver los conflictos de funciones:

   * Ajuste manualmente el número de funciones para cada mes de la iniciativa a un número menor.
   * Pase el ratón sobre el nombre del rol y haga clic en el icono **[!UICONTROL eliminar]** ![Eliminar icono](assets/delete.png) para eliminar el rol de la iniciativa.
   * Seleccione **[!UICONTROL Agregar funciones del puesto a los recursos disponibles del plan]** y, a continuación, haga clic en **[!UICONTROL Aplicar]**.

     Esto agrega el número que falta de jornadas completas u horas de la función al campo [!UICONTROL Disponible] del escenario.

     >[!NOTE]
     >
     >Las funciones que agrega para resolver los conflictos modifican las funciones [!UICONTROL Disponibles] para el escenario seleccionado y no para todos los escenarios del plan.

     Se muestra una flecha verde hacia arriba ![Flecha verde hacia arriba](assets/upward-green-arrow.png) para el mes en la escala de tiempo del plan para indicar que se agregaron más recursos al plan ese mes. Debe seleccionar la vista [!UICONTROL Mes] para ver este indicador.

   * (Condicional) Cierre el panel de detalles y asigne a la iniciativa una prioridad más alta para recibir primero los recursos de presupuesto del plan, si es posible. Para obtener información sobre cómo actualizar la prioridad de la iniciativa, consulte [Actualizar prioridades de la iniciativa en el planificador de escenarios](../scenario-planner/prioritize-initiatives.md).

1. (Opcional) Haga clic en **[!UICONTROL Ocultar detalles]** para cerrar el cuadro de detalles adicionales y, a continuación, haga clic en **[!UICONTROL Aplicar]** para guardar los cambios que realice en las funciones.

1. (Condicional) Para las iniciativas que tienen conflictos de costes, vaya a la sección **[!UICONTROL Costes]** del panel de detalles de la iniciativa para revisar los costes de cada mes durante la duración de la iniciativa. Identifique los meses en los que es posible que no haya suficiente dinero en el presupuesto del plan para cubrir los costes de la iniciativa seleccionada. El cuadro con el presupuesto disponible insuficiente se muestra con el contorno en color rojo.
1. (Opcional) Haga clic en la flecha que apunta hacia la derecha junto a los meses en la cronología de la iniciativa para ver los meses adicionales que tienen un presupuesto insuficiente para cubrir los costes.

   ![Flecha por costos insuficientes](assets/details-panel-insufficient-costs-350x239.png)

1. (Opcional) Haga clic en **[!UICONTROL Mostrar detalles]** debajo de la información de costes para ver dónde aparece el conflicto y para resaltar los meses en conflicto en el gráfico del plan. Se muestran los siguientes campos adicionales para cada tipo de coste:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Available]</td> 
      <td> <p>Los costes disponibles en el presupuesto del plan para cada mes. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Previously allocated]</td> 
      <td>La cantidad de dinero ya asignada del presupuesto del plan a iniciativas de mayor clasificación. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Overallocated]</td> 
      <td> <p>La diferencia mensual entre los costes necesarios para la iniciativa y la cantidad de dinero disponible del presupuesto del plan después de que las iniciativas de mayor clasificación también hayan utilizado parte del presupuesto disponible. [!DNL Workfront] calcula el número de costes sobreasignados mediante la siguiente fórmula:</p> <p><code>Overallocated costs = (Costs Previously Allocated to higher initiatives + Required costs for the current initiative) - Monthly available budget from the plan</code> </p> <p>[!DNL Workfront] calcula los costes requeridos para la iniciativa actual para cada mes mediante la fórmula siguiente:</p> <p><code>Required initiative costs = Initiative Fixed Costs + Initiative People Costs</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >En el gráfico del plan, los meses en los que los costes son insuficientes muestran el nombre y el número de funciones que aún se necesitan para la iniciativa. Debe seleccionar la vista Mes para ver las cantidades de coste.

   ![Costes en conflicto](assets/conflicting-costs-months-on-plan-after-clicking-show-details-350x139.png)

   >[!NOTE]
   >
   >Si se ha deshabilitado la configuración [!UICONTROL Incluir costes de las personas] en el cuadro [!UICONTROL Presupuesto] del plan al crear el plan, la línea [!UICONTROL Costes de las personas] no se muestra para ninguna iniciativa en ningún escenario. En este caso, Workfront no tiene en cuenta los Costes de las personas al realizar los cálculos para determinar los conflictos de costes. Para obtener información sobre cómo crear un plan, consulte [Crear y editar planes en  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

1. Realice una de las siguientes acciones para resolver los conflictos de costes:

   * Ajuste manualmente el número de [!UICONTROL Costes fijos] para cada mes de la iniciativa a un número menor.
   * En la sección **[!UICONTROL Funciones del puesto requeridas]**, ajuste manualmente el número de funciones para el mes con un presupuesto de Costes de las personas, si es posible. Esto reduce el número de Costes de las personas.

     >[!TIP]
     >
     >No puede ajustar manualmente los Costes de las personas.

   * Seleccione **[!UICONTROL Agregar cantidad al presupuesto del plan]** y, a continuación, haga clic en **[!UICONTROL Aplicar]**.

     Esto añade la cantidad insuficiente al presupuesto del escenario para los meses en los que faltaba, lo que también actualiza el presupuesto del escenario general.

     >[!NOTE]
     >
     >La cantidad que añada para resolver los conflictos de costes modificará el Presupuesto para el escenario seleccionado y no para todos los escenarios del plan.

   * (Condicional) Cierre el panel de detalles y asigne a la iniciativa una prioridad más alta para recibir primero los recursos de presupuesto del plan, si es posible. Para obtener información sobre cómo actualizar la prioridad de la iniciativa, consulte [Actualizar prioridades de la iniciativa en  [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Haga clic en **[!UICONTROL Aplicar]** cuando realice cambios en la sección Costes.
1. Haga clic en **[!UICONTROL Guardar plan]** para guardar los cambios.


