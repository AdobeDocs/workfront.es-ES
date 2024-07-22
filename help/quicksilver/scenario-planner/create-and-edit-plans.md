---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Crear y editar planes en el Scenario Planner
description: Puede crear planes como parte del uso de Workfront Scenario Planner, al priorizar la estrategia de nivel superior de su compañía. Para obtener más información sobre los planes, consulte Información general sobre planes en el Scenario Planner.
author: Alina
feature: Workfront Scenario Planner
exl-id: 15c0e519-0164-449d-84f3-470d0d4eb795
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '2389'
ht-degree: 0%

---

# Crear y editar planes en [!DNL Scenario Planner]

Puede crear planes como parte del uso de [!DNL Workfront Scenario Planner], al priorizar la estrategia de nivel superior de su compañía. Para obtener más información sobre los planes, consulte [Información general sobre los planes en [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: talk about:</p>
<p>- Show people conflicts >> this impacts the conflicts calculation for initiatives>> link to the conflicts article</p>
<p>- explain what hovering over the green upward-pointing arrow does, with screen shot)</p>
</div>
-->

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

## Crear o editar planes

Puede crear un plan desde cero o editar uno existente que se haya compartido con usted.

>[!NOTE]
>
>Después de crear un plan, se le considera el creador y propietario del plan. Cuando se desactiva un usuario, el plan no tiene propietario y nadie puede verlo a menos que se haya compartido previamente con un vínculo.

En este artículo se describe cómo crear un plan desde cero o cómo editar uno existente.

Para todas las consideraciones acerca de los planes, incluida la información disponible para un plan, vea [Información general sobre los planes en [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

Para obtener información sobre cómo eliminar planes, consulte [Eliminar planes en [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

Para crear o editar un plan:

{{step1-to-scenario-planner}}

Se muestra una lista de los planes existentes que ha creado en [!DNL Workfront Scenario Planner].

1. (Opcional) Haga clic en el icono **[!UICONTROL Filtro]** ![](assets/filter-icon-34x37.png)en la esquina superior derecha de la lista de planes y seleccione una de las siguientes opciones:

   | Filtro | Descripción |
   |---|---|
   | [!UICONTROL Todos] | Muestra todos los planes que ha creado o que se han compartido con usted. |
   | [!UICONTROL Mis planes] | Muestra los planes creados. |
   | [!UICONTROL Compartido conmigo] | Muestra los planes compartidos con usted. |

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Opcional) Haga clic en el icono **[!UICONTROL Buscar]** ![](assets/search-icon.png) para escribir una palabra clave y localizar rápidamente un plan en la lista.

1. Haga clic en el nombre de un plan existente para editarlo y continuar con el paso 7.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate) </p>
   -->

   O

   Haga clic en **[!UICONTROL Nuevo plan]** en la esquina superior izquierda para crear un plan y continuar con el paso 5.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate)</p>
   -->

   ![](assets/new-plan-button.png)

   Se muestra el cuadro [!UICONTROL Nuevo plan].

   ![](assets/new-plan-ui-adding-a-new-plan-350x306.png)

1. (Condicional) Cuando cree un nuevo plan, especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre]</td> 
      <td>Escriba un nombre para el plan. Este campo es obligatorio.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p>Importante: <span style="font-weight: normal;">No puede modificar las siguientes selecciones después de crear y guardar el plan.</span> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>FTE ([!UICONTROL Equivalente a tiempo completo]) o [!UICONTROL Horas]</span> </td> 
      <td> <p><span>Seleccione una de las siguientes opciones para indicar cómo desea calcular la información de rol para este plan:</span> </p> 
       <ul> 
      <li> <p><span><strong>ETC</strong>. Este es el valor predeterminado </span> </p> 
      <p><b>IMPORTANTE</b></p>  
      <p>Para todos los cálculos en [!DNL Scenario Planner], [!DNL Workfront] utiliza el siguiente valor: 1 FTE = 8 Horas. </p> </li> 
      <li> <p><strong>[!UICONTROL Horas]</strong> </p> </li> 
       </ul> <p><b>IMPORTANTE</b></p>

   La opción que seleccione aquí determina cómo se muestra la información de funciones del plan, los escenarios del plan y las iniciativas</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Fecha de inicio]</td> 
      <td> <p>Seleccione el mes y el año en que desea que comience el plan. Solo puede seleccionar meses en este campo. [!DNL Workfront] supone que la fecha de inicio del plan es el primer día del mes seleccionado y que la fecha de finalización es el último día del fin de mes de su duración. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Duración]</td> 
      <td> <p>En el menú desplegable, seleccione una de las siguientes duraciones:</p> 
       <ul> 
        <li>1 año. Esta es la duración predeterminada. </li> 
        <li>3 años</li> 
        <li> <p>5 años</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

<!--for table above - how FTE is calcualted: NOTE: snippet below: this is per Ani; it does NOT look at the system FTE.) </p>-->

1. (Condicional) Haga Clic En **[!UICONTROL Siguiente]**.

   La cronología del plan se muestra como **[!UICONTROL escenario inicial]**.

   Para obtener información acerca de cómo crear escenarios adicionales, vea [Crear y comparar escenarios de plan en [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Opcional) En el menú desplegable de la cronología, seleccione una de las opciones de la siguiente tabla para cambiar la forma en que ve la cronología del plan.

   ![](assets/month-dropdown-with-all-options.png)

   | Opción de menú desplegable | Descripción |
   |---|---|
   | [!UICONTROL Mes] | Muestra la cronología por mes. Esta es la única opción predeterminada para un plan de un año. |
   | [!UICONTROL Trimestre] | Muestra la escala de tiempo por trimestre. Esta opción solo está disponible cuando la [!UICONTROL duración] del plan es de 3 o 5 años. Esta es la opción predeterminada para un plan de 3 años. |
   | [!UICONTROL Año] | Muestra la cronología por año. Esta opción solo está disponible cuando la [!UICONTROL duración] del plan es de 5 años. Esta es la opción predeterminada para un plan de 5 años. |

1. (Opcional) Desplácese de izquierda a derecha para ver toda la duración del plan.
1. (Opcional) Haga clic en la línea del indicador **[!UICONTROL Hoy]** para regresar al día actual.

   ![](assets/today-indicator-350x160.png)

1. Haga clic en la casilla **[!UICONTROL Funciones del puesto]** del encabezado del plan para agregar las funciones del puesto que estarán disponibles para ejecutar el plan.

   Se muestran los detalles de la casilla [!UICONTROL Funciones del puesto].

   >[!TIP]
   >
   >La unidad de asignación de roles (ETC u horas) que [!DNL Workfront] utiliza para este plan se muestra entre paréntesis en el título del cuadro.

   ![](assets/adding-people-to-plan-350x206.png)

1. Haga clic en el campo **[!UICONTROL Empiece a escribir el rol]** y seleccione un rol de la lista o empiece a escribir el nombre de un rol activo.

   Todos los puestos de trabajo activos en el sistema se muestran al hacer clic en este campo.

   Esto agrega la función a la columna Funciones del puesto.

1. Actualice o revise la siguiente información para el rol:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Máx. disponible] (para FTE) </p> <p role="rowheader">o </p> <p role="rowheader"><span>[!UICONTROL Total disponible] (para horas)</span> </p> </td> 
      <td> <p><span>Dependiendo de si ha seleccionado utilizar horas o FTE para su plan, escriba</span> el número de jornadas completas de rol <span>u horas</span> disponibles para ejecutar trabajo en el plan en los siguientes campos: </p> 
       <ul> 
        <li> <p style="font-weight: normal;"><strong>[!UICONTROL Total disponible]</strong> (para horas): indique el número total de horas para todos los meses durante la duración del escenario. De manera predeterminada, [!DNL Workfront] divide equitativamente el número total disponible en todos los meses durante el escenario. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>Si escribe 1200 horas para un Designer, significa que el Designer estará disponible durante 100 horas cada mes durante la vigencia del plan, cuando el plan [!UICONTROL Duration] sea de 1 año. </p> </li> 
        <li> <p><b>[!UICONTROL Máximo disponible]</b> (para FTE): indique el número de FTE para el que el rol está disponible cada mes durante la duración del plan. De manera predeterminada, <strong>Workfront</strong> asigna el número [!UICONTROL Max available] a cada mes durante el escenario.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>Si introduce 1 FTE para un consultor, significa que el consultor está disponible para 1 FTE por cada mes durante la duración del plan. </p> <p>Puede introducir un número inferior a 1 FTE. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>Un rol de consultor de 0,5 significaría que un consultor dedicaría la mitad de su tiempo de espera completo (normalmente, 4 horas, donde 8 horas es 1 tiempo de espera completo) a trabajar en este plan. Para todos los cálculos del Scenario Planner, Workfront utiliza el siguiente valor: 1 FTE = 8 horas. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Max required] (para FTE)</p> <p role="rowheader">o </p> <p role="rowheader"><span>[!UICONTROL Total requerido] (para horas)</span> </p> </td> 
      <td> <p><span>Dependiendo de si ha seleccionado utilizar horas o ETC para su plan, revise</span> el número de ETC de rol <span>u horas</span> que son necesarias para completar las iniciativas en el escenario. Revise los campos siguientes:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Total requerido]</strong> (para horas): El número total de horas requeridas para todos los meses durante la duración del plan.</p> </li> 
        <li> <p><strong>[!UICONTROL Max required]</strong> (para FTE): El número máximo de FTE requerido para cualquiera de los meses durante la duración del plan. </p> </li> 
       </ul> <p>Sugerencia: Se muestra el número <span>máximo</span> de jornadas completas <span>o el número total de horas</span> necesarias para ese rol después de empezar a agregar iniciativas. Para obtener información acerca de cómo agregar iniciativas a un plan, vea <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">Crear y editar iniciativas en [!DNL Scenario Planner]</a>.</p> </td> 
     </tr> <!--
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">[!UICONTROL Avg utilization]</td> 
       <td> <p>(NOTE: this field was removed in 21.2 - May 2021) </p> <p>[!DNL Workfront] calculates the average utilization for each job role using the job role FTEs associated with initiatives (required) and the job role FTEs associated with the plan (available). </p> <p> [!DNL Workfront] calculates the job role utilization percentage for a plan using the following formula: </p> <p><code>Job role utilization percentage = Sum [(Required job roles for each month of the plan *100)/ (Available job roles for each month of the plan)] / Number of months in the Duration of the plan</code> </p> 
        <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Example: </b></span></span> 
         <p>For example, if you have a plan with a duration of 12 months and an initiative with the duration of 2 months, where you use 1 Designer for your initiative (required job role) and there are 2 Designers available on the plan (available), the Utilization percentage for the Designer job role is calculated as follows:</p> 
         <p><code>Designer utilization percentage = [(1/2 + 1/2) * 100] / 12 = 100 / 12 = 8.3%</code> </p> 
        </div> <p>As you add job roles to the plan and indicate the Available amount for each one, the [!UICONTROL Utilization] value for each role also updates and [!DNL Workfront] calculates a utilization percentage for the plan. For information about how [!DNL Workfront] calculates the Job Role Utilization for a plan, see <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Plans overview in the [!DNL Scenario Planner]</a>. </p> <p>Tip: The Utilization percentage is rounded and has one decimal. </p> </td> 
      </tr>
     --> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tarifa por hora]</td> 
      <td> <p>Es la tarifa de [!UICONTROL Hora de costo] para el rol. La tarifa por hora se muestra en la moneda de su sistema. Para obtener información sobre cómo configurar las tasas de cambio del sistema, consulte <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar tasas de cambio</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Pase el ratón sobre el nombre de un rol o haga clic en la pestaña después de actualizar la información del rol y, a continuación, haga clic en el icono de la papelera **[!UICONTROL 1} ![](assets/delete.png) para quitarla del plan.]**
1. Haga clic en **[!UICONTROL Distribución de funciones]**.

   El panel de distribución de funciones se muestra para todos los meses en la duración del escenario.

   ![](assets/job-role-monthly-distribution-box-fte-350x144.png)

1. Escriba el nombre de un rol para agregarlo al plan en el **[!UICONTROL campo Empiece a escribir el rol]** y, a continuación, haga clic en Entrar cuando aparezca en la lista. Esto agrega la función a la columna [!UICONTROL Funciones del puesto].
1. Actualice o revise la siguiente información para cada mes del escenario:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Funciones del puesto] (ETC o horas)</td> 
      <td>Tanto la función del puesto disponible para el escenario como las necesarias para las iniciativas del escenario se muestran en el panel de distribución de funciones. Hay una indicación de si las estimaciones de funciones del puesto están en ETC o en horas en el encabezado de la columna. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Disponible] (máximo &lt;número de FTE&gt;) </p> 
       <div> 
        <p>o</p> 
        <p>[!UICONTROL Disponible] (total &lt;número de horas&gt;) </p> 
       </div> </td> 
      <td> <p><span>Dependiendo de si seleccionó usar horas o ETC para su plan, revise o actualice</span> el número mensual de ETC de rol <span>u horas</span> disponibles para el escenario en los siguientes campos:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Disponible] (máximo &lt;número de FTE&gt;)</strong>: El número entre paréntesis muestra el número máximo de funciones disponibles para cualquiera de los meses del escenario. Revise o actualice el número de FTE para cada mes del escenario. Si se cambia la asignación mensual, puede que se actualice el número de FTE entre paréntesis. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Available] (total &lt;number of hours&gt;)</strong>: el número entre paréntesis muestra el número total de horas disponibles para todos los meses del escenario. Revise o actualice el número de horas de cada mes del escenario. Al cambiar la asignación mensual, se actualiza el número de horas entre paréntesis.</span> </p> </li> 
       </ul> <p>La actualización manual de las asignaciones mensuales de funciones es otra forma de resolver los conflictos de funciones entre iniciativas en el escenario. </p> <p>Sugerencia:   <p><span>Para actualizar la disponibilidad mensual de roles durante varios meses, escriba el número de horas o FTE en el campo [!UICONTROL Disponible] de cualquier mes y, a continuación, arrastre la esquina del campo sobre los meses adyacentes para copiar el mismo valor para cada mes. Colóquelo para actualizar todos los meses.</span> </p> <p> <img src="assets/job-role-distribution-draggable-corner-highlighted-350x83.png" style="width: 350;height: 83;"> </p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Requerido] (máximo &lt;número&gt;)</p> 
       <div> 
        <p role="rowheader">o</p> 
        <p role="rowheader">[!UICONTROL Requerido] (total &lt;número&gt;)</p> 
       </div> </td> 
      <td> <p><span>Dependiendo de si seleccionó usar horas o ETC para su plan, revise</span> la cantidad mensual de ETC de rol u horas requeridas para el escenario en los siguientes campos: </p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Obligatorio] (máximo &lt;número de FTE&gt;)</strong>: El número entre paréntesis muestra el número máximo de funciones requeridas para cualquiera de los meses del escenario. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Requerido] (total &lt;número de horas&gt;)</strong>: El número entre paréntesis muestra el número total de horas requeridas para todos los meses del escenario.</span> </p> </li> 
       </ul> <p>Sugerencia: no puede modificar el número requerido de jornadas completas <span> u horas</span> para el rol. Este número se rellena para el escenario después de empezar a añadir iniciativas y sus requisitos de rol. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Diferencia]</td> 
      <td> 
       <div> 
        <p>La diferencia mensual entre las cantidades de puestos requeridos y los puestos disponibles para el escenario. [!DNL Workfront] calcula la diferencia de cada rol para cada mes mediante la siguiente fórmula:</p> 
        <p><code>Monthly role difference = Monthly required roles - Monthly available roles</code> (en ETC o horas) </p> 
        <p>Sugerencia: Cuando la diferencia muestra un número negativo, el escenario requiere más funciones del puesto de las que el plan tiene disponibles. Sus recursos están sobreasignados. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Utilización] %</td> 
      <td> 
       <div> 
        <p>El porcentaje de utilización muestra cuántos de los puestos de trabajo disponibles se utilizan (o son obligatorios) en las iniciativas del escenario. </p> 
        <p>[!DNL Workfront] calcula la utilización por rol y mes mediante la fórmula siguiente: </p> 
        <p><code>Monthly role utilization % = Monthly required roles / Monthly available roles * 100</code> </p> 
        <p>El porcentaje de utilización puede mostrarse en los colores siguientes, según la asignación de los recursos:</p> 
        <ul> 
         <li> <p><b>Verde</b>: Las cantidades de roles disponibles y requeridos coinciden. Los recursos se asignan por completo y el porcentaje de utilización es del 100%. </p> </li> 
         <li> <p><b>Rojo</b>: hay más roles requeridos de los que el plan tiene disponibles. Los recursos están sobreasignados y el porcentaje de utilización es superior al 100%.</p> </li> 
         <li> <p><b>Azul</b>: hay más roles disponibles de los que se requieren. Los recursos están infraasignados y el porcentaje de utilización es inferior al 100 %. </p> </li> 
        </ul> 
       </div> <p> <img src="assets/utilization-percent-colors-sp-350x61.png" style="width: 350;height: 61;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Aplicar]** para guardar la distribución mensual de roles

   O

   Haga clic en **[!UICONTROL Cancelar]** para cerrar la lista de distribución de roles y volver al escenario.

1. Haga clic en el cuadro **[!UICONTROL Financiero]** del encabezado del plan para agregar el presupuesto para este plan.

   Se muestran los detalles del cuadro [!UICONTROL Financiero].

   >[!TIP]
   >
   >La moneda que [!DNL Workfront] usa para este plan se muestra entre paréntesis en el título del cuadro.

1. Especifique el **[!UICONTROL presupuesto anual]**.

   >[!NOTE]
   >
   >Si el plan abarca varios años, debe especificar una cantidad del presupuesto para cada año.

1. Presione Intro para guardar el presupuesto anual y después [!UICONTROL Tab] para pasar al año siguiente.

   El presupuesto anual se distribuye automáticamente de forma equitativa para cada mes del año seleccionado.

1. Haga clic en **[!UICONTROL Avanzado]** para ver la distribución de presupuesto mensual. Los presupuestos anuales y mensuales son siempre números redondeados. Cuando la cantidad del presupuesto no se puede distribuir equitativamente a todos los meses dentro de un año debido a los decimales, se muestra un indicador **[!UICONTROL Restante]** en la distribución del presupuesto anual.

   ![](assets/adanced-and-remaining-links-on-plan-budget-350x507.png)

1. Ajuste manualmente los presupuestos mensuales para eliminar los importes excesivos.

   Cuando el total de todas las cantidades del presupuesto mensual es mayor que el presupuesto anual, aparece un indicador de advertencia **[!UICONTROL Excediendo]** en la distribución del presupuesto anual. Ajuste manualmente las cantidades del presupuesto mensual hasta que sean iguales o inferiores al presupuesto disponible para el plan.

   ![](assets/exceeding-budget-warning-on-plan-350x483.png)

1. Deshabilite la configuración **[!UICONTROL Incluir costes de personas]** para excluir los costes asociados con los roles de trabajo de la contabilización en el coste total del plan. Los costos fijos siempre se contabilizan en el costo total del plan. Esta opción está habilitada de manera predeterminada y afecta a todos los escenarios del plan.
1. Haga clic en cualquier lugar fuera del cuadro [!UICONTROL Financiero] para cerrarlo. La información introducida se guarda automáticamente.

   Ahora puede empezar a crear las iniciativas en el plan y añadir escenarios.

1. (Recomendado) Haga clic en **[!UICONTROL Nueva iniciativa]** para agregar una nueva iniciativa.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Should this include information on how to create scenarios - see also information about scenarios in Manage Plans?)</p>
   -->

   Para obtener información acerca de cómo agregar iniciativas, vea el artículo [Crear y editar iniciativas en [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. (Opcional) Realice una copia del escenario existente para crear un nuevo escenario del mismo plan. Para obtener más información acerca de cómo crear y trabajar con varios escenarios, vea [Crear y comparar escenarios de plan en [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).
1. Haga clic en **[!UICONTROL Guardar plan]**.

   Se ha creado o actualizado su plan.

1. (Opcional) Haga clic en el icono **[!UICONTROL Favoritos]** ![](assets/favorites-icon-small.png) que aparece a la derecha del nombre del plan para agregar el plan a su lista de Favoritos.

1. (Opcional) Copie la dirección URL del plan y envíela a cualquier otro usuario que pueda necesitar revisarla o actualizarla. Deben tener al menos acceso de [!UICONTROL Ver] en su nivel de acceso para poder ver el plan. Deben tener acceso para [!UICONTROL editar] para editarlo. Si debe revisar información financiera del plan, como presupuestos, costos e información sobre tarifas de roles, también debe tener acceso a [!UICONTROL Datos financieros] en su nivel de acceso. Para obtener información acerca del acceso necesario para [!DNL Scenario Planner], vea [Acceso necesario para usar  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).
