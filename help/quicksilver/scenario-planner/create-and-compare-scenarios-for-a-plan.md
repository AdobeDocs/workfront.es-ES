---
product-previous: enterprise-scenario-planner
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Crear y comparar escenarios de plan en el planificador de escenarios
description: Cuando planea la estrategia a largo plazo de su empresa, hay mucha información que podría no tener o en la que podría no pensar al principio. Se necesita tiempo y experimentación para llegar a una estrategia final que las partes interesadas puedan aceptar. Realizar un análisis de “qué tal si” para crear múltiples escenarios para su plan puede ayudarle a predecir y evaluar con precisión las circunstancias potenciales y, en última instancia, a desarrollar el mejor plan posible.
author: Alina
feature: Workfront Scenario Planner
exl-id: 9a79ef81-6271-4cc9-b701-3ba0aeafb324
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '964'
ht-degree: 94%

---

# Crear y comparar escenarios de plan en el [!DNL Scenario Planner]

<!--Audited: 07/2024-->

Cuando planea la estrategia a largo plazo de su empresa, hay mucha información que podría no tener o en la que podría no pensar al principio. Se necesita tiempo y experimentación para llegar a una estrategia final que las partes interesadas puedan aceptar. Realizar un análisis de “qué tal si” para crear múltiples escenarios para su plan puede ayudarle a predecir y evaluar con precisión las circunstancias potenciales y, en última instancia, a desarrollar el mejor plan posible.

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

## Crear escenarios

Un escenario es una copia de un plan. Puede crear tantos escenarios como necesite. Sin embargo, le recomendamos que mantenga el número de escenarios al mínimo para que pueda compararlos fácilmente.

{{step1-to-scenario-planner}}

1. Cree un plan o haga clic en el nombre de uno existente.

   Para obtener información sobre la creación de planes, consulte [Crear y editar planes en el  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   El primer plan que cree se guardará automáticamente como “[!UICONTROL Initial scenario]”.

1. Haga clic en la flecha hacia abajo situada junto a un escenario existente y, a continuación, en el icono **[!UICONTROL Copy]**.

   ![Copiar escenario](assets/copy-scenarios-ui-and-highlighted-icon-350x95.png)

   De esta forma, se crea un nuevo escenario con la misma información que el escenario copiado. Se le denomina automáticamente “[!UICONTROL Scenario 2]” si es el segundo escenario de su plan, &quot;[!UICONTROL Scenario 3]&quot; si es el tercero, y así sucesivamente. No se puede cambiar el nombre de los escenarios. No hay límite en el número de copias que se pueden realizar.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE:this might change)
   </MadCap:conditionalText>
   -->

1. Actualice el nuevo escenario de cualquiera de las siguientes maneras:

   * Crear, actualizar o eliminar iniciativas

     >[!TIP]
     >
     >Cuando se elimina una iniciativa en un escenario, solo se elimina del escenario seleccionado, no de todos.

     Para obtener información sobre la creación de iniciativas, consulte [Crear y editar iniciativas en el  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   * Actualizar las prioridades de las iniciativas
   * Ajustar información sobre las personas o el presupuesto
   * Revisar y ajustar conflictos entre iniciativas en su escenario

     Para obtener información sobre la resolución de conflictos, consulte [Resolver conflictos entre iniciativas en el  [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. Haga clic en **[!UICONTROL Save Plan]** para guardar los cambios.

## Comparar escenarios

Después de crear los escenarios, puede compararlos para encontrar el mejor para su organización.

1. Vaya al plan para el que desea comparar escenarios.
1. Haga clic en **[!UICONTROL Comparar escenarios]**. Se muestra la página de comparación de escenarios.

   Todos los escenarios existentes del plan se muestran en formato de tarjeta en paralelo. El escenario inicial siempre aparece primero y es estático.

   ![Tarjetas de escenario](assets/scenario-cards-overlapping-350x166.png)

1. (Opcional) Desplácese a la derecha para ver todas las tarjetas de escenario.

   En una tarjeta de escenario se muestra la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Nombre del escenario</td> 
      <td> <p>Un nombre generado automáticamente por Workfront que no se puede editar. Por ejemplo, "[!UICONTROL Escenario inicial]", "[!UICONTROL Escenario 2]", etc. </p> </td> 
     </tr> 
     <tr> 
      <td>Descripción del escenario</td> 
      <td>Una entrada manual en la que puede describir detalles específicos sobre el escenario. </td> 
     </tr> 
     <tr> 
      <td>Funciones del puesto disponibles</td> 
      <td>Número de funciones del puesto disponibles con cargo al presupuesto del plan durante la durante del plan. </td> 
     </tr> 
     <tr> 
      <td>Funciones del puesto requeridas</td> 
      <td>El número de funciones del puesto requeridas, en función de sus iniciativas. </td> 
     </tr> 
     <tr> 
      <td>Presupuesto</td> 
      <td>Presupuesto total definido para el plan en este escenario. Para obtener información sobre el presupuesto de los planes, consulte <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Información general sobre los planes en [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Costes</td> 
      <td>Los costes asociados con las iniciativas en el escenario. Para obtener información acerca de los costes, consulte <a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">Introducción a las iniciativas en [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Utilización</td> 
      <td>Porcentaje de [!UICONTROL Utilización del presupuesto] para el plan en este escenario. Para obtener información acerca del porcentaje de [!UICONTROL Utilización del presupuesto], vea <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Información general sobre los planes en [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Valor neto</td> 
      <td>El [!UICONTROL Valor neto] del plan en este escenario. Para obtener información acerca del [!UICONTROL Valor neto] de un plan, vea <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Información general sobre planes en [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Iniciativas</td> 
      <td>Número de iniciativas del plan en este escenario.</td> 
     </tr> 
     <tr> 
      <td>Conflictivo</td> 
      <td>Número de iniciativas que muestran cualquier tipo de conflictos en el plan para este escenario. Para obtener información sobre conflictos de iniciativas, consulte <a href="../scenario-planner/resolve-conflicts-in-sp.md" class="MCXref xref">Resolver conflictos de iniciativas en [!DNL Scenario Planner]</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Cuando la información difiere entre el escenario inicial y los escenarios adicionales, aparece una flecha arriba o abajo junto al valor que ha cambiado para indicar un aumento o una disminución de ese valor, en comparación con el escenario inicial.
   >
   >
   >![Flechas en las tarjetas de escenario](assets/arrows-on-scenario-cards-highlighted-350x70.png)
   >
   >Por ejemplo, el presupuesto, el número de funciones del puesto y el número de iniciativas podrían cambiar de un escenario a otro.

1. Haga clic en el nombre de un escenario para acceder a él y realizar cambios.

   Para obtener más información, consulte la sección [Crear escenarios](#create-scenarios) en este artículo.

1. Haga clic en **[!UICONTROL Agregar descripción]** para agregar una descripción para el escenario

   O

   Haga clic en el campo de descripción para actualizarlo y, a continuación, haga clic en cualquier lugar de la pantalla para guardar los cambios.

1. (Opcional) Haga clic en el menú **[!UICONTROL Más]** ![Icono de más](assets/more-icon.png) para **[!UICONTROL Copiar]** o **[!UICONTROL Eliminar]** el escenario.

   ![Copiar o eliminar escenario](assets/copy-or-delete-scenario-links-from-card-350x109.png)

   Cuando copia un escenario, aparece automáticamente en la página de tarjeta y se le cambia el nombre según este patrón: &quot;[!UICONTROL Escenario] `<next number in order>`&quot;.

1. (Condicional) Si hizo clic en **[!UICONTROL Eliminar]**, haga clic en **[!UICONTROL Sí, eliminarlo]** para confirmar.

   Los escenarios eliminados no se pueden recuperar.

   Para obtener información acerca de cómo eliminar escenarios, vea [Eliminar planes en [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

1. Haga clic en **[!UICONTROL Guardar plan]** para guardar los escenarios y el plan.
