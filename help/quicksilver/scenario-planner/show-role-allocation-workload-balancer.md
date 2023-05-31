---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Mostrar la asignación de funciones para proyectos e iniciativas en el Distribuidor de cargas de trabajo
description: Después de conectar proyectos e iniciativas, puede administrar su asignación de recursos en paralelo para asegurarse de que
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 0%

---

# Mostrar la asignación de funciones para proyectos e iniciativas en [!UICONTROL Distribuidor de cargas de trabajo]

>[!IMPORTANT]
>
>Su organización debe adquirir una licencia adicional para [!DNL Adobe Workfront Scenario Planner] para poder ver la información de la iniciativa de un proyecto. Para obtener información sobre la obtención de [!DNL Workfront Scenario Planner], consulte [Acceso necesario para utilizar [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Después de conectar proyectos e iniciativas, puede administrar su asignación de recursos en paralelo para asegurarse de que coincidan. Esto evita una asignación excesiva o una infrautilización.

Este artículo describe cómo puede reconciliar recursos mediante el [!UICONTROL Asignación de funciones] panel en [!UICONTROL Distribuidor de cargas de trabajo] de un proyecto.

Para obtener información general sobre la conciliación de recursos entre proyectos e iniciativas, incluidos los requisitos previos, consulte [Resumen de la conciliación de asignaciones de recursos entre proyectos e iniciativas](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## Requisitos de acceso

Debe hacer lo siguiente:

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
   <td> <p>Debe adquirir una licencia adicional para el [!DNL Adobe Workfront Scenario Planner] para acceder a la funcionalidad descrita en este artículo.</p> <p>Para obtener información sobre la obtención de [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md">Acceso necesario para utilizar [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configuraciones de nivel de acceso*</strong> </td> 
   <td> <p>[!UICONTROL View] o acceso superior a Proyectos </p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo [!DNL Workfront] El administrador puede cambiar su nivel de acceso. Consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permisos de objeto</strong> </p> </td> 
   <td> <p>[!UICONTROL View] o permisos superiores en el proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional a un plan, consulte <a href="../scenario-planner/request-access-to-plan.md">[!UICONTROL Request] acceso a un plan en el [!DNL Workfront Scenario Planner]</a>.</p> <p>Para obtener información sobre cómo solicitar acceso adicional a un proyecto, consulte <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Mostrar la asignación de funciones para proyectos e iniciativas en [!UICONTROL Distribuidor de cargas de trabajo]

Si su empresa ha adquirido un [!DNL Workfront Scenario Planner] licencia, puede reconciliar las asignaciones de recursos entre la iniciativa y el proyecto vinculado en el nivel de proyecto [!UICONTROL Distribuidor de cargas de trabajo].

1. (Condicional) Conecte un proyecto con una iniciativa mediante uno de los métodos descritos en los siguientes artículos:

   * [Proyectos importados a planes en [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md).
   * [Actualice o cree proyectos publicando iniciativas en [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md).

   >[!IMPORTANT]
   >
   >Si realiza cambios en los recursos de la iniciativa, debe volver a publicar el escenario al que pertenece la iniciativa para que se actualice la información de recursos más reciente de la iniciativa en el proyecto.

1. Vaya al proyecto en el que desea revisar la asignación de funciones del puesto para el proyecto y para la iniciativa asociada.
1. Clic [!UICONTROL Distribuidor de cargas de trabajo] en el panel izquierdo.

   Es posible que tenga que hacer clic en **[!UICONTROL Programación]**, entonces **[!UICONTROL Cambiar al Distribuidor de cargas de trabajo]**.

1. Realice una de las siguientes acciones:

   * Clic **[!UICONTROL Mes]** para ver el Distribuidor de cargas de trabajo por mes, haga clic en el menú desplegable situado junto a un mes en la cronología ![](assets/drop-down-next-to-month-month-view-wb.png), luego haga clic en **[!UICONTROL Más]**.
   * Haga clic en **[!UICONTROL Mostrar asignación de funciones]** icono ![](assets/show-role-allocation-icon.png) en la esquina superior derecha de la barra de herramientas.

   El [!UICONTROL Asignación de funciones] se muestra el panel.

   ![](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >Aunque se puede ver la variable [!UICONTROL Asignación de funciones] panel incluso si su organización no ha comprado un [!DNL Workfront Scenario Planner] licencia, no puede ver información sobre los roles de las iniciativas.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Revise la siguiente información en la **[!UICONTROL Totales de proyecto]** del panel Asignación de funciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Rol]</td> 
      <td> <p>Los nombres de los roles asociados con cualquiera de los siguientes:</p> 
       <ul> 
        <li> <p>tareas en el proyecto</p> </li> 
        <li> <p>problemas en el proyecto</p> </li> 
        <li> <p>iniciativa vinculada al proyecto</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Horas de la iniciativa]</td> 
      <td>El número de horas requeridas asociadas con cada función del puesto en la iniciativa durante la duración total de la iniciativa. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Horas planificadas]</td> 
      <td>Cantidad de horas planificadas asociadas con cada rol en las tareas o problemas del proyecto por la duración total del proyecto. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Variance]</td> 
      <td> <p>La diferencia entre las horas requeridas en la iniciativa y las horas planificadas asociadas con el trabajo en el proyecto. [!DNL Workfront] calcula la [!UICONTROL Variance] mediante esta fórmula:</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>Cuando los recursos están planificados para más horas de las requeridas en la iniciativa, [!UICONTROL Variance] es negativo y se muestra en rojo. Esto significa que los recursos están sobreasignados. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Las horas planificadas del proyecto no se muestran en los siguientes casos:
   >
   >   
   >   
   >   * Cuando las tareas o los problemas no están asignados a funciones del puesto, o a usuarios con una función del puesto asociada a ellos.
   >   * Cuando las tareas o los problemas tengan un [!UICONTROL Duración] de cero.




1. (Opcional) Si la variable [!UICONTROL Desviación] La columna muestra que los recursos están sobreasignados y ajuste una de las siguientes opciones:

   * Reduzca el número de horas planificadas para un rol que muestre sobreasignado o agregue más recursos a las tareas y distribuya más horas planificadas a los nuevos recursos. Al editarlas, puede actualizar las asignaciones o el número de horas planificadas de las tareas o problemas. Para obtener más información, consulte los siguientes artículos:

      * [Editar tareas](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [Editar problemas](../manage-work/issues/manage-issues/edit-issues.md)

      >[!NOTE]
      >
      >Debe tener acceso y permisos adicionales para editar tareas y problemas.

   * Aumente el número de horas necesarias para el rol que muestra la sobreasignación en la iniciativa. Para obtener más información, consulte [Cree y edite iniciativas en [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

      >[!NOTE]
      >
      >Debe tener acceso y permisos adicionales para editar planes.


1. (Opcional) Haga clic en el icono desplegable para expandir uno de los meses en la [!UICONTROL Asignación de funciones] o en la cronología del panel [!UICONTROL Distribuidor de cargas de trabajo].

   ![](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   El mismo tipo de información que se muestra en la variable [!UICONTROL Totales de proyecto] también se muestra para cada mes.

   >[!TIP]
   >
   >Los meses enumerados en la [!UICONTROL Asignación de funciones] panel son los meses de la cronología mostrados en la pantalla del [!UICONTROL Distribuidor de cargas de trabajo]. Desplácese hacia atrás y hacia adelante en la cronología para ver meses adicionales.

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->


