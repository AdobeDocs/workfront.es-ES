---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: Redistribuir recursos en el [!UICONTROL gráfico Gantt]
description: Información sobre cómo redistribuir recursos en el gráfico Gantt.
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 98%

---

# Redistribuir recursos en el [!UICONTROL gráfico Gantt]

La redistribución de los recursos en un proyecto tiene dos propósitos:

* Para ajustar automáticamente la asignación excesiva de tiempo para los usuarios asignados.
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
   <td> <p>Acceso [!UICONTROL Edit] a proyectos</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creación o modificación de niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Acceso de [!UICONTROL Manage] al proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Información general sobre la redistribución de recursos

Si el mismo recurso está asignado a dos tareas diferentes, puede utilizar la redistribución de recursos para ajustar la línea de tiempo de las tareas de modo que no se produzcan al mismo tiempo.

Tenga en cuenta lo siguiente al redistribuir recursos en un proyecto:

* La redistribución de recursos sólo se aplica a un proyecto, por lo que [!DNL Adobe Workfront] no redistribuye los recursos en más de un proyecto a la vez.
* Si la opción **[!UICONTROL Condicionada por el esfuerzo]** está seleccionada como **[!UICONTROL Tipo de duración]**, [!DNL Workfront] los recursos no se redistribuirán.
* Cuando se asignan varios usuarios a la misma tarea, se cancela la redistribución.
* Las condiciones del tipo de **[!UICONTROL Restricción de tarea]** tendrán prioridad sobre la redistribución de recursos. Por ejemplo, si se selecciona **[!UICONTROL Fechas fijas]** como [!UICONTROL Restricción de tarea], la redistribución de recursos no cambiará las fechas de las tareas.
* Las relaciones de predecesoras tendrán prioridad sobre la redistribución de recursos.
* **[!UICONTROL Redistribución de recursos]** debe establecerse en **[!UICONTROL Manual]** para el proyecto a fin de ajustar la redistribución en el [!UICONTROL gráfico Gantt]. Si tiene permisos de administración en el proyecto, puede hacer que el sistema redistribuya recursos automáticamente ajustando esta configuración en el proyecto y seleccionando **[!UICONTROL Automático]** en lugar de **[!UICONTROL Manual]** en el cuadro **[!UICONTROL Editar proyecto]**.

  ![Modo de nivelación de recursos](assets/resource-leveling-mode-350x177.png)

* Como propietario del proyecto o usuario asignado de la tarea, puede introducir un retraso de redistribución para una tarea para indicar que es sumamente probable que la tarea pueda necesitar tiempo adicional. Para obtener información acerca de cómo añadir un retraso de redistribución a una tarea, consulte [Actualizar el retraso de redistribución de tareas](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## Aplicar redistribución de recursos en el [!UICONTROL gráfico Gantt]

Puede usar la Lista de tareas [!UICONTROL gráfico Gantt] para redistribuir los recursos.

1. Vaya al proyecto que desee redistribuir.
1. En el área **[!UICONTROL Tareas]**, haga clic en el icono **[!UICONTROL gráfico Gantt]**.

   Todos los cambios se guardan automáticamente cuando la opción **[!UICONTROL Guardar automáticamente]** se habilita. Está habilitada de forma predeterminada.

1. (Opcional) Haga clic en el icono del modo **[!UICONTROL Plan]** y seleccione **[!UICONTROL Guardar de forma manual como estándar]** o **[!UICONTROL Planificación de la línea de tiempo]** para guardar los cambios de forma manual.

   >[!TIP]
   >
   >No puede redistribuir recursos en el [!UICONTROL gráfico Gantt] cuando la opción [!UICONTROL Guardar automáticamente] está habilitada.

   ![Configuración manual habilitada](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Haga clic en el menú desplegable **[!UICONTROL Redistribuir recursos]**

   ![Level_resouces.png](assets/level-resouces.png)

1. Seleccione una de las siguientes opciones:

   * **[!UICONTROL Redistribuir ahora]**: aplica la redistribución de recursos a la tarea seleccionada.
   * **[!UICONTROL Borrar redistribución]**: elimina toda la redistribución de recursos de la tarea seleccionada.

   >[!NOTE]
   >
   >Es posible que los recursos se sobreasignen si se asignan a varias tareas que se producen durante el mismo lapso de tiempo.

1. (Opcional y condicional) Si ha deshabilitado la opción de guardado automático, haga clic en los iconos **[!UICONTROL Deshacer]** o&#x200B;**[!UICONTROL Rehacer]** si desea cancelar o duplicar cualquiera de los cambios.

   >[!TIP]
   >
   >Puede usar los siguientes métodos abreviados del teclado para deshacer o rehacer los cambios en el [!UICONTROL gráfico Gantt]:
   >
   >* [!DNL Mac]: utilice [!UICONTROL Comando + Z] para deshacer la acción y [!UICONTROL Comando + Mayús + Z] para rehacerla.
   >* Windows: utilice [!UICONTROL Ctrl + Z] para deshacer la acción y [!UICONTROL Ctrl + Y] para rehacerla.


1. Haga clic en **[!UICONTROL Guardar]** en la esquina superior derecha del [!UICONTROL gráfico Gantt].

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Overview of Leveling Delay</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article: /Content/Manage work/Tasks/Task information/task-leveling-delay.htm) </p>
<p>At times, there might be conflicts between task schedules on a project. You can level resources or address resource conflicts by rescheduling resources and tasks so that all tasks can be completed within a realistic schedule. </p>
<p>As the project manager, or the task assignee, you can also add a Leveling Delay on individual tasks to account for any resource or scheduling conflicts. In other words, a task might be scheduled with a delay to ensure that when Adobe Workfront levels the tasks a more realistic schedule overcomes resource conflicts.</p>
<p>To manually add a Leveling Delay to a task:</p>
<ol>
<li value="1">Navigate to a task for which you want to add a Leveling Delay.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the <strong>More icon</strong> to the right of the task name, then click <strong>Edit</strong>. </p>  </li>
<li value="3">Click <strong>Settings</strong>.<br></li>
<li value="4">Specify the <strong>Leveling Delay</strong>, in hours.<br>This is the time that the resource will be delayed starting the task due to resource conflicts.</li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
