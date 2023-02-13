---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Crear y editar planes en el planificador de escenarios
description: Puede crear planes como parte del uso de Workfront Scenario Planner, al priorizar la estrategia de nivel superior de su empresa. Para obtener más información sobre los planes, consulte Información general sobre los planes en el Planificador de escenarios.
author: Alina
feature: Workfront Scenario Planner
exl-id: 15c0e519-0164-449d-84f3-470d0d4eb795
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '2401'
ht-degree: 1%

---

# Cree y edite planes en el [!DNL Scenario Planner]

Puede crear planes como parte del uso de la variable [!DNL Workfront Scenario Planner], al priorizar la estrategia de más alto nivel de su empresa. Para obtener más información sobre los planes, consulte [Información general sobre los planes de la sección [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: talk about:</p>
<p>- Show people conflicts >> this impacts the conflicts calculation for initiatives>> link to the conflicts article</p>
<p>- explain what hovering over the green upward-pointing arrow does, with screen shot)</p>
</div>
-->

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td>[!UICONTROL Business] o superior</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licencia*</p> </td> 
   <td> <p>[!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td>Product</td> 
   <td> <p>Debe adquirir una licencia adicional para [!DNL Adobe Workfront Scenario Planner] para acceder a la funcionalidad descrita en este artículo.</p> <p>Para obtener información sobre la obtención del [!UICONTROL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Se necesita acceso para utilizar el [!UICONTROL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Configuraciones de nivel de acceso* </td> 
   <td> <p>Acceso de [!UICONTROL Edit] o superior a la variable [!DNL Scenario Planner]</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede cambiar el nivel de acceso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Permisos de objeto </p> </td> 
   <td> <p>[!DNL Manage] permisos para un plan</p> <p>Para obtener información sobre la solicitud de acceso adicional a un plan, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acceso a un plan en la [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Crear o editar planes

Puede crear un plan desde cero o editar uno existente que se compartió con usted.

>[!NOTE]
>
>Después de crear un plan, se le considera creador y propietario del plan. Cuando un usuario está desactivado, el plan no tiene propietario y no es visible para nadie a menos que se haya compartido previamente con un vínculo.

En este artículo se describe cómo crear un plan desde cero o cómo editar un plan existente.

Para todas las consideraciones sobre los planes, incluida la información disponible para un plan, consulte [Información general sobre los planes de la sección [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

Para obtener información sobre cómo eliminar planes, consulte [Eliminar planes en el [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

Para crear o editar un plan:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png)y haga clic en [!UICONTROL Situaciones].

   Una lista de los planes existentes que ha creado se muestra en la [!DNL Workfront Scenario Planner].

1. (Opcional) Haga clic en el **[!UICONTROL Filtro]** icono ![](assets/filter-icon-34x37.png)en la esquina superior derecha de la lista de planes y seleccione una de las siguientes opciones:

   | Filtro | Descripción |
   |---|---|
   | [!UICONTROL Todos] | Muestra todos los planes que ha creado o que se han compartido con usted. |
   | [!UICONTROL Mis planes] | Muestra los planes que ha creado. |
   | [!UICONTROL Compartido conmigo] | Muestra los planes compartidos con usted. |

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Opcional) Haga clic en el **[!UICONTROL Buscar]** icono ![](assets/search-icon.png) para escribir una palabra clave y localizar rápidamente un plan en la lista.

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

   La variable [!UICONTROL Nuevo plan] se muestra.

   ![](assets/new-plan-ui-adding-a-new-plan-350x306.png)

1. (Condicional) Al crear un nuevo plan, especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Escriba un nombre para el plan. Este campo es obligatorio.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p>Importante: <span style="font-weight: normal;">No puede modificar las siguientes selecciones después de crear y guardar el plan.</span> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>FTE ([!UICONTROL Equivalente a tiempo completo]) o [!UICONTROL Hours]</span> </td> 
      <td> <p><span>Seleccione una de las siguientes opciones para indicar cómo desea estimar la información de rol de trabajo para este plan:</span> </p> 
       <ul> 
        <li> <p><span><strong>FTE</strong>. Este es el valor predeterminado </span> </p> <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: snippet below: this is per Ani; it does NOT look at the system FTE.) </p>
         --> <p>Para todos los cálculos de la variable [!DNL Scenario Planner], [!DNL Workfront] utiliza el siguiente valor: 1 FTE = 8 horas. </p> </li> 
        <li> <p><strong>[!UICONTROL Horas]</strong> </p> </li> 
       </ul> <p>Importante: <span>La opción que seleccione aquí determina cómo se muestra la información de la función del trabajo para el plan, los escenarios del plan y las iniciativas.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Fecha de inicio]</td> 
      <td> <p>Seleccione el mes y el año en que desea que comience el plan. En este campo solo puede seleccionar meses. [!DNL Workfront] supone que la fecha de inicio del plan es el primer día del mes seleccionado y que la fecha de finalización es el último día del final del mes de su duración. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Duración]</td> 
      <td> <p>En el menú desplegable, seleccione entre las siguientes duraciones:</p> 
       <ul> 
        <li>1 año. Esta es la duración predeterminada. </li> 
        <li>3 años</li> 
        <li> <p>5 años</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Haga clic en **[!UICONTROL Siguiente]**.

   La cronología del plan se muestra como la **[!UICONTROL Situación inicial]**.

   Para obtener información sobre la creación de escenarios adicionales, consulte [Cree y compare escenarios de plan en la variable [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Opcional) En el menú desplegable cronología, seleccione una de las opciones de la tabla siguiente para cambiar la forma en que ve la cronología del plan.

   ![](assets/month-dropdown-with-all-options.png)

   | Opción de menú desplegable | Descripción |
   |---|---|
   | [!UICONTROL Mes] | Muestra la cronología por mes. Esta es la opción predeterminada y única para un plan de un año. |
   | [!UICONTROL Trimestre] | Muestra la cronología por trimestre. Esta opción solo está disponible cuando la variable [!UICONTROL Duración] del plan es de 3 o 5 años. Esta es la opción predeterminada para un plan de tres años. |
   | [!UICONTROL Año] | Muestra la cronología por año. Esta opción solo está disponible cuando la variable [!UICONTROL Duración] del plan es de 5 años. Esta es la opción predeterminada para un plan de 5 años. |

1. (Opcional) Desplácese de izquierda a derecha para ver toda la duración del plan.
1. (Opcional) Haga clic en el **[!UICONTROL Hoy]** línea del indicador para volver al día actual.

   ![](assets/today-indicator-350x160.png)

1. Haga clic en el **[!UICONTROL Funciones del trabajo]** en el encabezado del plan para agregar funciones de trabajo que estarán disponibles para ejecutar el plan.

   Los detalles del [!UICONTROL Funciones del trabajo] visualización de cuadro.

   >[!TIP]
   >
   >La unidad de asignación de funciones (FTE u horas) que [!DNL Workfront] los usos para este plan se muestran entre paréntesis en el título del cuadro.

   ![](assets/adding-people-to-plan-350x206.png)

1. Haga clic en el **[!UICONTROL Empezar a escribir la función de trabajo]** y seleccione una función de la lista o empiece a escribir el nombre de una función de trabajo activa.

   Todas las funciones de trabajo activas en el sistema se enumeran al hacer clic en este campo.

   Esto agrega la función de trabajo a la columna Funciones de trabajo .

1. Actualice o revise la siguiente información para la función de trabajo:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Max available] (para FTE) </p> <p role="rowheader">o </p> <p role="rowheader"><span>[!UICONTROL Total disponible] (para horas)</span> </p> </td> 
      <td> <p><span>Dependiendo de si ha seleccionado usar horas o FTE para su plan, escriba</span> el número de puestos de trabajo FTE <span>o horas</span> que están disponibles para ejecutar el trabajo en el plan en los campos siguientes: </p> 
       <ul> 
        <li> <p style="font-weight: normal;"><strong>[!UICONTROL Total disponible]</strong> (para horas): Indique el número total de horas para todos los meses durante la duración del escenario. De forma predeterminada, [!DNL Workfront] divide el número total disponible equitativamente entre todos los meses durante la duración del escenario. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>Si introduce 1200 horas para un Diseñador, significa que este estará disponible durante 100 horas cada mes durante la duración del plan, cuando el plan [!UICONTROL Duration] sea de 1 año. </p> </li> 
        <li> <p><b>[!UICONTROL Max disponible]</b> (para FTE): Indique el número de ETC que el puesto de trabajo está disponible para cada mes durante la duración del plan. De forma predeterminada, <strong>Workfront</strong> asigna el número [!UICONTROL Max available] a cada mes durante el escenario.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>Si introduce 1 FTE para un consultor, significa que el consultor está disponible para 1 FTE por cada mes durante la duración del plan. </p> <p>Puede introducir un número inferior a 1 FTE. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>Una función de consultor de 0,5 significaría que un consultor dedicaría la mitad de su tiempo libre (normalmente, 4 horas, donde 8 horas es 1 hora a largo plazo) a trabajar en este plan. Para todos los cálculos del Planificador de escenarios, Workfront utiliza el siguiente valor: 1 FTE = 8 horas. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Max obligatorio] (para FTE)</p> <p role="rowheader">o </p> <p role="rowheader"><span>[!UICONTROL Total requerido] (para horas)</span> </p> </td> 
      <td> <p><span>Dependiendo de si ha seleccionado usar horas o FTE para su plan, revise</span> el número de puestos de trabajo FTE <span>o horas</span> que son necesarias para completar las iniciativas en el escenario. Revise los campos siguientes:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Total requerido]</strong> (para horas): Número total de horas necesarias para todos los meses durante la duración del plan.</p> </li> 
        <li> <p><strong>[!UICONTROL Max obligatorio]</strong> (para FTE): Número máximo de ETC necesarios para cualquiera de los meses durante la duración del plan. </p> </li> 
       </ul> <p>Sugerencia: La variable <span>máximo</span> número de ETC <span>o el número total de horas</span> necesario para esa función de trabajo se muestra después de empezar a agregar iniciativas. Para obtener información sobre cómo agregar iniciativas a un plan, consulte <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">Cree y edite iniciativas en la [!DNL Scenario Planner]</a>.</p> </td> 
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
      <td role="rowheader">[!UICONTROL Frecuencia por hora]</td> 
      <td> <p>Es la tasa de [!UICONTROL Cost Hour] para la función de trabajo. La tasa por hora se muestra en la moneda del sistema. Para obtener información sobre la configuración de las tasas de cambio para su sistema, consulte <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar tipos de cambio</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Pase el ratón sobre el nombre de una función de trabajo o haga clic en la pestaña después de actualizar la información de la función y, a continuación, haga clic en la **[!UICONTROL icono de papelera]** ![](assets/delete.png) para quitarlo del plan.
1. Haga clic en **[!UICONTROL Distribución de funciones de trabajo]**.

   El panel de distribución de funciones de trabajo se muestra durante todos los meses mientras dure el escenario.

   ![](assets/job-role-monthly-distribution-box-fte-350x144.png)

1. Escriba el nombre de una función de trabajo para agregarla al plan en la **[!UICONTROL Empezar a escribir el campo de función del trabajo]** y, a continuación, haga clic en Intro cuando aparezca en la lista. Esto agrega la función de trabajo a la variable [!UICONTROL Funciones del trabajo] para abrir el Navegador.
1. Actualice o revise la siguiente información para cada mes del escenario:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Funciones de trabajo] (FTE u horas)</td> 
      <td>Tanto la función de trabajo disponible para el escenario como las necesarias para las iniciativas en el escenario se muestran en el panel de distribución de funciones de trabajo. Hay una indicación de si las estimaciones de funciones de trabajo están en FTE u horas en el encabezado de la columna. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Disponible] (máx. &lt;number of="" ftes=""&gt;) </p> 
       <div> 
        <p>o</p> 
        <p>[!UICONTROL Disponible] (total &lt;number of="" hours=""&gt;) </p> 
       </div> </td> 
      <td> <p><span>Dependiendo de si ha seleccionado usar horas o FTE para su plan, revise o actualice</span> el número mensual de puestos de trabajo FTE <span>o horas</span> disponible para el escenario en los campos siguientes:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Disponible] (máx. &lt;number of="" ftes=""&gt;)</strong>: El número entre paréntesis muestra el número máximo de funciones disponibles para cualquiera de los meses del escenario. Revise o actualice el número de ETC para cada mes del escenario. Cambiar la asignación mensual podría actualizar el número de ETC entre paréntesis. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Disponible] (total &lt;number of="" hours=""&gt;)</strong>: El número entre paréntesis muestra el número total de horas disponibles para todos los meses del escenario. Revise o actualice el número de horas para cada mes del escenario. Al cambiar la asignación mensual, se actualiza el número de horas entre paréntesis.</span> </p> </li> 
       </ul> <p>La actualización manual de las asignaciones mensuales de funciones de trabajo es otra manera de resolver los conflictos de funciones entre las iniciativas en el escenario. </p> <p>Sugerencia:   <p><span>Para actualizar la disponibilidad de la función mensual durante varios meses, escriba el número de horas o TLC en el campo [!UICONTROL Disponible] de cualquier mes y, a continuación, arrastre la esquina del campo durante los meses adyacentes para copiar el mismo valor para cada mes. Suéltelo para actualizar todos los meses.</span> </p> <p> <img src="assets/job-role-distribution-draggable-corner-highlighted-350x83.png" style="width: 350;height: 83;"> </p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Requerido] (máx. &lt;number&gt;)</p> 
       <div> 
        <p role="rowheader">o</p> 
        <p role="rowheader">[!UICONTROL Requerido] (total &lt;number&gt;)</p> 
       </div> </td> 
      <td> <p><span>Dependiendo de si ha seleccionado usar horas o FTE para su plan, revise</span> el número mensual de FTE o horas de función de trabajo necesarias para el escenario en los campos siguientes: </p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Requerido] (máx. &lt;number of="" ftes=""&gt;)</strong>: El número entre paréntesis muestra el número máximo de funciones necesarias para cualquiera de los meses del escenario. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Requerido] (total &lt;number of="" hours=""&gt;)</strong>: El número entre paréntesis muestra el número total de horas necesarias para todos los meses del escenario.</span> </p> </li> 
       </ul> <p>Sugerencia: No puede modificar el número requerido de FTE <span>o horas</span> para la función de trabajo. Este número se rellena para el escenario después de empezar a agregar iniciativas y sus requisitos de rol de trabajo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Diferencia]</td> 
      <td> 
       <div> 
        <p>Diferencia mensual entre las cantidades de funciones de trabajo requeridas y disponibles para el escenario. [!DNL Workfront] calcula la diferencia para cada función de trabajo para cada mes mediante la fórmula siguiente:</p> 
        <p><code>Monthly role difference = Monthly required roles - Monthly available roles</code> (en FTE u horas) </p> 
        <p>Sugerencia: Cuando la diferencia muestra un número negativo, el escenario requiere más funciones de trabajo de las que el plan tiene disponibles. Los recursos están sobreasignados. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Utilización] %</td> 
      <td> 
       <div> 
        <p>El porcentaje de utilización muestra cuántas de las funciones de trabajo disponibles se utilizan (o son necesarias) en las iniciativas del escenario. </p> 
        <p>[!DNL Workfront] calcula la utilización por función de trabajo por mes mediante la fórmula siguiente: </p> 
        <p><code>Monthly role utilization % = Monthly required roles / Monthly available roles * 100</code> </p> 
        <p>El porcentaje de utilización podría mostrarse en los colores siguientes, según la asignación de los recursos:</p> 
        <ul> 
         <li> <p><b>Verde</b>: Los números disponibles y requeridos de roles de trabajo coinciden. Los recursos se asignan por completo y el porcentaje de utilización es del 100%. </p> </li> 
         <li> <p><b>Rojo</b>: Hay más funciones de trabajo requeridas de las que el plan tiene disponibles. Los recursos están sobreasignados y el porcentaje de utilización es superior al 100%.</p> </li> 
         <li> <p><b>Azul</b>: Hay más funciones de trabajo disponibles de las necesarias. Los recursos están subasignados y el porcentaje de utilización es inferior al 100%. </p> </li> 
        </ul> 
       </div> <p> <img src="assets/utilization-percent-colors-sp-350x61.png" style="width: 350;height: 61;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Aplicar]** para guardar la distribución mensual de funciones de trabajo

   O

   Haga clic en **[!UICONTROL Cancelar]** para cerrar la lista de distribución de funciones de trabajo y volver al escenario.

1. Haga clic en el **[!UICONTROL Financiera]** en el encabezado del plan, para añadir el presupuesto para este plan.

   Los detalles del [!UICONTROL Financiera] visualización de cuadro.

   >[!TIP]
   >
   >La moneda que [!DNL Workfront] los usos para este plan se muestran entre paréntesis en el título del cuadro.

1. Especifique la variable **[!UICONTROL Presupuesto anual]**.

   >[!NOTE]
   >
   >Si el plan abarca varios años, debe especificar un importe presupuestario para cada año.

1. Pulse Intro para guardar el presupuesto anual y, a continuación, [!UICONTROL Tabulación] para pasar al año siguiente.

   El presupuesto anual se distribuye automáticamente por igual para cada mes del año seleccionado.

1. Haga clic en **[!UICONTROL Avanzadas]** para ver la distribución del presupuesto mensual. Los presupuestos anuales y mensuales siempre son números redondeados. Cuando el importe del presupuesto no se puede distribuir por igual a todos los meses de un año debido a decimales a **[!UICONTROL Restante]** se muestra en la distribución del presupuesto anual.

   ![](assets/adanced-and-remaining-links-on-plan-budget-350x507.png)

1. Ajuste manualmente los presupuestos mensuales para eliminar las cantidades excesivas.

   Cuando el total de todos los importes de presupuesto mensuales es mayor que el presupuesto anual, se muestra una **[!UICONTROL Excedente]** el indicador de advertencia se muestra en la distribución del presupuesto anual. Ajuste manualmente los importes del presupuesto mensual hasta que sean iguales o inferiores al presupuesto disponible para el plan.

   ![](assets/exceeding-budget-warning-on-plan-350x483.png)

1. Desactive el **[!UICONTROL Incluir costes de personal]** para excluir los costes asociados con funciones de trabajo de la contabilización al coste general del plan. Los costes fijos siempre se contabilizan en función del coste total del plan. Esta configuración está habilitada de forma predeterminada y afecta a todas las situaciones del plan.
1. Haga clic en cualquier lugar fuera de [!UICONTROL Financiera] para cerrarlo. La información introducida se guarda automáticamente.

   Ahora puede empezar a crear las iniciativas en el plan y a agregar escenarios.

1. (Recomendado) Haga clic en **[!UICONTROL Nueva iniciativa]** para agregar una nueva iniciativa.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Should this include information on how to create scenarios - see also information about scenarios in Manage Plans?)</p>
   -->

   Para obtener información sobre cómo agregar iniciativas, consulte el artículo [Cree y edite iniciativas en la [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. (Opcional) Realice una copia del escenario existente para crear un nuevo escenario del mismo plan. Para obtener más información sobre cómo crear y trabajar con varios escenarios, consulte [Cree y compare escenarios de plan en la variable [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).
1. Haga clic en **[!UICONTROL Guardar plan]**.

   El plan se crea o actualiza.

1. (Opcional) Haga clic en el **[!UICONTROL Icono Favoritos]** ![](assets/favorites-icon-small.png) a la derecha del nombre del plan para agregar el plan a su lista de Favoritos.

1. (Opcional) Copie la dirección URL del plan y envíela a cualquier otro usuario que necesite revisarlo o actualizarlo. Deben tener al menos [!UICONTROL Ver] acceso en su nivel de acceso para poder ver el plan. Deben tener [!UICONTROL Editar] para editarlo. Si deben revisar la información financiera sobre el plan, como los presupuestos, los costos y la información sobre las tasas de puestos de trabajo, también deben tener acceso a [!UICONTROL Datos financieros] en su nivel de acceso. Para obtener información sobre el acceso necesario para la variable [!DNL Scenario Planner], consulte [Acceso necesario para usar la variable [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).
