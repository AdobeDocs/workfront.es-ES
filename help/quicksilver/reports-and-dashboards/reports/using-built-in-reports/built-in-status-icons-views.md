---
product-area: reporting
navigation-topic: using-built-in-reports
title: Iconos de estado integrados en vistas
description: Puede añadir el campo Iconos de estado integrado como una columna en las vistas para mejorar la visibilidad de los puntos clave sobre los objetos.
author: Nolan
feature: Reports and Dashboards
exl-id: 7831d5c1-e982-4780-a5a8-54dc6decb3a1
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '1253'
ht-degree: 3%

---

# Iconos de estado integrados en vistas

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ALina: ***Link this from the Understanding Fields in Lists and Reports.) </p>
-->

Puede añadir el campo Iconos de estado integrado como una columna en las vistas para mejorar la visibilidad de los puntos clave sobre los objetos. Con los iconos de estado, puede ver de un vistazo cuando existen las siguientes condiciones:

* Un objeto tiene documentos adjuntos
* Un objeto está asociado a un proceso de aprobación
* Un objeto tiene notas adicionales asociadas
* Un gasto es facturable o reembolsable
* Una tarea se encuentra en una ruta crítica
* Un usuario pertenece a una empresa, a un equipo o está ubicado en una zona horaria diferente

Tenga en cuenta lo siguiente:

* La mayoría de los indicadores del campo Iconos de estado son vínculos rápidos al objeto o área real del objeto que representan.

* Si falta alguno de los elementos representados por los iconos en el objeto, el icono que representa el elemento que falta aparece atenuado en la columna Iconos de estado en lugar de en una imagen de color.

  ![iconos_estado_tarea.png](assets/task-status-icons.png)

  Para obtener más información, consulte la sección [Información general sobre los iconos y las marcas de estado](#overview-of-status-icons-and-flags) en este artículo.

* En algunas vistas, el campo **Iconos de estado** se llama **Marcas** o **Iconos de vista**.\
  No se puede personalizar el aspecto de los iconos que se incluyen en el campo Iconos de estado.

* No puede editar el número de iconos en el campo Iconos de estado.

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
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p>Editar el acceso a Informes, Tableros y Calendarios para agregar columnas a un informe</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos en una vista existente</p> <p>Administrar permisos para agregar columnas a un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Agregar el campo Iconos de estado a una vista

Algunas vistas e informes integrados ya incluyen el campo Iconos de estado.

No puede agregar el campo Iconos de estado a todas las vistas.

Para agregar el campo Iconos de estado a una vista personalizada que cree desde cero:

1. Ir a una lista de cualquiera de los siguientes objetos:

   * Tareas
   * Problemas
   * Proyectos
   * Tareas de plantilla
   * Plantillas
   * Gastos
   * Documentos
   * Usuarios\
     Solo estos objetos tienen disponible el campo **Iconos de estado**.\
     Para obtener información sobre las listas de objetos, consulte [Introducción a las listas en Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. En el menú desplegable **Vista**, seleccione **Nueva vista**.

1. Haga clic en **Añadir columna**.
1. En el cuadro **Mostrar en esta columna**, empiece a escribir cualquiera de los siguientes nombres de campo y selecciónelo cuando aparezca en la lista:

   * *Iconos de estado*
   * *Indicadores*
   * *Iconos de vista *(solo en vistas de documento).

   Los iconos integrados se enumeran con cualquiera de estos nombres.\
   Una vista de plantilla contiene los campos **Iconos de estado** y **Indicadores**. En este caso, las dos columnas contienen iconos idénticos.\
   Las vistas de documento contienen un campo **Ver iconos**.

1. Pulse **Guardar vista**.
1. (Opcional) Especifique un nuevo nombre para la vista y haga clic en **Guardar vista**.\
   Esto agrega la columna **Iconos de estado** a la vista.
1. (Opcional) Pase el ratón sobre un icono para comprender qué representa.
1. (Opcional) Haga clic en un icono para ir al área del objeto que representa.\
   No todos los iconos son vínculos a objetos.\
   Para obtener una lista completa de los atributos de cada icono, consulte la sección [Información general sobre iconos y marcas de estado](#overview-of-status-icons-and-flags).

## Información general sobre los iconos y las marcas de estado {#overview-of-status-icons-and-flags}

En la tabla siguiente se enumeran todos los iconos de estado disponibles en Workfront, el tipo de objetos que se pueden asociar a ellos y lo que sucede cuando se hace clic en ellos.

Debe tener permisos de al menos Ver los objetos para poder hacer clic en algunos de los iconos siguientes y acceder a esos objetos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Icono de estado o indicador</strong> </th> 
   <th><strong>Descripción</strong> </th> 
   <th><strong>Objeto</strong> </th> 
   <th>Al hacer clic</th> 
   <th> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <img src="assets/condition-update-icon-on-target-29x34.png" alt="condition_update_icon_on_target.png" style="width: 29;height: 34;">o <img src="assets/screen-shot-2018-08-17-at-9.49.36-am-29x37.png" alt="Screen_Shot_2018-08-17_at_9.49.36_AM.png" style="width: 29;height: 37;"><br><img src="assets/condition-update-icon--in-trouble-29x26.png" alt="condition_update_icon__in_issue.png" style="width: 29;height: 26;"> o <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-29x26.png" style="width: 29;height: 26;"><br><img src="assets/condition-update-at-risk-27x28.png" alt="condition_update_at_risk.png" style="width: 27;height: 28;"> o <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-33x34.png" alt="Screen_Shot_2018-08-17_at_9.49.23_AM.png" style="width: 33;height: 34;"></td> 
   <td>Indica que la condición del proyecto es En el destino (verde), Con problemas (rojo) o En riesgo (amarillo).<br>Para obtener información acerca de la condición del proyecto, vea <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Información general sobre la condición del proyecto y el tipo de condición</a>.</td> 
   <td>Proyectos</td> 
   <td>Haga clic en para abrir la lista de tareas del proyecto. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/notes-icon-44x34.png" alt="notes_icon.png" style="width: 44;height: 34;"> </td> 
   <td>Indica que el objeto tiene notas (actualizaciones) en la ficha Actualizaciones.</td> 
   <td> <p>Proyectos<br>Tareas<br>Problemas<br>Plantillas<br>Tareas de plantillas</p> </td> 
   <td> <p>Haga clic para abrir la pestaña Actualizaciones del objeto. </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-icon-35x42.png" alt="document_icon.png" style="width: 35;height: 42;">o <img src="assets/new-documents-icon-36x43.png" alt="new_documents_icon.png" style="width: 36;height: 43;"></td> 
   <td>Indica que el objeto tiene documentos adjuntos. </td> 
   <td> Proyectos<br>Tareas<br>Problemas<br>Plantillas<br>Tareas de plantillas </td> 
   <td>Haga clic para abrir la pestaña Documentos del objeto. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/open-issu-icon-34x36.png" alt="open_issue_icon.png" style="width: 34;height: 36;">o <img src="assets/new-open-issues-25x30.png" alt="new_open_issues.png" style="width: 25;height: 30;"></td> 
   <td>Indica que hay problemas pendientes en el proyecto o la tarea.</td> 
   <td> Proyectos<br>Tareas </td> 
   <td>Haga clic en para abrir el objeto. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/approval-icon-42x38.png" alt="approval_icon.png" style="width: 42;height: 38;"> o <img src="assets/new-approval-icon-33x35.png" alt="new_approval_icon.png" style="width: 33;height: 35;"></td> 
   <td>Indica que hay una aprobación en el objeto.</td> 
   <td> Proyectos<br>Tareas<br>Problemas<br>Plantillas<br>Tareas de plantillas </td> 
   <td>Haga clic en para abrir el objeto. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expenses-icon-52x40.png" alt="Expenses_icon.png" style="width: 52;height: 40;"> </td> 
   <td> <p>Puede agregar una columna Icono de gastos en la vista para mostrar este icono. Esto indica que el proyecto o la tarea tienen gastos asociados.</p> </td> 
   <td> <p>Proyectos</p> <p>Tareas</p> </td> 
   <td>Haga clic para abrir la pestaña Gastos del proyecto o de la tarea. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-progress-status-icon-on-time-44x39.png" alt="task_progress_status_icon_on_time.png" style="width: 44;height: 39;"> <br> <img src="assets/task-progress-status-late-44x43.png" alt="task_progress_status_late.png" style="width: 44;height: 43;"> <br> <img src="assets/task-progress-status-at-risk-44x35.png" alt="task_progress_status_at_risk.png" style="width: 44;height: 35;"> <br> <img src="assets/task-progress-status-icon-behind-44x35.png" style="width: 44;height: 35;"> </td> 
   <td> <p>Indica que el estado de progreso de una tarea es uno de los siguientes:</p> 
    <ul> 
     <li>Tiempo de activación (cuadrado verde)</li> 
     <li>Retrasado (círculo rojo)</li> 
     <li>En riesgo (diamante azul)</li> 
     <li>Detrás (triángulo amarillo)</li> 
    </ul> <p>Para obtener información sobre el estado de progreso de las tareas, consulte <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Resumen del estado de progreso de la tarea</a>.</p> </td> 
   <td>Tareas</td> 
   <td>Haga clic en para abrir la tarea. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-critical-path-icon-36x35.png" alt="task_critical_path_icon.png" style="width: 36;height: 35;"> o <img src="assets/new-critical-path-icon-34x34.png" alt="new_critical_path_icon.png" style="width: 34;height: 34;"></td> 
   <td>Indica que la tarea se encuentra actualmente en la ruta crítica. <br>Para obtener información acerca de las tareas en una ruta crítica del proyecto, consulte <a href="../../../manage-work/tasks/manage-tasks/critical-path.md" class="MCXref xref">Información general sobre la ruta crítica del proyecto</a>.</td> 
   <td>Tareas</td> 
   <td>Haga clic en para abrir la tarea.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/milestone-icon-50x43.png" alt="milestone_icon.png" style="width: 50;height: 43;"> </td> 
   <td>Indica que la tarea está asociada a un hito. El administrador del sistema puede personalizar el color del diamante en su entorno.<br>Para obtener información acerca de los hitos, vea <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Crear una ruta de hitos</a>.</td> 
   <td>Tareas</td> 
   <td>Haga clic en para abrir la tarea. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/issue-source-link-icon-44x41.png" alt="issue_source_link_icon.png" style="width: 44;height: 41;"> </td> 
   <td>Vínculo al objeto de origen de un problema. El objeto de origen de un problema es el objeto en el que se registró el problema. Una tarea o un proyecto pueden ser objetos de origen para los problemas. </td> 
   <td>Problemas</td> 
   <td>Haga clic para abrir el objeto de origen (tarea o proyecto) de un problema. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resolving-object-icon-43x45.png" alt="resolve_object_icon.png" style="width: 43;height: 45;"> </td> 
   <td>Indica que hay un objeto de resolución que, en última instancia, resuelve el problema. En este caso, no puede completar el problema. Se completa cuando finaliza el objeto de resolución. <br>Para obtener información acerca de la resolución de objetos, vea <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Información general sobre la resolución y los objetos solucionables </a>.</td> 
   <td>Problemas</td> 
   <td>Haga clic en para abrir el objeto de resolución del problema. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/view-doc-icon-45x48.png" alt="view_doc_icon.png" style="width: 45;height: 48;"> </td> 
   <td>Ver un documento.</td> 
   <td>Documentos</td> 
   <td>Haga clic en para descargar el documento.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/download-doc-icon.png"> </td> 
   <td>Descargue un documento.</td> 
   <td>Documentos</td> 
   <td>Haga clic en para descargar el documento.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-type-icon.png"> </td> 
   <td>Indica el tipo de documento.</td> 
   <td>Documentos</td> 
   <td>Haga clic en para descargar el documento.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-belongs-to-company-icon-44x44.png" alt="user_belonging_to_company_icon.png" style="width: 44;height: 44;"> </td> 
   <td>Indica que el usuario está asociado con una compañía. </td> 
   <td>Usuarios</td> 
   <td>No disponible</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-with-team-icon-40x48.png" alt="user_with_team_icon.png" style="width: 40;height: 48;"> </td> 
   <td>Indica que el usuario está asociado a un equipo.</td> 
   <td>Usuarios</td> 
   <td>Haga clic en para abrir el perfil de usuario.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resource-grid-icon-44x46.png" alt="resource_grid_icon.png" style="width: 44;height: 46;"> </td> 
   <td>Acceso directo a la pestaña Asignación del usuario. </td> 
   <td>Usuarios</td> 
   <td>Haga clic para abrir la pestaña Asignación del usuario y conocer los elementos de trabajo que está asignado al usuario.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/screen-shot-2018-07-26-at-2.31.40-pm-44x40.png" alt="Screen_Shot_2018-07-26_at_2.31.40_PM.png" style="width: 44;height: 40;"> </td> 
   <td>Indica que el usuario se encuentra en una zona horaria diferente a la del sistema.</td> 
   <td>Usuarios</td> 
   <td>No disponible</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/billable-expense-icon-44x45.png" alt="billable_cost_icon.png" style="width: 44;height: 45;"> </td> 
   <td>Indica que un gasto es facturable.<br>Para obtener información sobre los gastos, consulte <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Administrar gastos de proyecto </a>.</td> 
   <td>Gastos</td> 
   <td>No disponible</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expense-reimbursable-icon-44x45.png" alt="cost_reembolsable_icon.png" style="width: 44;height: 45;"> </td> 
   <td> Indica que un gasto es reembolsable.<br>Para obtener información sobre los gastos, consulte <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Administrar gastos de proyecto </a>.</td> 
   <td>Gastos</td> 
   <td>No disponible</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/reimbursed-expense-icon-44x43.png" alt="reembolsed_cost_icon.png" style="width: 44;height: 43;"></td> 
   <td> Indica que se ha reembolsado un gasto.<br>Para obtener información sobre los gastos, consulte <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Administrar gastos de proyecto </a>.</td> 
   <td>Gastos</td> 
   <td>No disponible</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
