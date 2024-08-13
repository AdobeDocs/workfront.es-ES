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
source-git-commit: f3641e2207563f3fc9d9ed059d889ab6c22f05b1
workflow-type: tm+mt
source-wordcount: '2529'
ht-degree: 2%

---

# Editar problemas

Puede editar la información sobre los problemas que ha creado o que otros usuarios han creado si han compartido los problemas con usted.

Puede editar un solo problema o editar problemas de una lista. Para obtener información sobre cómo editar problemas en una lista, consulte [Editar problemas en una lista](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> <p>Revise o consiga una licencia superior para editar problemas en la sección Problemas de una tarea o proyecto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre el acceso a los problemas de su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Conceder acceso a los problemas</a>. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de Contribute para resolver un problema con el fin de editar los siguientes campos en el área Detalles: </p>
   <ul>
   <li>Descripción</li>
   <li>Estado</li>
   <li>Gravedad</li>
   </ul>
   <p>Administre los permisos de un problema para editar todos los campos del área de Detalles o del cuadro Editar problema</p> <p> Para obtener información sobre la concesión de permisos a los problemas, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema </a></p> <p>Para obtener información sobre cómo solicitar permisos adicionales, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Limitaciones al editar problemas

Existen algunas limitaciones que podrían impedir la edición de problemas.

* No puede editar problemas que se encuentren en un proceso de aprobación. Solo puede registrar el tiempo o actualizar el estado de un problema que esté en Aprobación pendiente.
* Solo puede editar y agregar documentos a problemas de un proyecto que tenga el estado Completo, Inactivo o Pendiente de aprobación cuando el administrador de Workfront o un administrador de grupo hayan habilitado esta funcionalidad en el área Preferencias del proyecto. Para obtener información sobre cómo establecer las preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Editar un solo problema

Puede editar un problema mediante las áreas Editar problema o Detalles del problema. Los siguientes pasos describen la edición de un problema en el cuadro Editar problema.

1. Ir al **Menú principal**.
1. Haga clic en **Proyectos** y, a continuación, haga clic en el nombre de un proyecto para abrirlo.
1. (Opcional) Haga clic en **Tareas** y, a continuación, haga clic en el nombre de una tarea para abrirla.
1. Haga clic en **Problemas** en el panel izquierdo.

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. (Opcional) Para editar información limitada sobre un problema, haga clic en **Detalles del problema** en el panel izquierdo.

   >[!NOTE]
   >
   >Según la forma en la que el administrador de Workfront o del grupo haya modificado la plantilla de diseño, los campos del área Detalles del problema podrían volver a organizarse o no mostrarse. Para obtener más información, consulte [Personalizar la vista de detalles con una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Para editar la información de la sección Detalles, haga lo siguiente:

   1. (Opcional) Haga clic en el icono **Contraer todo** de la esquina superior derecha para contraer todas las áreas.
   1. (Opcional y condicional) Cuando un área esté contraída, haga clic en la **flecha que señala a la derecha** ![](assets/right-pointing-arrow.png) junto a cada área para expandir el área que desea editar.
   1. (Opcional) Para adjuntar un formulario personalizado, empiece a escribir el nombre de un formulario en el campo **Agregar formulario personalizado**, selecciónelo cuando se muestre en la lista y, a continuación, haga clic en **Guardar cambios**.
   1. (Opcional) Haga clic en el icono **Exportar** ![](assets/export.png) para exportar la información general y de los formularios personalizados a un archivo de PDF y, a continuación, haga clic en **Exportar**. Seleccione una de las siguientes opciones:

      * Seleccionar todo (solo se muestra cuando hay al menos un formulario personalizado adjunto)
      * Información general
      * El nombre de uno o varios formularios personalizados

      El archivo del PDF se descarga en el equipo.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

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

   ![](assets/issue-name-section-edit-issue-box-nwe-350x127.png)

1. Actualice el campo **Nombre del problema**.
1. Haga clic en **Guardar** o continúe editando las secciones siguientes.

### Información general {#overview}

1. Comience a editar un problema como se ha descrito anteriormente.
1. Haga clic en **Información general**.

   ![](assets/overview-section-edit-issue-box-nwe-350x284.png)

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
      <td colspan="2" role="rowheader">Sección de información básica</td> 
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
        <li> <p><strong>Baja</strong> </p> </li> 
        <li> <p><strong>Normal</strong> </p> </li> 
        <li> <p><strong>Alta</strong> </p> </li> 
        <li> <p><strong>Urgente</strong> </p> </li> 
       </ul> <p>Según las Preferencias del proyecto seleccionadas por el administrador de Workfront, los nombres de las prioridades pueden ser diferentes para usted. Para obtener más información acerca de cómo editar prioridades, vea <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Crear y personalizar prioridades</a>.</p> </td> 
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

   <p>Al agregar un usuario de Contacto principal, observe el avatar, la función principal del usuario y su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos. Los usuarios deben estar asociados con al menos un rol para verlo a medida que los agregue.</p>
      <p> Debe tener activada la configuración Ver información de contacto en su nivel de acceso para que los usuarios vean los correos electrónicos de los usuarios. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md">Conceder acceso a usuarios</a>.</p>


   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Confirmar fecha y hora</td> 
      <td> <p>Es la fecha en la que el usuario asignado del problema calcula que se resolverá el problema. Solo las personas asignadas pueden editar este campo.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha planificada de inicio</td> 
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

   <b>NOTA</b>

   Cuando selecciona un objeto para resolver un problema, el estado del problema está vinculado al estado del objeto de resolución y no se puede cambiar en el problema. Para obtener más información acerca de la resolución de objetos, vea <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Información general sobre la resolución y los objetos solucionables </a>.

   <b>SUGERENCIA</b>

   Cuando el administrador del sistema o del grupo agrega el campo &quot;Resuelto por&quot; a un encabezado personalizado de problema, el campo cambia a &quot;Resolviendo problema&quot;, &quot;Resolviendo tarea&quot; o &quot;Resolviendo proyecto&quot; cuando hay un objeto de resolución asociado con el problema.

   No puede editar este campo cuando se muestra en el encabezado de problema. Para obtener más información acerca de cómo personalizar encabezados de problema, vea <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md">Personalizar encabezados de objeto mediante una plantilla de diseño </a>
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

   ![](assets/assignments-section-edit-issue-box-nwe-350x230.png)

1. Haga clic en **Buscar personas, roles y equipos** y empiece a escribir el nombre del usuario, rol o equipo que desee asignar a la tarea; a continuación, haga clic en él o presione Entrar cuando aparezca en la lista.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this is still called this; asked Anna to change it to "roles" and add a comma)</p>
   -->

   >[!NOTE]
   >
   >Si el nombre del usuario contiene un carácter especial, debe incluirlo en el campo de búsqueda.

   >[!TIP]
   >
   >Puede asignar varios usuarios, roles o equipos. Solo puede asignar usuarios activos, roles y equipos.
   >
   >
   >Si un usuario, un rol o un equipo se han asignado antes de que se desactiven, permanecerán asignados al elemento de trabajo. En este caso, se recomienda lo siguiente:
   >
   >* Reasignar el elemento de trabajo a los recursos activos.
   >* Asocie los usuarios de un equipo desactivado a un equipo activo y reasigne el elemento de trabajo al equipo activo.

1. (Opcional) Indique si un usuario asignado es el principal asignado al problema; para ello, pase el ratón sobre el nombre del usuario asignado y haga clic en **Convertir en principal**. Un equipo no puede ser el principal asignado a un problema.
1. Actualice los campos siguientes:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Horas planificadas</td> 
      <td> <p>Es la cantidad de tiempo real que tardarían los usuarios asignados del problema en completarlo. Escriba el número de horas planificadas para el problema.<br></p> <p>Nota: Si cambia las horas planificadas del problema, no se cambiará la fecha planificada de finalización del problema. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Rol de asignado</td> 
      <td> <p>Seleccione un rol del menú desplegable <strong>Rol de asignado</strong> cuando haya seleccionado una persona como asignado. Esta es la función que el usuario asignado puede desempeñar en este problema. </p> <p><b>SUGERENCIA</b>

   En el menú desplegable solo aparecen los roles asociados con cada usuario asignado en su perfil.</p> </td>
   </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar** o continúe editando las secciones siguientes.

### Forms personalizado

1. Comience a editar un problema como se ha descrito anteriormente.
1. Haga clic en **Forms personalizado**.

   ![](assets/custom-forms-section-edit-issue-box-nwe-350x132.png)

1. En el campo **Agregar formulario personalizado**, seleccione el formulario o formularios personalizados que desee asociar con el problema. Debe crear los formularios personalizados antes de que estén disponibles para seleccionarlos en este campo. En la lista solo se muestran los formularios personalizados activos. Para obtener más información acerca de cómo crear formularios personalizados, vea [Diseñar un formulario con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). Puede agregar hasta diez formularios personalizados a un problema.

1. (Condicional) Si adjuntó un formulario personalizado al problema, edite los campos del formulario. Debe especificar todos los campos obligatorios antes de guardar el problema.

   >[!NOTE]
   >
   >Según la forma en que el administrador de Workfront haya establecido los permisos para las secciones del formulario personalizado, no todos podrán ver o editar los mismos campos en un formulario personalizado determinado. Los permisos para editar campos dentro de una sección de un formulario personalizado dependen de los permisos que tenga sobre el propio problema. Para obtener información acerca de cómo establecer permisos en secciones de un formulario personalizado, vea [Diseñar un formulario con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). Para obtener información sobre cómo establecer permisos para problemas, consulte [Compartir un problema](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

1. Haga clic en **Guardar** o continúe editando la siguiente sección.

### Configuración {#settings}

1. Comience a editar un problema como se ha descrito anteriormente.
1. Haga clic en **Configuración**.

   ![](assets/settings-section-edit-issue-box-nwe-350x240.png)

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
       <p>Tenga en cuenta lo siguiente al añadir procesos de aprobación: </p> 
       <ul> 
       <li>En la lista solo se muestran los procesos de aprobación activos. </li> 
       <li> <p>Los procesos de aprobación de todo el sistema y específicos del grupo se muestran en la lista. Un proceso de aprobación asociado a un grupo que no sea el del proyecto no se muestra en la lista.</p> <p>Importante: Si el grupo del proyecto cambia, el proceso de aprobación específico del grupo se convierte en un proceso de aprobación de un solo uso. Para obtener más información acerca de cómo afectan los cambios en el grupo del proyecto o los cambios en el proceso de aprobación a la configuración de aprobación, vea <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Cómo afectan los cambios en el grupo y el proceso de aprobación a los procesos de aprobación asignados</a>. </p> </li> 
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

1. Haga clic en **Guardar.**

## Editar un problema en el encabezado del mismo (lim.)

Puede editar una cantidad limitada de información en el encabezado del problema.

El administrador del sistema o del grupo puede personalizar los campos que ve en el encabezado del problema. Para obtener más información, vea [Personalizar encabezados de objeto mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

![](assets/issue-header-350x19.png)

Los siguientes campos se incluyen en el encabezado de problema de forma predeterminada:

* Nombre del problema
* Porcentaje completado
* Asignaciones
* Fecha y hora planificadas de finalización
* Estado
* Tome decisiones de aprobación si se establece como aprobador en un proceso de aprobación actual
