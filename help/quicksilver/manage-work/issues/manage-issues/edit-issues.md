---
product-area: projects
navigation-topic: manage-issues
title: Editar problemas
description: Puede editar la información sobre los problemas que ha creado o que otros usuarios han creado si han compartido los problemas con usted. Este artículo describe cómo buscar, buscar y editar un problema si tiene los permisos para hacerlo.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 1449374a-ab0d-4c98-83cd-4e511467633a
source-git-commit: 0358e79bd606d0035959bba2a47256456b529b18
workflow-type: tm+mt
source-wordcount: '2532'
ht-degree: 26%

---

# Editar problemas

<!--Audited: 10/2025-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>-->

Puede editar la información sobre los problemas que ha creado o que otros usuarios han creado si han compartido los problemas con usted.

Puede editar un solo problema o editar problemas de una lista. Para obtener información sobre cómo editar problemas en una lista, consulte [Editar problemas en una lista](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <ul><li>Colaborador o superior</li>
   <li>Ligero o superior para editar problemas en la sección Problemas de una tarea o proyecto</li></ul>
   O
   <ul><li>Solicitud o superior</li> <li>Revise o superior para editar problemas en la sección Problemas de una tarea o proyecto</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso</td> 
   <td> <p>Editar acceso a Problemas</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>permisos de contribución para un problema con el fin de editar los siguientes campos en el área de detalles: </p>
   <ul>
   <li>Descripción</li>
   <li>Estado</li>
   <li>Gravedad</li>
   </ul>
   <p>Administre los permisos de un problema para editar todos los campos del área de Detalles o del cuadro Editar problema</p> <p> Para obtener información sobre la concesión de permisos a los problemas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema </a></p> <p>Para obtener información sobre cómo solicitar permisos adicionales, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New license:</p>
   <ul><li>Contributor or higher</li>
   <li>Light or higher to edit issues in the Issues section of a task or project</li></ul>
   <p>Current license:</p>
  <ul><li>Request or higher</li> <li>Review or higher to edit issues in the Issues section of a task or a project</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Issues</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to an issue to edit the following fields in the Details area: </p>
   <ul>
   <li>Description</li>
   <li>Status</li>
   <li>Severity</li>
   </ul>
   <p>Manage permissions to an issue to edit all the fields in the Details area or in the Edit Issue box</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a></p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Limitaciones al editar problemas

Existen algunas limitaciones que podrían impedir la edición de problemas.

* No puede editar problemas que se encuentren en un proceso de aprobación. Solo puede registrar el tiempo o actualizar el estado de un problema que esté en Aprobación pendiente.
* Solo puede editar y agregar documentos a problemas de un proyecto que tenga el estado Completo, Inactivo o Pendiente de aprobación cuando el administrador de Workfront o un administrador de grupo hayan habilitado esta funcionalidad en el área Preferencias del proyecto. Para obtener información sobre cómo establecer las preferencias del proyecto, consulte [Configurar las preferencias de proyecto en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Editar un solo problema

Puede editar un problema mediante las áreas Editar problema o Detalles del problema. Los siguientes pasos describen la edición de un problema en el cuadro Editar problema.

1. Vaya al **Menú principal**.
1. Haga clic en **Proyectos** y, a continuación, haga clic en el nombre de un proyecto para abrirlo.
1. (Opcional) Haga clic en **Tareas** y, a continuación, haga clic en el nombre de una tarea para abrirla.
1. Haga clic en **Problemas** en el panel izquierdo.

   ![Icono de problemas](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. (Opcional) Para editar información limitada sobre un problema, haga clic en **Detalles del problema** en el panel izquierdo.

   >[!NOTE]
   >
   >Según la forma en la que el administrador de Workfront o del grupo haya modificado la plantilla de diseño, los campos del área Detalles del problema podrían volver a organizarse o no mostrarse. Para obtener más información, consulte [Personalizar la vista de detalles con una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Para editar la información de la sección Detalles, haga lo siguiente:

   1. (Opcional) Haga clic en el icono **Contraer todo** en la esquina superior derecha para contraer todas las áreas.
   1. (Opcional y condicional) Cuando un área esté contraída, haga clic en la **flecha que señala a la derecha** ![flecha que señala a la derecha](assets/right-pointing-arrow.png) junto a cada área para expandir el área que desea editar.
   1. (Opcional) Para adjuntar un formulario personalizado, empiece a escribir el nombre de un formulario en el campo **Añadir formulario personalizado**, selecciónelo cuando se muestre en la lista y, a continuación, haga clic en **Guardar cambios**.
   1. (Opcional) Haga clic en el icono **Exportar** ![Icono de exportar](assets/export.png) para exportar la información general y de los formularios personalizados a un archivo de PDF y, a continuación, haga clic en **Exportar**. Seleccione entre las siguientes opciones:

      * Seleccionar todo (solo se muestra cuando hay al menos un formulario personalizado adjunto)
      * Información general
      * El nombre de uno o varios formularios personalizados

      El archivo PDF se descarga en el equipo.

      ![Detalles del problema de exportación](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      Para obtener más información, consulte [Exportar formularios personalizados y detalles de objetos](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

   Para obtener información sobre los campos visibles en la sección Detalles del problema, continúe editando el problema en el cuadro Editar problema como se describe a continuación.

1. Para editar toda la información sobre un problema, selecciona un problema en una lista y luego haz clic en **Editar** en la parte superior de la lista

   O

   Haga clic en el nombre de un problema en una lista, luego haga clic en el menú **Más** junto al nombre del problema y, a continuación, **Editar.**

   Se muestra el cuadro de diálogo **Editar problema**.

   >[!IMPORTANT]
   >
   >Debe tener permisos de administración para ver el vínculo Editar.

   Todos los campos de problema están disponibles en el cuadro Editar problema y se agrupan por las áreas enumeradas en el panel izquierdo.

1. Considere la posibilidad de especificar información en cualquiera de las siguientes secciones:

   * [Nombre del problema](#issue-name)
   * [Información general](#overview)
   * [Asignaciones](#assignments)
   * [Formularios personalizados](#Custom%C2%A0F)
   * [Configuración](#settings)

   >[!NOTE]
   >
   >Según la forma en que el administrador de Workfront configure la plantilla de diseño, los campos del cuadro Editar problema podrían ser diferentes en su entorno. Para obtener más información, consulte [Personalizar la vista de detalles con una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).
   >
   >La mayoría de los campos enumerados en las secciones siguientes también están accesibles desde el cuadro Nuevo problema al crear un problema. Las secciones en las que se encuentran los campos no coinciden con el cuadro Nuevo problema. Para obtener información sobre cómo crear problemas, consulte [Crear problemas](../../issues/manage-issues/create-issues.md).

### Nombre del problema {#issue-name}

1. Comience a editar un problema como se ha descrito anteriormente.
1. Haga clic en **Nombre de problema**.

   ![Sección de nombre de problema](assets/issue-name-section-edit-issue-box-nwe-350x127.png)

1. Actualice el campo **Nombre del problema**.
1. Haga clic en **Guardar** o continúe editando las secciones siguientes.

### Información general {#overview}

1. Comience a editar un problema como se ha descrito anteriormente.
1. Haga clic en **Información general**.

   ![Sección de información general del problema](assets/overview-section-edit-issue-box-nwe-350x284.png)

1. Actualice o revise cualquiera de los campos de la siguiente tabla:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td> <p>Añada información adicional sobre el problema.</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">Estado</td> 
      <td> <p>Seleccione el estado del problema. Para obtener más información sobre los estados de problemas, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Acceso a la lista de estados de problemas del sistema</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prioridad</td> 
      <td> <p>Este es un indicador visual para usted que le permite priorizar problemas.</p> <p>Seleccione entre las siguientes opciones:</p> 
       <ul> 
        <li> <p><strong>Ninguno</strong> </p> </li> 
        <li> <p><strong>Bajo</strong> </p> </li> 
        <li> <p><strong>Normal</strong> </p> </li> 
        <li> <p><strong>Alto</strong> </p> </li> 
        <li> <p><strong>Urgente</strong> </p> </li> 
       </ul> <p>Según las Preferencias del proyecto seleccionadas por el administrador de Workfront, los nombres de las prioridades pueden ser diferentes para usted. Para obtener más información acerca de cómo editar prioridades, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Crear y personalizar prioridades</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gravedad</td> 
      <td> <p>Este es un indicador visual para usted que indica la gravedad del problema descrito en el problema. Las gravedades son específicas de los problemas. Seleccione entre las siguientes opciones:</p> 
       <ul> 
        <li> <p style="font-weight: bold;">Cosmético</p> </li> 
        <li> <p style="font-weight: bold;">Causa confusión</p> </li> 
        <li> <p style="font-weight: bold;">Error con solución</p> </li> 
        <li> <p style="font-weight: bold;">Error sin solución</p> </li> 
        <li> <p style="font-weight: bold;">Error fatal</p> </li> 
       </ul> <p>Según las Preferencias del proyecto seleccionadas por el administrador de Workfront, los nombres de las gravedades podrían ser diferentes para usted. Para obtener más información sobre cómo editar gravedades, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md" class="MCXref xref">Crear o personalizar gravedades de problemas</a>.</p> </td> 
     </tr>

   <tr> 
   <td role="rowheader">Condición del problema</td> 
   <td> <p>La condición de un problema es un indicador que se coloca para indicar cómo va.</p> 
   <p>Puede establecer la condición de una tarea o un problema de forma automática o manual.</p>
   <p>Debe estar asignado al problema para cambiar su condición.</p>
   <p>Seleccione entre las siguientes opciones:</p> 
      <ul> 
   <li> <p style="font-weight: bold;">Sin problemas</p> </li> 
   <li> <p style="font-weight: bold;">Algunas preocupaciones</p> </li> 
   <li> <p style="font-weight: bold;">Impedimentos mayores</p> </li> 
   </ul> </td> 
     </tr>

   <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>Escriba un vínculo web relacionado con la información sobre el problema.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo</td> 
      <td> <p>Según las Propiedades de la cola seleccionadas por el jefe de proyecto en el área Detalles de la cola del proyecto, es posible que pueda especificar el tipo de problema. Seleccione entre las siguientes opciones del menú desplegable <b>Tipo</b>: </p> 
       <ul> 
        <li> <p><strong>Informe de errores</strong> </p> </li> 
        <li> <p><strong>Solicitud de cambio</strong> </p> </li> 
        <li> <p><strong>Problema</strong> </p> </li> 
        <li> <p><strong>Solicitud</strong> </p> </li> 
       </ul> <p>Según las Preferencias del proyecto seleccionadas por el administrador de Workfront, los nombres de los tipos de problemas pueden ser diferentes para usted.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Contacto primario</td> 
      <td>De forma predeterminada, el autor del problema es el contacto principal. Para modificar esto, empiece a escribir el nombre de cualquier usuario activo en Workfront y, a continuación, selecciónelo en la lista. Un problema solo puede tener un contacto principal.<br> Si cambia el Contacto principal, el contacto principal original seguirá teniendo acceso de administración al problema. Cuando comparta un problema, debe quitar manualmente este acceso del cuadro Acceso a problemas.

   <b>SUGERENCIA</b>

   <p>Al agregar un usuario de Contacto principal, observe el avatar, la función principal del usuario y su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos. Los usuarios deben estar asociados con al menos una función para verla a medida que los añade.</p>
      <p> Debe tener habilitada la configuración Ver información de contacto en su nivel de acceso para que los usuarios vean los correos electrónicos de los usuarios. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md">Conceder acceso a usuarios</a>.</p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha y hora de confirmación</td> 
      <td> <p>Es la fecha en la que el usuario asignado del problema calcula que se resolverá el problema. Solo las personas asignadas pueden editar este campo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha de inicio planificada</td> 
      <td>De forma predeterminada, la Fecha planificada de inicio es la fecha y la hora en que se creó el problema. Puede actualizar la <strong>fecha planificada de inicio</strong> del problema. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha y hora planificadas de finalización</td> 
      <td> De forma predeterminada, la Fecha planificada de finalización es 24 horas desde la Fecha planificada de inicio predeterminada. De forma predeterminada, los problemas tienen una duración de 1 día. Puede actualizar la <strong>fecha planificada de finalización</strong> del problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha y hora de inicio reales</td> 
      <td>La fecha real de inicio se rellena automáticamente cuando cambia el estado del problema a <strong>En curso</strong>. Puede actualizar la <strong>fecha real de inicio</strong> del problema. Si es necesario, puede actualizar la fecha manualmente. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha y hora reales de finalización</td> 
      <td>La fecha real de finalización se completa automáticamente cuando cambia el estado del problema a <strong>Cerrado</strong> o<strong>Resuelto</strong>. Puede actualizar la <strong>fecha real de finalización</strong> del problema. Si es necesario, puede actualizar la fecha manualmente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resuelto por</td> 
      <td> <p>Esto muestra si el problema se resuelve mediante otro objeto. Puede seleccionar si este problema se resuelve mediante una tarea, un proyecto u otro problema en el menú desplegable y, a continuación, empezar a escribir el nombre de la tarea, el proyecto o el problema que resolverá el problema. Selecciónelo cuando aparezca en la lista.</p>

   <b>NOTAS</b>

   <ul><li>Cuando selecciona un objeto para resolver un problema, el estado del problema está vinculado al estado del objeto de resolución y no se puede cambiar en el problema. Para obtener más información acerca de la resolución de objetos, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Información general sobre resolución de objetos y objetos solucionables </a>.</li>

   <li>Cuando conecta un problema para que lo resuelva otra tarea, problema o proyecto, ninguna información del problema se transfiere al objeto de resolución (la tarea, problema o proyecto enumerados en el campo Resuelto por ). </li>

   <li>Cuando el administrador del sistema o del grupo agrega el campo "Resuelto por" a un encabezado personalizado de problema, el campo cambia a "Resolviendo problema", "Resolviendo tarea" o "Resolviendo proyecto" cuando hay un objeto de resolución asociado con el problema.

   No puede editar este campo cuando se muestra en el encabezado de problema. Para obtener más información acerca de cómo personalizar encabezados de problema, vea <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md">Personalizar encabezados de objeto mediante una plantilla de diseño </a></li></ul>
   </td> 
     </tr>

   <tr> 
      <td role="rowheader">Resolver problemas, resolver tareas o resolver proyectos</td> 
      <td>El nombre vinculado del problema, la tarea o el problema que resuelve el problema.  </td> 
     </tr> 
      <tr> 
      <td role="rowheader">Esto resuelve</td> 
      <td>El nombre vinculado del problema que se resuelve cuando se resuelve el problema al que accede.  </td> 
     </tr> 
    </tbody> 
   </table>


1. Haga clic en **Guardar** o continúe editando las secciones siguientes.

#### Asignaciones {#assignments}

1. Empiece a editar el problema como se ha descrito anteriormente.
1. Haga clic en **Asignaciones** en el panel izquierdo.

   ![Sección de asignaciones de problemas](assets/assignments-section-edit-issue-box-nwe-350x230.png)

1. Haga clic en **Buscar personas, roles y equipos** y empiece a escribir el nombre del usuario, rol o equipo que desee asignar al problema; a continuación, haga clic en él o presione Entrar cuando aparezca en la lista.

   <!--
   (NOTE: ensure this is still called this; asked Anna to change it to "roles" and add a comma)
   -->

   >[!NOTE]
   >
   >Si el nombre del usuario contiene un carácter especial, debe incluirlo en el campo de búsqueda.

   Puede asignar varios usuarios, funciones o equipos. Solo puede asignar usuarios, funciones y equipos activos.

   >[!TIP]
   >
   >
   >Si un usuario, un rol o un equipo se han asignado antes de que se desactiven, permanecerán asignados al elemento de trabajo. En este caso, se recomienda lo siguiente:
   >
   >* Reasignar el elemento de trabajo a los recursos activos.
   >* Asocie los usuarios de un equipo desactivado a un equipo activo y reasigne el elemento de trabajo al equipo activo.

   <!--1. In the Production environment:
         1. Indicate whether an assignee is the primary assignee on the issue, by hovering over the name of the assignee and clicking **Make Primary**. A team cannot be the primary assignee of an issue.
         1. Update the following fields: 
         <table style="table-layout:auto"> 
         <col> 
         </col> 
         <col> 
         </col> 
         <tbody> 
         <tr> 
            <td role="rowheader">Planned Hours</td> 
            <td> <p>This is the amount of actual time it would take the assignees of the issue to complete it. Type the number of Planned Hours for the issue.<br></p> <p><b>NOTE</b></p>  <p>Changing the Planned Hours of the issue will not change the issue Planned Completion Date. </p> </td> 
         </tr> 
         <tr data-mc-conditions=""> 
            <td role="rowheader">Assignee's Role</td> 
            <td> <p>Select a role from the <strong>Assignee's Role</strong> drop-down menu when you selected a person as an assignee. This is the role that the assignee can fulfill on this issue. </p> <p><b>TIP</b>
            
            Only the job roles associated with each assignee in their profile appear in the drop-down menu.</p> </td> 
         </tr> 
         </tbody> 
         </table>-->


1. (Opcional) Haga clic en **Asignármelo** para asignarse el problema a sí mismo.
1. (Opcional) Actualice el campo **Horas planificadas**.

   Las **horas planificadas** son la cantidad de horas que los usuarios asignados del problema necesitarían para completarlo.

   >[!NOTE]
   >
   >Al cambiar las horas planificadas del problema, no se cambiará la fecha planificada de finalización del problema.

1. Para quitar asignaciones de todos los problemas, consulte [Asignar problemas](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md).

1. Haga clic en **Guardar** o continúe editando las secciones siguientes.

### Formularios personalizados

1. Comience a editar un problema como se ha descrito anteriormente.
1. Haga clic en **Formularios personalizados**.

   ![Sección de formularios personalizados de problema](assets/custom-forms-section-edit-issue-box-nwe-350x132.png)

1. En el campo **Agregar formulario personalizado**, seleccione el formulario o formularios personalizados que desee asociar con el problema. Debe generar los formularios personalizados antes de que estén disponibles para seleccionarlos en este campo. En la lista solo se muestran los formularios personalizados activos. Para obtener más información sobre la creación de formularios personalizados, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). Puede agregar hasta diez formularios personalizados a un problema.

1. (Condicional) Si adjuntó un formulario personalizado al problema, edite los campos del formulario. Debe especificar todos los campos obligatorios antes de guardar el problema.

   >[!NOTE]
   >
   >Según la forma en que el administrador de Workfront haya establecido los permisos para las secciones del formulario personalizado, no todos podrán ver o editar los mismos campos en un formulario personalizado determinado. Los permisos para editar campos dentro de una sección de un formulario personalizado dependen de los permisos que tenga sobre el propio problema. Para obtener información sobre cómo establecer permisos en secciones de un formulario personalizado, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). Para obtener información sobre cómo establecer permisos para problemas, consulte [Compartir un problema](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

1. Haga clic en **Guardar** o continúe editando la siguiente sección.

### Configuración {#settings}

1. Comience a editar un problema como se ha descrito anteriormente.
1. Haga clic en **Configuración**.

   ![Icono de configuración de problema](assets/settings-section-edit-issue-box-nwe-350x240.png)

   Actualice la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Proceso de aprobación</td> 
      <td> 
       <div> 
       <p>Seleccione un proceso de aprobación que desee asociar con el problema. El administrador de Workfront debe definir los procesos de aprobación en el nivel de sistema para poder asociarlos a problemas. Los usuarios con acceso administrativo a los procesos de aprobación <span> también pueden crear procesos de aprobación específicos del grupo.</span>Para obtener más información acerca de cómo crear procesos de aprobación, vea <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Crear un proceso de aprobación para elementos de trabajo</a>. </p> 
       <p>Tenga en cuenta lo siguiente a la hora de añadir procesos de aprobación: </p> 
       <ul> 
       <li>En la lista solo se muestran los procesos de aprobación activos. </li> 
       <li> <p>Los procesos de aprobación de todo el sistema y específicos del grupo se muestran en la lista. Un proceso de aprobación asociado a un grupo que no sea el del proyecto no se muestra en la lista.</p> <p>Importante: Si el grupo del proyecto cambia, el proceso de aprobación específico del grupo se convierte en un proceso de aprobación de un solo uso. Para obtener más información acerca de cómo afectan los cambios en el grupo del proyecto o los cambios en el proceso de aprobación a la configuración de aprobación, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Cómo afectan los cambios en el grupo y el proceso de aprobación a los procesos de aprobación asignados</a>. </p> </li> 
       <li> <p>Puede definir los procesos de aprobación predeterminados que se adjuntarán automáticamente a los problemas al crear colas de solicitudes o temas de colas. Para obtener información acerca de cómo actualizar los detalles de cola, vea <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Crear una cola de solicitudes</a>. Para obtener información acerca de cómo crear temas de colas, vea <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Crear temas de colas</a>. </p> </li> 
       <li>Cuando se producen problemas de edición masiva, existen los siguientes escenarios: 
       <ul> 
       <li><p>Cuando se seleccionan varios problemas del mismo grupo, en este campo se muestran tanto los procesos de aprobación de nivel de sistema como los específicos del grupo.</p></li> 
       <li><p>Cuando se seleccionan varios problemas de diferentes grupos, solo se muestran en este campo los procesos de aprobación de nivel de sistema.</p></li> 
       <li><p>Cuando alguno de los problemas tiene un proceso de aprobación de un solo uso adjunto, se reemplaza por el proceso de aprobación de nivel de sistema o de grupo que seleccione. </p></li> 
       </ul></li> 
       </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificaciones de recordatorio</td> 
      <td> <p>Seleccione la casilla de verificación para la que desea adjuntar notificaciones de recordatorio a este problema. Se muestran todas las notificaciones de recordatorio de problemas. El administrador de Workfront debe configurar las notificaciones de recordatorio antes de poder seleccionarlas en caso de problemas. Para obtener más información acerca de cómo configurar notificaciones de recordatorio, consulte <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configurar notificaciones de recordatorio</a></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.

## Editar un problema en el encabezado del mismo (lim.)

Puede editar una cantidad limitada de información en el encabezado del problema.

El administrador del sistema o del grupo puede personalizar los campos que ve en el encabezado del problema. Para obtener más información, consulte [Personalizar encabezados de objeto mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

![Encabezado del problema](assets/issue-header-350x19.png)

Los siguientes campos se incluyen en el encabezado de problema de forma predeterminada:

* Nombre del problema
* Porcentaje completado

  Para obtener más información, consulte [Ver y actualizar el porcentaje completado de las tareas](/help/quicksilver/manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).
* Asignaciones
* Fecha y hora planificadas de finalización
* Estado
* Tomar decisiones de aprobación si se establece como aprobador en un proceso de aprobación actual
