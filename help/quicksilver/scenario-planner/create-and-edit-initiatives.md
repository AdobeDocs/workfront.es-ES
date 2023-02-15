---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Crear y editar iniciativas en el planificador de escenarios
description: Al utilizar el Planificador de escenario de Adobe Workfront, puede crear iniciativas en un plan que haya creado o compartido con usted. Al crear iniciativas, puede mostrar cómo las unidades organizativas más pequeñas contribuyen a la finalización del plan. Por ejemplo, si su organización tiene un plan para los próximos tres años para expandirse a un nuevo mercado, puede crear iniciativas dentro de este plan para que cada departamento calcule las necesidades de personal y presupuesto de cada departamento para llevar a cabo este plan.
author: Alina
feature: Workfront Scenario Planner
exl-id: a811bad0-d3c0-4cba-8b78-d9a14ffc8482
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '1635'
ht-degree: 0%

---

# Cree y edite iniciativas en la [!DNL Scenario Planner]

Al usar la variable [!UICONTROL Planificador de escenario de Adobe Workfront], puede crear iniciativas en un plan que haya creado o que se haya compartido con usted. Al crear iniciativas, puede mostrar cómo las unidades organizativas más pequeñas contribuyen a la finalización del plan. Por ejemplo, si su organización tiene un plan para los próximos tres años para expandirse a un nuevo mercado, puede crear iniciativas dentro de este plan para que cada departamento calcule las necesidades de personal y presupuesto de cada departamento para llevar a cabo este plan.

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
   <td> <p>[!DNL Adobe Workfront] licencia* </p> </td> 
   <td> <p>[!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td>Product </td> 
   <td> <p>Debe adquirir una licencia adicional para [!DNL Adobe Workfront Scenario Planner] para acceder a la funcionalidad descrita en este artículo. </p> <p>Para obtener información sobre cómo obtener la variable [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acceso necesario para usar la variable [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Configuraciones de nivel de acceso* </td> 
   <td> <p>Acceso de [!UICONTROL Edit] o superior a la variable [!DNL Scenario Planner]</p> <p>Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede cambiar el nivel de acceso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Permisos de objeto </p> </td> 
   <td> <p>Permisos de [!UICONTROL Administrar] para un plan</p> <p>Para obtener información sobre la solicitud de acceso adicional a un plan, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acceso a un plan en la [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Requisitos previos

Debe crear un plan u otro usuario debe compartir un plan con usted antes de poder crear una iniciativa dentro de ese plan. Para obtener información sobre la creación de planes, consulte [Cree y edite planes en el [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Para obtener más información sobre las iniciativas, consulte [Información general sobre las iniciativas de [!DNL Scenario Planner]](../scenario-planner/initiatives-overview.md).

## Crear iniciativas

Puede crear iniciativas de las siguientes maneras:

* Desde cero.
* Al importar proyectos en un plan

   Para obtener información sobre la importación de proyectos como iniciativas en un plan, consulte [Importar proyectos a planes en el [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Copie las iniciativas existentes.

   Para obtener información sobre cómo copiar iniciativas, consulte [Copiar iniciativas en la [!DNL Scenario Planner]](../scenario-planner/copy-initiatives.md).

Para crear iniciativas desde cero:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png)y haga clic en [!UICONTROL Situaciones].

1. Haga clic en el nombre del plan para el que desea crear una iniciativa.
1. Haga clic en el **+ icono** a la izquierda de **[!UICONTROL Nueva iniciativa]**

   O

   Haga clic en el **[!UICONTROL Nueva iniciativa]** menú desplegable y seleccione **[!UICONTROL Nueva iniciativa]** o **[!UICONTROL Importar proyectos].**

1. Escriba un nombre para la iniciativa en la **[!UICONTROL Iniciativa sin título]** a continuación, pulse Intro o haga clic en cualquier otra parte de la página.

   La iniciativa se muestra en la cronología del plan, como una barra azul. De forma predeterminada, la duración de una iniciativa es de un mes y siempre comienza en el primer mes del plan.

1. (Opcional) Arrastre la barra de separación entre el panel izquierdo y la cronología para cambiar el tamaño del panel izquierdo.

1. (Opcional) Arrastre el final de la barra de iniciativas para ampliar su duración a más de un mes y suéltela donde desee que termine el mes de la iniciativa.
1. (Opcional y condicional) Si la duración de la iniciativa es menor que la del plan, arrastre y suelte la barra de la iniciativa en una posición diferente en el cronograma del plan, para moverla a otro lapso de tiempo.

   ![](assets/move-initiative-back-and-forth-on-the-timeline-350x71.png)

   >[!IMPORTANT]
   >
   >Solo puede seleccionar una duración en meses. La duración de una iniciativa que cree desde cero nunca podrá exceder la duración del plan.

1. (Opcional) Desde la **[!UICONTROL Mes]** menú desplegable, seleccione una de las siguientes opciones para cambiar la cronología del plan:

   | Opción de menú desplegable | Descripción |
   |---|---|
   | [!UICONTROL Mes] | Muestra la cronología por mes. Esta es la opción predeterminada para un plan de un año. |
   | [!UICONTROL Trimestre] | Muestra la cronología por trimestre. Esta opción solo está disponible cuando la variable [!UICONTROL Duración] del plan es de 3 o 5 años. Esta es la opción predeterminada para un plan de tres años. |
   | [!UICONTROL Año] | Muestra la cronología por año. Esta opción solo está disponible cuando la variable [!UICONTROL Duración] del plan es de 5 años. Esta es la opción predeterminada para un plan de 5 años. |


1. (Opcional) Desplácese de izquierda a derecha para ver toda la duración de la iniciativa.
1. (Opcional) Haga clic en el **[!UICONTROL Hoy]** línea del indicador para volver a la fecha actual.

   ![](assets/today-indicator-350x160.png)

   >[!TIP]
   >
   >Si su plan es futuro o pasado y no incluye la fecha actual, el indicador Hoy no se muestra.

1. Haga clic en la barra de una iniciativa. El panel de detalles de la iniciativa se abre a la derecha.

   ![](assets/initiative-details-panel-multiple-months-350x626.png)

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
      <td role="rowheader">Fechas de inicio y finalización</td> 
      <td>Fechas de inicio y finalización de la iniciativa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sección Funciones de Trabajo Necesarias </td> 
      <td> <p>Haga clic en el <strong>[!UICONTROL Empiece a escribir la función de trabajo]</strong> y seleccione una función de la lista o empiece a escribir el nombre de un<span>n activo</span> función del trabajo. </p> <p><span>Dependiendo de si el plan está configurado para utilizar FTE u horas,</span> añadir el número de funciones de trabajo necesarias para esta iniciativa en FTE <span><span>o horas</span></span><span> para cada mes en la iniciativa</span>. <span>Los tres primeros meses de la iniciativa se muestran de forma predeterminada.</span></p> <p><span>Al actualizar la información de la función de trabajo de la iniciativa también se actualiza la información de la función de trabajo necesaria para el plan.</span> </p> <p>Para obtener información sobre la configuración del plan para utilizar FTE u horas, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Cree y edite planes en el [!DNL Scenario Planner]</a>. </p>
      <p><b>IMPORTANTE</b></p>  
      <p>Para todos los cálculos de la variable [!DNL Scenario Planner], [!DNL Workfront] utiliza el siguiente valor: 1 FTE = 8 horas. </p>

   <p><b>SUGERENCIA</b></p>

   <ul> 
       <li> <p><span>Utilice la tecla [!UICONTROL Tab] para pasar al mes siguiente.</span> </p> </li> 
      <li> <p> Todo <span>active</span> las funciones de trabajo del sistema se enumeran al hacer clic en este campo. </p> </li> 
       <li> <p>Las funciones de trabajo que ya se han agregado a las funciones de trabajo disponibles del plan se muestran primero. Para obtener información sobre cómo agregar funciones de trabajo disponibles a un plan, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Crear y editar planes en el planificador de escenarios</a>. </p> </li> 
       <li> <p>[!DNL Workfront] considera que un equivalente a tiempo completo es de 160 horas durante un mes. </p> <p>Para todos los cálculos del Planificador de escenarios, Workfront utiliza el siguiente valor: 1 FTE = 8 horas. </p></li> 
      </ul> </p> <p>Puede introducir un número inferior a 1 FTE o números decimales para FTE <span>o</span> <span>horas</span>. Por ejemplo, una función de consultor de 0,5 significaría que un consultor dedicaría la mitad de su FTE (normalmente, 4 horas, donde 8 horas es 1 FTE) a trabajar en esta iniciativa. </p>  </td> 
     </tr> 
     <tr> 
      <td rowspan="3" role="rowheader">Sección Costos</td> 
      <td> <p>Los costes totales de la iniciativa se muestran a la derecha de la sección [!UICONTROL Costs]. [!DNL Workfront] calcula los costes de una iniciativa mediante la fórmula siguiente:</p> <p><code>[!UICONTROL Initiative Costs] = [!UICONTROL Fixed Costs] + [!UICONTROL People] Costs</code> </p> </td> 
     </tr> 
     <tr> 
      <td> <p>En el <strong>[!UICONTROL Costes fijos]</strong> , introduzca manualmente una estimación aproximada de lo que cree que costará completar esta iniciativa. Esto no debe incluir los costos asociados con las funciones de trabajo estimadas para la iniciativa.</p> <p><span>Introduzca una cantidad para cada mes de la iniciativa pasando de un mes al siguiente a medida que utiliza la tecla Tab.</span> </p> </td> 
     </tr> 
     <tr> 
      <td> 
       <div> 
        <p>En función de si el plan está configurado para utilizar FTE u horas, [!UICONTROL Workfront] utiliza las siguientes fórmulas para calcular [!UICONTROL People Cost]:</p> 
        <ul> 
         <li> <p>Cuando se utilizan FTE: </p> <p><code>[!UICONTROL People Costs] = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>, donde 160 es el número total de horas de trabajo en un mes. </p> </li> 
         <li> <p style="font-weight: normal;">Al utilizar horas: </p> <p style="font-weight: normal;"><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> <p style="font-weight: normal;">Para obtener información sobre la configuración del plan para utilizar horas o FTE, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Crear y editar planes en el planificador de escenarios</a>.</p> </li> 
        </ul> 
        <p>Los costes de personas se calculan en la moneda base seleccionada en las preferencias de tipos de cambio. Para obtener información sobre las tasas de cambio, consulte <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar tipos de cambio</a>.</p> 
        <p>Al actualizar la información de coste de una iniciativa también se actualiza el área [!UICONTROL Costs] del plan. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"> <p style="font-weight: normal;">Después de definir la función de trabajo y los valores de coste necesarios para la iniciativa y de modificar la duración de la misma, puede darse una de las siguientes situaciones:</p> 
       <ul> 
        <li> <p style="font-weight: normal;">Si acortas la iniciativa, [!DNL Workfront] elimina la cantidad requerida de recursos y los costos asociados con el tiempo eliminado del Plan. Las funciones de trabajo permanecen en el plan, pero no tienen FTE obligatorio o <span data-mc-edit-date="2021-04-19T13:46:01.5004065-04:00" data-mc-editor="alinawilson" data-mc-comment="drafted, yellow" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-04-19T13:45:58.7938344-04:00">horas</span>. Los recursos disponibles para el plan y el presupuesto permanecen inalterados.<br>Para obtener información actualizada sobre el plan, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Cree y edite planes en el [!DNL Scenario Planner]</a>. </p> </li> 
        <li> <p style="font-weight: normal;">Si hace que la iniciativa sea más larga, debe especificar la cantidad de funciones de trabajo y los costes para los meses recién añadidos en la iniciativa. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Net Value] sección</td> 
      <td>En el <strong>[!DNL Net Value]</strong> , introduzca manualmente un importe de estimación aproximada en la <strong>[!UICONTROL Beneficio planificado]</strong> campo . Esto es lo que usted cree que será el beneficio de lograr esta iniciativa. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Si ya ha definido el número de funciones de trabajo y el presupuesto de su plan, el número de funciones y los costes de la iniciativa que está editando y de todas las iniciativas anteriores, y todos exceden las cantidades especificadas para el plan, [!DNL Workfront] puede que descubra que no tiene recursos suficientes para finalizar la iniciativa. [!DNL Workfront] marca esto como un conflicto al intentar lograr esta iniciativa y la muestra como una barra roja. Todas las iniciativas que siguen a la iniciativa en conflicto se muestran en un fondo rojo. Es posible que deba ajustar algunas de las necesidades de sus iniciativas, empezando por la primera que no disponga de recursos suficientes. Para obtener información sobre el ajuste de iniciativas en conflicto, consulte [Resolver conflictos de iniciativa en el [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. (Opcional) Pase el ratón sobre el nombre de una función de trabajo y, a continuación, haga clic en la **[!UICONTROL icono de papelera]** ![](assets/delete.png) para eliminarlo de la iniciativa.

1. (Condicional) Si ha realizado cambios en la iniciativa, haga clic en **[!UICONTROL Aplicar]**.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Add more steps here as you can do more in the Initiative box over time)
   </MadCap:conditionalText>
   -->

1. (Condicional) Si no ha realizado ningún cambio, haga clic en el **X** en la parte superior derecha del panel de detalles de la iniciativa para cerrarlo.
1. (Opcional) Actualice la prioridad de sus iniciativas.

   Para obtener información sobre cómo priorizar iniciativas, consulte [Actualizar las prioridades de la iniciativa en el planificador de escenarios](../scenario-planner/prioritize-initiatives.md).

   >[!TIP]
   >
   >Las iniciativas que aparecen en primer lugar en la lista tienen una prioridad mayor y obtienen recursos antes de las iniciativas que aparecen en la parte inferior de la lista.

1. Haga clic en **[!UICONTROL Guardar plan]**.

   La iniciativa está ahora incluida en su plan.

   Para obtener información sobre la eliminación de iniciativas de un plan, consulte [Elimine iniciativas en [!DNL Scenario Planner]](../scenario-planner/delete-initiatives.md).
