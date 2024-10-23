---
product-area: projects
navigation-topic: manage-tasks
title: Editar tareas
description: Puede editar información sobre las tareas que ha creado o para las que tiene permisos de Contribute o de Administración. Este artículo describe cómo buscar, buscar y editar una tarea, si tiene los permisos para hacerlo.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 572c6008-3a67-47ae-8f5d-6b871ef1f37b
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '3681'
ht-degree: 3%

---

# Editar tareas

<!--Audited: 07/2024-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: some information in this area is repeated in the following articles. If you need to update a field, update it in both:</p>
<p>** Task finances in details</p>
<p>** Task information in overview)</p>
</div>
-->


Puede editar información sobre las tareas que ha creado o para las que tiene permisos de Contribute o de Administración.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nuevo: estándar</p>
   <p>Actual: Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso</td> 
   <td> <p>Editar acceso a Tareas y Proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> 
    <ul> 
     <li> <p>Permisos de Contribute para editar la siguiente información en el área Detalles de la tarea: </p>
     <ul>
     <li>Descripción</li>
     <li>Estado</li>
     </ul>  
      </li> 
     <li> <p>Administre permisos a una tarea para editar toda la información del área Detalles y del cuadro Editar tarea</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Contribute o permisos superiores para el proyecto</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Limitaciones para editar tareas

Hay algunas limitaciones que pueden impedir que edite tareas.

Tenga en cuenta lo siguiente al editar tareas:

* Actualizar tareas déclencheur notificaciones para proyectos que están en estado Actual. Para evitar confusiones a los usuarios asignados a las tareas, limite las tareas de edición en la medida de lo posible cuando el proyecto se encuentre en el estado Actual.
* No se pueden editar las tareas que se encuentran en un proceso de aprobación. Solo puede registrar el tiempo o actualizar el estado de una tarea en un proceso de aprobación.

  ![](assets/edit-task-in-approval-process-nwe-350x148.png)

* Solo puede editar y agregar documentos a tareas de un proyecto que tenga el estado Completo, Inactivo o Pendiente de aprobación cuando el administrador de Workfront o un administrador de grupo hayan habilitado esta funcionalidad en el área Preferencias del proyecto. Para obtener información sobre cómo establecer las preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Siempre puede editar la siguiente información en una tarea cuando el proyecto se ha marcado como Completado, Inactivo o se encuentra en proceso de aprobación:

   * Hora de registro
   * Editar gastos existentes
   * Adjuntar un formulario personalizado

* Otros usuarios deben actualizar sus páginas para poder ver las actualizaciones que realice en una tarea.

## Edición de una tarea en una lista

Puede editar la información de las tareas en una lista de tareas mediante la edición en línea de los campos mostrados en la vista de la lista.

Para obtener información acerca de la edición de tareas en listas, vea [Editar tareas en una lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

## Edición de una tarea en una lista mediante el Resumen

Puede editar una tarea de una lista mediante el panel Resumen. Para obtener información sobre cómo editar una tarea en el Panel de resumen, consulte la sección &quot;Editar una tarea en el resumen&quot; en el artículo [Editar tareas en una lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

## Editar una tarea en el cuadro Editar tarea

Puede editar una tarea mediante las áreas Editar tarea o Detalles de la tarea. Los siguientes pasos describen la edición de una tarea en el cuadro Editar tarea.

{{step1-click-main-menu}}

1. Haga clic en **Proyectos** y, a continuación, haga clic en el nombre de un proyecto para abrirlo.
1. Haga clic en **Tareas** en el panel izquierdo.
1. Haga clic en la tarea que desee editar.
1. (Condicional) Para editar información limitada sobre una tarea, haga clic en **Detalles de la tarea** en el panel izquierdo.

   ![](assets/nwe-task-details-expanded-350x273.png)

   Considere la posibilidad de editar información en las siguientes áreas de la sección Detalles de la tarea:

   * **Información general**

     Esta área se expande de forma predeterminada.

   * **Formularios personalizados**

     Los nombres de los formularios personalizados solo se muestran si hay formularios personalizados adjuntos al objeto.

   * **Finanzas**

   >[!NOTE]
   >
   >Según la forma en la que el administrador de Workfront o del grupo haya modificado la plantilla de diseño, los campos del área Detalles de la tarea podrían volver a organizarse o no mostrarse. Para obtener más información, consulte [Personalizar la vista de detalles con una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Para obtener información sobre los campos visibles en la sección Detalles de la tarea, continúe editando la tarea en el cuadro Editar tarea como se describe a continuación.

   Para editar la información de la sección Detalles, haga lo siguiente:

   1. (Opcional) Haga clic en el icono **Contraer todo** ![](assets/collapse-all-icon.png) en la esquina superior derecha para contraer todas las áreas.
   1. (Opcional y condicional) Cuando un área esté contraída, haga clic en la **flecha que señala a la derecha** ![](assets/right-pointing-arrow.png) junto a cada área para expandir el área que desea editar.
   1. Para obtener más información sobre cómo editar la información en la ficha Detalles de la tarea, consulte los siguientes artículos:

      * [Administrar información de tarea en el área Información general de detalles de la tarea](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)
      * [Administrar finanzas de tareas en la sección Detalles de tareas](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)

   1. (Opcional) Si no hay formularios personalizados adjuntos a la tarea, empiece a escribir el nombre de un formulario en el campo **Agregar formulario personalizado**, selecciónelo cuando se muestre en la lista y haga clic en **Guardar cambios**.
   1. (Opcional) Haga clic en el icono **Exportar** ![](assets/export.png) para exportar la información general y de los formularios personalizados a un archivo de PDF y, a continuación, haga clic en **Exportar**. Seleccione una de las siguientes opciones:

      * Seleccionar todo (solo se muestra cuando hay al menos un formulario personalizado adjunto)
      * Información general
      * El nombre de uno o varios formularios personalizados

      El archivo del PDF se descarga en el equipo.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      Para obtener más información, consulte [Exportar formularios personalizados y detalles de objetos](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

1. (Condicional) Para editar toda la información sobre la tarea, como usuario con permisos de administración para la tarea, haga clic en el menú **Más** ![](assets/more-icon.png) junto al nombre de la tarea y, a continuación, haga clic en **Editar**.

   O

   En una lista de tareas, seleccione una tarea y haga clic en el icono **Editar** ![](assets/edit-icon.png) que se encuentra en la parte superior de la lista.

   Se abrirá el cuadro Editar tarea.

   >[!IMPORTANT]
   >
   >Debe tener permisos de administración en la tarea para ver la opción de edición.

   Todos los campos de tarea están disponibles en el cuadro Editar tarea y se agrupan por las áreas enumeradas en el panel izquierdo.

   >[!NOTE]
   >
   >Según la forma en la que el administrador de Workfront o del grupo haya modificado la plantilla de diseño, los campos del área Detalles de la tarea podrían volver a organizarse o no mostrarse. Para obtener más información, consulte [Personalizar la vista de detalles con una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Considere la posibilidad de especificar información en cualquiera de las siguientes secciones:

   * [Nombre de la tarea](#task-name)
   * [Información general](#overview)
   * [Asignaciones](#assignments)
   * [Formularios personalizados](#Custom%C2%A0F)
   * [Finanzas](#finance)
   * [Configuración](#settings)

   >[!NOTE]
   >
   >Según la forma en que el administrador de Workfront o el administrador del grupo configuren la plantilla de diseño, los campos del cuadro Editar tarea podrían volver a organizarse o no mostrarse. Para obtener más información, consulte [Personalizar la vista de detalles con una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### Nombre de la tarea {#task-name}

1. Comience a editar la tarea como se ha descrito anteriormente.
1. Haga clic en **Nombre de tarea** en el panel izquierdo.

   ![](assets/nwe-task-name-section-edit-task-box-350x122.png)

1. Actualice el nombre de la tarea.

1. Haga clic en **Guardar** o continúe con las siguientes secciones.

### Información general {#overview}

1. Comience a editar la tarea como se ha descrito anteriormente.
1. Haga clic en **Información general** en el panel izquierdo.

   ![](assets/nwe-overview-section-edit-task-box-350x257.png)

1. Actualice la siguiente información sobre la tarea:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Agregue información adicional sobre la tarea. </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">Sección de información básica</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estado</td> 
      <td> <p>Seleccione el estado de la tarea que indica en qué fase de desarrollo se encuentra la tarea.</p> <p><b>SUGERENCIA</b>

   Puede actualizar el estado de la tarea en el encabezado de la tarea. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Prioridad</td> 
      <td> <p>Se trata de un indicador visual que le permite priorizar las tareas. </p> <p>Seleccione entre las siguientes opciones: </p> 
       <ul> 
      <li> <p> Ninguno</p> </li> 
      <li> <p> Bajo </p> </li> 
      <li> <p>Normal </p> </li> 
      <li> <p>Alto </p> </li> 
      <li> <p> Urgente </p> </li> 
       </ul> <p>Según las Preferencias del proyecto seleccionadas por el administrador de Workfront, los nombres de las prioridades pueden ser diferentes para usted. Para obtener información acerca de las prioridades de tareas, vea <a href="../../../manage-work/tasks/task-information/task-priority.md" class="MCXref xref">Actualizar prioridad de tareas</a>. </p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">Sección de restricciones y fechas de la tarea</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Restricción de tarea</td> 
      <td> <p>Decida cuándo debe completarse la tarea especificando una restricción de tarea. </p> <p>Seleccione entre las siguientes opciones: </p> 
       <ul> 
      <li> <p><span>Fechas fijas</span> </p> <p>Especifique un <strong>Inicio planificado</strong> y una <strong>Fecha planificada de finalización</strong>. </p> </li> 
      <li> <p><span>Debe Iniciar El</span> </p> <p>Especifique una <strong>Fecha planificada de inicio</strong>. </p> </li> 
      <li> <p><span>Debe Finalizar El</span> </p> <p>Especifique una <strong>Fecha planificada de finalización</strong>. </p> </li> 
       </ul> 
       <ul> 
      <li> <p><span>Lo antes posible</span></p> </li> 
      <li> <p><span>Lo más tarde posible</span></p> </li> 
      <li> <p><span>Lo más temprano disponible</span></p> </li> 
      <li> <p> <span>Última hora disponible</span></p> </li> 
      <li> <p><span>No iniciar después de</span> </p> </li> 
      <li> <p>Especificar una fecha planificada de inicio</p> </li> 
      <li> <p><span>No iniciar antes del</span> </p> <p>Especifique una <strong>Fecha planificada de inicio</strong>. </p> </li> 
      <li> <p> Finalizar <span>No después de </span></p> <p>Especifique una <strong>Fecha planificada de finalización</strong>. </p> </li> 
      <li> <p> Finalizar <span>No antes de </span></p> <p>Especificar una <strong>fecha planificada de finalización</strong></p> </li> 
       </ul> <p>Para obtener más información sobre la restricción de tarea, vea <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Información general sobre la restricción de tarea</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Confirmar fecha y hora</td> 
      <td> <p>Es la fecha en la que el usuario asignado a la tarea se compromete a completarla. Puede ser diferente a la Fecha planificada de finalización. Solo las personas asignadas pueden editar este campo. Para obtener información sobre las fechas de confirmación en Workfront, consulte <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Resumen de la fecha de confirmación</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha y hora planificadas para el inicio</td> 
      <td> <p>Cuando se planea que comience la tarea. La fecha planificada de inicio de una tarea está establecida y afectada por una serie de factores:</p> 
       <ul> 
      <li>Según la preferencia de todo el sistema para la fecha de inicio planeada de la tarea, la fecha de inicio de una nueva tarea en un proyecto puede ser hoy o la fecha de inicio del proyecto de forma predeterminada. <span>El administrador del grupo asociado con el proyecto también puede establecer esta preferencia para el grupo.</span> Para obtener más información acerca de las preferencias de tareas a nivel de sistema o de grupo, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configurar las preferencias de tareas y problemas a nivel de sistema</a>.</li> 
      <li>Según las predecesoras de la tarea, Workfront elige la fecha de comienzo planeada para que sea la siguiente fecha disponible después de que finalicen o comiencen las predecesoras, según la relación de predecesoras. Para obtener más información acerca de las relaciones de predecesoras, vea <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Información general sobre las tareas predecesoras</a>.</li> 
      <li>El jefe de proyecto o el propietario de la tarea pueden establecer manualmente la fecha planificada de inicio cuando la delimitación de la tarea sea Fechas fijas o Debe comenzar el. Para obtener más información acerca de las restricciones de tareas, vea <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Información general sobre la restricción de tareas</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha y hora planificadas de finalización</td> 
      <td> <p>Fecha de finalización anticipada, tal como se muestra cuando se planifica la tarea. Workfront establece la fecha planificada de finalización teniendo en cuenta algunos de los siguientes factores:</p> 
       <ul> 
      <li>La fecha planificada de finalización se calcula a partir de la fecha planificada de inicio añadiendo la duración de la tarea a la fecha planificada de inicio. Cuando el administrador del proyecto o Workfront especifican la duración de la tarea, se déclencheur una actualización a la fecha planificada de finalización. Si la fecha planificada cambia, a menudo se debe a que se ha actualizado la Duración de la tarea.</li> 
      <li>El jefe de proyecto o el propietario de la tarea pueden establecer manualmente la fecha planificada de finalización cuando la delimitación de la tarea sea Fechas fijas o Debe finalizar el. Para obtener más información acerca de las restricciones de tareas, vea <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Información general sobre la restricción de tareas</a>.</li> 
      <li>Si el Tipo de duración de la tarea cambia y el número de recursos de las tareas cambia al mismo tiempo, también cambiará la fecha planificada de finalización. Para obtener más información acerca de los tipos de duración, vea <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Información general sobre la duración de la tarea y el tipo de duración</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha y hora de inicio reales</td> 
      <td> <p>Especifique una Fecha de inicio real para la tarea. El valor predeterminado suele rellenarse automáticamente al cambiar el estado de la tarea a En curso. El jefe de proyecto o el propietario de la tarea también pueden modificar manualmente la fecha real de inicio. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha y hora reales de finalización</td> 
      <td> <p>Especifique la fecha y la hora reales en que se completa la tarea. La fecha y hora predeterminadas en las que se completa una tarea siempre coinciden con la hora real en la que el estado se convierte en Completado. El jefe de proyecto o el propietario de la tarea también pueden modificar manualmente la fecha real de finalización. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><b>Sección Tiempo de trabajo</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Esfuerzo de trabajo </td> 
      <td>

   <p>Cantidad de esfuerzo necesario para completar la tarea. Es posible que el jefe de proyecto decida utilizar este campo en lugar de Horas planificadas para estimar el esfuerzo necesario para completar una tarea. Este campo solo está visible cuando se cumplen las siguientes condiciones:</p> 
      <ul> 
      <li> <p>La tarea tiene un tipo de duración simple. </p> <p><b>SUGERENCIA</b>

   Si cambia el Tipo de duración de la tarea, este campo se atenúa. </p> </li>
   <li>El jefe de proyecto ha habilitado el campo Usar esfuerzo de trabajo para calcular automáticamente las horas planificadas para la tarea en el proyecto. </li> 
      </ul> 
      <p>Seleccione entre las siguientes opciones:</p> 
      <ul> 
      <li>Pequeño</li> 
      <li>Medium <span style="font-weight: normal;">(este es el valor predeterminado para una nueva tarea)</span></li> 
      <li>Grande</li> 
      </ul> 
      <p><b>NOTA</b>

   Si actualiza la cantidad de esfuerzo, se podrían actualizar las horas planificadas de la tarea. La actualización es inmediata si el tipo de actualización del proyecto es Automática. Cuando el tipo de actualización del proyecto es Manual, debe volver a calcular la escala de tiempo para ver las horas planificadas actualizadas. </p>

   <p>Para obtener información sobre cómo usar Esfuerzo de trabajo en lugar de Horas planificadas para estimar el esfuerzo de la tarea, consulte <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Resumen del esfuerzo de trabajo</a>. </p> 
    </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar** o continúe con las siguientes secciones.

### Asignaciones {#assignments}

1. Comience a editar la tarea como se ha descrito anteriormente.
1. Haga clic en **Asignaciones** en el panel izquierdo.

   ![](assets/nwe-assignments-section-edit-task-box-350x217.png)

1. Haga clic en **Buscar personas, roles y equipos** y empiece a escribir el nombre del usuario, rol o equipo que desee asignar a la tarea; a continuación, haga clic en él o presione Entrar cuando aparezca en la lista.

   >[!NOTE]
   >
   >Si el nombre del usuario contiene un carácter especial, debe incluirlo en el campo de búsqueda.

   >[!TIP]
   >
   >Puede asignar varios usuarios, roles o equipos. Solo puede asignar usuarios activos, roles y equipos.
   >
   >Si se asignó un usuario, un rol o un equipo antes de desactivarlos, permanecen asignados al elemento de trabajo. En este caso, se recomienda lo siguiente:
   >
   >* Reasignar el elemento de trabajo a los recursos activos.
   >* Asocie los usuarios de un equipo desactivado a un equipo activo y reasigne el elemento de trabajo al equipo activo.

1. (Opcional) Indique si un usuario asignado es el principal asignado a la tarea, seleccionando el botón de opción **Propietario** junto a su nombre. Un equipo no puede ser el principal asignado a una tarea.
1. (Condicional y opcional) Actualice los campos siguientes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tipo de duración</td> 
      <td> <p>Esto identifica la relación entre lo siguiente: </p> 
       <ul> 
      <li> <p>El número de recursos asignados a una tarea </p> </li> 
      <li> <p>Esfuerzo total necesario para completar la tarea </p> </li> 
      <li> <p> Duración total de la tarea. </p> </li> 
       </ul> <p>El administrador de Workfront o de un grupo selecciona la configuración predeterminada de Tipo de duración para las tareas del sistema o del grupo. Para obtener información sobre cómo establecer los valores predeterminados del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>. </p> <p>Los tipos de duración permiten establecer asignaciones de recursos coherentes según las necesidades de la tarea. Para obtener más información acerca del tipo de duración de una tarea, vea <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Información general sobre la duración de la tarea y el tipo de duración</a>. </p> <p>Seleccione entre las siguientes opciones: </p> 
       <ul> 
      <li> <p>Asignación calculada </p> </li> 
      <li> <p> Trabajo calculado </p> </li> 
      <li> <p>Condicionada por el esfuerzo </p> </li> 
      <li> <p>Simple</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Duración por resolicitud</td> 
      <td> <p>Esto solo se muestra en el elemento principal de las tareas recurrentes. Muestra la duración de cada tarea recurrente, tal como se definió cuando se creó la tarea. Para obtener información acerca de la creación de tareas recurrentes, vea <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Crear tareas recurrentes</a>. </p> <p> <b>NOTA</b>

   Las duraciones modificadas en tareas recurrentes individuales no muestran el valor indicado en este campo. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Duración</td> 
      <td> 
      <div> 
      <div> 
      <p>Es la cantidad de tiempo que permite que una tarea permanezca abierta antes de completarse. </p> 
      <p><b>IMPORTANTE</b>

   Debido a que la duración de la tarea suele ser la cantidad de tiempo entre las fechas planificadas de inicio y planificadas de finalización, afecta a la cronología del proyecto.</p>

   <p>Para indicar la Duración de la tarea y la unidad de tiempo, haga lo siguiente:</p> 
      <ul> 
      <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Escriba la cantidad de tiempo y seleccione una de las unidades de tiempo disponibles en el menú desplegable.</p> <p><b>SUGERENCIA</b></p>
      Al actualizar la Duración de las tareas en una lista de tareas, puede utilizar la abreviatura para la unidad de tiempo. </p> </li> 
      </ul> 
      <p> Puede elegir entre las opciones de tiempo normal o tiempo transcurrido en la siguiente tabla: </p> 
      <table style="table-layout:auto"> 
      <col> 
      <col data-mc-conditions=""> 
      <tbody> 
      <tr> 
      <td>Unidad de tiempo</td> 
      <td>Abreviatura</td> 
      </tr> 
      <tr> 
      <td>minutos</td> 
      <td>L</td> 
      </tr> 
      <tr> 
      <td>Horas</td> 
      <td>H</td> 
      </tr> 
      <tr> 
      <td>Días. Esta es la opción predeterminada. </td> 
      <td>D</td> 
      </tr> 
      <tr> 
      <td>Semanas</td> 
      <td>S</td> 
      </tr> 
      <tr> 
      <td>Meses</td> 
      <td>M</td> 
      </tr> 
      <tr> 
      <td>Minutos transcurridos</td> 
      <td>EM</td> 
      </tr> 
      <tr> 
      <td>Horas transcurridas</td> 
      <td>EH</td> 
      </tr> 
      <tr> 
      <td>Días transcurridos</td> 
      <td>ED</td> 
      </tr> 
      <tr> 
      <td>Semanas transcurridas</td> 
      <td>EW</td> 
      </tr> 
      <tr> 
      <td>Meses transcurridos</td> 
      <td>ET</td> 
      </tr> 
      </tbody> 
   </table>

   <p><b>NOTA</b>

   <p>El tiempo transcurrido es una unidad de tiempo de la duración de una tarea. Es el tiempo entre la Fecha planificada de inicio y la Fecha planificada de finalización de una tarea que incluye días festivos, fines de semana y días libres. En otras palabras, el tiempo transcurrido es el paso de los días del calendario.

   El tiempo normal tiene en cuenta los días festivos, los fines de semana y los días libres, y los excluye de la duración de la tarea. Para obtener más información acerca de la duración de la tarea, vea <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Información general sobre la duración de la tarea y el tipo de duración</a>. </p>
   </div> 
   </div> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Horas planificadas</td> 
   <td> <p>Especifique el número de horas planificadas para la tarea, en horas. Es la cantidad de tiempo real que tardarían los usuarios asignados de la tarea en completarla. Solamente puede especificar el número de horas planificadas para una tarea cuando el tipo de duración está establecido en Asignación calculada. Para obtener más información acerca de los tipos de duración, vea <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Información general sobre la duración de la tarea y el tipo de duración</a>.</p> 
   <b>NOTA</b>
   <p>
   Al crear tareas recurrentes, las horas planificadas son las de cada ocurrencia. Las horas planificadas de las tareas principales son el total de todas las horas planificadas de todas las ocurrencias. Para obtener información acerca de la creación de tareas recurrentes, vea <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Crear tareas recurrentes</a>.
   </p>

   </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Asignación</td> 
   <td> <p>Si la restricción de tarea se calcula por trabajo o por esfuerzo, especifique el <strong>porcentaje de asignación</strong> (porcentaje de asignación) para cada usuario asignado. Cantidad de tiempo desde la programación de la persona asignada que puede dedicar a esta tarea. Si se cambia el porcentaje de asignación de un usuario asignado, se cambiarán las horas planificadas de una tarea. </p> <p>Cuando la restricción de tarea es simple, puede especificar lo siguiente:</p> 
      <ul> 
      <li> <p>Horas de asignación de cada usuario asignado.</p> </li> 
      <li> <p>Horas planificadas de la tarea</p> </li> 
      <li> <p>Duración de la tarea</p> </li> 
      </ul> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Rol de asignado</td> 
   <td> <p>Seleccione un rol del menú desplegable <strong>Rol de asignado</strong> cuando haya seleccionado una persona como asignado. Esta es la función que el usuario asignado puede desempeñar en esta tarea. </p> <p><b>SUGERENCIA</b>

   En el menú desplegable solo aparecen los roles asociados con cada usuario asignado en su perfil.</p> </td>
   </tr> 
      </tbody> 
      </table>

1. Haga clic en **Guardar** o continúe con las siguientes secciones.

### Formularios personalizados

Puede definir formularios personalizados predeterminados que se adjuntarán automáticamente a las tareas cuando estas se agreguen a un proyecto. Para obtener información acerca de cómo configurar el proyecto para que incluya formularios personalizados de tareas predeterminados para todas las tareas nuevas, consulte la sección &quot;Tareas&quot; en el artículo [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Comience a editar la tarea como se ha descrito anteriormente.
1. Haga clic en **Forms personalizado** en el panel izquierdo, o haga clic en el nombre de un formulario personalizado si ya está adjunto.

   ![](assets/nwe-custom-forms-section-edit-task-box-350x127.png)

1. Haga clic en **Agregar formulario personalizado** y seleccione el formulario o formularios personalizados que desee asociar con la tarea. Debe crear los formularios personalizados antes de que estén disponibles para seleccionarlos en este campo. En la lista solo se muestran los formularios personalizados activos.

   Para obtener más información sobre cómo crear formularios personalizados, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).Puede agregar hasta diez formularios personalizados a una tarea

1. (Condicional) Si adjuntó un formulario personalizado a la tarea, edite los campos del formulario. Debe especificar todos los campos obligatorios antes de guardar la tarea.

   >[!NOTE]
   >
   >Según la forma en que el administrador de Workfront haya establecido los permisos para las secciones del formulario personalizado, no todos podrán ver o editar los mismos campos en un formulario personalizado determinado. Los permisos para editar campos dentro de una sección de un formulario personalizado dependen de los permisos que tenga sobre la propia tarea. Para obtener información acerca de cómo establecer permisos para tareas, vea [Compartir una tarea](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

1. Haga clic en **Guardar** o continúe con las siguientes secciones.

### Finanzas {#finance}

1. Empiece a editar la tarea tal como se describe en la sección [Editar tareas](#Edit2) de este artículo.
1. Haga clic en **Finanzas** en el panel izquierdo.

   ![](assets/nwe-finance-section-edit-task-box-350x298.png)

1. Actualice los campos siguientes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tipo de costo</td> 
      <td> <p>Especifique el Tipo de coste de la tarea. Esto determina cómo se calcula el coste de la tarea, en función del número de horas de las tareas. </p> <p>Seleccione entre las siguientes opciones: </p> 
       <ul> 
        <li> <p>Sin coste</p> </li> 
        <li> <p>Fijo por hora </p> </li> 
        <li> <p> Usuario por hora </p> </li> 
        <li> <p> Rol por hora</p> </li> 
       </ul> <p>Para obtener más información sobre los costos de seguimiento, vea <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Costos de seguimiento</a> . El administrador de Workfront o de un grupo selecciona la configuración predeterminada Tipo de coste para las tareas del sistema o del grupo. Para obtener información sobre cómo establecer los valores predeterminados del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de ingresos</td> 
      <td> <p>Especifique el Tipo de ingresos para la tarea. Esto determina cómo se calculan los ingresos de la tarea, en función del número de horas de las tareas. </p> <p>Seleccione entre las siguientes opciones: </p> 
       <ul> 
      <li> <p> No facturable </p> </li> 
      <li> <p>Usuario por hora </p> </li> 
      <li> <p>Rol por hora </p> </li> 
      <li> <p>Fijo por hora </p> </li> 
      <li> <p>Usuario por hora sin límite </p> </li> 
      <li> <p>Rol por hora con límite </p> </li> 
      <li> <p>Usuario por hora más fijos </p> </li> 
      <li> <p>Rol por hora más fijos </p> </li> 
      <li> <p>Ingresos fijos </p> </li> 
       </ul> <p>Para obtener más información sobre el seguimiento de los ingresos, consulte<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Información general sobre facturación e ingresos</a> . </p> <p>El administrador de Workfront o del grupo selecciona la configuración predeterminada Tipo de ingresos para las tareas del sistema o del grupo. Para obtener información sobre cómo establecer los valores predeterminados del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar** o continúe con la siguiente sección.

### Configuración {#settings}

1. Empiece a editar la tarea tal como se describe en la sección [Editar tareas](#Edit2) de este artículo.
1. Haga clic en **Configuración** en el panel izquierdo.

   ![](assets/nwe-settings-section-edit-task-box-350x304.png)

1. Actualice los campos siguientes:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Modo de seguimiento</td> 
      <td> <p>Especifique cómo se rastrea el estado de progreso de la tarea. </p> <p>Seleccione entre las siguientes opciones: </p> 
       <ul> 
      <li> <p> El usuario debe actualizar </p> </li> 
      <li> <p>Asumir a tiempo </p> </li> 
      <li> <p>Ignorar advertencias tardías</p> </li> 
      <li> <p> Autocompletar </p> </li> 
      <li> <p>Predecesora </p> </li> 
       </ul> <p>Para obtener más información sobre el modo de seguimiento de las tareas, consulte <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Información general sobre el modo de seguimiento de tareas</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nivelación de recursos</td> 
      <td> <p>Seleccione el campo <strong>Excluir de la redistribución de recursos</strong> si desea que los recursos asignados a la tarea se excluyan de la redistribución.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Retraso de nivelación</td> 
      <td> <p>Especifique la demora de nivelación en horas. </p> <p> Para obtener más información acerca de los retrasos de redistribución, vea <a href="../../../manage-work/tasks/task-information/task-leveling-delay.md" class="MCXref xref">Actualizar tarea Retraso de redistribución</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proceso de aprobación</td> 
      <td> <p>Seleccione un proceso de aprobación que desee asociar con la tarea. El administrador de Workfront debe definir los procesos de aprobación en el sistema para poder asociarlos a las tareas. Un usuario con acceso administrativo a los procesos de aprobación también puede crear procesos de aprobación específicos del grupo. </p> <p>Para obtener más información acerca de cómo crear procesos de aprobación, vea <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md">Crear un proceso de aprobación para elementos de trabajo</a>. Tenga en cuenta lo siguiente al añadir procesos de aprobación: </p> 
       <ul>

   <li> <p>En la lista solo se muestran los procesos de aprobación activos. </p> </li>

   <li> <p>Los procesos de aprobación de todo el sistema y específicos del grupo se muestran en la lista. Un proceso de aprobación asociado a un grupo que no sea el del proyecto no se muestra en la lista. </p>

   <p><b>IMPORTANTE</b>

   Si el grupo del proyecto cambia, el proceso de aprobación específico del grupo que se adjuntó anteriormente se convierte en un proceso de aprobación de un solo uso. Para obtener más información acerca de cómo afectan los cambios en el grupo del proyecto o los cambios en el proceso de aprobación a la configuración de aprobación, vea <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">Cómo afectan los cambios en el grupo y el proceso de aprobación a los procesos de aprobación asignados</a>. </p>

   </li>

   <li> <p>Puede definir los procesos de aprobación predeterminados que se adjuntarán automáticamente a las tareas cuando estas se agreguen a un proyecto. Para obtener información acerca de cómo configurar el proyecto para que incluya procesos predeterminados de aprobación de tareas, consulte la sección "Tareas" en el artículo <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Editar proyectos</a>. </p> </li>

   <li> <p>Cuando se realizan tareas de edición masiva, existen los siguientes escenarios: </p> 
      <ul> 
      <li> <p>Cuando se seleccionan varias tareas del mismo grupo, en este campo se muestran tanto los procesos de aprobación de nivel de sistema como los de nivel de grupo. </p> </li> 
      <li> <p>Al seleccionar varias tareas de diferentes grupos, solo se muestran en este campo los procesos de aprobación de nivel de sistema. </p> </li> 
      <li> <p>Cuando cualquiera de las tareas tiene un proceso de aprobación de un solo uso adjunto, se reemplaza por el proceso de aprobación de nivel de sistema o de nivel de grupo que seleccione. </p> </li>

   </ul> </li> 
      </ul> </td> 
     </tr> 
    </tbody> 
   </table>
    </li>

1. Haga clic en **Guardar**.

<!--notes from the table: <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)</p>       -->

## Editar una tarea en el encabezado de la tarea (limitada)

Puede editar una cantidad limitada de información en el encabezado de la tarea.

El administrador del sistema o del grupo puede personalizar los campos que se ven en el encabezado de la tarea. Para obtener más información, vea [Personalizar encabezados de objeto mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).


![](assets/qs-task-header-without-approvals-and-with-dependecies-350x17.png)

Los campos siguientes se incluyen en el encabezado de la tarea de forma predeterminada:

* Nombre de la tarea
* Porcentaje completado
* Asignaciones
* Fecha planificada de finalización

  >[!CAUTION]
  >
  >Algunas restricciones de tarea y otras dependencias pueden impedir la edición de este campo. Para obtener información acerca de las restricciones de tarea, vea [Introducción a las restricciones de tarea](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Estado
* Tome decisiones de aprobación si se establece como aprobador en un proceso de aprobación actual

## Editar tareas de forma masiva

Puede editar las tareas de forma masiva en una lista y actualizar toda su información al mismo tiempo cuando selecciona guardar automáticamente los cambios que está realizando en las tareas de la lista.

Para obtener información acerca de cómo guardar tareas de forma masiva, consulte la sección &quot;Editar tareas de forma masiva&quot; en el artículo [Editar tareas de una lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).
