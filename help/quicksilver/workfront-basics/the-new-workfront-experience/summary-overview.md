---
content-type: overview
title: Información general sobre el resumen
description: Puede usar el Panel de resumen para revisar y actualizar la información del elemento de trabajo directamente desde una lista de tareas, problemas, documentos o desde otras áreas de  [!DNL Adobe Workfront] que muestran tareas y problemas.
feature: Get Started with Workfront
author: Nolan
exl-id: 5e4026b2-5f2f-45c1-bef1-04e20c62ed8a
source-git-commit: 66fc75ed9a7fca4b44ac776c314a6e08a6fbd450
workflow-type: tm+mt
source-wordcount: '986'
ht-degree: 93%

---

# Información general sobre el [!UICONTROL resumen]

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers or in Production for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span> -->

Puede usar el panel [!UICONTROL Resumen] para revisar y actualizar la información del elemento de trabajo directamente desde una lista de tareas, problemas, documentos o desde otras áreas de [!DNL Adobe Workfront] que muestran tareas y problemas.

El administrador de Workfront o de grupo puede modificar las áreas y los campos que se muestran en el Panel de resumen. Se pueden añadir hasta 16 campos al panel Resumen.

>[!IMPORTANT]
>
>Se recomienda añadir campos que se deben actualizar con frecuencia al Panel de resumen para poder acceder fácilmente a ellos y actualizarlos sin tener que acceder a la página principal del objeto.
>
>Por ejemplo, puede añadir los siguientes campos actualizados con frecuencia a los paneles Resumen de tareas y problemas:
>
>* Estado
>* Porcentaje completado
>* Fecha de confirmación
>* Fecha planificada de finalización
>* Condición



En la tabla siguiente se muestran las áreas en las que puede encontrar y usar el panel [!UICONTROL Resumen]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td><b>Tareas</b></td> 
  </tr> 
  <tr> 
   <td> <p>Listas de tareas dentro de un</p> 
    <ul> 
     <li>Proyecto</li> 
     <li>Subtarea</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Tareas en las áreas de trabajo de [!UICONTROL Unassigned] y [!UICONTROL Assigned] del [!UICONTROL Workload Balancer]</td> 
  </tr> 
   <tr> 
   <td>Tareas en una [!UICONTROL Timesheet]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><b>Problemas</b></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Listas de problemas dentro de un</p> 
    <ul> 
     <li>Proyecto</li> 
     <li>Tarea</li> 
     <li>Subtarea</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Problemas en el área de [!UICONTROL Assigned Work] del [!UICONTROL Workload Balancer]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Problemas en la sección [!UICONTROL Submitted] del área de [!UICONTROL Requests]</td> 
  </tr> 
</tr> 
   <tr> 
   <td>Problemas en una [!UICONTROL Timesheet]</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td><b>Documentos</b></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Área de [!UICONTROL Documents]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Sección de [!UICONTROL Documents] de cualquier objeto (proyecto, tarea, problema, programa, portafolio, plantilla, tarea de plantilla, usuario)</td> 
  </tr> 
 </tbody> 
</table>

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront administrators can customize the Summary in the Layout Template. For more information, see <a href="../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
-->

En este artículo se describe cómo acceder y utilizar el panel [!UICONTROL Resumen] para tareas y problemas en listas.

Para obtener información sobre cómo obtener acceso al [!UICONTROL Resumen] en el [!UICONTROL Distribuidor de cargas de trabajo], consulte [Actualizar elementos de trabajo en el [!UICONTROL Distribuidor de cargas de trabajo] mediante el [!UICONTROL Resumen]](../../resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

Para obtener información sobre cómo acceder al [!UICONTROL Resumen] para documentos, consulte la información general del [[!UICONTROL Resumen] para documentos](../../documents/managing-documents/summary-for-documents.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>Nuevo: colaborador o superior</p>
   O
   <p>Actual:[!UICONTROL Request] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuración de nivel de acceso</strong></td> 
   <td> <p>[!UICONTROL View] o acceso superior a tareas, problemas o documentos</p> <p>[!UICONTROL View] o acceso superior a cualquier objeto para el que desee ver documentos [!UICONTROL Summary]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>[!UICONTROL View] o permisos superiores para una tarea, problema o documento</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront]. Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Ver el panel [!UICONTROL Resumen] en una lista de tareas o problemas

1. Vaya a una tarea o problema y seleccione un elemento de la lista.
1. Haga clic en el icono **[!UICONTROL Resumen]**![](assets/qs-summary-in-new-toolbar-small.png)

   o

   Haga clic en el icono **[!UICONTROL Abrir resumen]** ![](assets/open-summary-with-text-nwe.png) en la sección [!UICONTROL Enviados] del área [!UICONTROL Solicitudes].

   Después de abrir el Resumen, permanece abierto a medida que hace clic en otras tareas o problemas o los selecciona y permanece abierto hasta que lo cierra manualmente.

   >[!TIP]
   >
   >Solo puede seleccionar una tarea o un problema a la vez para ver sus detalles en el panel [!UICONTROL Resumen].

   ![Panel de resumen](assets/summary-panel-for-task-new-comments.png)

1. (Opcional) Para cerrar el panel [!UICONTROL Resumen], siga uno de estos procedimientos:

   * En una tarea o lista de problemas, haga clic en el icono **[!UICONTROL Abrir resumen]** ![](assets/summary-panel-icon.png)

     O

     Haga clic en el icono **X** en la esquina superior derecha del panel [!UICONTROL Resumen].

   * En la sección [!UICONTROL Enviadas] del área de [!UICONTROL Solicitudes], haga clic en el icono **[!UICONTROL Cerrar resumen]** ![](assets/close-summary-with-text-nwe.png)

     O

     Haga clic en el botón **X** en la esquina superior derecha del panel de resumen.

## [!UICONTROL Porcentaje completado]

Use la burbuja azul de progreso en la parte superior de [!UICONTROL Resumen] para actualizar el porcentaje completado de la tarea o el problema que ha seleccionado. Introduzca un número o arrastre la burbuja hasta el porcentaje correcto.

Cuando arrastra y suelta la burbuja en el panel Resumen, el porcentaje completado se actualiza en un punto. No puede introducir un número decimal.

![Porcentaje completado en el panel de resumen](assets/summary-overview-percent-complete.png)

## [!UICONTROL Actualizaciones]

Utilice la sección [!UICONTROL Actualizaciones] del [!UICONTROL Resumen] para ver las actualizaciones recientes y hacer actualizaciones sobre la tarea o problema que haya seleccionado. Haga clic en **[!UICONTROL Ver todo]** para ir directamente a la pestaña [!UICONTROL Actualizaciones] de la tarea.

![Actualiza la sección en el panel de resumen](assets/summary-updates-section.png)

## [!UICONTROL Documentos]

Use la sección [!UICONTROL Documentos] del [!UICONTROL Resumen] para ver los documentos adjuntos a la tarea o al problema que seleccionó. Haga clic en la miniatura para abrir una vista previa del documento. Para ir directamente a la ficha [!UICONTROL Documentos] en la tarea o problema, haga clic en el título **[!UICONTROL Documentos]**.

![Sección de documentos en el panel de resumen](assets/summary-documents-section.png)

## [!UICONTROL Detalles]

Utilice la sección [!UICONTROL Detalles] del [!UICONTROL Resumen] para ver los detalles de alto nivel del elemento de trabajo, realizar asignaciones o añadir fechas de inicio. Haga clic en **[!UICONTROL Ver todo]** para ir directamente a la ficha [!UICONTROL Detalles] de la tarea o problema.



![Sección de detalles en el panel de resumen](assets/summary-details-section.png)

## [!UICONTROL Subtareas]

Esta sección solo está disponible para las tareas. Use la sección [!UICONTROL Subtareas] del [!UICONTROL Resumen] para ver las subtareas [!UICONTROL Nuevas], [!UICONTROL En curso] y [!UICONTROL Cerradas] de la tarea que haya seleccionado. Haga clic en el menú desplegable **[!UICONTROL Estado]** para cambiar de estado. Para ir directamente a la pestaña [!UICONTROL Subtareas] en la tarea, haga clic en el título **[!UICONTROL Subtareas]**.

Si no ha añadido ninguna subtarea a la tarea, haga clic en **[!UICONTROL Añadir una aquí]** para ir directamente a la ficha [!UICONTROL Subtareas] de la tarea.

![Sección de subtareas en el panel de resumen](assets/summary-subtasks-section.png)

## [!UICONTROL Horas]

Utilice la sección [!UICONTROL Horas] del [!UICONTROL Resumen] para registrar horas en la tarea o el problema que haya seleccionado. Haga clic en **[!UICONTROL Registrar hora]** e introduzca sus horas. Para ir directamente a la ficha Horas en la tarea o problema, haga clic en el título **[!UICONTROL Horas]**.

El recuento de horas en el [!UICONTROL Resumen] muestra las horas que registra. Otros usuarios tendrán diferentes recuentos totales de horas en el [!UICONTROL Resumen], según la hora a la que inicien sesión en la tarea.

Si no hay [!UICONTROL horas] planificadas en la tarea o problema y ha registrado tiempo, la barra de horas se mostrará en rojo.

![Sección de horas en el panel de resumen](assets/summary-hours-section.png)

## Rutas de aprobación

Utilice la sección [!UICONTROL Aprobaciones] del [!UICONTROL Resumen] para ver las aprobaciones adjuntas a la tarea o problema que haya seleccionado. Si no ha añadido ninguna aprobación, seleccione una aprobación existente en el menú desplegable o haga clic en **[!UICONTROL Crear proceso de aprobación de un solo uso]** para ir directamente a la pestaña [!UICONTROL Aprobaciones] en la tarea o problema.

Para ir directamente a la pestaña [!UICONTROL Aprobaciones] en la tarea o problema, haga clic en el título **[!UICONTROL Aprobaciones]**.

![Sección de aprobaciones en el panel de resumen](assets/summary-approvals-section.png)
