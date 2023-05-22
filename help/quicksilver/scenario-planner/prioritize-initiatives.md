---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Actualizar las prioridades de iniciativa en el Scenario Planner
description: La priorización de iniciativas es importante porque las iniciativas reciben funciones de trabajo y recursos presupuestarios del plan en el orden en que se enumeran en el plan.
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# Actualizar prioridades de iniciativa en [!DNL Scenario Planner]

La priorización de iniciativas es importante porque las iniciativas reciben funciones de trabajo y recursos presupuestarios del plan en el orden en que se enumeran en el plan.

Puede priorizar iniciativas en un plan que haya creado o en un plan que alguien haya compartido con usted.

Para obtener información sobre la creación de planes, consulte [Crear y editar planes en [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Para obtener información sobre la creación de iniciativas, consulte [Cree y edite iniciativas en [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Requisitos de acceso

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
   <td><b>Product</b> </td> 
   <td> <p>Debe adquirir una licencia adicional para el [!DNL Adobe Workfront Scenario Planner] para acceder a la funcionalidad descrita en este artículo.</p> <p>Para obtener información sobre la obtención de [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acceso necesario para utilizar [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configuraciones de nivel de acceso*</strong> </td> 
   <td> <p>[!UICONTROL Edit] acceso o superior a [!DNL Scenario Planner]</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo [!DNL Workfront] El administrador puede cambiar su nivel de acceso. Consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permisos de objeto</strong> </p> </td> 
   <td> <p>Permisos de [!UICONTROL Manage] para un plan</p> <p>Para obtener información sobre cómo solicitar acceso adicional a un plan, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicite acceso a un plan en el [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Actualizar prioridades de iniciativa

Al cambiar la prioridad de las iniciativas, se modifica el orden de listado en el plan.

Le recomendamos que coloque las iniciativas más urgentes en la parte superior de un plan y las más fluidas -que se podrían hacer en cualquier momento y solo si hay recursos disponibles- en la parte inferior del plan.

>[!NOTE]
>
>[!DNL Workfront] asigna recursos del plan a iniciativas en el orden en que aparecen en el plan.
>
>Por ejemplo, si el plan tiene 3 ingenieros disponibles y la Iniciativa 1 y la Iniciativa 2 necesitan 2 ingenieros para completarse y ambos están programados para el mismo lapso de tiempo, Workfront asocia 2 ingenieros con la Iniciativa 1 y un ingeniero disponible restante con la Iniciativa 2. En este caso, la Iniciativa 2 se muestra como si tuviera un conflicto, ya que le falta un ingeniero. A veces, cambiar la prioridad de sus iniciativas es la única manera de evitar conflictos en un plan.

Para actualizar la prioridad de la iniciativa:

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png), luego haga clic en [!UICONTROL Escenarios].

   Se muestra una lista de planes.

1. Haga clic en el nombre de un plan para abrirlo y luego busque las iniciativas que desee priorizar.
1. Haga clic en la casilla a la izquierda del nombre de una o más iniciativas y realice una de las siguientes acciones:

   * Haga clic en el controlador de la izquierda de uno de los nombres de iniciativas seleccionadas y, a continuación, arrástrelo hacia arriba o hacia abajo en la lista para cambiar la prioridad de la iniciativa.

      Workfront muestra el número de iniciativas seleccionadas.

      ![](assets/multi-select-initiative-number.png)

   * Haga clic en **[!UICONTROL Priorizar]** en la parte inferior del plan y, a continuación, elija una de las siguientes opciones:

      * **[!UICONTROL Superior]**: Mueve las iniciativas seleccionadas al principio de la lista de iniciativas. Las iniciativas seleccionadas se enumeran primero en el plan.
      * **[!UICONTROL Inferior]**: mueve las iniciativas seleccionadas al final de la lista de iniciativas. Las iniciativas seleccionadas se muestran en último lugar del plan.
      * **[!UICONTROL Seleccione un número]**: mueve las iniciativas seleccionadas después de la iniciativa que indique aquí.

         ![](assets/prioritize-initiatives-expanded-highlighted-350x171.png)
      [!DNL Workfront] coloca inmediatamente las iniciativas seleccionadas donde indique y los números de todas las iniciativas se actualizan en consecuencia.


1. Clic **[!UICONTROL Guardar plan]** para guardar los cambios.
