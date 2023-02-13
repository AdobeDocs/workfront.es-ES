---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: Nivel Recursos en la  [!UICONTROL Diagrama de Gantt]
description: Información sobre cómo nivelar recursos en el diagrama de Gantt.
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 0%

---

# Nivel Recursos en la [!UICONTROL Diagrama de Gantt]

La redistribución de los recursos en un proyecto tiene dos propósitos:

* Ajustar automáticamente la sobreasignación de tiempo para los usuarios asignados.
* Para crear automáticamente una programación de tareas realista para un proyecto.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de [!UICONTROL Edit] a Proyectos</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Acceso de [!UICONTROL Administrar] al proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Resumen de la Nivelación de Recursos

Si se asigna el mismo recurso a dos tareas diferentes, se puede utilizar la redistribución de recursos para ajustar la cronología de las tareas de modo que no ocurran al mismo tiempo.

Tenga en cuenta lo siguiente al redistribuir recursos en un proyecto:

* La redistribución de recursos solo se aplica a un proyecto, por lo que [!DNL Adobe Workfront] no nivela los recursos en más de un proyecto a la vez.
* If **[!UICONTROL Impulsado por el esfuerzo]** se selecciona como **[!UICONTROL Tipo de duración]**, [!DNL Workfront] no nivelará los recursos.
* Cuando se asignan varios usuarios a la misma tarea, la redistribución se cancela.
* Condiciones para el tipo de **[!UICONTROL Restricción de tarea]** prevalecerá sobre la nivelación de recursos. Por ejemplo, si **[!UICONTROL Fechas fijas]** se selecciona como [!UICONTROL Restricción de tarea], la redistribución de recursos no cambiará las fechas de la tarea.
* Las relaciones de los predecesores tendrán prioridad sobre la nivelación de recursos.
* **[!UICONTROL Nivelación de recursos]** necesita configurarse como **[!UICONTROL Manual]** para el proyecto con el fin de ajustar la nivelación en el [!UICONTROL Diagrama de Gantt]. Si tiene permisos de gestión para el proyecto, puede hacer que el sistema nivele los recursos automáticamente ajustando esta configuración en el proyecto y seleccionando **[!UICONTROL Automático]** en lugar de **[!UICONTROL Manual]** en el **[!UICONTROL Editar proyecto]** en la ventana

   ![](assets/resource-leveling-mode-350x177.png)

* Como propietario del proyecto o como usuario asignado de la tarea, puede introducir un retraso de redistribución para una tarea que indique que existe una buena posibilidad de que la tarea necesite un tiempo adicional. Para obtener información sobre cómo agregar un retraso de redistribución a una tarea, consulte [Actualizar retraso de redistribución de tareas](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## Aplicar nivelación de recursos en la variable [!UICONTROL Diagrama de Gantt]

Puede utilizar la Lista de tareas [!UICONTROL Diagrama de Gantt] para nivelar sus recursos.

1. Vaya al proyecto que desea nivelar.
1. En el **[!UICONTROL Tareas]** , haga clic en el **[!UICONTROL Diagrama de Gantt]** icono.

   Todos los cambios se guardan automáticamente cuando el **[!UICONTROL Autoguardar]** está activada. Está activada de forma predeterminada.

1. (Opcional) Haga clic en el **[!UICONTROL Plan] mode** y seleccione **[!UICONTROL Estándar de guardado manual]** o **[!UICONTROL Planificación de la cronología]** para guardar los cambios manualmente.

   >[!TIP]
   >
   >No puede nivelar los recursos en la variable  [!UICONTROL Diagrama de Gantt] cuando la variable [!UICONTROL Autoguardar] está activada.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Haga clic en el **[!UICONTROL Recursos de nivel]** menú desplegable.

   ![Level_resources.png](assets/level-resouces.png)

1. Seleccione una de las siguientes opciones:

   * **[!UICONTROL Nivel ahora]**: Aplica la redistribución de recursos a la tarea seleccionada.
   * **[!UICONTROL Nivelación clara]**: Quita toda la redistribución de recursos de la tarea seleccionada.

   >[!NOTE]
   >
   >Es posible que los recursos se sobreasignen si se asignan a varias tareas que se producen durante el mismo intervalo de tiempo.

1. (Opcional y condicional) Si ha desactivado la opción Autoguardar , haga clic en el botón **[!UICONTROL Deshacer]** o &#x200B;**[!UICONTROL Rehacer]** si desea cancelar o duplicar cualquiera de los cambios.

   >[!TIP]
   >
   >Puede utilizar los siguientes métodos abreviados del teclado para deshacer o rehacer cambios en la [!UICONTROL Diagrama de Gantt]:
   >
   >* [!DNL Mac]: Uso [!UICONTROL Comando + Z] para deshacer y [!UICONTROL Comando + Mayús + Z] para rehacer.
   >* Windows: Uso [!UICONTROL Ctrl + Z] para deshacer y [!UICONTROL Ctrl + Y] para rehacer.



1. Haga clic en **[!UICONTROL Guardar]** en la esquina superior derecha del [!UICONTROL Diagrama de Gantt].

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Overview of Leveling Delay</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article: /Content/Manage work/Tasks/Task information/task-leveling-delay.htm) </p>
<p>At times, there might be conflicts between task schedules on a project. You can level resources or address resource conflicts by rescheduling resources and tasks so that all tasks can be completed within a realistic schedule. </p>
<p>As the project manager, or the task assignee, you can also add a Leveling Delay on individual tasks to account for any resource or scheduling conflicts. In other words, a task might be scheduled with a delay to ensure that when Adobe Workfront levels the tasks a more realistic schedule overcomes resource conflicts.</p>
<p>To manually add a Leveling Delay to a task:</p>
<ol>
<li value="1">Navigate to a task for which you want to add a Leveling Delay.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the <strong>More icon</strong> to the right of the task name, then click <strong>Edit</strong>. </p> <p> <img src="assets/qs-task-edit-icon-highlighted-350x154.png" style="width: 350;height: 154;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Click <strong>Settings</strong>.<br></li>
<li value="4">Specify the <strong>Leveling Delay</strong>, in hours.<br>This is the time that the resource will be delayed starting the task due to resource conflicts.</li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
