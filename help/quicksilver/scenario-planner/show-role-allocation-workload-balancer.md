---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Mostrar la asignación de funciones para proyectos e iniciativas en el Distribuidor de cargas de trabajo
description: Después de conectar proyectos e iniciativas, puede administrar su asignación de recursos en paralelo para asegurarse de que
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '816'
ht-degree: 57%

---

# Mostrar la asignación de roles para proyectos e iniciativas en el [!UICONTROL Distribuidor de cargas de trabajo]

<!--Audited: 07/2024-->

Después de conectar proyectos e iniciativas, puede administrar la asignación de recursos en paralelo para asegurarse de que coinciden. Esto evita su sobreasignación o infrautilización.

Este artículo describe cómo puede reconciliar recursos mediante el panel [!UICONTROL Asignación de funciones] en el [!UICONTROL Distribuidor de cargas de trabajo] de un proyecto.

Para obtener información general sobre cómo conciliar recursos entre proyectos e iniciativas, incluidos los requisitos previos, consulte [Información general sobre la conciliación de asignaciones de recursos entre proyectos e iniciativas](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

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
   <td> <p>Acceso de visualización o superior a Proyectos.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Permisos de objeto </p> </td> 
   <td> <p> Permiso de visualización o superior para un proyecto.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso a la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mostrar la asignación de roles para proyectos e iniciativas en el [!UICONTROL Distribuidor de cargas de trabajo]

Si su compañía ha adquirido una licencia de [!DNL Workfront Scenario Planner], puede reconciliar las asignaciones de recursos entre la iniciativa y el proyecto vinculado a ella en el nivel de proyecto [!UICONTROL Distribuidor de cargas de trabajo].

1. (Condicional) Conecte un proyecto con una iniciativa mediante uno de los métodos descritos en los siguientes artículos:

   * [Importar proyectos a planes en [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md).
   * [Actualice o cree proyectos publicando iniciativas en [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md).

   >[!IMPORTANT]
   >
   >Si realiza cambios en los recursos de la iniciativa, debe volver a publicar el escenario al que pertenece la iniciativa para que se actualice la información de recursos más reciente de la iniciativa en el proyecto.

1. Vaya al proyecto en el que desea revisar la asignación de las funciones del puesto para el proyecto y la iniciativa asociada.
1. Haga clic en [!UICONTROL Distribuidor de cargas de trabajo] en el panel de la izquierda.

   Es posible que tenga que hacer clic en **[!UICONTROL Programación]** y luego **[!UICONTROL Cambiar al Distribuidor de cargas de trabajo]**.

1. Realice una de las siguientes acciones:

   * Haga clic en **[!UICONTROL Mes]** para ver el Distribuidor de cargas de trabajo por mes, haga clic en el menú desplegable situado junto a un mes en el menú desplegable de la cronología ![junto al mes](assets/drop-down-next-to-month-month-view-wb.png) y, a continuación, haga clic en **[!UICONTROL Más]**.
   * Haga clic en el icono **[!UICONTROL Mostrar asignación de funciones]** ![Mostrar asignación de funciones](assets/show-role-allocation-icon.png) en la esquina superior derecha de la barra de herramientas.

   Se muestra el panel [!UICONTROL Asignación de funciones].

   ![Panel de asignación de funciones](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >Aunque puede ver el panel [!UICONTROL Asignación de funciones] aunque su organización no haya adquirido una licencia de [!DNL Workfront Scenario Planner], no podrá ver información sobre las funciones del puesto de las iniciativas.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Revise la siguiente información en el área **[!UICONTROL Totales del proyecto]** del panel Asignación de roles:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Job Role]</td> 
      <td> <p>Nombres de las funciones asociadas a cualquiera de las siguientes:</p> 
       <ul> 
        <li> <p>tareas del proyecto</p> </li> 
        <li> <p>problemas del proyecto</p> </li> 
        <li> <p>iniciativa vinculada al proyecto</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative Hours]</td> 
      <td>Cantidad de horas obligatorias asociadas a cada función de la iniciativa durante la duración total de la iniciativa. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Planned Hours]</td> 
      <td>Cantidad de horas planificadas asociadas a cada función en las tareas o problemas del proyecto para la duración total del proyecto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Variance]</td> 
      <td> <p>Diferencia entre las horas obligatorias de la iniciativa y las horas planificadas asociadas al trabajo en el proyecto. [!DNL Workfront] calcula la [!UICONTROL Variance] con esta fórmula:</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>Cuando los recursos se han planificado para más horas de las obligatorias en la iniciativa, la [!UICONTROL Variance] es negativa y se muestra en rojo. Esto significa que los recursos están sobreasignados. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Las horas planificadas del proyecto no se muestran en los siguientes casos:
   >
   >   
   >   
   >   * Cuando las tareas o los problemas no se asignan a las funciones o a usuarios con una función asociada a ellos.
   >   * Cuando las tareas o los problemas tienen una [!UICONTROL Duración] de cero.
   >   
   >

1. (Opcional) Si la columna [!UICONTROL Variación] muestra que sus recursos están sobreasignados, ajuste una de las siguientes opciones:

   * Reduzca el número de horas planificadas para una función que se muestre como sobreasignado, o añada más recursos a las tareas y distribuya más horas planificadas a los nuevos recursos. Durante la edición, puede actualizar las asignaciones o el número de horas planificadas de las tareas o problemas. Para obtener más información, consulte los siguientes artículos:

      * [Editar tareas](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [Editar problemas](../manage-work/issues/manage-issues/edit-issues.md)

     >[!NOTE]
     >
     >Debe tener acceso y permisos adicionales para editar tareas y problemas.

   * Aumente el número de horas necesarias para el rol que muestra la sobreasignación en la iniciativa. Para obtener más información, consulte [Crear y editar iniciativas en [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

     >[!NOTE]
     >
     >Debe tener acceso y permisos adicionales para editar planes.

1. (Opcional) Haga clic en el icono desplegable para expandir uno de los meses en el panel [!UICONTROL Asignación de funciones] o en la cronología del [!UICONTROL Distribuidor de cargas de trabajo].

   ![Expandir mes en el panel de asignación de funciones](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   El mismo tipo de información que se muestra en el área [!UICONTROL Totales de proyectos] también se muestra para cada mes.

   >[!TIP]
   >
   >Los meses enumerados en el panel [!UICONTROL Asignación de funciones] son los meses de la cronología mostrados en la pantalla del [!UICONTROL Distribuidor de cargas de trabajo]. Desplácese hacia atrás y hacia adelante en la cronología para ver meses adicionales.

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->


