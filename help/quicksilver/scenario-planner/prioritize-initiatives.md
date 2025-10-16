---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Actualizar las prioridades de la iniciativa en el Scenario Planner
description: La priorización de iniciativas es importante porque las iniciativas reciben funciones de trabajo y recursos presupuestarios del plan en el orden en que se enumeran en el plan.
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 13%

---

# Actualizar prioridades de iniciativa en [!DNL Scenario Planner]

La priorización de iniciativas es importante porque las iniciativas reciben funciones de trabajo y recursos presupuestarios del plan en el orden en que se enumeran en el plan.

Puede priorizar iniciativas en un plan que haya creado o en un plan que alguien haya compartido con usted.

Para obtener información sobre cómo crear planes, consulte [Crear y editar planes en el  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Para obtener información sobre cómo crear iniciativas, consulte [Crear y editar iniciativas en el  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

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

<!--<table style="table-layout:auto"> 
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

## Actualizar prioridades de iniciativa

Al cambiar la prioridad de las iniciativas, se modifica el orden de listado en el plan.

Le recomendamos que coloque las iniciativas más urgentes en la parte superior de un plan y las más fluidas -que se podrían hacer en cualquier momento y solo si hay recursos disponibles- en la parte inferior del plan.

>[!NOTE]
>
>[!DNL Workfront] asigna recursos de plan a iniciativas en el orden en que aparecen en el plan.
>
>Por ejemplo, si el plan tiene 3 ingenieros disponibles y la Iniciativa 1 y la Iniciativa 2 necesitan 2 ingenieros para completarse y ambos están programados para el mismo lapso de tiempo, Workfront asocia 2 ingenieros con la Iniciativa 1 y un ingeniero disponible restante con la Iniciativa 2. En este caso, la Iniciativa 2 se muestra como si tuviera un conflicto, ya que le falta un ingeniero. A veces, cambiar la prioridad de sus iniciativas es la única manera de evitar conflictos en un plan.

Para actualizar la prioridad de la iniciativa:

{{step1-to-scenario-planner}}

Se muestra una lista de planes.

1. Haga clic en el nombre de un plan para abrirlo y luego busque las iniciativas que desee priorizar.
1. Haga clic en la casilla a la izquierda del nombre de una o más iniciativas y realice una de las siguientes acciones:

   * Haga clic en el controlador de la izquierda de uno de los nombres de iniciativas seleccionadas y, a continuación, arrástrelo hacia arriba o hacia abajo en la lista para cambiar la prioridad de la iniciativa.

     Workfront muestra el número de iniciativas seleccionadas.

     ![Número de iniciativa de selección múltiple](assets/multi-select-initiative-number.png)

   * Haga clic en el cuadro **[!UICONTROL Priorizar]** de la parte inferior del plan y elija una de las siguientes opciones:

      * **[!UICONTROL Principales]**: mueve las iniciativas seleccionadas al principio de la lista de iniciativas. Las iniciativas seleccionadas se enumeran primero en el plan.
      * **[!UICONTROL Inferior]**: mueve las iniciativas seleccionadas al final de la lista de iniciativas. Las iniciativas seleccionadas se muestran en último lugar del plan.
      * **[!UICONTROL Seleccionar un número]**: mueve las iniciativas seleccionadas después de la iniciativa indicada aquí.

        ![Priorizar iniciativas](assets/prioritize-initiatives-expanded-highlighted-350x171.png)

     [!DNL Workfront] coloca inmediatamente las iniciativas seleccionadas donde usted indica y los números de todas las iniciativas se actualizan en consecuencia.

1. Haga clic en **[!UICONTROL Guardar plan]** para guardar los cambios.
