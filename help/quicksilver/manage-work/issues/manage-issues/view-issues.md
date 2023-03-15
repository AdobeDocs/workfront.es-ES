---
product-area: projects
navigation-topic: manage-issues
title: Ver problemas
description: Puede ver los problemas asociados a un proyecto, una tarea o una iteración.
author: Alina
feature: Work Management
exl-id: b6791c8f-b356-4235-8b0e-952e29a88952
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1038'
ht-degree: 0%

---

# Ver problemas

Puede ver los problemas asociados a un proyecto, una tarea o una iteración.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> <p>Revise o otorgue una licencia superior para ver los problemas de la sección Problemas de un proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver acceso a Problemas</p> <p>Ver o acceder más a Proyectos y tareas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre el acceso a los problemas en el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Concesión de acceso a problemas</a>. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos para el problema</p> <p> Para obtener información sobre la concesión de permisos a problemas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema </a></p> <p>Para obtener información sobre la solicitud de permisos adicionales, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Ver problemas según el estado

Para ver los problemas de un proyecto, tarea o iteración:

1. Abra un proyecto, tarea o iteración que contenga problemas y haga clic en **Problemas** en el panel izquierdo.

1. Para mostrar todos los problemas, sean abiertos o cerrados, haga clic en cualquiera de los filtros que se enumeran a continuación en el **Filtro** menú desplegable.

>[!TIP]
>
>La lista de filtros varía según el sistema o el administrador de grupo que haya seleccionado para mostrarse en ella.

* **Abra:** Muestra los problemas abiertos.

   Esto incluye los asociados a un objeto resuelto y los que están en estado Cerrado - Pendiente de aprobación .

   Para obtener información sobre la resolución de objetos, consulte [Información general sobre la resolución y resolución de objetos](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

* **Finalizado:** Muestra todos los problemas que tienen una fecha de finalización real.
* **Todo** Muestra todos los problemas.

## Comprender la información sobre problemas

Puede ver información sobre un problema al acceder a él.

Para acceder a un problema y ver información sobre él:

1. Abra un proyecto, tarea o iteración que contenga problemas y haga clic en **Problemas** en el panel izquierdo.
1. En el **Filtro** menú desplegable, seleccione el filtro para mostrar los problemas que está intentando ver.

   Seleccione una de las siguientes opciones:

   * Abrir
   * Finalizado
   * Todas

1. Haga clic en el nombre de un problema.

   Cuando tenga permisos de gestión del problema, puede editar cualquier campo editable del problema y agregar aprobaciones, horas o documentos al problema.

1. En el panel izquierdo, haga clic en cualquiera de las siguientes opciones para ver más información sobre el problema:

* **Actualizaciones**: Puede realizar las siguientes acciones :

   * Comente el problema o responda a un comentario existente.
   * Tiempo de registro.
   * Cambie el estado del problema.

      Para obtener más información sobre la actualización de trabajos en Workfront, consulte [Actualizar trabajo](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* **Documentos**: Adjunte documentos al problema. Para obtener más información sobre cómo agregar documentos a Workfront, consulte [Agregar documentos a Adobe Workfront desde el sistema de archivos](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

* **Detalles del problema**: Expanda este vínculo para mostrar la **Información general** y **Forms personalizado** áreas.

   Si tiene permisos de administración para el problema y derechos de edición en el formulario personalizado, puede editar parte de la información aquí.

   Vea o edite los campos siguientes en la sección **Información general** área:

   * **Nombre**
   * **Ruta**: la ruta a través de la cual se registró el problema en el proyecto.

      Si se ha enviado un problema como solicitud en una cola de solicitudes, los nombres del proyecto, el grupo de temas y el tema de cola se enumeran aquí. Este campo no se puede editar.

      Para obtener más información sobre el envío de solicitudes, consulte [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

   * **Descripción**
   * **URL**: cualquier dirección web relacionada con el problema.
   * **Prioridad**: un indicador visual que permite priorizar problemas.
   * **Gravedad**: un indicador visual que indica la gravedad del problema descrito en el problema.
   * **Contacto principal**: el contacto principal predeterminado es el usuario que creó el problema. Este campo se puede editar.
   * **Horas planificadas**: muestra la cantidad de tiempo que tardará alguien en completar el problema. El valor predeterminado es de 8 horas. Este campo se puede editar.
   * **Horas reales**: muestra la cantidad de tiempo que se tardó en completar el problema. Esta es la hora real a la que alguien registra el problema.
   * **Fecha de inicio planeada**: la fecha en la que se planea iniciar el problema. El valor predeterminado es la fecha y la hora en que se creó el problema.
   * **Fecha de inicio real**: la fecha y la hora en que se cambió el estado del problema a En curso.
   * **Fecha de finalización planeada**: la fecha en la que se planea completar la emisión.
   * **Fecha de finalización real**: la fecha en la que se haya completado realmente el problema. Este campo se rellena automáticamente cuando el estado del problema cambia a Cerrado o Resuelto, o se puede editar manualmente.
   * **Costo real**: el coste basado en las horas reales registradas en el problema. Este campo no es editable. El coste real de un problema se calcula en función de la fórmula siguiente, donde la tasa de coste del usuario es la tasa de coste asociada con el usuario que registra el tiempo del problema:

      Costo real del problema = Horas registradas * Tasa de costo del usuario

   * **Introducido por**: este es el usuario que creó el problema. Este campo no es editable.
   * **Última actualización por**: este es el usuario que actualizó cualquier campo sobre el problema en último lugar. Este campo no es editable.

      En el **Forms personalizado** área , vista de seleccionar uno o varios formularios personalizados para asociarlos al problema.

* **Horas**: Muestra una lista de entradas de hora sobre el problema.
* **Aprobaciones:** Muestra las rutas de aprobación asociadas al problema.

   Para obtener más información sobre cómo asociar aprobaciones con un problema, consulte la [Asociación de un proceso de aprobación a un elemento de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md#associating-the-approval-process-with-an-object) en [Creación de un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Ver qué proyectos y tareas tienen problemas

Puede añadir iconos en la vista de un proyecto, un informe de tareas o una lista para mostrar si tienen problemas adjuntos. Añadir iconos a la vista de un informe o una lista es similar para los proyectos y las tareas.

Para agregar iconos que muestren si un proyecto tiene problemas en un informe de proyecto:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.
1. Haga clic en **Informes** > **Nuevo informe** > **Informe de proyecto**.
1. En el **Mostrar en esta columna** campo, empezar a escribir **Iconos de estado** y, a continuación, selecciónela cuando aparezca en la lista.

1. Haga clic en **Guardar + Cerrar** .

   Los iconos de los problemas se muestran en los proyectos que tienen problemas en la variable **Iconos de estado** para abrir el Navegador.

   ![project_list_with_issue_icon.png](assets/project-list-with-issue-icon-350x132.png)
