---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Actualizar las prioridades de la iniciativa en el planificador de escenarios
description: Las iniciativas de priorización son importantes porque las iniciativas reciben funciones de trabajo y recursos presupuestarios del plan en el orden en que aparecen en el plan.
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# Actualizar las prioridades de la iniciativa en el [!DNL Scenario Planner]

Las iniciativas de priorización son importantes porque las iniciativas reciben funciones de trabajo y recursos presupuestarios del plan en el orden en que aparecen en el plan.

Puede priorizar las iniciativas en un plan que haya creado o en un plan que alguien haya compartido con usted.

Para obtener información sobre la creación de planes, consulte [Cree y edite planes en el [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Para obtener información sobre la creación de iniciativas, consulte [Cree y edite iniciativas en la [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Requisitos de acceso

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
   <td> <p>Acceso de [!UICONTROL Edit] o superior a la variable [!DNL Scenario Planner]</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede cambiar el nivel de acceso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permisos de objeto</strong> </p> </td> 
   <td> <p>Permisos de [!UICONTROL Administrar] para un plan</p> <p>Para obtener información sobre la solicitud de acceso adicional a un plan, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acceso a un plan en la [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Actualizar las prioridades de la iniciativa

Cuando cambia la prioridad de las iniciativas, modifica su orden de inclusión en el plan.

Le recomendamos que coloque iniciativas más urgentes en la parte superior de un plan y las más fluidas, que podrían hacerse en cualquier momento y sólo si se dispone de recursos, en la parte inferior del plan.

>[!NOTE]
>
>[!DNL Workfront] asigna recursos del plan a iniciativas en el orden en que aparecen en el plan.
>
>Por ejemplo, si el plan cuenta con 3 ingenieros disponibles y la Iniciativa 1 e Iniciativa 2, cada uno de los cuales necesita 2 ingenieros para completarlo y ambos están programados para el mismo período de tiempo, Workfront asocia 2 ingenieros con la Iniciativa 1 y un ingeniero disponible restante con la Iniciativa 2. En este caso, la Iniciativa 2 muestra que tiene un conflicto, porque le falta un ingeniero. A veces, cambiar la prioridad de las iniciativas es la única manera de evitar conflictos en un plan.

Para actualizar la prioridad de la iniciativa:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png)y haga clic en [!UICONTROL Situaciones].

   Se muestra una lista de planes.

1. Haga clic en el nombre de un plan para abrirlo y, a continuación, busque las iniciativas que desea priorizar.
1. Haga clic en el cuadro de la izquierda de uno o más nombres de las iniciativas y realice una de las siguientes acciones:

   * Haga clic en el control a la izquierda de uno de los nombres de las iniciativas seleccionadas y arrástrelo hacia arriba o hacia abajo en la lista para cambiar la prioridad de la iniciativa.

      Workfront muestra el número de iniciativas seleccionadas.

      ![](assets/multi-select-initiative-number.png)

   * Haga clic en el **[!UICONTROL Prioridad]** en la parte inferior del plan, elija una de las siguientes opciones:

      * **[!UICONTROL Superior]**: Mueve las iniciativas seleccionadas a la parte superior de la lista de iniciativas. Las iniciativas seleccionadas aparecen primero en el plan.
      * **[!UICONTROL Inferior]**: Mueve las iniciativas seleccionadas al final de la lista de iniciativas. Las iniciativas seleccionadas se enumeran en último lugar del plan.
      * **[!UICONTROL Seleccionar un número]**: Mueve las iniciativas seleccionadas después de la iniciativa que indicó aquí.

         ![](assets/prioritize-initiatives-expanded-highlighted-350x171.png)
      [!DNL Workfront] inmediatamente coloca las iniciativas seleccionadas donde usted indica y el número de todas las iniciativas se actualiza en consecuencia.


1. Haga clic en **[!UICONTROL Guardar plan]** para guardar los cambios.
