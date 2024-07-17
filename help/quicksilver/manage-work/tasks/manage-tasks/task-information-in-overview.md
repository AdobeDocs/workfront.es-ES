---
product-area: projects
navigation-topic: manage-tasks
title: Administrar información de tareas en el área Información general de Detalles de tareas
description: Administrar información de tareas en el área Información general de Detalles de tareas
author: Alina
feature: Work Management
exl-id: 4980b28f-914d-4cf9-813f-14983aac660b
source-git-commit: 5b7a5aff0f8bdf7cf8429ac29b50c3beaf4bd3b4
workflow-type: tm+mt
source-wordcount: '2089'
ht-degree: 4%

---

# Administrar información de tareas en el área Información general de Detalles de tareas

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, do it in both articles)</p>
-->

Puede ver o editar la información de una tarea accediendo al área Información general de la sección Detalles de la tarea Hay un número limitado de campos que puede ver o editar en esta área. Para obtener información sobre cómo editar toda la información de una tarea, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

Este artículo describe cómo ver o editar información en el área Información general de Detalles de la tarea. Para obtener información sobre cómo actualizar otras áreas de Detalles de tareas, consulte los siguientes artículos:

* [Administrar finanzas de tareas en la sección Detalles de tareas](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)
* [Agregar un formulario personalizado a un objeto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)
* [Administrar formularios personalizados adjuntos a objetos](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md)

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <caption style="text-align: left;">
   *Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront. 
 </caption> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>plan Adobe Workfront<b>*</b> </p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td> <p>Licencia Adobe Workfront<b>*</b> </p> </td> 
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configuraciones de nivel de acceso*</strong> </td> 
   <td> <p>Acceso de visualización o superior a Proyectos y tareas</p> <p>Si tiene el nivel de acceso correcto pero aún no puede editar la sección Detalles de la tarea, pregunte a su Adobe Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permisos de objeto</strong> </p> </td> 
   <td> <p>Contribute o permisos superiores para el proyecto</p> <p>Vea los permisos de la tarea para ver información en la sección Detalles. </p> 
   <p>Permisos de Contribute para que la tarea actualice la siguiente información en la sección Detalles:</p>

<ul>
   <li>Descripción</li>
   <li>Estado</li>
   </ul>

<p>Administre permisos para que la tarea actualice toda la información en la sección Detalles.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Edite la información de la tarea en la sección Información general sobre los detalles de la tarea

1. Vaya a una tarea que desee ver o editar.
1. Haga clic en **Detalles de la tarea** en el panel izquierdo
1. Vaya al área **Información general** para ver más información sobre la tarea.

   De forma predeterminada, Información general es la primera área de la sección Detalles de la tarea y se expande.

   >[!NOTE]
   >
   >Según la forma en que el administrador de Workfront o el administrador del grupo configuren la plantilla de diseño, los campos de la sección Detalles de la tarea podrían volver a organizarse o no mostrarse. Para obtener más información, consulte [Personalizar la vista de detalles con una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Haga clic en el icono **Editar** ![](assets/edit-icon.png) en la esquina superior derecha de la sección Detalles y, a continuación, haga clic en **Información general**.

   >[!TIP]
   >
   >No puede editar campos que Workfront genere automáticamente o para los que no tenga permisos de edición.

1. Edite cualquier campo que esté disponible para la edición haciendo clic en el campo o haga clic en **+Agregar** para agregar información a un campo vacío.
1. Vea o edite cualquiera de los campos siguientes de la lista.

   No todos los campos son editables.  

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td> <p>Información adicional sobre la tarea</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Número de referencia</td> 
      <td>Es un valor único para la tarea generada por Workfront para todos los objetos del sistema. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>Los usuarios con permisos de administración de una tarea pueden especificar un vínculo a una página interna o externa en este campo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estado</td> 
      <td> <p>Seleccione el estado de la tarea que indica en qué fase de desarrollo se encuentra la tarea.</p> <p>Sugerencia: Puede actualizar el estado de la tarea en el encabezado de la tarea. </p> </td> 
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
      <td role="rowheader">Tipo de duración</td> 
      <td> <p>Esto identifica la relación entre lo siguiente: </p> 
       <ul> 
        <li> <p>El número de recursos asignados a una tarea </p> </li> 
        <li> <p>Esfuerzo total necesario para completar la tarea </p> </li> 
        <li> <p> Duración total de la tarea. </p> </li> 
       </ul> <p>El administrador de Workfront <span> o un administrador de grupo</span> selecciona la configuración predeterminada de Tipo de duración para las tareas del sistema o del grupo. Para obtener información sobre cómo establecer los valores predeterminados del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>. </p> <p>Los tipos de duración permiten establecer asignaciones de recursos coherentes según las necesidades de la tarea. Para obtener más información acerca del tipo de duración de una tarea, vea <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Información general sobre la duración de la tarea y el tipo de duración</a>. </p> <p>Seleccione entre las siguientes opciones: </p> 
       <ul> 
        <li> <p>Asignación calculada </p> </li> 
        <li> <p> Trabajo calculado </p> </li> 
        <li> <p>Condicionada por el esfuerzo </p> </li> 
        <li> <p>Simple</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duración</td> 
      <td> 
       <div> 
        <div> 
         <p>Es la cantidad de tiempo que permite que una tarea permanezca abierta antes de completarse. </p> 
         <p>Importante: Debido a que la duración de la tarea suele ser la cantidad de tiempo entre las fechas planificadas de inicio y finalización, afecta a la cronología del proyecto.</p> 
         <p>Para indicar la Duración de la tarea y la unidad de tiempo, haga lo siguiente:</p> 
         <ul> 
          <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Escriba la cantidad de tiempo y seleccione una de las unidades de tiempo disponibles en el menú desplegable.</p> </li> </ul>

   <p><strong>SUGERENCIA</strong></p> <p> Al actualizar la Duración de las tareas en una lista de tareas, puede utilizar la abreviatura para la unidad de tiempo. </p>      <p> Puede elegir entre las opciones de tiempo normal o tiempo transcurrido en la siguiente tabla: </p> 
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
            <td>Días. Esta es la opción predeterminada. </td> 
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
         <p><strong>NOTA</strong> </p>
         <p> El tiempo transcurrido es una unidad de tiempo de la duración de una tarea. Es el tiempo entre la Fecha planificada de inicio y la Fecha planificada de finalización de una tarea que incluye días festivos, fines de semana y días libres. En otras palabras, el tiempo transcurrido es el paso de los días del calendario. El tiempo normal tiene en cuenta los días festivos, los fines de semana y los días libres, y los excluye de la duración de la tarea. Para obtener más información acerca de la duración de la tarea, vea <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Información general sobre la duración de la tarea y el tipo de duración</a>. </p> 
         <p> 
         <!--You cannot specify the Duration of a task when the Duration Type of the task is Simple, or when the Task Constraint is Fixed Dates. (NOTE: Anna said this is now possible for all duration types in the Assignments area. It's not here, but to clear confusion, I am drafting this out of here.)--></p> 
        </div> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duración proyectada</td> 
      <td> <p>Diferencia en días entre la fecha proyectada de inicio y la fecha proyectada de finalización. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duración real</td> 
      <td> <p>Diferencia en días entre la fecha real de inicio y la fecha real de finalización. Este es el tiempo que realmente se tardó en completar el trabajo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Horas planificadas</td> 
      <td> <p>Especifique la cantidad de horas planificadas para la tarea, en horas. Es la cantidad de tiempo real que tardarían los usuarios asignados de la tarea en completarla. Sólo puede especificar la cantidad de horas planificadas para una tarea cuando el tipo de duración está establecido en Asignación calculada. Para obtener más información acerca de los tipos de duración, vea <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Información general sobre la duración de la tarea y el tipo de duración</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Horas reales</td> 
      <td>Horas registradas por los usuarios de la tarea. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Esfuerzo de trabajo </td> 
      <td> 
       <div> 
        <p>Cantidad de esfuerzo necesario para completar la tarea. Es posible que el jefe de proyecto decida utilizar este campo en lugar de Horas planificadas para estimar el esfuerzo necesario para completar una tarea. Este campo solo está visible cuando se cumplen las siguientes condiciones:</p> 
        <ul> 
         <li> <p>La tarea tiene un tipo de duración simple. </p> <p>Sugerencia: Si cambia el Tipo de duración de la tarea, este campo se atenúa. </p> </li> 
         <li>El jefe de proyecto ha habilitado el campo Usar esfuerzo de trabajo para calcular automáticamente las horas planificadas para la tarea en el proyecto. </li> 
        </ul> 
        <p>Seleccione entre las siguientes opciones:</p> 
        <ul> 
         <li>Pequeño</li> 
         <li>Medium <span style="font-weight: normal;">(este es el valor predeterminado para una nueva tarea)</span></li> 
         <li>Grande</li> 
        </ul> 
        <p><strong>NOTA</strong></p> 
        <p> Si actualiza la cantidad de esfuerzo, se podrían actualizar las horas planificadas de la tarea. La actualización es inmediata si el tipo de actualización del proyecto es Automática. Cuando el tipo de actualización del proyecto es Manual, debe recalcular la escala de tiempo para ver las horas planificadas actualizadas. </p> 
        <p>Para obtener información sobre cómo usar Esfuerzo de trabajo en lugar de Horas planificadas para estimar el esfuerzo de la tarea, consulte <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Resumen del esfuerzo de trabajo</a>. </p> 
       </div> </td> 
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
      <td role="rowheader">Fecha planificada de inicio</td> 
      <td> <p>Cuando se planea que comience la tarea. La fecha planificada de inicio de una tarea está establecida y afectada por una serie de factores:</p> 
       <ul> 
        <li>Según la preferencia de todo el sistema para la fecha de inicio planeada de la tarea, la fecha de inicio de una nueva tarea en un proyecto puede ser hoy o la fecha de inicio del proyecto de forma predeterminada. <span>El administrador del grupo asociado con el proyecto también puede establecer esta preferencia para el grupo.</span> Para obtener más información acerca de las preferencias de tareas a nivel de sistema o de grupo, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configurar las preferencias de tareas y problemas a nivel de sistema</a>.</li> 
        <li>Según las predecesoras de la tarea, Workfront elige la fecha de comienzo planeada para que sea la siguiente fecha disponible después de que finalicen o comiencen las predecesoras, según la relación de predecesoras. Para obtener más información acerca de las relaciones de predecesoras, vea <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Información general sobre las tareas predecesoras</a>.</li> 
        <li>El jefe de proyecto o el propietario de la tarea pueden establecer manualmente la fecha planificada de inicio cuando la delimitación de la tarea sea Fechas fijas o Debe comenzar el. Para obtener más información acerca de las restricciones de tareas, vea <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Información general sobre la restricción de tareas</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha proyectada de inicio</td> 
      <td> <p>La fecha "real" de cuando la tarea va a comenzar en función del progreso y la finalización de tareas anteriores. Este es un campo calculado y no se puede editar manualmente.</p> <p> La fecha de inicio proyectada y la fecha planificada de inicio son la misma en la que se planifica por primera vez un proyecto. La fecha proyectada de inicio puede alejarse de la fecha planificada de inicio si el proyecto evoluciona y la tarea aún no se ha iniciado. Para obtener más información sobre las fechas de inicio proyectadas, consulte <a href="../../../manage-work/projects/planning-a-project/project-projected-start-date.md" class="MCXref xref">Información general sobre la fecha de inicio proyectada del proyecto</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha real de inicio</td> 
      <td> <p>Especifique una Fecha de inicio real para la tarea. El valor predeterminado suele rellenarse automáticamente al cambiar el estado de la tarea a En curso. El jefe de proyecto o el propietario de la tarea también pueden modificar manualmente la fecha real de inicio. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha planificada de finalización</td> 
      <td> <p>Fecha de finalización anticipada, tal como se muestra cuando se planifica la tarea. La fecha planificada de finalización puede establecerse por varios factores:</p> 
       <ul> 
        <li>La fecha planificada de finalización se calcula a partir de la fecha planificada de inicio añadiendo la duración de la tarea a la fecha planificada de inicio. Cuando el administrador del proyecto o Workfront especifican la duración de la tarea, se déclencheur una actualización a la fecha planificada de finalización. Si la fecha planificada cambia, a menudo se debe a que se ha actualizado la Duración del.</li> 
        <li>El jefe de proyecto o el propietario de la tarea pueden establecer manualmente la fecha planificada de finalización cuando la delimitación de la tarea sea Fechas fijas o Debe finalizar el. Para obtener más información acerca de las restricciones de tareas, vea <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Información general sobre la restricción de tareas</a>.</li> 
        <li>Si el Tipo de duración de la tarea cambia y el número de recursos de las tareas cambia al mismo tiempo, también cambiará la fecha planificada de finalización. Para obtener más información acerca de los tipos de duración, vea <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Información general sobre la duración de la tarea y el tipo de duración</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha proyectada de finalización</td> 
      <td> <p>La fecha "real" de cuando se va a completar la tarea en función del progreso de tareas anteriores y de las actualizaciones de progreso realizadas en la tarea por el usuario asignado. Este es un campo calculado y no se puede editar manualmente.</p> <p> La fecha proyectada de finalización y la fecha planificada de finalización comienzan siendo la misma, cuando se planifica un proyecto por primera vez. La fecha proyectada de finalización puede apartarse de la fecha planificada de finalización si el proyecto evoluciona y la tarea aún no se ha iniciado. Para obtener más información sobre las fechas de finalización proyectadas, vea <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Información general sobre la fecha de finalización proyectada para proyectos, tareas y problemas</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha real de finalización</td> 
      <td> <p>Especifique la fecha y la hora reales en que se completa la tarea. La fecha y hora predeterminadas en las que se completa una tarea siempre coinciden con la hora real en la que el estado se convierte en Completado. El jefe de proyecto o el propietario de la tarea también pueden modificar manualmente la fecha real de finalización. </p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Fecha de confirmación</td> 
      <td> <p>Es la fecha en la que el usuario asignado a la tarea se compromete a completarla. Puede ser diferente a la fecha planificada de finalización. Solo las personas asignadas pueden editar este campo. Para obtener información sobre las fechas de confirmación en Workfront, consulte <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Resumen de la fecha de confirmación</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Fecha de entrada</td> 
      <td>La fecha en la que se creó la tarea.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ingresado por</td> 
      <td>Persona que creó la tarea.</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Fecha de última actualización</td> 
      <td> <p>La fecha en la que se actualizó la tarea por última vez. </p> <p>Sugerencia: Workfront registra una fecha de actualización cada vez que alguien edita y guarda una tarea.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Última actualización por</td> 
      <td> <p>Persona que actualizó la tarea por última vez.</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Frecuencia de periodicidad</td> 
      <td> <p>Esto solo se muestra en el elemento principal de las tareas recurrentes. Es la frecuencia con la que ocurren las tareas en la periodicidad. Para obtener información acerca de la creación de tareas recurrentes, vea <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Crear tareas recurrentes</a>. </p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Duración por resolicitud</td> 
      <td> <p>Esto solo se muestra en el elemento principal de las tareas recurrentes. Muestra la duración de cada tarea recurrente. Para obtener información acerca de la creación de tareas recurrentes, vea <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Crear tareas recurrentes</a>. </p> <p><strong>NOTA</strong></p> <p> Las duraciones modificadas en tareas recurrentes individuales no muestran el valor indicado en este campo. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted, to keep it focused JUST on the Overview section and not others.) </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Custom Forms</strong> to add or forms or edit information on the existing custom forms.&nbsp;</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Expand any of the existing custom forms to edit them, or start typing in the <strong>Add custom form</strong> box in the upper-right corner to add a new form. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about adding or editing custom forms, see the following articles:</p>
   -->

   <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md" class="MCXref xref">Add a custom form to an object</a> </li>   
     -->

   <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md" class="MCXref xref">Manage custom forms attached to objects</a> </li>   
     -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click&nbsp;<strong>Finance</strong>, then <strong>Edit Finance</strong> to view or edit financial information for the task. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Expand the <strong>Finance</strong> area in the Details section, then double-click any editable field to update it. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about editing financial information for a task, see <a href="../../../manage-work/tasks/manage-tasks/task-finances-in-details.md" class="MCXref xref">Manage task finances in the Task Details section</a>. </p>
   -->

1. Haga clic en **Guardar cambios**.
