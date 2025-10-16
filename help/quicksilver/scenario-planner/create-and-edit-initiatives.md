---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Crear y editar iniciativas en el planificador de escenarios
description: Al usar el Planificador de escenarios de Adobe Workfront, es posible crear iniciativas en un plan que haya creado o que se haya compartido con usted. Al crear iniciativas, es posible mostrar cómo las unidades organizativas más pequeñas contribuyen a la finalización del plan. Por ejemplo, si la organización tuviera un plan para los próximos tres años con el fin de expandirse a un nuevo mercado, cree iniciativas dentro de este plan para cada departamento para estimar la necesidad de las personas y el presupuesto de cada departamento para llevar a cabo este plan.
author: Alina
feature: Workfront Scenario Planner
exl-id: a811bad0-d3c0-4cba-8b78-d9a14ffc8482
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '1604'
ht-degree: 94%

---

# Creación y edición de iniciativas en el [!DNL Scenario Planner]

<!--Audited: 07/2024-->

Al usar el [!UICONTROL Planificador de escenarios de Adobe Workfront], se pueden crear iniciativas en un plan que haya creado o que se haya compartido con usted. Al crear iniciativas, es posible mostrar cómo las unidades organizativas más pequeñas contribuyen a la finalización del plan. Por ejemplo, si la organización tuviera un plan para los próximos tres años con el fin de expandirse a un nuevo mercado, cree iniciativas dentro de este plan para cada departamento para estimar la necesidad de las personas y el presupuesto de cada departamento para llevar a cabo este plan.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] paquete</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>NOTA</b></p>
<p>Hable con su representante de Workfront si tiene un paquete de Workfront diferente.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licencia</p> </td> 
   <td> <p>[!UICONTROL Light] o superior</p> 
   <p>[!UICONTROL Review] o superior</p> </td> 
  </tr> 
    <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de [!UICONTROL Edit] al [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permisos de objeto </p> </td> 
   <td> <p>Permisos de [!UICONTROL Manage] para un plan</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el acceso al Scenario Planner, consulte [Acceso necesario para usar el [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Para obtener información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso a la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Requisitos previos

Deberá crear un plan u otro usuario deberá compartir un plan con usted antes de que pueda crear una iniciativa dentro de ese plan. Para obtener información sobre cómo crear planes, consulte [Crear y editar planes en  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Para obtener más información acerca de las iniciativas, consulte [Información general sobre iniciativas en  [!DNL Scenario Planner]](../scenario-planner/initiatives-overview.md).

## Crear iniciativas

Es posible crear iniciativas de las siguientes maneras:

* Desde cero
* Al importar proyectos en un plan

  Para obtener información acerca de cómo importar proyectos como iniciativas en un plan, consulte [Importación de proyectos a planes en el [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Copiando las iniciativas existentes.

  Para obtener información sobre cómo copiar iniciativas, consulte [Copiar iniciativas en  [!DNL Scenario Planner]](../scenario-planner/copy-initiatives.md).

Para crear iniciativas desde cero:

{{step1-to-scenario-planner}}

1. Haga clic en el nombre del plan para el que quiera crear una iniciativa.
1. Haga clic en el **icono +** situado a la izquierda de **[!UICONTROL Nueva iniciativa]**

   O

   Haga clic en el menú desplegable **[!UICONTROL Nueva iniciativa]** y seleccione **[!UICONTROL Nueva iniciativa]** o **[!UICONTROL Importar proyectos].**

1. Escriba un nombre para la iniciativa en el campo **[!UICONTROL Iniciativa sin título]** y, a continuación, presione Entrar o haga clic en cualquier otro lugar de la página.

   La iniciativa se mostrará en la línea de tiempo del plan como una barra azul. De forma predeterminada, la duración de una iniciativa es de un mes y siempre comienza en el primer mes del plan.

1. (Opcional) Arrastre la barra de separación que hay entre el panel izquierdo y la línea de tiempo para cambiar el tamaño del panel izquierdo.

1. (Opcional) Arrastre el final de la barra de iniciativa para ampliar su duración a más de un mes y suéltela donde desee que esté el mes de finalización.
1. (Opcional y condicional) Si la duración de la iniciativa fuese más corta que la del plan, arrastre y suelte la barra de iniciativa en una posición diferente de la línea de tiempo del plan para moverla a otro lapso de tiempo.

   ![Mover iniciativa en la cronología](assets/move-initiative-back-and-forth-on-the-timeline-350x71.png)

   >[!IMPORTANT]
   >
   >Solo es posible seleccionar la duración en meses. La duración de una iniciativa que cree desde cero nunca podrá superar la duración del plan.

1. (Opcional) En el menú desplegable **[!UICONTROL Mes]**, seleccione una de las siguientes opciones para cambiar la línea de tiempo del plan:

   | Opción de menú desplegable | Descripción |
   |---|---|
   | [!UICONTROL Mes] | Muestra la línea de tiempo por mes. Es la opción predeterminada para un plan de un año. |
   | [!UICONTROL Trimestre] | Muestra la línea de tiempo por trimestre. Esta opción solo está disponible cuando la [!UICONTROL duración] del plan es de 3 o 5 años. Esta es la opción predeterminada para un plan de tres años. |
   | [!UICONTROL Año] | Muestra la línea de tiempo por año. Esta opción solo está disponible cuando la [!UICONTROL duración] del plan es de 5 años. Esta es la opción predeterminada para un plan de 5 años. |


1. (Opcional) Desplácese de izquierda a derecha para ver toda la duración de la iniciativa.
1. (Opcional) Haga clic en la línea del indicador **[!UICONTROL Hoy]** para regresar a la fecha actual.

   ![Indicador de hoy](assets/today-indicator-350x160.png)

   >[!TIP]
   >
   >Si su plan está en el futuro o el pasado y no incluye la fecha actual, el indicador Hoy no se muestra.

1. Haga clic en la barra de una iniciativa. El panel de detalles de la iniciativa se abre a la derecha.

   ![Panel de detalles de la iniciativa](assets/initiative-details-panel-multiple-months-350x626.png)

   Especifique o revise la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Duración de la iniciativa</td> 
      <td>La duración de la iniciativa en meses. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Fechas de inicio y de finalización</td> 
      <td>Las fechas de inicio y finalización de la iniciativa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sección Funciones de trabajo necesarias </td> 
      <td> <p>Haga clic en el campo <strong>[!UICONTROL Start typing job role]</strong> y seleccione una función de la lista o empiece a escribir el nombre de una función<span></span> activa. </p> <p><span>Dependiendo de si el plan se ha configurado para utilizar FTE u horas,</span> añada el número de funciones del puesto necesarias para esta iniciativa en EJC <span><span>u horas</span></span><span> para cada mes en la iniciativa</span>. <span>De forma predeterminada, se muestran los tres primeros meses de la iniciativa.</span></p> <p><span>Al actualizar la información de la función de la iniciativa, también se actualiza la información de función necesaria para el plan.</span> </p> <p>Para obtener información sobre cómo configurar el plan para que utilice EJC u horas, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Crear y editar planes en el [!DNL Scenario Planner]</a>. </p>
      <p><b>IMPORTANTE</b></p>  
      <p>Para todos los cálculos en [!DNL Scenario Planner], [!DNL Workfront] utiliza el siguiente valor: 1 EJC = 8 Horas. </p>

   <p><b>Sugerencia</b></p>

   <ul> 
       <li> <p><span>Use la tecla [!UICONTROL Tab] para pasar al mes siguiente.</span> </p> </li> 
      <li> <p> Al hacer clic en este campo, se muestran todas las funciones de trabajo <span>activas</span> del sistema. </p> </li> 
       <li> <p>Las funciones que ya se han añadido a las funciones disponibles se muestran primero. Para obtener información sobre cómo añadir funciones del puesto disponibles a un plan, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Crear y editar planes en el Planificador de escenarios</a>. </p> </li> 
       <li> <p>[!DNL Workfront] considera que un equivalente a jornada completa es de 160 horas por mes. </p> <p>Para todos los cálculos del planificador de escenarios, Workfront utiliza el siguiente valor: 1 FTE = 8 horas. </p></li> 
      </ul> </p> <p>Puede escribir un número inferior a 1 EJC o números decimales para EJC <span> u </span> <span>horas</span>. Por ejemplo, un puesto de consultor de 0,5 significaría que un consultor dedicaría la mitad de su FTE (normalmente, 4 horas, donde 8 horas es 1 jornada completa) a trabajar en esta iniciativa. </p>  </td> 
     </tr> 
     <tr> 
      <td rowspan="3" role="rowheader">Sección Costes</td> 
      <td> <p>Los costes totales de la iniciativa se muestran a la derecha de la sección [!UICONTROL Costs]. [!DNL Workfront] calcula los costes de una iniciativa mediante la fórmula siguiente:</p> <p><code>[!UICONTROL Initiative Costs] = [!UICONTROL Fixed Costs] + [!UICONTROL People] Costs</code> </p> </td> 
     </tr> 
     <tr> 
      <td> <p>En el campo <strong>[!UICONTROL Fixed Costs]</strong>, escriba manualmente una cantidad aproximada de lo que cree que costará completar esta iniciativa. Esto no debe incluir los costes asociados a las funciones estimadas para la iniciativa.</p> <p><span>Escriba una cantidad por cada mes de la iniciativa pasando de un mes al siguiente mientras usa la tecla Tab.</span> </p> </td> 
     </tr> 
     <tr> 
      <td> 
       <div> 
        <p>Dependiendo de si el plan se ha configurado para utilizar EJC u horas, [!UICONTROL Workfront] utiliza las siguientes fórmulas para calcular [!UICONTROL People Cost]:</p> 
        <ul> 
         <li> <p>Cuando se utilizan EJC: </p> <p><code>[!UICONTROL People Costs] = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>, donde 160 es el número total de horas laborables al mes. </p> </li> 
         <li> <p style="font-weight: normal;">Al utilizar horas: </p> <p style="font-weight: normal;"><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> <p style="font-weight: normal;">Para obtener información acerca de cómo configurar el plan para usar horas o EJC, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Crear y editar planes en el planificador de escenarios</a>.</p> </li> 
        </ul> 
        <p>Los costes de las personas se calculan en la moneda base seleccionada en las preferencias de tasas de cambio. Para obtener más información sobre los tipos de cambio, consulte <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configuración de los tipos de cambio</a>.</p> 
        <p>Al actualizar la información de coste de una iniciativa, también se actualiza el área de [!UICONTROL Costs] del plan. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"> <p style="font-weight: normal;">Después de definir los valores de función y coste necesarios para la iniciativa y de modificar su duración, puede producirse uno de los siguientes casos:</p> 
       <ul> 
        <li> <p style="font-weight: normal;">Si acorta la iniciativa, [!DNL Workfront] elimina la cantidad de recursos necesaria y los costes asociados con el tiempo eliminado del plan. Las funciones permanecen en el plan, pero no tienen un valor de FTE requerido u <span data-mc-edit-date="2021-04-19T13:46:01.5004065-04:00" data-mc-editor="alinawilson" data-mc-comment="drafted, yellow" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-04-19T13:45:58.7938344-04:00">horas</span>. Los recursos disponibles para el plan y el presupuesto permanecen inalterados.<br>Para actualizar información sobre el plan, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Crear y editar planes en [!DNL Scenario Planner]</a>. </p> </li> 
        <li> <p style="font-weight: normal;">Si alarga la iniciativa, debe especificar la cantidad de funciones y los costes para los meses recién añadidos en la iniciativa. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Net Value] sección</td> 
      <td>En la sección <strong>[!DNL Net Value]</strong>, escriba manualmente una cantidad aproximada en el campo <strong>[!UICONTROL Planned Benefit]</strong>. Esto es lo que se cree que será el beneficio de lograr esta iniciativa. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Si ya ha definido las funciones del trabajo y el presupuesto para su plan, así como las funciones del trabajo y los costes de la iniciativa que está editando, además de todas las iniciativas por encima de esta, y todas exceden las cantidades especificadas para el plan, [!DNL Workfront] podría darse el caso de no tener suficientes recursos para finalizar la iniciativa. [!DNL Workfront] marca esto como un conflicto al intentar conseguir esta iniciativa y lo muestra como una barra roja. Todas las iniciativas que siguen a la iniciativa en conflicto se muestran en un fondo rojo. Es posible que tenga que ajustar algunas de las necesidades de sus iniciativas, empezando por la primera que no tenga recursos suficientes. Para obtener información sobre cómo ajustar iniciativas en conflicto, consulte [Resolver conflictos de iniciativas en  [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. (Opcional) Pase el ratón sobre el nombre de un rol y luego haga clic en el **[!UICONTROL icono de la papelera]** ![Eliminar icono](assets/delete.png) para quitarlo de la iniciativa.

1. (Condicional) Si realizó cambios en la iniciativa, haga clic en **[!UICONTROL Aplicar]**.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Add more steps here as you can do more in the Initiative box over time)
   </MadCap:conditionalText>
   -->

1. (Condicional) Si no ha realizado cambios, haga clic en el icono **X** en la parte superior derecha del panel de detalles de la iniciativa para cerrarlo.
1. (Opcional) Actualice la prioridad de sus iniciativas.

   Para obtener información sobre cómo priorizar iniciativas, consulte [Actualizar prioridades de iniciativas en el planificador de escenarios](../scenario-planner/prioritize-initiatives.md).

   >[!TIP]
   >
   >Las iniciativas que aparecen primero en la lista tienen una prioridad más alta y obtienen recursos antes que las iniciativas que aparecen más abajo.

1. Haga clic en **[!UICONTROL Guardar plan]**.

   La iniciativa ahora se ha incluido en su plan.

   Para obtener información acerca de cómo eliminar iniciativas de un plan, vea [Eliminar iniciativas en el  [!DNL Scenario Planner]](../scenario-planner/delete-initiatives.md).
