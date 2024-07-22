---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Resolución de conflictos de iniciativas en el Scenario Planner
description: Cuando las iniciativas entran en conflicto entre sí, compiten por los mismos recursos. Los recursos que tiene disponibles para un escenario no son suficientes para cubrir todos los recursos requeridos por todas las iniciativas del escenario.
author: Alina
feature: Workfront Scenario Planner
exl-id: d3a3e177-bece-4e03-89d7-9cee6127bc55
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '2164'
ht-degree: 0%

---

# Resolver conflictos de iniciativas en [!DNL Scenario Planner]

Cuando las iniciativas entran en conflicto entre sí, compiten por los mismos recursos. Los recursos que tiene disponibles para un escenario no son suficientes para cubrir todos los recursos requeridos por todas las iniciativas del escenario.

Esto puede ocurrir en cualquiera de los siguientes casos:

* El número de funciones del puesto necesarias para la iniciativa es mayor que el número de funciones presupuestadas para el plan.
* Los costes de la iniciativa son mayores que el importe presupuestario disponible para el plan.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <p>Actual: [!UICONTROL Empresa] o superior</p>
   <p>Nuevo: Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licencia*</p> </td> 
   <td> <p>Nuevo: claro o superior</p> 
   <p>Actual: [!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td>Producto* </td> 
   <td> 
   <p>Para los planes actuales de Workfront: </p>
   <p>Debe adquirir una licencia adicional para la funcionalidad [!DNL Adobe Workfront Scenario Planner] de acceso descrita en este artículo.</p> <p>Para obtener información acerca del acceso y los permisos para [!DNL Workfront Scenario Planner], vea <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acceso necesario para usar [!DNL Scenario Planner]</a>. </p> </td> 
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

## Resumen de resolución de conflictos

* Un conflicto también se entiende como una sobreasignación de las funciones del puesto o el presupuesto de un escenario.
* Cuando [!DNL Workfront] detecta un conflicto, la barra correspondiente al mes en conflicto durante la duración de la iniciativa se muestra en rojo. Esto puede ocurrir en cualquiera de los siguientes casos:

   * El número de funciones del puesto requeridas mensualmente para una iniciativa es mayor que el número de funciones presupuestadas para el plan después de que todas las iniciativas anteriores hayan utilizado los recursos presupuestados para el plan.
   * Los costos mensuales de la iniciativa son mayores que el presupuesto disponible para el plan después de que todas las iniciativas anteriores hayan utilizado el presupuesto del plan para cubrir sus costos.

>[!TIP]
>
>De manera predeterminada, [!DNL Scenario Planner] supone que ha presupuestado 0 roles y $0 o el equivalente de $0 en la moneda del sistema para un escenario, a menos que especifique lo contrario. El número de funciones del puesto indica el número de jornadas completas (equivalentes a tiempo completo) u horas presupuestadas para el rol.
>
>Para todos los cálculos del Scenario Planner, Workfront utiliza el siguiente valor: 1 FTE = 8 horas.
>
>Para obtener información acerca de cómo actualizar los roles disponibles para un plan y un presupuesto, consulte [Crear y editar planes en [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

* Para resolver un conflicto, siga uno de estos procedimientos:

   * Añadir automáticamente los recursos necesarios que faltan de las iniciativas en el escenario. Este artículo describe cómo resolver conflictos mediante esta opción.
   * Ajuste de la función de trabajo y los recursos del presupuesto para el escenario mediante la edición del plan. Para obtener más información, consulte [Crear y editar planes en [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Resolución de conflictos entre iniciativas

1. Vaya a un plan para el que desee resolver conflictos.

   Para obtener información sobre cómo crear planes, consulte [Crear y editar planes en [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   Para obtener información acerca de cómo crear iniciativas, vea [Crear y editar iniciativas en [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. (Opcional) En el menú desplegable **[!DNL Initial scenario]**, seleccione el escenario que desee revisar.

   >[!TIP]
   >
   >Un plan puede tener varios escenarios. Al observar los conflictos del plan, [!DNL Workfront] se refiere a los recursos disponibles actualmente en el escenario seleccionado y a los necesarios en las iniciativas de ese escenario. Para obtener información acerca de los escenarios, vea [Crear y comparar escenarios de plan en [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. Asegúrese de que **[!UICONTROL Mostrar conflictos]** esté habilitado. Está activada de forma predeterminada.

   ![](assets/show-scenarios-toggle-on.png)

   La primera iniciativa en conflicto muestra los meses que tienen conflictos en rojo y aparece un icono de advertencia junto al nombre de la iniciativa.

   El fondo de todas las iniciativas que comienzan con la primera en conflicto se muestra en rojo en el gráfico del plan.

   Cuando una iniciativa muestra un conflicto, significa que el número de funciones del puesto para al menos una función específica, los costes incurridos o ambas exceden el número de funciones del puesto o el presupuesto definido para el plan para un mes específico.

   ![](assets/initiatives-on-plan-with-conflicts-350x126.png)

1. Realice una de las siguientes acciones para obtener más información sobre los conflictos que pueden existir:

   * Pase el ratón sobre el icono de advertencia situado junto al nombre de la iniciativa para saber si tiene un rol o un conflicto presupuestario.

     ![](assets/budget-job-role-conflict-tooltip-on-warning-icon-350x109.png)

     Dependiendo de si ha sobreasignado funciones o ha sobreestimado los costes de su iniciativa, puede ver una de las siguientes opciones al pasar el ratón por encima del icono de advertencia:

      * Mostrar detalles de los conflictos de las funciones del puesto
      * Mostrar detalles de los conflictos del presupuesto
      * Mostrar rol y detalles de presupuesto

   * Cuando visualice el plan por mes, pase el ratón sobre un mes de la cronología del plan para ver los recursos necesarios para ese mes y si los conflictos del mes están relacionados con las personas o los costes.

     ![](assets/details-of-conflicts-on-monthly-plan-timeline-pop-up-350x178.png)

     Revise la siguiente información mensual en el nivel de plan:

      * Número de funciones del puesto disponibles, requeridas y sobreasignadas en el mes para todas las iniciativas planificadas para ese mes
      * Los costes disponibles, requeridos y sobreasignados del mes para todas las iniciativas planificadas para ese mes

        >[!TIP]
        >
        >Los costos [!UICONTROL Disponibles] son el presupuesto del escenario para ese mes.

   * Pase el ratón sobre la barra roja de una iniciativa durante un mes para ver el cuadro de información adicional sobre el conflicto que se produce ese mes.

     ![](assets/details-of-conflicts-on-initiative-timeline-pop-up-350x113.png)

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
        <td role="rowheader">[!UICONTROL Funciones del puesto]</td> 
        <td> <p>Los puestos asociados con esta iniciativa que están sobreasignados para el mes seleccionado. Las siguientes columnas muestran información sobre cada rol necesario para el mes seleccionado que entra en conflicto con el número de roles disponibles para ese mes:</p> 
         <ul> 
          <li> <p><strong>[!UICONTROL Disponible]</strong>: El número de cada rol disponible en el escenario para el mes seleccionado.</p> </li> 
          <li> <p><strong>[!UICONTROL Requerido]</strong>: El número de cada rol requerido para la iniciativa en el mes seleccionado.</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[!UICONTROL sobreasignado]:</strong> La diferencia entre el número requerido en la iniciativa y el número disponible en el escenario. </p> </li> 
         </ul> <p>Sugerencia: A veces, el número de funciones de [!UICONTROL Disponible] coincide o es mayor que el número de funciones de [!UICONTROL Necesario], pero [!DNL Scenario Planner] sigue mostrando una sobreasignación. Esto significa que hay iniciativas de mayor clasificación que ya utilizaron los roles disponibles en el plan para el mismo mes. </p> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Costes</td> 
        <td> <p>Los costes de la iniciativa para el mes seleccionado. Las siguientes columnas muestran información sobre los costes necesarios y el presupuesto disponible del mes seleccionado:</p> 
         <ul> 
          <li> <p><strong>[!UICONTROL Disponible]</strong>: El presupuesto disponible del plan para el mes seleccionado</p> </li> 
          <li> <p><strong>[!UICONTROL Requerido]</strong>: Los costos asociados con esta iniciativa para el mes seleccionado.</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[!UICONTROL Sobreasignado]:</strong> La diferencia entre los costos de la iniciativa y el presupuesto disponible en el plan. </p> </li> 
         </ul> <p>Sugerencia: A veces, los costos de [!UICONTROL Disponible] coinciden o son superiores al costo de [!UICONTROL Requerido] de la iniciativa para el mes seleccionado y [!DNL Scenario Planner] sigue mostrando una sobreasignación de costos. Esto significa que hay iniciativas de mayor clasificación que ya utilizan el presupuesto disponible en el plan para el mismo mes. </p> </td> 
       </tr> 
      </tbody> 
     </table>

1. Realice una de las siguientes acciones para abrir el panel de detalles de la iniciativa y ver más información sobre dónde se producen los conflictos y resolverlos:

   * Haga clic en el icono de advertencia junto al nombre de la iniciativa.
   * Haga clic en la barra de una iniciativa.
   * Haga clic en el icono **[!UICONTROL Más]** ![](assets/more-icon.png) a la derecha del nombre de la iniciativa y luego haga clic en **[!UICONTROL Editar]**.

     El panel de detalles de la iniciativa aparece a la derecha.

     Cuando no hay suficientes personas o presupuesto disponibles para su iniciativa, aparece un icono de advertencia rojo junto a las siguientes secciones:

   * [!UICONTROL Funciones del puesto requeridas]
   * [!UICONTROL Costos]

1. (Condicional) Para las iniciativas que tienen conflictos de roles, vaya a la sección **[!UICONTROL Roles requeridos]** para ver todos los roles requeridos para su iniciativa. Identifique qué funciones del puesto pueden estar sobreasignadas. Revise el número de jornadas completas u horas necesarias para cada rol en cada mes de la iniciativa. El cuadro con el valor de FTE o el número de horas de los meses que tienen sobreasignaciones se muestra en un contorno rojo.

   ![](assets/details-panel-overallocated-roles-350x275.png)

1. (Opcional) Haga clic en la flecha que apunta a la derecha junto a los meses en la cronología de la iniciativa para ver qué meses adicionales muestran conflictos de roles.

   ![](assets/right-arrow-initiative-months-inside-details-box-highlighted-350x145.png)

1. (Opcional) Haga clic en **[!UICONTROL Mostrar detalles]** en el rol que muestra un conflicto para ver dónde aparecen los conflictos y para resaltar los meses en conflicto en el área de gráfico del plan. Se muestra información adicional para cada rol.

   Se muestran los campos siguientes para cada rol:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Disponible]</td> 
      <td> <p>El número de funciones del puesto disponibles en el plan para cada mes. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL asignado anteriormente]</td> 
      <td>El número de funciones del puesto ya asignadas del presupuesto del plan a iniciativas de mayor clasificación para un mes específico. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL sobreasignado]</td> 
      <td> <p>La diferencia entre el número de funciones del puesto requeridas en la iniciativa y el número disponible en el plan después de las iniciativas de mayor clasificación también utilizó algunas de las funciones. Workfront calcula el número de roles de trabajo de [!UICONTROL sobreasignados] mediante la siguiente fórmula:</p> <p><code>Overallocated roles = (Roles Previously Allocated to higher initiatives + Required roles for current initiative) - Monthly available roles from the plan</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >En el gráfico del plan, los meses en los que se asignan los roles muestran el nombre y el número de roles necesarios para cada iniciativa donde son necesarios. Debe seleccionar la vista [!UICONTROL Mes] para ver el nombre de los roles

   ![](assets/conflicting-job-role-months-on-plan-after-clicking-show-details-350x158.png)

1. Realice una de las siguientes acciones para resolver los conflictos de roles:

   * Ajuste manualmente el número de funciones del puesto para cada mes de la iniciativa a un número menor.
   * Pase el ratón sobre el nombre del rol y haga clic en el icono **[!UICONTROL eliminar]** ![](assets/delete.png) para eliminar el rol de la iniciativa.
   * Seleccione **[!UICONTROL Agregar roles a los recursos disponibles del escenario]** y, a continuación, haga clic en **[!UICONTROL Aplicar]**.

     Esto agrega el número que falta de jornadas completas de rol u horas al campo [!UICONTROL Disponible] del escenario.

     >[!NOTE]
     >
     >Las funciones que agrega para resolver los conflictos modifican las funciones del puesto [!UICONTROL Disponibles] para el escenario seleccionado y no para todos los escenarios del plan.

     Se muestra una flecha verde ![](assets/upward-green-arrow.png) orientada hacia arriba para el mes en la escala de tiempo del plan para indicar que se agregaron más recursos al plan ese mes. Debe seleccionar la vista [!UICONTROL Mes] para ver este indicador.

   * (Condicional) Cierre el panel de detalles y asigne a la iniciativa una prioridad más alta para recibir primero los recursos del presupuesto del plan, si es posible. Para obtener información acerca de cómo actualizar la prioridad de la iniciativa, consulte [Actualizar prioridades de la iniciativa en el Scenario Planner](../scenario-planner/prioritize-initiatives.md).

1. (Opcional) Haga clic en **[!UICONTROL Ocultar detalles]** para cerrar la casilla de detalles adicionales y, a continuación, haga clic en **[!UICONTROL Aplicar]** para guardar los cambios que realice en los roles.

1. (Condicional) Para las iniciativas que tienen conflictos de costes, vaya a la sección **[!UICONTROL Costes]** del panel de detalles de la iniciativa para revisar los costes de cada mes de duración de la iniciativa. Identifique los meses en los que es posible que no haya suficiente dinero en el presupuesto del plan para cubrir los costes de la iniciativa seleccionada. El cuadro con el presupuesto insuficiente disponible se muestra en un contorno rojo.
1. (Opcional) Haga clic en la flecha que apunta a la derecha junto a los meses en la cronología de la iniciativa para ver los meses adicionales que tienen un presupuesto insuficiente para cubrir los costes.

   ![](assets/details-panel-insufficient-costs-350x239.png)

1. (Opcional) Haga clic en **[!UICONTROL Mostrar detalles]** debajo de la información de costos para ver dónde aparece el conflicto y para resaltar los meses en conflicto en el gráfico del plan. Se muestran los siguientes campos adicionales para cada tipo de coste:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Disponible]</td> 
      <td> <p>Los costos disponibles en el presupuesto del plan para cada mes. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL asignado anteriormente]</td> 
      <td>La cantidad de dinero ya asignada del presupuesto del plan a iniciativas de mayor rango. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL sobreasignado]</td> 
      <td> <p>La diferencia mensual entre los costos necesarios para la iniciativa y la cantidad de dinero disponible del presupuesto del plan después de iniciativas de mayor rango también utilizó parte del presupuesto disponible. [!DNL Workfront] calcula el número de costos sobreasignados mediante la siguiente fórmula:</p> <p><code>Overallocated costs = (Costs Previously Allocated to higher initiatives + Required costs for the current initiative) - Monthly available budget from the plan</code> </p> <p>[!DNL Workfront] calcula los costes necesarios para la iniciativa actual para cada mes mediante la fórmula siguiente:</p> <p><code>Required initiative costs = Initiative Fixed Costs + Initiative People Costs</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >En el gráfico del plan, los meses en los que los costes son insuficientes muestran el nombre y el número de funciones que aún se necesitan para la iniciativa. Debe seleccionar la vista Mes para ver los importes de coste.

   ![](assets/conflicting-costs-months-on-plan-after-clicking-show-details-350x139.png)

   >[!NOTE]
   >
   >Si deshabilitaste la configuración [!UICONTROL Incluir costo de personas] para la casilla [!UICONTROL Presupuesto] del plan cuando creaste el plan, la línea [!UICONTROL Costos de personas] no se muestra para ninguna iniciativa en ningún escenario. En este caso, Workfront no tiene en cuenta los cálculos de Costes de personas para determinar los conflictos de costes. Para obtener información sobre cómo crear un plan, consulte [Crear y editar planes en [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

1. Realice una de las siguientes acciones para resolver los conflictos de costes:

   * Ajuste manualmente la cantidad de [!UICONTROL costos fijos] por cada mes de la iniciativa a un número menor.
   * En la sección **[!UICONTROL Funciones del puesto requeridas]**, ajuste manualmente el número de funciones del puesto para el mes con un presupuesto de Costos de personas, si es posible. Esto reduce el número de costes de personas.

     >[!TIP]
     >
     >No puede ajustar manualmente los costes de personas.

   * Seleccione **[!UICONTROL Agregar cantidad al presupuesto del escenario]** y haga clic en **[!UICONTROL Aplicar]**.

     Esto añade la cantidad insuficiente al presupuesto del escenario para los meses en los que faltaba, lo que también actualiza el presupuesto del escenario general.

     >[!NOTE]
     >
     >La cantidad que agregue para resolver los conflictos de costos modificará el Presupuesto para el escenario seleccionado y no para todos los escenarios del plan.

   * (Condicional) Cierre el panel de detalles y asigne a la iniciativa una prioridad más alta para recibir primero los recursos del presupuesto del plan, si es posible. Para obtener información acerca de cómo actualizar la prioridad de la iniciativa, vea [Actualizar prioridades de la iniciativa en [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Haga clic en **[!UICONTROL Aplicar]** cuando realice cambios en la sección Costos.
1. Haga clic en **[!UICONTROL Guardar plan]** para guardar los cambios.


