---
content-type: overview
title: Resumen, descripción general
description: Puede usar el Panel de resumen para revisar y actualizar la información del elemento de trabajo directamente desde una lista de tareas, problemas, documentos o desde otras áreas de  [!DNL Adobe Workfront] que muestran tareas y problemas.
feature: Get Started with Workfront
author: Nolan
exl-id: 5e4026b2-5f2f-45c1-bef1-04e20c62ed8a
source-git-commit: 5d6e9788ccbae7a8970cff56558233a57ceee1ab
workflow-type: tm+mt
source-wordcount: '992'
ht-degree: 2%

---

# [!UICONTROL Resumen] información general

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers or in Production for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span> -->

Puede usar el panel [!UICONTROL Resumen] para revisar y actualizar la información del elemento de trabajo directamente desde una lista de tareas, problemas, documentos o desde otras áreas de [!DNL Adobe Workfront] que muestran tareas y problemas.

El administrador de Workfront o de grupo puede modificar las áreas y los campos que se muestran en el Panel de resumen. Pueden agregar hasta 16 campos al panel Resumen.

>[!IMPORTANT]
>
>Se recomienda agregar campos que se deben actualizar con frecuencia al Panel de resumen para poder acceder fácilmente a ellos y actualizarlos sin tener que acceder a la página principal del objeto.
>
>Por ejemplo, puede agregar los siguientes campos actualizados con frecuencia a los paneles Resumen de tareas y problemas:
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
   <td>Tareas en las áreas de trabajo de [!UICONTROL sin asignar] y [!UICONTROL asignado] del Distribuidor de cargas de trabajo de [!UICONTROL]</td> 
  </tr> 
   <tr> 
   <td>Tareas en una hoja de horas de [!UICONTROL]</td> 
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
   <td>Problemas en el área de [!UICONTROL Trabajo asignado] del Distribuidor de cargas de trabajo de [!UICONTROL]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Problemas en la sección [!UICONTROL Enviado] del área de [!UICONTROL Solicitudes]</td> 
  </tr> 
</tr> 
   <tr> 
   <td>Problemas en una hoja de horas de [!UICONTROL]</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td><b>Documentos</b></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Área de [!UICONTROL Documents]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Sección [!UICONTROL Documents] de cualquier objeto (proyecto, tarea, problema, programa, portafolio, plantilla, tarea de plantilla, usuario)</td> 
  </tr> 
 </tbody> 
</table>

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront administrators can customize the Summary in the Layout Template. For more information, see <a href="../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
-->

Este artículo describe cómo acceder y utilizar el panel [!UICONTROL Resumen] para tareas y problemas en listas.

Para obtener información sobre cómo obtener acceso a [!UICONTROL Summary] en el [!UICONTROL Distribuidor de cargas de trabajo], consulte [Actualizar elementos de trabajo en el [!UICONTROL Distribuidor de cargas de trabajo] mediante [!UICONTROL Summary]](../../resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

Para obtener información sobre el acceso a [!UICONTROL Summary] para documentos, consulte [[!UICONTROL Summary] para obtener información general sobre documentos](../../documents/managing-documents/summary-for-documents.md).

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
   <td> <p>Nuevo: Colaborador o superior</p>
   O
   <p>Actual:[!UICONTROL Request] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuración del nivel de acceso</strong></td> 
   <td> <p>[!UICONTROL View] o acceso superior a Tareas, Problemas, Documentos</p> <p>[!UICONTROL Vista] o acceso superior a cualquier objeto para el que desee ver documentos [!UICONTROL Resumen]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>[!UICONTROL View] o permisos superiores para una tarea, un problema o un documento</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront]. Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Ver el panel [!UICONTROL Resumen] en una lista de tareas o problemas

1. Vaya a una tarea o problema y seleccione un elemento de la lista.
1. Haga clic en el icono **[!UICONTROL Resumen]** ![](assets/qs-summary-in-new-toolbar-small.png)

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

     Haga clic en el icono **X** en la esquina superior derecha del Panel de resumen.

## [!UICONTROL Porcentaje completado]

Utilice la barra de progreso de la parte superior de [!UICONTROL Resumen] para actualizar el porcentaje completado de la tarea o el problema que ha seleccionado. Introduzca un número o arrastre la barra hasta el porcentaje correcto.

![Porcentaje completado en el panel de resumen](assets/summary-overview-percent-complete.png)

## [!UICONTROL Actualizaciones]

Use la sección [!UICONTROL Actualizaciones] del [!UICONTROL Resumen] para ver las actualizaciones recientes y hacer actualizaciones sobre la tarea o el problema que seleccionó. Haga clic en **[!UICONTROL Ver todo]** para ir directamente a la ficha [!UICONTROL Actualizaciones] de la tarea.

![Actualiza la sección en el Panel de resumen](assets/summary-updates-section.png)

## [!UICONTROL Documentos]

Use la sección [!UICONTROL Documentos] del [!UICONTROL Resumen] para ver los documentos adjuntos a la tarea o al problema que seleccionó. Haga clic en la miniatura para abrir una vista previa del documento. Para ir directamente a la ficha [!UICONTROL Documentos] en la tarea o el problema, haz clic en el título de **[!UICONTROL Documentos]**.

![Sección de documentos en el panel de resumen](assets/summary-documents-section.png)

## [!UICONTROL Detalles]

Utilice la sección [!UICONTROL Detalles] del [!UICONTROL Resumen] para ver detalles de elementos de trabajo de alto nivel, realizar asignaciones o agregar fechas de inicio. Haga clic en **[!UICONTROL Ver todo]** para ir directamente a la ficha [!UICONTROL Detalles] de la tarea o el problema.

>[!NOTE]
>
>Los campos que aparecen en esta sección son los mismos campos que aparecen en el panel derecho de Inicio. Puede personalizar estos campos [Personalizar [!UICONTROL Inicio] y [!UICONTROL Resumen] con una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).

![Sección de detalles en el panel de resumen](assets/summary-details-section.png)

## [!UICONTROL Subtareas]

Esta sección solo está disponible para tareas. Use la sección [!UICONTROL Subtareas] del [!UICONTROL Resumen] para ver las subtareas [!UICONTROL Nuevas], [!UICONTROL En curso] y [!UICONTROL Cerradas] de la tarea que seleccionó. Haga clic en el menú desplegable **[!UICONTROL Estado]** para cambiar de estado. Para ir directamente a la ficha [!UICONTROL Subtareas] en la tarea, haga clic en el título de **[!UICONTROL Subtareas]**.

Si no ha agregado ninguna subtarea a la tarea, haga clic en **[!UICONTROL Agregar una aquí]** para ir directamente a la ficha [!UICONTROL Subtareas] de la tarea.

![Sección de subtareas en el panel de resumen](assets/summary-subtasks-section.png)

## [!UICONTROL Horas]

Use la sección [!UICONTROL Horas] del [!UICONTROL Resumen] para registrar horas en la tarea o el problema que seleccionó. Haga clic en **[!UICONTROL Registrar tiempo]** e introduzca sus horas. Para ir directamente a la ficha Horas en la tarea o el problema, haz clic en el título **[!UICONTROL Horas]**.

El recuento de horas en [!UICONTROL Summary] muestra las horas que registra. Otros usuarios tendrán diferentes totales de horas en [!UICONTROL Resumen] según la hora en que inicien sesión en la tarea.

Si no hay [!UICONTROL horas] planeadas en la tarea o el problema y ha registrado tiempo, la barra de horas se mostrará en rojo.

![Sección de horas en el panel de resumen](assets/summary-hours-section.png)

## Rutas de aprobación

Use la sección [!UICONTROL Aprobaciones] del [!UICONTROL Resumen] para ver las aprobaciones adjuntas a la tarea o al problema que seleccionó. Si no ha agregado ninguna aprobación, seleccione una aprobación existente en el menú desplegable o haga clic en **[!UICONTROL Crear proceso de aprobación de un solo uso]** para ir directamente a la pestaña [!UICONTROL Aprobaciones] en la tarea o el problema.

Para ir directamente a la ficha [!UICONTROL Aprobaciones] en la tarea o el problema, haga clic en el título de **[!UICONTROL Aprobaciones]**.

![Sección de aprobaciones en el panel de resumen](assets/summary-approvals-section.png)
