---
product-area: projects
navigation-topic: manage-issues
title: Ver problemas
description: Puede ver los problemas asociados a un proyecto, tarea o iteración.
author: Alina
feature: Work Management
exl-id: b6791c8f-b356-4235-8b0e-952e29a88952
source-git-commit: dc4b6dc284c59281206a457395765e634067ba91
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 95%

---

# Ver problemas

<!--Audited: 10/2025-->

Puede ver los problemas asociados a un proyecto, tarea o iteración.

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
   <td> 
   <ul><li><p>Colaborador o superior</p></li> <li><p>Licencia básica o superior para ver problemas en la sección Problemas de un proyecto.</p></li>

O

<ul><li><p>Solicitud o superior</p></li> <li><p>Revise la licencia o una superior para ver los problemas en la sección Problemas de un proyecto.</p></li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Ver acceso a Problemas</p> <p>Acceso de visualización o superior a proyectos y tareas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de Vista para el problema</p> </td> 
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
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> <p>Review or higher license to view issues in the Issues section of a project.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Issues</p> <p>View or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to issues in your Access Level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the issue</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a></p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

## Ver problemas según el estado

Para ver los problemas de un proyecto, tarea o iteración:

1. Abra un proyecto, tarea o iteración que contenga problemas y haga clic en **Problemas** en el panel izquierdo.

1. Para mostrar todos los problemas, los problemas abiertos o los problemas cerrados, haz clic en cualquiera de los filtros que aparecen a continuación en el menú desplegable **Filtro**.

>[!TIP]
>
>La lista de filtros varía según lo que haya seleccionado el administrador del sistema o del grupo para mostrarla.

* **Abierto:** muestra los problemas que están abiertos.

  Esto incluye los asociados a un objeto de resolución y los que están en estado Cerrado - Pendiente de aprobación.

  Para obtener información acerca de la resolución de objetos, consulte [Información general sobre la resolución y los objetos solucionables](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

* **Completado:** muestra todos los problemas que tienen una fecha real de finalización.
* **Todos** muestra todos los problemas.

## Comprensión de la información sobre problemas

Puede ver información sobre un problema al acceder a él.

Para acceder a un problema y ver información sobre él:

1. Abra un proyecto, tarea o iteración que contenga problemas y haga clic en **Problemas** en el panel izquierdo.
1. En el menú desplegable **Filtro**, seleccione el filtro para mostrar los problemas que está intentando ver.

   Seleccione entre las siguientes opciones:

   * Abrir
   * Finalizado
   * Todas

1. Haga clic en el nombre de un problema.

   Cuando tenga permisos de administración sobre el problema, podrá editar cualquier campo editable del mismo y añadir aprobaciones, horas o documentos al problema.

1. En el panel izquierdo, haga clic en cualquiera de las siguientes opciones para ver más información sobre el problema:

* **Actualizaciones**: puede realizar las siguientes acciones:

   * Comentar el problema o responder a un comentario existente.
   * Registrar tiempo.
   * Cambiar el estado del problema.

     Para obtener más información sobre cómo actualizar el trabajo en Workfront, consulte [Actualizar trabajo](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* **Documentos**: adjunte documentos al problema. Para obtener más información sobre la adición de documentos a Workfront, consulte [Añadir documentos a Adobe Workfront desde el sistema de archivos](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

* **Detalles del problema**: expanda este vínculo para mostrar las áreas de **Información general** y **Formularios personalizados**.

  Si tiene permisos de administración del problema y derechos de edición en el formulario personalizado, puede editar parte de la información aquí.

  Vea o edite los campos siguientes en el área **Información general**:

   * **Nombre**
   * **Ruta**: la ruta a través de la cual se registró el problema en el proyecto.

     Si un problema se envió como solicitud en una cola de solicitudes, los nombres del proyecto, el grupo de temas y el tema de la cola se enumeran aquí. Este campo no se puede editar.

     Para obtener más información sobre el envío de solicitudes, consulte [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

   * **Descripción**
   * **URL**: cualquier dirección web relacionada con el problema.
   * **Prioridad**: un indicador visual que le permite priorizar los problemas.
   * **Gravedad**: un indicador visual que indica la gravedad del problema que se describe en el problema.
   * **Contacto principal**: el contacto principal predeterminado es el usuario que creó el problema. Este campo se puede editar.
   * **Horas planificadas**: muestra la cantidad de tiempo que tardará una persona en completar el problema. El valor predeterminado es de 8 horas. Este campo se puede editar.
   * **Horas reales**: muestra la cantidad de tiempo que se tardó en completar el problema. Es el tiempo real que alguien registra para el problema.
   * **Fecha planificada de inicio**: la fecha de inicio de la planficación del problema. El valor predeterminado es la fecha y la hora de creación del problema.
   * **Fecha de inicio real**: la fecha y la hora en que se cambió el estado del problema a En curso.
   * **Fecha planificada de finalización**: la fecha planificada de finalización del problema.
   * **Fecha de finalización real**: la fecha en la que se resuelve el problema. Este campo se rellena automáticamente cuando el estado del problema cambia a Cerrado o Resuelto, o se puede editar manualmente.
   * **Coste real**: el coste basado en las horas reales registradas en el problema. Este campo no se puede editar. El coste real de un problema se calcula según la fórmula siguiente, donde la Tarifa de coste de usuario es la tarifa de coste asociada al registro del usuario en el momento del problema:

     Coste real del problema = Horas registradas * Tarifa de coste de usuario

   * **Introducido por**: es el usuario que creó el problema. Este campo no se puede editar.
   * **Última actualización por**: es el usuario que actualizó por última vez cualquier campo del problema. Este campo no se puede editar.

     En el área **Formularios personalizados**, consulte y seleccione uno o varios formularios personalizados para asociarlos al problema.

* **Horas**: muestra una lista de entradas de horas sobre el problema.
* **Aprobaciones:** muestra las rutas de aprobación asociadas al problema.

  Para obtener más información sobre la asociación de aprobaciones a un problema, consulte la sección [Asociación de un proceso de aprobación a un elemento de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md#associating-the-approval-process-with-an-object) en [Crear un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Ver qué proyectos y tareas tienen problemas

Puede agregar iconos en la vista de un informe o lista de proyectos o tareas para mostrar si tienen problemas adjuntos.

Añadir iconos a la vista de un informe o lista es similar para proyectos y tareas.

Para añadir iconos que muestren si un proyecto tiene problemas en un informe de proyecto:

{{step1-click-main-menu}}

1. Haga clic en **Informes** > **Nuevo informe** > **Informe del proyecto**.
1. En el campo **Mostrar en esta columna**, empiece a escribir **Iconos de estado** y, a continuación, selecciónelo cuando aparezca en la lista.

1. Haga clic en **Guardar + Cerrar**.

   Los iconos de problemas se muestran en los proyectos que tienen problemas en la columna **Iconos de estado**.

   ![Lista de proyectos con icono de problema](assets/project-list-with-issue-icon-350x132.png)
