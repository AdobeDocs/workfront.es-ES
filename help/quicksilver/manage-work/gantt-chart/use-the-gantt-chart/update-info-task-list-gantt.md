---
product-area: projects
navigation-topic: use-the-gantt-chart
title: Actualización de la información en el gráfico Gantt de la lista de tareas
description: El gráfico Gantt de la lista de tareas muestra detalles sobre las tareas de un proyecto o plantilla.
author: Alina
feature: Work Management
exl-id: 0a8e6fd5-985c-49e5-842d-67ade29ee1c9
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '1041'
ht-degree: 98%

---

# Actualizar información en el [!UICONTROL gráfico Gantt] de la lista de tareas

El [!UICONTROL gráfico Gantt] de la lista de tareas muestra detalles acerca de las tareas de un proyecto o plantilla.

En una plantilla, el [!UICONTROL gráfico Gantt] de la lista de tareas refleja las actualizaciones realizadas en la lista de tareas de la plantilla en el nivel de tarea. No es posible editar el [!UICONTROL gráfico Gantt] asociado a una plantilla.

En un proyecto, es posible actualizar la información de la tarea directamente en el [!UICONTROL gráfico Gantt] de la lista de tareas.

En este artículo se describen las siguientes acciones, que se pueden realizar directamente en el [!UICONTROL gráfico Gantt] de la lista de tareas:

* Modificar la duración de la tarea
* Creación o eliminación de relaciones predecesoras
* Cambiar las fechas de inicio y finalización de la tarea
* Actualizar el porcentaje completado
* Nivelar recursos del proyecto

## Requisitos de acceso

Debe tener lo siguiente para seguir los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de [!UICONTROL Edit] a proyectos y tareas</p> <p>Nota: Si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Acceso de [!UICONTROL Manage] al proyecto y a las tareas </p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Modificar la duración de la tarea

1. Vaya al proyecto que quiera modificar.
1. Haga clic en **[!UICONTROL Tareas]**, en el panel izquierdo.

   ![Área de tareas](assets/qs-tasks-area-highlighted-in-the-secondary-nav-350x206.png)

1. Haga clic en el icono del **[!UICONTROL gráfico Gantt]**.

   ![Haga clic en el icono del gráfico Gantt](assets/click-gantt-chart-icon.png)

   Todos los cambios se guardarán automáticamente cuando la opción **[!UICONTROL Guardar automáticamente]** se habilite. Está habilitada de forma predeterminada.

1. (Opcional) Haga clic en el icono **[!UICONTROL Modo de planificación]** y seleccione **[!UICONTROL Guardar de forma manual como estándar]** o **[!UICONTROL Planificación de la cronología]** para guardar los cambios de forma manual.

   ![Configuración manual habilitada](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Pase el puntero por encima de la cronología de una tarea y arrastre el indicador de línea de tiempo a una fecha diferente.
1. Suelte el indicador cuando haya alcanzado la nueva fecha de finalización correcta de la tarea.
1. (Opcional y condicional) En caso de seleccionar la opción de guardar manualmente los cambios, haga clic en los iconos **[!UICONTROL Deshacer]** o **[!UICONTROL Rehacer]** para cancelar o duplicar cualquiera de los cambios.

   >[!TIP]
   >
   >Use los siguientes métodos abreviados de teclado para deshacer o rehacer los cambios en el gráfico Gantt:
   >
   >   
   >   
   >   * [!DNL Mac]: use [!UICONTROL Comando + Z] para deshacer y [!UICONTROL Comando + Mayús + Z] para rehacer.
   >   * [!DNL Windows]: use [!UICONTROL Ctrl + Z] para deshacer y [!UICONTROL Ctrl + Y] para rehacer.
   >   
   >

1. Haga clic en **[!UICONTROL Guardar]**, en la esquina superior derecha del [!UICONTROL gráfico Gantt].

## Creación o eliminación de relaciones predecesoras

1. Vaya al proyecto que quiera modificar.
1. En el área **[!UICONTROL Tareas]**, haga clic en el icono del **[!UICONTROL gráfico Gantt]**.

   La opción **[!UICONTROL Guardar automáticamente]** está seleccionada de forma predeterminada, por lo que todos los cambios se guardan automáticamente.

   ![Haga clic en el icono del gráfico Gantt](assets/click-gantt-chart-icon.png)

1. (Opcional) Haga clic en el icono **[!UICONTROL Modo de planificación]** y seleccione **[!UICONTROL Guardar de forma manual como estándar]** o **[!UICONTROL Planificación de la cronología]** para guardar los cambios de forma manual.

   ![Configuración manual habilitada](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Para crear una relación predecesora, haga clic en el punto de inicio de una tarea y arrástrela hasta el punto final de la tarea.
1. Para eliminar una relación predecesora, haga clic en una línea predecesora que conecte dos tareas para seleccionarla y, a continuación, pulse **[!UICONTROL Eliminar]** en el teclado.\
   ![Delete_predecessor.png](assets/delete-predecessor-350x152.png)

1. (Opcional y condicional) Si seleccionó que se guarden los cambios manualmente, haga clic en los iconos **[!UICONTROL Deshacer]** o **[!UICONTROL Rehacer]** para cancelar o duplicar cualquier cambio.

   >[!TIP]
   >
   >Use los siguientes métodos abreviados de teclado para deshacer o rehacer los cambios en el gráfico Gantt:
   >
   >   
   >   
   >   * [!DNL Mac]: use [!UICONTROL Comando + Z] para deshacer y [!UICONTROL Comando + Mayús + Z] para rehacer.
   >   * [!DNL Windows]: [!UICONTROL use Ctrl + Z] para deshacer y [!UICONTROL Ctrl + Y] para rehacer.
   >   
   >

1. Haga clic en **[!UICONTROL Guardar]**.

## Cambiar las fechas de inicio y finalización de la tarea

1. Vaya al proyecto que quiera modificar.
1. En el área **[!UICONTROL Tareas]**, haga clic en el icono del **[!UICONTROL gráfico Gantt]**.

   Todos los cambios se guardan automáticamente cuando la opción **[!UICONTROL Guardar automáticamente]** se habilita. Está habilitada de forma predeterminada.

   ![Haga clic en el icono del gráfico Gantt](assets/click-gantt-chart-icon.png)

1. (Opcional) Haga clic en el icono **[!UICONTROL Modo de planificación]** y seleccione **[!UICONTROL Guardar de forma manual como estándar]** o **[!UICONTROL Planificación de la cronología]** para guardar los cambios de forma manual.

   ![Configuración manual habilitada](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Pase el puntero del ratón por encima del centro de la tarea y busque la flecha multidireccional.
1. Haga clic en la tarea y arrástrela a la fecha deseada.

   ![Change_start_end_date.png](assets/change-start-end-date.png)

1. En caso de cambiar la fecha de la tarea de forma que afecte a la restricción de tarea, haga clic en **[!UICONTROL Aceptar]** para confirmar el cambio de la restricción de tarea.

   >[!NOTE]
   >
   >Si la tarea tuviera una de las restricciones siguientes, el sistema actualizará la [!UICONTROL restricción de tarea] a [!UICONTROL No comenzar antes del], si el proyecto estuviera programado según la [!UICONTROL Fecha de inicio], o [!UICONTROL No finalizar después del], si el proyecto estuviera programado según la [!UICONTROL Fecha de finalización]:
   >
   >   
   >   
   >   * [!UICONTROL Lo antes posible]
   >   * [!UICONTROL Lo más tarde posible]
   >   * [!UICONTROL Lo más temprano disponible]
   >   * [!UICONTROL Lo más tarde posible]
   >   
   >   
   >En algunos casos, las relaciones predecesoras podrían impedir que las tareas comiencen antes y no se permita el movimiento de tareas.

1. (Opcional y condicional) Si se seleccionó la opción de guardar los cambios manualmente, haga clic en los iconos **[!UICONTROL Deshacer]** o **[!UICONTROL Rehacer]** en caso de querer cancelar o duplicar cualquiera de los cambios.

   >[!TIP]
   >
   >Use los siguientes métodos abreviados de teclado para deshacer o rehacer cambios en el [!UICONTROL gráfico Gantt]:
   >
   >   
   >   
   >   * [!DNL Mac]: use [!UICONTROL Comando + Z] para deshacer y [!UICONTROL Comando + Mayús + Z] para rehacer.
   >   * [!DNL Windows]: use [!UICONTROL Ctrl + Z] para deshacer y [!UICONTROL Ctrl + Y] para rehacer.
   >   
   >

1. Haga clic en **[!UICONTROL Guardar]**.

## Actualizar el porcentaje completado

1. Vaya al proyecto que quiera modificar.
1. En el área **[!UICONTROL Tareas]**, haga clic en el icono del **[!UICONTROL gráfico Gantt]**.

   ![Haga clic en el icono del gráfico Gantt](assets/click-gantt-chart-icon.png)

   Todos los cambios se guardarán automáticamente cuando la opción **[!UICONTROL Guardar automáticamente]** se habilite. Está habilitada de forma predeterminada.

1. (Opcional) Haga clic en el icono **[!UICONTROL Modo de planificación]** y seleccione **[!UICONTROL Guardar de forma manual como estándar]** o **[!UICONTROL Planificación de la cronología]** para guardar los cambios de forma manual.
1. Haga doble clic en el número porcentual de la tarea e introduzca el número.

   >[!IMPORTANT]
   >
   >Es necesario tener seleccionado [!UICONTROL % completado] en el cuadro de diálogo [!UICONTROL Opciones] para que se actualice el porcentaje completado. Para ello, haga clic en el icono **[!UICONTROL Opciones]** y seleccione **[!UICONTROL % completado]**.
   >
   >
   >![update_percent_complete.png](assets/update-percent-complete-350x175.png)   >
   >

1. (Opcional y condicional) Si se seleccionó la opción de guardar los cambios manualmente, haga clic en los iconos **[!UICONTROL Deshacer]** o&#x200B;**[!UICONTROL Rehacer]** en caso de querer cancelar o duplicar cualquiera de los cambios.

   >[!TIP]
   >
   >Use los siguientes métodos abreviados de teclado para deshacer o rehacer los cambios en el [!UICONTROL gráfico Gantt]:
   >
   >   
   >   
   >   * [!DNL Mac]: use [!UICONTROL Comando + Z] para deshacer y [!UICONTROL Comando + Mayús + Z] para rehacer.
   >   * [!DNL Windows]: use [!UICONTROL Ctrl + Z] para deshacer y [!UICONTROL Ctrl + Y] para rehacer.
   >   
   >

1. Haga clic en **[!UICONTROL Guardar]**, en la esquina superior derecha del [!UICONTROL gráfico Gantt].

## Nivelar recursos del proyecto

Use el [!UICONTROL gráfico Gantt] de la lista de tareas para nivelar los recursos.

Para obtener información acerca de la nivelación de recursos en el [!UICONTROL gráfico Gantt], consulte [Nivelación de recursos en el [!UICONTROL gráfico Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;this is drafted because I moved the whole content to the article linked above)</p>
<ol>
<li value="1">Go to the project you want to level.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> In the <strong>Tasks</strong> area, click the <strong>Gantt chart</strong> icon.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">All changes are saved automatically when the <strong>Autosave</strong> option is enabled. It is enabled by default. </p> </li>
<li value="3">
<div>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) Click the <strong>Plan mode</strong> icon and select <strong>Manual save Standard</strong> or <strong>Timeline Planning</strong> to save your changes manually.</p> <note type="tip">
You cannot level resources in the Gantt chart when the Autosave option is enabled.
</note>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png" style="width: 350;height: 493;"> </p>
</div> </li>
<li value="4"> <p>Click the <strong>Level Resources</strong> drop-down menu.</p> <p> <img src="assets/level-resouces.png" alt="Level_resouces.png"> </p> </li>
<li value="5">Select one of following options:
<ul>
<li><strong>Level Now</strong>: Applies resource leveling to the selected task.</li>
<li><p><strong>Clear Leveling</strong>: Removes all resource leveling from the selected task.</p></li>
</ul><note type="note">
Your resources might be overallocated if they are assigned to multiple tasks which occur during the same time frame.
</note></li>
<li value="6"> <p>(Optional and conditional) If you have disabled the Autosave option, click the <strong>Undo</strong> or<strong>Redo</strong> icons if you want to cancel or duplicate any of the changes. </p> <note type="tip">
<p>You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:</p>
<ul>
<li>Mac: Use Command + Z to undo and Command + Shift + Z to redo.</li>
<li>Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.</li>
</ul>
</note> </li>
<li value="7">Click <strong>Save</strong> in the upper-right corner of the Gantt chart.</li>
</ol>
</div>
-->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"> </h2>
-->
