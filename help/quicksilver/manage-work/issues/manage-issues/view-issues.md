---
product-area: projects
navigation-topic: manage-issues
title: Ver problemas
description: Puede ver los problemas asociados a un proyecto, tarea o iteración.
author: Alina
feature: Work Management
exl-id: b6791c8f-b356-4235-8b0e-952e29a88952
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1035'
ht-degree: 0%

---

# Ver problemas

Puede ver los problemas asociados a un proyecto, tarea o iteración.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> <p>Revise la licencia o una superior para ver los problemas en la sección Problemas de un proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver acceso a Problemas</p> <p>Acceso de visualización o superior a Proyectos y tareas</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre el acceso a los problemas de su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Conceder acceso a los problemas</a>. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos para el problema</p> <p> Para obtener información sobre la concesión de permisos a los problemas, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema </a></p> <p>Para obtener información sobre cómo solicitar permisos adicionales, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Ver problemas según el estado

Para ver los problemas de un proyecto, tarea o iteración:

1. Abra un proyecto, tarea o iteración que contenga problemas y haga clic en **Problemas** en el panel izquierdo.

1. Para mostrar todos los problemas, los problemas abiertos o los problemas cerrados, haz clic en cualquiera de los filtros que aparecen a continuación en el menú desplegable **Filtro**.

>[!TIP]
>
>La lista de filtros varía según lo que haya seleccionado el administrador del sistema o del grupo para mostrarla.

* **Abrir:** muestra los problemas que están abiertos.

  Esto incluye los asociados a un objeto de resolución y los que están en estado Cerrado - Pendiente de aprobación.

  Para obtener información acerca de la resolución de objetos, vea [Información general sobre la resolución y los objetos solucionables](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

* **Completado:** muestra todos los problemas que tienen una fecha real de finalización.
* **Todos** muestra todos los problemas.

## Comprensión de la información sobre problemas

Puede ver información sobre un problema al acceder a él.

Para acceder a un problema y ver información sobre él:

1. Abra un proyecto, tarea o iteración que contenga problemas y haga clic en **Problemas** en el panel izquierdo.
1. En el menú desplegable **Filtro**, seleccione el filtro para mostrar los problemas que está intentando ver.

   Seleccione una de las siguientes opciones:

   * Abrir
   * Finalizado
   * Todas

1. Haga clic en el nombre de un problema.

   Cuando tenga permisos de administración sobre el problema, podrá editar cualquier campo editable del mismo y añadir aprobaciones, horas o documentos al problema.

1. En el panel izquierdo, haga clic en cualquiera de las siguientes opciones para ver más información sobre el problema:

* **Actualizaciones**: puede realizar las siguientes acciones:

   * Comentar el problema o responder a un comentario existente.
   * Registrar el tiempo.
   * Cambie el estado del problema.

     Para obtener más información sobre cómo actualizar el trabajo en Workfront, consulte [Actualizar trabajo](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* **Documentos**: adjunte documentos al problema. Para obtener más información sobre cómo agregar documentos a Workfront, consulte [Agregar documentos a Adobe Workfront desde el sistema de archivos](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

* **Detalles del problema**: expanda este vínculo para mostrar las áreas de **Información general** y **Forms personalizado**.

  Si tiene permisos de administración del problema y derechos de edición en el formulario personalizado, puede editar parte de la información aquí.

  Vea o edite los campos siguientes en el área **Información general**:

   * **Nombre**
   * **Ruta**: la ruta a través de la cual se registró el problema en el proyecto.

     Si un problema se envió como solicitud en una cola de solicitudes, los nombres del proyecto, el grupo de temas y el tema de la cola se enumeran aquí. Este campo no se puede editar.

     Para obtener más información sobre cómo enviar solicitudes, consulte [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

   * **Descripción**
   * **URL**: cualquier dirección web relacionada con el problema.
   * **Prioridad**: un indicador visual que le permite priorizar los problemas.
   * **Gravedad**: un indicador visual que indica la gravedad del problema descrito en el problema.
   * **Contacto principal**: el contacto principal predeterminado es el usuario que creó el problema. Este campo se puede editar.
   * **Horas planificadas**: muestra la cantidad de tiempo que tardará alguien en completar el problema. El valor predeterminado es de 8 horas. Este campo se puede editar.
   * **Horas reales**: muestra la cantidad de tiempo que se tardó en completar el problema. Esta es la hora real en la que alguien inicia sesión en el problema.
   * **Fecha planificada de inicio**: la fecha en la que se planea que comience el problema. El valor predeterminado es la fecha y la hora en que se creó el problema.
   * **Fecha real de inicio**: la fecha y la hora en que se cambió el estado del problema a En curso.
   * **Fecha planificada de finalización**: la fecha en la que se planea completar el problema.
   * **Fecha real de finalización**: la fecha en la que se resuelve el problema. Este campo se rellena automáticamente cuando el estado del problema cambia a Cerrado o Resuelto, o se puede editar manualmente.
   * **Costo real**: el costo basado en las horas reales registradas en el problema. Este campo no se puede editar. El coste real de un problema se calcula según la fórmula siguiente, donde Tasa de coste de usuario es la tasa de coste asociada al registro del usuario en el momento del problema:

     Costo real de problema = Horas registradas * Tasa de costo de usuario

   * **Ingresado por**: este es el usuario que creó el problema. Este campo no se puede editar.
   * **Última actualización por**: este es el usuario que actualizó por última vez cualquier campo del problema. Este campo no se puede editar.

     En el área **Forms personalizado** , vea y seleccione uno o varios formularios personalizados para asociarlos al problema.

* **Horas**: muestra una lista de entradas de horas sobre el problema.
* **Aprobaciones:** Muestra las rutas de aprobación asociadas con el problema.

  Para obtener más información sobre cómo asociar aprobaciones con un problema, consulte la sección [Asociar un proceso de aprobación con un elemento de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md#associating-the-approval-process-with-an-object) en [Crear un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Ver qué proyectos y tareas tienen problemas

Puede agregar iconos en la vista de un informe o lista de proyectos o tareas para mostrar si tienen problemas adjuntos. Agregar iconos a la vista de un informe o lista es similar para proyectos y tareas.

Para agregar iconos que muestren si un proyecto tiene problemas en un informe de proyecto:

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.
1. Haga clic en **Informes** > **Nuevo informe** > **Informe del proyecto**.
1. En el campo **Mostrar en esta columna**, empiece a escribir **Iconos de estado** y, a continuación, selecciónelo cuando aparezca en la lista.

1. Haga clic en **Guardar + Cerrar** .

   Los iconos de problema se muestran en los proyectos que tienen problemas en la columna **Iconos de estado**.

   ![lista_de_proyectos_con_icono_de_problema.png](assets/project-list-with-issue-icon-350x132.png)
