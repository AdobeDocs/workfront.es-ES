---
product-area: requests
navigation-topic: create-requests
title: Ver solicitudes enviadas
description: Obtenga información sobre las áreas de Adobe Workfront en las que puede ver solicitudes que usted u otra persona ha enviado o solicitudes que nunca ha enviado y que se han guardado como borradores.
author: Alina
feature: Requests
topic: Collaboration
role: User
exl-id: cfa2383a-9594-4867-9b48-11b8ea281486
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/wph4vcZj6iJCRSWrh6CHLwRhspLqbV-HL0qoZEwV-OI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 1561
ht-degree: 38%

---

# Vista de solicitudes enviadas

<!--
Remove production and preview references at release
-->


<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después del lanzamiento en Vista previa, las mismas funciones también están disponibles mensualmente en el entorno de producción para los clientes que habilitaron lanzamientos rápidos. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


Puede ver las solicitudes que usted u otra persona ha enviado, o las solicitudes que ha iniciado pero que nunca ha terminado de enviar. Las solicitudes no finalizadas se guardarán como borradores.

Puede localizar las solicitudes enviadas en las siguientes áreas de Adobe Workfront:

* El área Solicitudes de Workfront
* El widget Mis solicitudes en Inicio

El área Solicitudes muestra las siguientes solicitudes, en función de cómo decida consultarlas:

* Solicitudes de Workfront al utilizar la experiencia heredada
* Workfront, así como las solicitudes de Planning, al utilizar la nueva experiencia.

  >[!NOTE]
  >
  >* Solo puede ver sus propias solicitudes de borrador.
  >* En la nueva experiencia solicitante, las solicitudes enviadas y los borradores se encuentran en la misma lista.
  >* Los borradores creados en la experiencia heredada no se muestran en la nueva experiencia de solicitud.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquier paquete de Adobe Workfront o Adobe Workflow</p> 
   <p>Cualquier paquete de Adobe Workfront Planning</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Colaborador o superior</p>
   <p>Solicitud o superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td><p>Editar acceso a Problemas</p></td> 
  </tr>
  <tr>
   <td role="rowheader">Permisos de objeto</td> 
   <td><p>Ver permisos o superiores en las solicitudes</p></td> 
  </tr> 
  <!--
  tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
  </tr> 
  -->
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ver las solicitudes enviadas en el área Solicitudes

Puede ver las solicitudes enviadas en el área de Solicitudes o en el widget Mis solicitudes de Inicio.

Para obtener información sobre Mis solicitudes, consulte [Usar el widget Mis solicitudes](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md).

La visualización de las solicitudes enviadas difiere en función de si utiliza la experiencia de solicitud nueva o heredada.

* [Ver las solicitudes enviadas en la nueva experiencia de solicitud](#view-submitted-requests-in-the-new-requesting-experience)
* [Ver las solicitudes enviadas en la experiencia de solicitud heredada](#view-submitted-requests-in-the-legacy-requesting-experience)

### Ver las solicitudes enviadas en la nueva experiencia de solicitud

>[!NOTE]
>
>* Si tiene Workfront Planning, las solicitudes de Workfront y Planning aparecen en la misma lista.
>     El **tipo de objeto** de una solicitud de Planning recibe el nombre siguiendo este patrón: `< Name of workspace > > < Name of record type >`. Por ejemplo, el tipo de objeto de una solicitud de Planning podría llamarse `Marketing workspace > Campaigns`.\
>     El **tipo de objeto** de una solicitud de Workfront es `Issue`.
>* De forma predeterminada, se muestran hasta 50 solicitudes en la lista del área Solicitudes. Para ver más solicitudes, desplácese hasta la parte inferior de la lista.

Puede ver las solicitudes enviadas en el área de Solicitudes y en el widget Mis solicitudes de Inicio.

>[!NOTE]
>
>Los siguientes objetos tienen vínculos de la lista de solicitudes del área de solicitudes y del widget Mis solicitudes, al habilitar la nueva experiencia de solicitudes:
>
>* Solicitudes de Planning y Workfront en el campo Asunto.
>* Registros de Planning creados a partir de solicitudes de Planning en el campo Objeto creado.
>* Las tareas y problemas de Workfront se convirtieron desde solicitudes de Workfront en el campo Objeto creado.

Para ver las solicitudes que usted u otros usuarios han enviado en la nueva experiencia de solicitud:

{{step1-to-requests}}

1. Asegúrese de que la opción **Usar nueva experiencia** de la esquina superior derecha de la pantalla esté activada.

   Se muestra la lista de solicitudes.

1. (Opcional) Para buscar una solicitud, empiece a escribir en la barra de búsqueda de la esquina superior derecha de la lista. Los resultados de la búsqueda aparecen a medida que escribe.
1. (Opcional) Para administrar la forma en que se muestra la información en la lista de solicitudes, actualice los siguientes elementos de vista para la lista:

   * Ver
   * Filtro
   * Columnas
   * Agrupación
   * Formatear celdas
   * Altura de la fila

   Para obtener más información sobre la administración de información en la lista de solicitudes, vea [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

1. (Opcional) Compruebe el estado de una solicitud comprobando la columna **Estado**.

   >[!IMPORTANT]
   >
   >El administrador de Workfront puede configurar algunos estados de solicitudes de Workfront en el área **Configuración**. Para obtener más información, consulte [Crear o editar un estado](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
   >
   >Workfront codifica algunos estados de solicitudes de Workfront y todos los estados de solicitudes de Planning. No puede personalizarlos, cambiarles el nombre ni agregar más del mismo tipo.

   Los siguientes estados están disponibles en la nueva experiencia solicitante:

   * <span class="preview">**Nuevo**: la solicitud es nueva y nadie ha comenzado a trabajar en ella. </span>
   * **Borrador**: esta solicitud aún no se ha enviado. Este estado está codificado.
   * **Revisión pendiente**: (Solo en Planning) Esta solicitud tiene aprobadores y ninguno de ellos ha abierto la solicitud. Este estado está codificado.
   * **En revisión**: (solo en planeación) Esta solicitud tiene aprobadores y al menos un aprobador ha abierto la solicitud, pero no se ha tomado ninguna decisión. Este estado está codificado.
   * **Rechazada**: (Solo en Planning) Esta solicitud tiene aprobadores y ha sido rechazada. Esta solicitud no creará un registro. Este estado está codificado.
   * **En curso**:
      * Solicitudes Workfront: la solicitud se ha convertido y el trabajo está en curso.
      * Solicitudes de Workfront Planning: la finalización de la solicitud se asigna a un campo de Planning específico y el valor del campo aún no coincide con el valor de finalización.
   * **En espera**: esto está disponible para solicitudes de Workfront y lo establecen manualmente los usuarios.
   * <span class="preview">**Cancelado**: esto es para solicitudes de Workfront.</span> <!--checking with Khach)-->
   * <span class="preview">**Completar**: se ha creado el registro de Planning que completa la solicitud. (Solo en Planning)</span>

### Ver las solicitudes enviadas en la experiencia de solicitud heredada

Para ver las solicitudes que usted u otros usuarios han enviado en la experiencia de solicitud heredada:

{{step1-to-requests}}

1. (Condicional) Si su organización compró un paquete de Workfront Planning, haga clic en la pestaña **Workfront** para ver las solicitudes de Workfront.
1. Haga clic en **Enviado** en el panel izquierdo para ver todas las solicitudes enviadas.

   Puede ver hasta 2000 solicitudes, que pueden mostrarse en varias páginas.

   >[!TIP]
   >
   >No puede personalizar las columnas en la lista de solicitudes enviadas.

   ![Solicitudes enviadas en una nueva lista](assets/nwe-submitted-requests-new-list-350x57.png)


1. Las siguientes columnas se muestran de forma predeterminada:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
         <td role="rowheader">Nombre</td> 
         <td> <p>Nombre de la solicitud.</p> <p>Seleccione el nombre de una solicitud para abrirla. </p> <p><b>Sugerencia</b>

   Si el problema no se ha conservado al convertirse en una tarea o en un proyecto, el nombre del problema aparece atenuado y ya no se puede hacer clic en él. Para obtener información sobre la conversión de problemas, consulte <a href="../../../manage-work/issues/convert-issues/convert-issues.md" class="MCXref xref">Información general sobre la conversión de problemas en Adobe Workfront</a>. </p> </td>
   </tr> 
      <tr> 
         <td role="rowheader">Se ha convertido a</td> 
         <td> <p>Nombre del objeto de resolución, que puede ser una tarea o un proyecto al que se haya convertido la solicitud. </p> <p>Haga clic en el nombre de la tarea o proyecto para abrirlos. </p> <p>Si la solicitud no se ha convertido, este campo está vacío. </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader">Ruta</td> 
         <td>Nombre de la cola de solicitudes, grupos de temas y temas de colas en los que se haya enviado originalmente la solicitud. </td> 
      </tr> 
      <tr> 
         <td role="rowheader">Estado</td> 
         <td>Estado actual de la solicitud o del objeto de resolución (tarea o proyecto)</td> 
      </tr> 
      <tr> 
         <td role="rowheader">Fecha de entrada</td> 
         <td>Fecha en la que se envió la solicitud o fecha en la que se creó el objeto de resolución si la solicitud se eliminó al convertirse. </td> 
      </tr> 
      <tr> 
         <td role="rowheader">Fecha de última actualización</td> 
         <td> <p>Fecha en la que se actualizó la solicitud por última vez.</p> <p>La lista de solicitudes enviadas se ordena por este campo de forma predeterminada. </p> </td> 
      </tr> 
      </tbody> 
      </table>

1. (Opcional) Haga clic en el encabezado de una columna para ordenar los datos por ella.

   >[!TIP]
   >
   >Cuando se aleja de la lista de solicitudes enviadas, se conserva la opción de ordenación seleccionada.

1. (Opcional) Seleccione una solicitud en la lista y, a continuación, haga clic en el icono **Abrir resumen** ![Abrir resumen con texto](assets/open-summary-with-text-nwe.png) para abrir el panel Resumen y mostrar información adicional sobre la solicitud, agregar comentarios, documentos o asignarla. Para obtener información sobre el panel Resumen, consulte [Información general sobre el resumen](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

   >[!TIP]
   >
   >* Si el panel Resumen ya está abierto, el icono Abrir resumen cambia a Cerrar resumen.
   >
   >* Si su organización utiliza el almacenamiento en la nube de Adobe para documentos, no puede agregar documentos a las solicitudes de almacenamiento en la nube de Adobe en el Panel de resumen.
   >
   >Para obtener más información, vea [Información general sobre la administración de documentos de proyectos y objetos relacionados](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md).

1. (Opcional y condicional) Haga clic en el icono **X** en la esquina superior derecha o en el icono **Cerrar resumen** ![Cerrar resumen con texto](assets/close-summary-with-text-nwe.png) para cerrar el Panel de resumen.

   Si un problema se convirtió en una tarea o proyecto y el problema se eliminó en el proceso de conversión, el panel Resumen está en blanco. Para obtener información sobre la conversión de problemas, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. Desde el **icono de filtro** ![icono de filtro](assets/filter-nwepng.png) en la parte superior derecha de la lista, seleccione cualquiera de los filtros enumerados en la tabla siguiente.

   >[!TIP]
   >
   >No se pueden modificar los filtros en la sección Enviadas del área Solicitudes.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Todas</td> 
      <td>Todas las solicitudes enviadas, independientemente del estado o de quién las envió.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abrir</td> 
      <td> <p>Todas las solicitudes enviadas que están abiertas actualmente, independientemente de quién las envió. Solo las solicitudes para las que tenga al menos permisos de visualización se muestran aquí si no las había enviado usted mismo. </p> <p>Las solicitudes sin una fecha de finalización real o cuyo objeto de resolución no tenga una fecha de finalización real se muestran en la subpestaña Abrir.</p> <p><b>Sugerencia</b>

   Las solicitudes con cualquier estado que no sea igual a Cerrado se consideran abiertas.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Mis solicitudes</td> 
      <td>Solicitudes enviadas independientemente de su estado. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mis solicitudes abiertas</td> 
      <td> <p>Solicitudes que ha enviado que aún están abiertas. </p> <p>Las solicitudes sin fecha de finalización real o cuyo objeto de resolución no tenga una fecha de finalización real se muestran en la subpestaña Mis solicitudes abiertas. </p> <p><b>Sugerencia</b>

   Las solicitudes que no están en un estado equivalente a Cerrado se consideran abiertas.</p> </td>
   </tr> 
    </tbody> 
   </table>

1. (Opcional) Haga clic en el icono **Filtrar página** ![Icono de búsqueda](assets/search-icon.png) en la parte superior de la lista para buscar una solicitud por su nombre. La lista se actualiza con los resultados que coinciden con los criterios de búsqueda.

   <!--

   1. (Conditional) To display only Workfront Request queues, search or filter for `Issue` object types.</span>
   -->

   <!--
   <li> <p>Click the <strong>Complete</strong> subtab to view requests that have been completed.</p> <p>(NOTE: this step will stay drafted even after release. We can't see Completed at this time!) <br>Requests with an Actual Completion Date or whose resolving object has an Actual Completion Date are listed in the Complete subtab.<br>Once a request receives an Actual Completion Date, it stays in the Recently Completed area for 10 business days. After that, it is moved to the Completed area. <br>For information about resolving and resolvable objects, see the article <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </li>
   -->

   <!--
   <li>(Optional) Select an option from the <strong>Sort by</strong> drop-down menu to sort the requests by the following criteria:   (NOTE: this step will stay drafted even after release. We can't see Completed at this time!)  
   <ul>
   <li><strong>Assigned To</strong>: Requests are sorted alphabetically by the name of the assignee using the following criteria: 
   <ul>
   <li>All requests assigned to users are sorted first, in the order of the users' names.</li>
   <li>Requests assigned to job roles are sorted secondly, in the order of the job roles' names and are listed after all the requests assigned to users.</li>
   <li>Requests that are assigned to teams are sorted last, in the order of the teams' names and are listed after all the requests assigned to users and those assigned to job roles.</li>
   <li>All unassigned requests are listed last, in the order of their Entry Date. </li>
   </ul></li>
   <li><strong>Submitted On</strong>: Requests are sorted chronologically by the date when they were submitted.</li>
   <li><strong>Recently Updated</strong> (this is the default): Requests are sorted chronologically by the date of their last update.</li>
   <li><strong>Name</strong>: Requests are sorted alphabetically by name. </li>
   <li><strong>Priority</strong>: Requests are sorted in the order of their priority.</li>
   <li><strong>Queue</strong>: Requests are sorted alphabetically by the name of the requests queue where they were submitted. </li>
   <li><strong>Status</strong>: Requests are sorted alphabetically by their status. </li>
   </ul></li>
   -->

1. Haga clic en **Borradores** para ver todas las solicitudes redactadas. Workfront guarda un número ilimitado de borradores para cada cola de solicitudes en esta carpeta. Cuando se introduce una nueva solicitud para un tema de la cola que ya tiene un borrador, se le pedirá que utilice uno existente. Para obtener más información, consulte [Crear solicitudes a partir de borradores](../../../manage-work/requests/create-requests/create-requests-from-drafts.md).

   <!--
   Planning tab has been removed and no longer visible in legacy Requests area: 
   (Optional and conditional) If your organization purchased a Workfront Planning package, click the **Planning** tab, then click **Submitted** in the left panel to view Workfront Planning requests. 
      Use **Filters** and **Columns** to update the information in the Planning request list. 
      ![Planning tab submitted section in Requests area](assets/workfront-planning-tab-submitted-section-in-requests-area.png)
      For information, see [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md).
   -->


1. (Opcional) Compruebe el estado de una solicitud comprobando la columna **Estado**. Los siguientes estados están disponibles en la nueva experiencia solicitante:

   * **borrador**. Esta solicitud aún no se ha enviado.
   * **En curso**
   * **Completado**


