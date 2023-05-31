---
content-type: overview
title: Resumen, descripción general
description: Puede utilizar el Panel de resumen para revisar y actualizar la información del elemento de trabajo directamente desde una lista de tareas, problemas, documentos o desde otras áreas de [!DNL Adobe Workfront] que muestran tareas y problemas.
feature: Get Started with Workfront
exl-id: 5e4026b2-5f2f-45c1-bef1-04e20c62ed8a
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 2%

---

# [!UICONTROL Resumen] descripción general

Puede usar el complemento [!UICONTROL Resumen] panel para revisar y actualizar la información del elemento de trabajo directamente desde una lista de tareas, problemas, documentos o desde otras áreas de [!DNL Adobe Workfront] que muestran tareas y problemas.

En la tabla siguiente se muestran las áreas en las que puede localizar y utilizar [!UICONTROL Resumen] panel:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Tareas</td> 
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
  <tr data-mc-conditions=""> 
   <td>Problemas</td> 
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
  <tr data-mc-conditions=""> 
   <td>Documentos</td> 
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

Este artículo describe cómo acceder y utilizar el [!UICONTROL Resumen] panel para tareas y problemas en listas.

Para obtener información sobre el acceso a [!UICONTROL Resumen] en el [!UICONTROL Distribuidor de cargas de trabajo], consulte [Actualizar elementos de trabajo en [!UICONTROL Distribuidor de cargas de trabajo] uso del [!UICONTROL Resumen]](../../resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

Para obtener información sobre el acceso a [!UICONTROL Resumen] para ver los documentos, consulte [[!UICONTROL Resumen] información general sobre para documentos](../../documents/managing-documents/summary-for-documents.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>[!UICONTROL Request] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>[!UICONTROL View] o acceso superior a Tareas, Problemas, Documentos</p> <p>[!UICONTROL Vista] o acceso superior a cualquier objeto para el que desee ver el [!UICONTROL Resumen] de los documentos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo [!DNL Workfront] El administrador puede modificar su nivel de acceso. Consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>[!UICONTROL View] o permisos superiores para una tarea, un problema o un documento</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Ver el [!UICONTROL Resumen] panel en una lista de tareas o problemas

1. Vaya a una tarea o problema y seleccione un elemento de la lista.
1. Haga clic en **[!UICONTROL Resumen]** icono ![](assets/qs-summary-in-new-toolbar-small.png)

   o

   Haga clic en **[!UICONTROL Abrir resumen]** icono ![](assets/open-summary-with-text-nwe.png) en el [!UICONTROL Enviado] de la sección [!UICONTROL Solicitudes] área.

   Después de abrir el Resumen, permanece abierto a medida que hace clic en otras tareas o problemas o los selecciona y permanece abierto hasta que lo cierra manualmente.

   >[!TIP]
   >
   >Solo puede seleccionar una tarea o un problema a la vez para ver sus detalles en la [!UICONTROL Resumen] panel.

   ![](assets/summary-overview--open-task-from-summary-icon-350x112.png)

1. (Opcional) Para cerrar el [!UICONTROL Resumen] , realice una de las siguientes acciones:

   * En una tarea o lista de problemas, haga clic en **[!UICONTROL Abrir resumen]** icono ![](assets/summary-panel-icon.png)

      O

      Haga clic en **X** en la esquina superior derecha de la ventana [!UICONTROL Resumen] panel.

   * En el [!UICONTROL Enviado] de la sección [!UICONTROL Solicitudes] , haga clic en el **[!UICONTROL Cerrar resumen]** icono ![](assets/close-summary-with-text-nwe.png)

      O

      Haga clic en **X** en la esquina superior derecha del panel Resumen.

## [!UICONTROL Porcentaje completado]

Utilice la barra de progreso de la parte superior de la [!UICONTROL Resumen] para actualizar el porcentaje completado de la tarea o el problema que ha seleccionado. Introduzca un número o arrastre la barra hasta el porcentaje correcto.

![](assets/summary-overview-percent-complete-350x395.png)

## [!UICONTROL Actualizaciones]

Utilice el [!UICONTROL Actualizaciones] de la sección [!UICONTROL Resumen] para ver las actualizaciones recientes y actualizar la tarea o el problema seleccionados. Clic **[!UICONTROL Ver todo]** para ir directamente a [!UICONTROL Actualizaciones] de la tarea.

![](assets/summary-updates-with-block-quote-350x290.png)

## [!UICONTROL Documentos]

Utilice el [!UICONTROL Documentos] de la sección [!UICONTROL Resumen] para ver los documentos adjuntos a la tarea o al problema seleccionado. Haga clic en la miniatura para abrir una vista previa del documento. Para ir directamente a [!UICONTROL Documentos] en la tarea o problema, haga clic en el botón **[!UICONTROL Documentos]** título.

![](assets/summary-overview-documents-350x84.png)

## [!UICONTROL Detalles]

Utilice el [!UICONTROL Detalles] de la sección [!UICONTROL Resumen] para ver detalles de elementos de trabajo de nivel superior, realizar asignaciones o agregar fechas de inicio. Clic **[!UICONTROL Ver todo]** para ir directamente a [!UICONTROL Detalles] en la tarea o el problema.

>[!NOTE]
>
>Los campos que aparecen en esta sección son los mismos campos que aparecen en el panel derecho de Inicio. Puede personalizar estos campos [Personalizar [!UICONTROL Inicio] y [!UICONTROL Resumen] uso de una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).

![](assets/summary-overview-details-new-350x278.png)

## [!UICONTROL Subtareas]

Esta sección solo está disponible para tareas. Utilice el [!UICONTROL Subtareas] de la sección [!UICONTROL Resumen] para ver [!UICONTROL Nuevo], [!UICONTROL En curso], y [!UICONTROL Cerrado] subtareas de la tarea seleccionada. Haga clic en **[!UICONTROL Estado]** menú desplegable para cambiar entre estados. Para ir directamente a [!UICONTROL Subtareas] en la tarea, haga clic en el icono **[!UICONTROL Subtareas]**&#x200B;title.

Si no ha agregado ninguna subtarea a la tarea, haga clic en **[!UICONTROL Agregue uno aquí]** para ir directamente a [!UICONTROL Subtareas] de la tarea.

![](assets/summary-overview-subtasks-350x140.png)

## [!UICONTROL Horas]

Utilice el [!UICONTROL Horas] de la sección [!UICONTROL Resumen] para registrar horas en la tarea o el problema seleccionado. Clic **[!UICONTROL Hora de registro]** e introduzca sus horas. Para ir directamente a la pestaña Horas de la tarea o del problema, haga clic en **[!UICONTROL Horas]** título.

El recuento de horas en [!UICONTROL Resumen] muestra las horas que ha registrado. Otros usuarios tendrán diferentes totales de horas en la [!UICONTROL Resumen] en función de la hora en la que inicien sesión en la tarea.

Si no hay ninguna actividad planificada [!UICONTROL horas] cuando se selecciona la tarea o el problema y se ha registrado el tiempo, la barra de horas se muestra en rojo.

![](assets/summary-overview-hours-350x96.png)

## Rutas de aprobación

Utilice el [!UICONTROL Aprobaciones] de la sección [!UICONTROL Resumen] para ver las aprobaciones adjuntas a la tarea o al problema seleccionado. Si no ha añadido ninguna aprobación, seleccione una aprobación existente en el menú desplegable o haga clic en **[!UICONTROL Crear proceso de aprobación de un solo uso]** para ir directamente a [!UICONTROL Aprobaciones] en la tarea o el problema.

Para ir directamente a [!UICONTROL Aprobaciones] en la tarea o problema, haga clic en el botón **[!UICONTROL Aprobaciones]** título.

![](assets/summary-overview-approvals-350x122.png)
