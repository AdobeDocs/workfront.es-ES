---
product-previous: enterprise-scenario-planner
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Crear y comparar escenarios de plan en el planificador de escenarios
description: Cuando planifica la estrategia a largo plazo de su empresa, hay mucha información que podría no tener o no pensar al principio. Se necesita tiempo y experimentación para llegar a una estrategia final que sus partes interesadas puedan aceptar. Realizar un análisis de "qué tal si" para crear múltiples escenarios para su plan puede ayudarle a predecir y evaluar con precisión las circunstancias potenciales y, en última instancia, a desarrollar el mejor plan posible.
author: Alina
feature: Workfront Scenario Planner
exl-id: 9a79ef81-6271-4cc9-b701-3ba0aeafb324
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '950'
ht-degree: 1%

---

# Cree y compare escenarios de plan en la variable [!DNL Scenario Planner]

Cuando planifica la estrategia a largo plazo de su empresa, hay mucha información que podría no tener o no pensar al principio. Se necesita tiempo y experimentación para llegar a una estrategia final que sus partes interesadas puedan aceptar. Realizar un análisis de &quot;qué tal si&quot; para crear múltiples escenarios para su plan puede ayudarle a predecir y evaluar con precisión las circunstancias potenciales y, en última instancia, a desarrollar el mejor plan posible.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
   <td>[!UICONTROL Business] o superior</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licencia*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td><b>Product</b> </td> 
   <td> <p>Debe adquirir una licencia adicional para [!DNL Adobe Workfront Scenario Planner] para acceder a la funcionalidad descrita en este artículo.</p> <p>Para obtener información sobre cómo obtener la variable [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acceso necesario para usar la variable [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configuraciones de nivel de acceso*</strong> </td> 
   <td> <p>Editar acceso o superior a la variable [!DNL Scenario Planner]</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permisos de objeto</strong> </p> </td> 
   <td> <p>Permisos de [!UICONTROL Administrar] para un plan</p> <p>Para obtener información sobre la solicitud de acceso adicional a un plan, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acceso a un plan en la [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Crear escenarios

Un escenario es una copia de un plan. Puede crear tantos escenarios como necesite. Sin embargo, le recomendamos que mantenga el número mínimo de escenarios para que pueda compararlos fácilmente.

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png)y haga clic en [!UICONTROL Situaciones].

1. Cree un plan.

   Para obtener información sobre la creación de planes, consulte [Cree y edite planes en el [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   El primer plan que cree se guarda automáticamente como el[!UICONTROL Situación inicial].&quot;

1. Haga clic en la flecha que apunta hacia abajo junto a un escenario existente y, a continuación, haga clic en la **[!UICONTROL Copiar]** icono.

   ![](assets/copy-scenarios-ui-and-highlighted-icon-350x95.png)

   Esto crea un nuevo escenario con la misma información que el escenario copiado. Se denomina automáticamente &quot;[!UICONTROL Escenario 2]&quot; si es el segundo escenario de su plan, &quot;[!UICONTROL Escenario 3]&quot; si es la tercera, y así sucesivamente. No puede cambiar el nombre de los escenarios.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE:this might change)
   </MadCap:conditionalText>
   -->

1. Actualice el nuevo escenario de cualquiera de estas formas:

   * Crear, actualizar o eliminar iniciativas

      >[!TIP]
      >
      >Cuando elimina una iniciativa en un escenario, solo se elimina del escenario seleccionado, no de todos los escenarios.

      Para obtener información sobre la creación de iniciativas, consulte [Cree y edite iniciativas en la [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   * Actualizar las prioridades de sus iniciativas
   * Ajustar información de personas o presupuestos
   * Revise y ajuste los conflictos de iniciativa en su escenario

      Para obtener información sobre la resolución de conflictos, consulte [Resolver conflictos de iniciativa en el [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. Haga clic en **[!UICONTROL Guardar plan]** para guardar los cambios.

## Comparar escenarios

Después de crear los escenarios, puede compararlos para encontrar el mejor para su organización.

1. Vaya al plan para el que desea comparar escenarios.
1. Haga clic en **[!UICONTROL Comparar escenarios]**. Se muestra la página de comparación de escenarios.

   Todos los escenarios existentes para el plan se muestran en un formato de tarjeta contiguo. El escenario Initial siempre se enumera primero y es estático.

   ![](assets/scenario-cards-overlapping-350x166.png)

1. (Opcional) Desplácese a la derecha para ver todas las tarjetas del escenario.

   La siguiente información se muestra en una tarjeta de escenario:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Nombre del escenario</td> 
      <td> <p>Un nombre generado automáticamente por Workfront y no se puede editar. Por ejemplo, "[!UICONTROL Initial scenario]", "[!UICONTROL Scenario 2]", etc. </p> </td> 
     </tr> 
     <tr> 
      <td>Descripción del escenario</td> 
      <td>Una entrada manual en la que puede describir aspectos específicos sobre el escenario. </td> 
     </tr> 
     <tr> 
      <td>Funciones de trabajo disponibles</td> 
      <td>Número de funciones laborales disponibles en el presupuesto del plan durante la duración del plan. </td> 
     </tr> 
     <tr> 
      <td>Funciones del puesto requeridas</td> 
      <td>Número de funciones de trabajo necesarias, según sus iniciativas. </td> 
     </tr> 
     <tr> 
      <td>Presupuesto</td> 
      <td>El presupuesto total definido para el plan en este escenario. Para obtener información presupuestaria sobre los planes, consulte <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Información general sobre los planes de la sección [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Costes</td> 
      <td>Los costes asociados con las iniciativas en el escenario. Para obtener información sobre los costes, consulte <a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">Información general sobre las iniciativas de [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Utilización</td> 
      <td>El porcentaje de [!UICONTROL Budget Utilization] para el plan en este escenario. Para obtener información sobre el porcentaje de [!UICONTROL Budget Utilization] , consulte <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Información general sobre los planes de la sección [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Valor neto</td> 
      <td>El [!UICONTROL Valor neto] del plan en este escenario. Para obtener información sobre el [!UICONTROL Net Value] de un plan, consulte <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Información general sobre los planes de la sección [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Iniciativas</td> 
      <td>Número de iniciativas para el plan en este escenario.</td> 
     </tr> 
     <tr> 
      <td>Conflictivo</td> 
      <td>Número de iniciativas que muestran cualquier tipo de conflicto en el plan para este escenario. Para obtener información sobre los conflictos de iniciativas, consulte <a href="../scenario-planner/resolve-conflicts-in-sp.md" class="MCXref xref">Resolver conflictos de iniciativa en el [!DNL Scenario Planner]</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Cuando la información difiere entre el escenario inicial y los escenarios adicionales, aparece una flecha hacia arriba o hacia abajo junto al valor que cambió para indicar un aumento o una disminución en ese valor, en comparación con el escenario inicial.
   >
   >
   >![](assets/arrows-on-scenario-cards-highlighted-350x70.png)
   >
   >Por ejemplo, el presupuesto, el número de funciones, el número de iniciativas puede cambiar de un escenario a otro.

1. Haga clic en el nombre de un escenario para acceder a él y realizar cambios.

   Para obtener más información, consulte la [Crear escenarios](#create-scenarios) en este artículo.

1. Haga clic en **[!UICONTROL Agregar descripción]** para agregar una descripción para el escenario

   O

   Haga clic en el campo de descripción para actualizarlo y, a continuación, haga clic en cualquier lugar de la pantalla para guardar los cambios.

1. (Opcional) Haga clic en el **[!UICONTROL Más]** menú ![](assets/more-icon.png) a **[!UICONTROL Copiar]** o **[!UICONTROL Eliminar]** el escenario.

   ![](assets/copy-or-delete-scenario-links-from-card-350x109.png)

   Al copiar un escenario, aparece automáticamente en la página de la tarjeta y se le cambia el nombre según este patrón: &quot;[!UICONTROL Situación] `<next number in order>`.&quot;

1. (Condicional) Si ha hecho clic en **[!UICONTROL Eliminar]**, haga clic en **[!UICONTROL Sí, elimínelo]** para confirmar.

   Los escenarios eliminados no se pueden recuperar.

   Para obtener información sobre la eliminación de escenarios, consulte [Eliminar planes en el [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

1. Haga clic en **[!UICONTROL Guardar plan]** para guardar los escenarios y su plan.
