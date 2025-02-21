---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Mostrar la asignación de las funciones para proyectos e iniciativas en la lista de tareas
description: Después de conectar proyectos e iniciativas, puede administrar la asignación de recursos en paralelo para asegurarse de que coinciden. Esto evita su sobreasignación o infrautilización.
author: Alina
feature: Workfront Scenario Planner
exl-id: 77152e46-0b7b-4937-9d16-1a20c2a7fdf1
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 86%

---

# Mostrar la asignación de las funciones para proyectos e iniciativas en la lista de tareas

<!--Audited: 07/2024-->

Después de conectar proyectos e iniciativas, puede administrar la asignación de recursos en paralelo para asegurarse de que coinciden. Esto evita su sobreasignación o infrautilización.

Este artículo describe cómo puede reconciliar los recursos mediante el panel [!UICONTROL Asignación de funciones] en la lista de tareas de un proyecto.

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

## Mostrar la asignación de las funciones para proyectos e iniciativas en la lista de tareas

Si su compañía ha adquirido una licencia de [!DNL Workfront Scenario Planner], puede reconciliar las asignaciones de recursos entre la iniciativa y el proyecto vinculado a ella en la sección [!UICONTROL Tareas] del proyecto.

1. (Condicional) Un proyecto debe estar conectado a una iniciativa mediante uno de los métodos descritos en la sección [Mostrar asignación de funciones para proyectos e iniciativas de la lista de tareas](#show-role-allocation-for-projects-and-initiatives-in-the-task-list) de este artículo.

   >[!IMPORTANT]
   >
   >Si realiza cambios en los recursos de la iniciativa, debe volver a publicar el escenario al que pertenece la iniciativa para que se actualice la información de recursos más reciente de la iniciativa en el proyecto.

1. Vaya al proyecto en el que desea revisar la asignación de las funciones del puesto para el proyecto y la iniciativa asociada.
1. Haga clic en **[!UICONTROL Tareas]** en el panel izquierdo.
1. Haga clic en el icono **[!UICONTROL Mostrar asignación de funciones]** ![Mostrar asignación de funciones](assets/show-role-allocation-icon.png) en la esquina superior derecha de la barra de herramientas.

   Se muestra el panel [!UICONTROL Asignación de funciones].

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Revise la siguiente información en el área **[!UICONTROL Totales de proyecto]** del panel [!UICONTROL Asignación de funciones]:

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
   >   * Cuando las tareas o problemas tienen una duración de cero.
   >   
   >



1. (Opcional) Si la columna [!UICONTROL Variación] muestra que sus recursos están sobreasignados, ajuste una de las siguientes opciones:

   * Reduzca el número de horas planificadas para una función que se muestre como sobreasignado, o añada más recursos a las tareas y distribuya más horas planificadas a los nuevos recursos. Durante la edición, puede actualizar las asignaciones o el número de horas planificadas de las tareas o problemas. Para obtener más información, consulte los siguientes artículos:

      * [Editar tareas](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [Editar problemas](../manage-work/issues/manage-issues/edit-issues.md)

     >[!NOTE]
     >
     >Debe tener acceso y permisos adicionales para editar tareas y problemas.

   * Aumente el número de horas necesarias para la función que muestra la sobreasignación en la iniciativa. Para obtener más información, consulte [Crear y editar iniciativas en [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

     >[!NOTE]
     >
     >Debe tener acceso y permisos adicionales para editar planes.


