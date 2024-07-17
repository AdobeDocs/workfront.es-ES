---
product-previous: enterprise-scenario-planner
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Crear y comparar escenarios de plan en el Planificador de escenarios
description: Cuando planea la estrategia a largo plazo de su empresa, hay mucha información que podría no tener o en la que podría pensar al principio. Se necesita tiempo y experimentación para llegar a una estrategia final que las partes interesadas puedan aceptar. Realizar un análisis de "qué tal si" para crear múltiples escenarios para su plan puede ayudarle a predecir y evaluar con precisión las circunstancias potenciales y, en última instancia, a desarrollar el mejor plan posible.
author: Alina
feature: Workfront Scenario Planner
exl-id: 9a79ef81-6271-4cc9-b701-3ba0aeafb324
source-git-commit: 296de69a1c444659c60bcf767bdacdd9e6e36830
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 1%

---

# Crear y comparar escenarios de plan en [!DNL Scenario Planner]

Cuando planea la estrategia a largo plazo de su empresa, hay mucha información que podría no tener o en la que podría pensar al principio. Se necesita tiempo y experimentación para llegar a una estrategia final que las partes interesadas puedan aceptar. Realizar un análisis de &quot;qué tal si&quot; para crear múltiples escenarios para su plan puede ayudarle a predecir y evaluar con precisión las circunstancias potenciales y, en última instancia, a desarrollar el mejor plan posible.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
   <td>[!UICONTROL Empresa] o superior</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licencia*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td><b>Producto</b> </td> 
   <td> <p>Debe adquirir una licencia adicional para la funcionalidad [!DNL Adobe Workfront Scenario Planner] de acceso descrita en este artículo.</p> <p>Para obtener información acerca de cómo obtener [!DNL Workfront Scenario Planner], vea <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acceso necesario para usar [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configuraciones de nivel de acceso*</strong> </td> 
   <td> <p>Editar acceso o superior a [!DNL Scenario Planner]</p> <p>Nota: si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permisos de objeto</strong> </p> </td> 
   <td> <p>Permisos de [!UICONTROL Manage] para un plan</p> <p>Para obtener información sobre cómo solicitar acceso adicional a un plan, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acceso a un plan en [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Creación de escenarios

Un escenario es una copia de un plan. Puede crear tantos escenarios como necesite. Sin embargo, le recomendamos que mantenga el número de escenarios al mínimo para que pueda compararlos fácilmente.

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) y luego haga clic en [!UICONTROL Escenarios].

1. Cree un plan.

   Para obtener información sobre cómo crear planes, consulte [Crear y editar planes en [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   El primer plan que cree se guardará automáticamente como &quot;[!UICONTROL Escenario inicial]&quot;.

1. Haga clic en la flecha hacia abajo situada junto a un escenario existente y, a continuación, haga clic en el icono **[!UICONTROL Copiar]**.

   ![](assets/copy-scenarios-ui-and-highlighted-icon-350x95.png)

   Esto crea un nuevo escenario con la misma información que el escenario copiado. Se le denomina automáticamente &quot;[!UICONTROL escenario 2]&quot; si es el segundo escenario de su plan, &quot;[!UICONTROL escenario 3]&quot; si es el tercero, y así sucesivamente. No puede cambiar el nombre de los escenarios. No hay límite en el número de copias que puede hacer.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE:this might change)
   </MadCap:conditionalText>
   -->

1. Actualice el nuevo escenario de cualquiera de las siguientes maneras:

   * Crear, actualizar o eliminar iniciativas

     >[!TIP]
     >
     >Cuando se elimina una iniciativa en un escenario, solo se elimina del escenario seleccionado, no de todos los escenarios.

     Para obtener información acerca de cómo crear iniciativas, vea [Crear y editar iniciativas en [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   * Actualizar las prioridades de las iniciativas
   * Ajustar personas o información de presupuesto
   * Revisar y ajustar conflictos de iniciativas en su escenario

     Para obtener información sobre la resolución de conflictos, consulte [Resolver conflictos de iniciativas en [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. Haga clic en **[!UICONTROL Guardar plan]** para guardar los cambios.

## Comparar escenarios

Después de crear los escenarios, puede compararlos para encontrar el mejor para su organización.

1. Vaya al plan para el que desea comparar escenarios.
1. Haga clic en **[!UICONTROL Comparar escenarios]**. Se muestra la página de comparación de escenarios.

   Todos los escenarios existentes del plan se muestran en formato de tarjeta en paralelo. El escenario inicial siempre aparece primero y es estático.

   ![](assets/scenario-cards-overlapping-350x166.png)

1. (Opcional) Desplácese a la derecha para ver todas las tarjetas de escenario.

   La siguiente información se muestra en una tarjeta de escenario:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Nombre del escenario</td> 
      <td> <p>Un nombre generado automáticamente por Workfront y no se puede editar. Por ejemplo, "[!UICONTROL Escenario inicial]", "[!UICONTROL Escenario 2]", etc. </p> </td> 
     </tr> 
     <tr> 
      <td>Descripción del escenario</td> 
      <td>Una entrada manual en la que puede describir detalles específicos sobre el escenario. </td> 
     </tr> 
     <tr> 
      <td>Funciones del puesto disponibles</td> 
      <td>Número de funciones del puesto disponibles con cargo al presupuesto del plan durante la vigencia del plan. </td> 
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
      <td>Los costes asociados con las iniciativas en el escenario. Para obtener información acerca de los costos, vea <a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">Introducción a las iniciativas en [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Utilización</td> 
      <td>Porcentaje de [!UICONTROL Utilización del presupuesto] para el plan en este escenario. Para obtener información acerca del porcentaje de [!UICONTROL Utilización del presupuesto], vea <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Información general sobre los planes en [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Valor neto</td> 
      <td>El [!UICONTROL Valor neto] del plan en este escenario. Para obtener información acerca del [!UICONTROL Net Value] de un plan, vea <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Información general sobre planes en [!DNL Scenario Planner]</a>. </td> 
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
   >![](assets/arrows-on-scenario-cards-highlighted-350x70.png)
   >
   >Por ejemplo, el presupuesto, el número de funciones del puesto y el número de iniciativas podrían cambiar de un escenario a otro.

1. Haga clic en el nombre de un escenario para acceder a él y realizar cambios en él.

   Para obtener más información, consulte la sección [Crear escenarios](#create-scenarios) en este artículo.

1. Haga clic en **[!UICONTROL Agregar descripción]** para agregar una descripción para el escenario

   O

   Haga clic en el campo de descripción para actualizarlo y, a continuación, haga clic en cualquier lugar de la pantalla para guardar los cambios.

1. (Opcional) Haga clic en el menú **[!UICONTROL Más]** ![](assets/more-icon.png) para **[!UICONTROL Copiar]** o **[!UICONTROL Eliminar]** el escenario.

   ![](assets/copy-or-delete-scenario-links-from-card-350x109.png)

   Cuando copia un escenario, aparece automáticamente en la página de tarjeta y se le cambia el nombre según este patrón: &quot;[!UICONTROL Escenario] `<next number in order>`&quot;.

1. (Condicional) Si hizo clic en **[!UICONTROL Eliminar]**, haga clic en **[!UICONTROL Sí, eliminarlo]** para confirmar.

   Los escenarios eliminados no se pueden recuperar.

   Para obtener información acerca de cómo eliminar escenarios, vea [Eliminar planes en [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

1. Haga clic en **[!UICONTROL Guardar plan]** para guardar los escenarios y el plan.
