---
product-area: projects
navigation-topic: manage-projects
title: Editar proyectos
description: Puede editar un proyecto en Adobe Workfront tantas veces como sea necesario. Lo ideal es editar un proyecto cuando este esté en estado de Planning.
author: Alina
feature: Work Management
exl-id: a6a1f178-189a-4c41-835b-7726081a2b49
source-git-commit: bbd99435bb07d68bf9058bcd3e8c6ef5d9df75a9
workflow-type: tm+mt
source-wordcount: '7705'
ht-degree: 2%

---

# Editar proyectos

<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa.</span>

<!--
<p>***Linked to many articles,</p>
<p>The Resource Pools part also duplicates in the "Working with Resource Pools" article </p>
<p>The Update Type section is also documented in Selecting the Project Update Type article</p>
<p>Keep the reference link to the other article that also documents the Update Type) </p>
<p>(NOTE 2: information described here also exists in these articles:</p>
<p>** Project Overview area</p>
<p>**Manage project Finance area</p>
<p>If you need to update just one field, check to see if that field is also listed there and update in both places.)</p>
</div>
-->

Puede editar un proyecto en Adobe Workfront tantas veces como sea necesario. Le recomendamos que edite los proyectos mínimamente después de que su estado cambie a Actual para evitar confusiones enviando notificaciones sobre los cambios a todo el equipo del proyecto. Lo ideal es editar un proyecto cuando este esté en estado de Planning. Para obtener información sobre el equipo del proyecto, consulte [Información general del equipo del proyecto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Requisitos de acceso

<!--drafted - replace table at P&P:

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
   <td><p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> 
    <ul> 
     <li> <p>Contribute permissions to a project to edit it in the Project Details area </p> </li> 
     <li> <p>Manage permissions to a project to edit it in the Edit Project box</p> </li> 
    </ul> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos</p> <p>Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre el acceso a los proyectos, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Concesión de acceso a proyectos</a>. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> 
    <ul> 
     <li> <p>Contribuir con permisos a un proyecto para editarlo en el área Detalles del proyecto </p> </li> 
     <li> <p>Administre permisos de un proyecto para editarlo en el cuadro Editar proyecto</p> </li> 
    </ul> <p> Para obtener información sobre los permisos del proyecto, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Uso compartido de un proyecto en Adobe Workfront</a>.</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Limitaciones para editar proyectos

Existen algunas limitaciones que pueden impedir la edición de proyectos.

Tenga en cuenta lo siguiente al editar proyectos:

* Los proyectos que se encuentran en un proceso de aprobación no se pueden editar, salvo en el momento de registro.
* Puede adjuntar documentos o plantillas a un proyecto que tenga el estado Completado, Finalizado o Pendiente de aprobación solo si el administrador de Workfront o un administrador de grupo han activado esta funcionalidad en el área Preferencias del proyecto. Para obtener información sobre cómo definir las preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Solo se puede editar la siguiente información en un proyecto en estado Muerto o Completado:

   * Modificar los gastos existentes.
   * Agregar, quitar o editar formularios personalizados.

## Editar un proyecto

Al editar un proyecto, puede modificar la información y la configuración del proyecto, así como las tareas y los problemas del proyecto.

Algunos ajustes mencionados en este artículo pueden modificarse del estado predeterminado por su estado en la plantilla desde la que se creó el proyecto. Para obtener información sobre la edición de plantillas, consulte [Editar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Proyectos**.
1. (Opcional) Haga clic en **Proyectos en los que estoy** o **Proyectos de los que soy propietario** en la esquina superior derecha para mostrar los proyectos donde es el propietario o los proyectos donde forma parte del equipo del proyecto.

   ![](assets/projects-on-my-own-buttons-350x302.png)

1. Haga clic en el nombre del proyecto que desea editar para abrir la página del proyecto.

   >[!NOTE]
   >
   >Si es administrador de grupos, puede ver y editar los proyectos del grupo en el área Grupos y en el área Proyectos . Para obtener más información, consulte [Creación y modificación de los proyectos de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. (Opcional) Para editar información limitada sobre un proyecto, haga clic en **Detalles del proyecto** en el panel izquierdo.

   ![](assets/nwe-project-details-expanded-350x298.png)

   >[!NOTE]
   >
   >Según la forma en que el administrador de Workfront o el administrador de grupo hayan modificado la plantilla de diseño, los campos del área Detalles del proyecto podrían reorganizarse o no mostrarse. Para obtener más información, consulte [Personalización de la vista Detalles mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Para editar la información de la sección Detalles , haga lo siguiente:

   1. (Opcional) Haga clic en el **Contraer todo** en la esquina superior derecha para contraer todas las áreas.
   1. (Opcional y condicional) Cuando un área esté contraída, haga clic en el botón **flecha hacia la derecha** ![](assets/right-pointing-arrow.png) junto a cada área para expandir el área que desea editar.
   1. Para obtener más información sobre la edición de información en la ficha Detalles del proyecto , consulte los siguientes artículos:

      * [Administrar información en el área Información general del proyecto](../../../manage-work/projects/manage-projects/understand-project-overview-area.md)
      * [Administrar información en el área de finanzas del proyecto](../../../manage-work/projects/project-finances/manage-project-finance-area.md)
   1. (Opcional) Para adjuntar un formulario personalizado, empiece a escribir el nombre de un formulario en el **Agregar formulario personalizado** , selecciónelo cuando aparezca en la lista y haga clic en **Guardar cambios**.
   1. (Opcional) Haga clic en el **Exportar** icono ![](assets/export.png) para exportar la información general y de formularios personalizados a un archivo PDF, haga clic en **Exportar**. Seleccione una de las siguientes opciones:

      * Seleccionar todo (solo se muestra cuando hay al menos un formulario personalizado adjunto)
      * Información general
      * El nombre de uno o varios formularios personalizados

      El archivo del PDF se descarga a su equipo.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      Para obtener más información, consulte [Exportar formularios personalizados y detalles de objetos](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).
   Para obtener información sobre los campos visibles en la sección Detalles del proyecto , continúe editando el proyecto en el cuadro Editar proyecto como se describe a continuación.
1. Para editar toda la información sobre el proyecto, haga clic en el botón **Más** menú ![](assets/qs-more-menu.png) junto al nombre del proyecto y, a continuación, haga clic en **Editar**.

   O

   En una lista de proyectos, seleccione un proyecto y haga clic en el **Editar** icono ![](assets/edit-icon.png) en la parte superior de la lista.

   La variable **Editar proyecto** se abre.

   >[!IMPORTANT]
   >
   >Debe tener permisos de gestión para ver la opción Editar del proyecto.

   Todos los campos del proyecto están disponibles en el cuadro Editar proyecto y se agrupan por las áreas que aparecen en el panel izquierdo.

   >[!NOTE]
   >
   >Según la forma en que el administrador de Workfront o el administrador de grupo hayan modificado la plantilla de diseño, las áreas del panel izquierdo del cuadro Editar proyecto o cualquier campo enumerado en estas áreas se pueden reorganizar o no mostrar. Para obtener más información, consulte [Personalización de la vista Detalles mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. (Condicional) Si hizo clic en el **Más** y **Editar**, considere actualizar la información en cualquiera de las siguientes áreas enumeradas en el panel izquierdo:

   * [Nombre del proyecto](#project-name)
   * [Información general](#overview)
   * [Formularios personalizados](#custom-forms)
   * [Finanzas](#finance)
   * [Configuración de proyecto](#project-settings)
   * [Configuración de tarea](#task-settings)
   * [Configuración de problema](#issue-settings)
   * [Acceso](#access)

   >[!NOTE]
   >
   >Dependiendo de cómo configure el administrador de Workfront nuestra plantilla de diseño para el área Detalles del proyecto, las secciones y los campos del cuadro Editar proyecto pueden ser diferentes en el entorno. Para obtener más información, consulte [Personalización de la vista Detalles mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### Nombre del proyecto {#project-name}

1. Comience a editar el proyecto como se describe anteriormente.
1. Haga clic en **Nombre del proyecto** en el panel izquierdo.

   ![](assets/nwe-project-name-in-edit-project-box-350x125.png)

1. Actualice el nombre del proyecto.

   No se puede editar el nombre del proyecto cuando se editan proyectos de forma masiva.

### Información general {#overview}

1. Comience a editar el proyecto como se describe anteriormente.
1. Haga clic en **Información general** en el panel izquierdo.

   ![](assets/nwe-overview-in-edit-project-box-350x172.png)

1. Actualice la siguiente información sobre el proyecto:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Descripción</strong> </td> 
      <td> <p>Agregue información adicional sobre el proyecto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Estado</strong> </td> 
      <td> <p>Seleccione el estado del proyecto. No puede marcar un proyecto como Finalizado antes de que se hayan completado todas las tareas y problemas. Para obtener información sobre los estados de los proyectos, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref">Acceso a la lista de estados de proyectos del sistema</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioridad</strong> </td> 
      <td> <p> <p>Este es solo un indicador visual que le permite priorizar sus proyectos.</p> <p>Según las preferencias de proyecto seleccionadas por el administrador de Workfront, los nombres de las prioridades pueden ser diferentes para usted. Para obtener más información sobre las prioridades de edición, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Crear y personalizar prioridades</a></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Dirección URL</strong> </td> 
      <td> <p>Especifique un vínculo web relacionado con información sobre este proyecto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Tipo de condición</strong> </td> 
      <td> <p>Seleccione entre los siguientes tipos de condición: 
       <ul> 
       <li><strong>Manual:</strong> El propietario del proyecto establece la condición manualmente en el proyecto.</li> 
       <li><strong>Estado de progreso:</strong> Workfront establece automáticamente la condición en función del estado de progreso de las tareas en la ruta crítica. Para obtener más información sobre la comprensión del estado de progreso, consulte <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Información general sobre el estado de progreso de la tarea</a>.</li> 
       </ul><p>Su administrador de Workfront<span> o un administrador de grupo</span> selecciona el valor predeterminado para calcular la condición de los proyectos para su sistema <span>o su grupo</span>. Para obtener información sobre la configuración de los valores predeterminados del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>. </p></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Condición</strong> </td> 
      <td> <p> <p>(Solo se muestra después de seleccionar <strong>Manual</strong> para el <strong>Tipo de condición</strong>): Seleccione una condición para indicar cómo va el proyecto. </p> <p>Para obtener información sobre cómo se pueden configurar las condiciones del proyecto de forma automática o manual, consulte <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Descripción general de la condición y el tipo de condición del proyecto</a></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Modo de horario</strong> </td> 
      <td> <p>Especifique si el proyecto está programado desde la fecha de inicio o desde la fecha de finalización. Esta selección determina las fechas planificadas de las tareas del proyecto. 
       <ul> 
       <li><strong>Fecha de inicio</strong>: La primera tarea del proyecto tiene la misma fecha de inicio prevista que el proyecto de forma predeterminada. Para obtener información sobre la tarea Fecha de inicio planificada, consulte <a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Descripción general de la tarea Fecha de inicio planificada</a>. La línea de tiempo del proyecto calcula a partir de la fecha de inicio y la fecha de finalización del proyecto la calcula el sistema en función de la duración de todas las tareas. </li> 
       <li><strong>Fecha de finalización</strong>: La última tarea del proyecto tiene la misma fecha de finalización prevista que el proyecto. La línea de tiempo del proyecto se calcula a partir de la fecha de finalización y la fecha de inicio del proyecto se calcula mediante el sistema, restando la duración de todas las tareas de la fecha de finalización del proyecto. </li> 
       </ul><p>Su administrador de Workfront<span> o un administrador de grupo</span> selecciona la configuración predeterminada Modo de programación para su sistema o grupo. Para obtener información sobre la configuración de los valores predeterminados del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fecha y hora de inicio planificadas</strong> </td> 
      <td> <p> <p>Especifique la fecha cuando seleccione <strong>Programar desde fecha de inicio</strong>. <br></p> <p>Se trata de un campo de solo lectura al seleccionar <strong>Programar desde fecha de finalización</strong>.<br></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fecha y hora de finalización planificadas</strong> </td> 
      <td> <p>Especifique la fecha cuando seleccione <strong>Programar desde fecha de finalización</strong>. </p> <p>Se trata de un campo de solo lectura al seleccionar <strong>Programar desde fecha de inicio</strong>.<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Portafolio</strong></td> 
      <td>Indique a un Portfolio al que pertenece el proyecto. Primero debe crear un Portfolio, antes de que aparezca en la lista desplegable. Solo las carteras activas se pueden asociar a un proyecto. Para obtener más información sobre la creación de portafolios, consulte <a href="../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md" class="MCXref xref">Crear un portafolio </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Programar</strong></td> 
      <td> <p>Si seleccionó un Portfolio para el proyecto, especifique un Programa para el proyecto. Es posible que algunos Portfolio no tengan Programas. Primero debe crear un programa, antes de que aparezca en esta lista desplegable. Solo los programas activos se pueden asociar a un proyecto. </p> <p>Para obtener más información sobre la creación de programas, consulte <a href="../../../manage-work/portfolios/create-and-manage-programs/create-program.md" class="MCXref xref">Crear un programa</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Grupo</strong></td> 
      <td> <p> <p>Especifique el nombre del grupo asociado al proyecto. </p>Este campo es obligatorio. No puede tener un proyecto que no esté asociado a un grupo. </p> <p>Puede asegurarse de que está seleccionando el grupo correcto pasando el ratón por encima de él y haciendo clic en el icono de información <img src="assets/info-icon.png"> que se muestra junto a él. Esto muestra información sobre herramientas acerca del grupo, como la jerarquía de grupos por encima de él y sus administradores.</p> De forma predeterminada, uno de los siguientes grupos se asocia automáticamente a un proyecto cuando se crea, a menos que especifique un grupo diferente:</p> 
       <ul> 
       <li> <p><span>Cuando el proyecto se crea desde el área Proyectos , el grupo de inicio del creador del proyecto se asocia al proyecto.</span> </p> <p>Esto también ocurre cuando el proyecto se crea desde la sección Proyectos de un portafolio o programa.</p> </li> 
       <li> <p>Cuando el proyecto se crea a partir de la página principal de un grupo en el área Configuración, ese grupo se asocia al proyecto.</p> </li> 
       </ul> </p> <p> <img src="assets/group-details-widget-350x351.png" style="width: 350;height: 351;"> </p> 
       <p><b>NOTAS</b></p>

   <ul>
      <li><p>Si el proyecto, sus tareas o problemas están asociados a un estado personalizado de nivel de grupo, cambiar el grupo del proyecto puede provocar que el estado del proyecto, las tareas o los problemas cambien para que coincidan con el nuevo grupo.</p></li>
      <li><p>Si el proyecto, sus tareas o problemas ya están asociados a un proceso de aprobación de nivel de grupo mediante estados personalizados de nivel de grupo, cambiar el grupo podría crear un conflicto entre los estados de aprobación del grupo anterior y los existentes a nivel de sistema.</p>
      <p>Considere la posibilidad de eliminar los procesos de aprobación de nivel de grupo en el proyecto, o sus tareas o problemas antes de actualizar el grupo.</p>
      <p>Para obtener información sobre la creación de procesos de aprobación a nivel de grupo, consulte <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">Procesos de aprobación a nivel de grupo</a>.</p>
      <p>Para obtener información sobre la creación de un estado personalizado de nivel de grupo, consulte <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md" class="MCXref xref">Crear o editar un estado de grupo</a></p></li></ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Compañía</strong> </td> 
      <td> <p>Especifique una empresa asociada al proyecto. Debe crear una empresa para poder asociarla a un proyecto. Solo las empresas activas pueden asociarse con un proyecto. Para obtener información sobre la creación de empresas, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Crear y editar empresas</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Propietario del proyecto</strong> </td> 
      <td> <p>Empiece a escribir el nombre de un usuario para agregarlo al proyecto y, a continuación, selecciónelo cuando aparezca en la lista. El usuario se añade al equipo del proyecto y se le otorgan automáticamente permisos de gestión para el proyecto. El usuario designado como propietario del proyecto debe ser un usuario activo de Workfront.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Patrocinador de proyecto</strong> </td> 
      <td> <p>Empiece a escribir el nombre de un usuario para agregarlo al proyecto y, a continuación, selecciónelo cuando aparezca en la lista. El usuario se añade al equipo del proyecto y se le otorgan automáticamente los permisos de visualización del proyecto. El usuario designado como patrocinador del proyecto debe ser un usuario activo de Workfront.<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Gerente de recursos</strong> </td> 
      <td> <p> Empiece a escribir los nombres de los usuarios que desea agregar al proyecto y selecciónelos cuando aparezcan en la lista. Los usuarios se añaden al equipo del proyecto y se les asignan automáticamente permisos de gestión al proyecto, y pueden asignar recursos a las tareas y los problemas del proyecto. Los usuarios mantienen permisos de administración en el proyecto incluso cuando se eliminan del campo Administrador de recursos . Puede especificar más de un Administrador de recursos.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Al actualizar los campos Propietario del proyecto, Patrocinador del proyecto y Administrador de recursos, observe el avatar, la función principal del usuario o su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos. Los usuarios deben estar asociados con al menos una función de trabajo para verla a medida que los agrega.

1. (Opcional) Continúe editando las secciones siguientes, según la información que desee modificar.

   O

   Haga clic en **Guardar**.

### Formularios personalizados {#custom-forms}

Según el nivel de acceso y el permiso del proyecto, existen las siguientes situaciones:

* Si no tiene permisos de edición de formulario personalizado en el proyecto, no puede editar los campos de ninguno de los formularios personalizados adjuntos. Solo puede ver los campos de los formularios personalizados adjuntos al proyecto.
* Si tiene acceso de vista (y no de edición) a una sección de un formulario personalizado, no puede editar los campos de esa sección.
* Si no tiene acceso a una sección de uno de los formularios personalizados adjuntos al proyecto, la sección no se muestra en el cuadro Editar proyecto.

Al seleccionar más de un proyecto para editarlo de forma masiva, se dan las siguientes situaciones:

* Si no tiene permisos de edición de formularios personalizados en al menos uno de los proyectos seleccionados, no puede editar los campos de ninguno de los formularios personalizados adjuntos. Solo puede ver los campos en los formularios personalizados adjuntos
* Si tiene acceso de vista (y no de edición) a una sección de un formulario personalizado, no puede editar los campos de esa sección. Solo puede ver los campos de esa sección.
* Si no tiene acceso a una sección de uno de los formularios personalizados adjuntos al menos a uno de los proyectos, la sección no se muestra en el cuadro Editar proyectos .

Para obtener información sobre el acceso a formularios personalizados, consulte los siguientes artículos:

* [Compartir un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)
* [Agregar un salto de sección a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)

Para editar información sobre formularios personalizados:


1. Comience a editar el proyecto como se describe anteriormente.
1. Haga clic en **Forms personalizado** en el panel izquierdo.

   ![](assets/nwe-custom-forms-in-edit-project-box-350x170.png)

1. Haga clic en el **Agregar formulario personalizado** y seleccione un formulario de la lista para adjuntarlo al proyecto. De forma predeterminada, los 40 primeros formularios se muestran en orden alfabético. Si no ve el formulario en la lista, empiece a escribir su nombre y selecciónelo cuando aparezca en la lista.

   >[!NOTE]
   >
   >Debe crear los formularios personalizados antes de que estén disponibles para seleccionarlos en este campo. En la lista solo aparecen los formularios personalizados activos. Para obtener más información sobre la creación de formularios personalizados, consulte [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). Puede agregar hasta diez formularios personalizados a un proyecto.


1. (Condicional) Si adjuntó un formulario personalizado al proyecto, edite los campos del formulario. Debe especificar todos los campos obligatorios para poder guardar el proyecto.
1. (Opcional) Haga clic en el **Icono X** a la derecha del nombre de un formulario personalizado para quitarlo y, a continuación, haga clic en **Eliminar**.
1. (Opcional) Continúe editando las secciones siguientes, según la información que desee modificar

   O

   Haga clic en **Guardar**.

### Finanzas {#finance}

Según el nivel de acceso y el permiso del proyecto, existen las siguientes situaciones:

* Si tiene permiso Ver para acceder a Datos financieros y Ver finanzas en el proyecto, solo puede ver los campos de la sección Finanzas. Los campos de esta sección no se pueden editar.
* Si tiene permisos de edición para datos financieros y administración de finanzas en el proyecto, puede actualizar los campos de esta sección.

Al seleccionar más de un proyecto para editarlo de forma masiva y, existen los siguientes escenarios:

* Si selecciona al menos un proyecto en el que tiene permisos de Ver finanzas (en lugar de Administrar finanzas), solo puede ver los campos de esta sección para todos los proyectos seleccionados. Los campos de la sección Finanzas no se pueden editar de forma masiva.
* Si selecciona al menos un proyecto en el que no tiene permisos de financiación, esta sección no se muestra en absoluto.

Para editar campos en el área Finanzas:


1. Comience a editar el proyecto como se describe anteriormente.
1. Haga clic en **Finanzas** en el panel izquierdo.

   ![](assets/nwe-finance-in-edit-project-box-350x183.png)

1. Actualice la siguiente información financiera para el proyecto:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Divisa</strong> </td> 
      <td> <p> <p>Especifique la moneda del proyecto si es diferente a la moneda predeterminada del sistema. No puede cambiar la moneda de un proyecto si ya hay información financiera sobre el proyecto. Este campo no está visible si solo tiene la moneda predeterminada en el sistema. </p> <p>Para obtener más información sobre la moneda, consulte <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar tipos de cambio</a>.<br></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Presupuesto</strong> </td> 
      <td> <p>Especifique un presupuesto para el proyecto.<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Método de índice de rendimiento</strong> </td> 
      <td> <p>Select <b>Basado en horas</b>o <b>Basado en los costos</b> para indicar si las métricas Valor acumulado del proyecto (como Índice de rendimiento de costes o Costo real estimado) se calculan utilizando horas o costes. </p> <p>Para obtener más información sobre el método de índice de rendimiento, consulte <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Definir el método del índice de rendimiento (PIM)</a>. </p> <p>Su administrador de Workfront<span> o un administrador de grupo</span> selecciona la configuración predeterminada Método del índice de rendimiento para su sistema o grupo. Para obtener información sobre la configuración de los valores predeterminados del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Estimar al finalizar</strong> </td> 
      <td> <p> <p>Especifique cómo debe calcular Workfront la estimación al finalizar (EAC). </p>
      Seleccione entre las siguientes opciones: 
      <ul><li><b>Calcular a nivel de proyecto</b></li>
      <li><b>Resumir a partir de tareas/subtareas</b></li> </ul>
      <p>Para obtener más información sobre cómo se calcula la estimación al finalizar, consulte <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Calcular estimación al finalizar (CAO)</a>.</p> <p>El administrador de Workfront o de grupo selecciona la configuración predeterminada Estimación al finalizar para su sistema o grupo. Para obtener información sobre la configuración de los valores predeterminados del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Beneficio planificado</strong> </td> 
      <td> <p>Calcule cuál es el beneficio planeado del proyecto. Se utiliza en el caso empresarial del proyecto y en el optimizador de Portfolio. Para obtener más información sobre los beneficios planificados de un proyecto, consulte <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Descripción general de los beneficios previstos para el proyecto</a>. El beneficio planeado de un proyecto se tiene en cuenta cuando se calcula el valor neto de un proyecto. </p> <p>Para obtener más información, consulte <a href="../../../manage-work/portfolios/portfolio-optimizer/manage-projects-in-portfolio-optimizer.md" class="MCXref xref">Administrar proyectos en el Optimizador de Portfolio</a> .<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Beneficio real</strong> </td> 
      <td> <p>Calcular el beneficio real del proyecto. Se trata de una cantidad de divisa que representa el beneficio que su empresa o departamento obtendría una vez que se haya completado este proyecto. </p> </td> 
     </tr> 
      <tr> 
      <td role="rowheader"><strong>Costo fijo</strong> </td> 
      <td> <p>Especifique el costo fijo del proyecto. Esto es diferente al Coste de Trabajo que proviene de las horas del proyecto y el Coste de Gastos que proviene de la cantidad de gastos del proyecto. El coste fijo de un proyecto se tiene en cuenta al calcular el valor neto de un proyecto y forma parte del coste presupuestado.<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ingresos fijos</strong> </td> 
      <td> <p>Especifique los ingresos fijos del proyecto.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Continúe editando las secciones siguientes, según la información que desee modificar.

   O

   Haga clic en **Guardar**.

### Configuración de proyecto {#project-settings}

1. Comience a editar el proyecto como se describe anteriormente.
1. Haga clic en **Configuración del proyecto** en el panel izquierdo.

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. Actualice la siguiente información:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>Ruta de hitos</strong> </td> 
       <td> <p>Seleccione una ruta de Milestone para el proyecto. En la lista solo aparecen las rutas de hitos activas.</p> <p>Para obtener más información sobre las rutas de Milestone, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Crear una ruta de hitos</a>.</p> </td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Modo de finalización</strong> </td> 
      <td> <p>Controla cómo se marca el proyecto como Completado. Seleccione entre las siguientes opciones: 
       <ul> 
       <li><p><strong>Automático</strong>: El proyecto se marca como Completado cuando se completan todas las tareas y problemas.</p><p>El estado del proyecto se cambia automáticamente a Complete solo cuando el estado del proyecto es Current cuando se completan las tareas. </p></li> 
       <li><strong>Manual</strong>: Debe seleccionar manualmente el estado de finalización del proyecto cuando se hayan completado todas las tareas y problemas.</li> 
       </ul></p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Modo de finalización de resumen</strong></td> 
       <td> <p>Controla cómo se marcan las tareas principales como Completadas. Seleccione entre las siguientes opciones: 
       <ul> 
       <li><strong>Automático</strong>: Las tareas principales se marcan como Completadas y actualizan su porcentaje completado automáticamente, a medida que se completan las tareas secundarias y se actualiza el porcentaje completado de las tareas secundarias. </li> 
       <li><strong>Manual</strong>: Debe actualizar manualmente el porcentaje completado y el estado de las tareas principales, independientemente de los cambios realizados en las tareas secundarias.</li> 
       </ul></p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Tipo de actualización</strong></td> 
       <td> <p>Controla cuándo los cambios realizados en la línea de tiempo del proyecto se guardan en el proyecto o en las tareas principales. Por ejemplo, los siguientes cambios en el déclencheur del proyecto pueden actualizar la cronología del proyecto: 
       <ul> 
       <li>Actualizar las fechas de las tareas</li> 
       <li>Cambiar las relaciones predecesoras de las tareas</li> 
       <li><p>Cambiar las relaciones padre-hijo, agregar o quitar asignaciones además de cambiar la restricción de tarea o el tipo de duración.</p><p>Cuando se actualizan las tareas, sus objetos principales (tareas principales o el proyecto) se actualizan en el momento indicado por el tipo de actualización. </p><p>Si los objetos principales no se actualizan inmediatamente después del cambio al seleccionar Tipo de actualización "Automático y Activado" o "Solo cambio", actualice la página</p><p>Seleccione entre las siguientes opciones: </p><p>- <strong>Automático y en cambio</strong> (Configuración predeterminada): La cronología del proyecto se actualiza cada vez que se produce un cambio en el proyecto o en otro proyecto del que depende (al cambiar) el proyecto. La línea de tiempo del proyecto también se actualiza cada noche (automático).</p><p>Esta es la configuración recomendada para este campo porque garantiza que el proyecto esté siempre actualizado.</p><p>Cuando se realiza una acción en una tarea o proyecto que déclencheur un cálculo de línea de tiempo, se muestran inmediatamente todas las fechas disponibles, lo que le permite continuar trabajando. En proyectos con más de 100 tareas, las fechas que requieren nuevos cálculos se muestran brevemente como un signo de interrogación (entre 1 y 5 segundos o hasta un minuto para proyectos grandes). Esto indica que el nuevo cálculo aún no ha finalizado y que las fechas están sujetas a cambios.</p><p>- <strong>Cambiar solo</strong>: La cronología del proyecto se actualiza cada vez que se produce un cambio en el proyecto o en otro proyecto del que depende. Es posible que desee seleccionar esta opción si los cambios se producen con poca frecuencia en el proyecto o en otros proyectos de los que depende la cronología.</p><p>- <strong>Solo automático</strong>: La cronología del proyecto se actualiza cada noche; la cronología no se actualiza inmediatamente después de realizar los cambios.</p><p>Puede que desee seleccionar esta opción si se producen muchos cambios cada día en el proyecto o en otros proyectos de los que depende la cronología. Sin embargo, tenga en cuenta que eligió esta configuración, ya que el proyecto no se actualizará al mismo tiempo que se realizan los cambios.</p><p>- <strong>Solo manual</strong>: La línea de tiempo del proyecto solo se actualiza cuando selecciona la opción para volver a calcular la línea de tiempo. Para obtener más información sobre cómo volver a calcular manualmente la cronología del proyecto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Volver a calcular las líneas de tiempo del proyecto</a>. </p><p>Es posible que desee seleccionar esta opción si está realizando muchos cambios en el proyecto al mismo tiempo y desea que el cálculo de la cronología se produzca después de que se hayan realizado todos los cambios (en lugar de después de cada cambio individual).</p></li> 
       </ul></p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Horario</strong> </td> 
       <td> <p>Seleccione una programación para el proyecto. Debe ser la misma programación asignada a la mayoría de las personas que trabajan en el proyecto. Debe crear una programación para poder asignarla a un proyecto o a un usuario. Si no ha creado programas personalizados en su sistema, se selecciona la opción Programación predeterminada.</p> <p>Para obtener más información sobre la creación de programaciones, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Crear una programación</a>. </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Tiempo libre del usuario</strong> </td> 
       <td> <p>Determina si el tiempo de espera del usuario asignado principal de una tarea ajusta las fechas planificadas de la tarea en el proyecto. </p><p>Su administrador de Workfront<span> o un administrador de grupo</span> selecciona el valor predeterminado de esta configuración para su sistema <span>o su grupo</span>. Para obtener información sobre la configuración de los valores predeterminados del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>. </p><p>Seleccione entre las siguientes opciones:<br>- <strong>Considere el tiempo de espera del usuario en las duraciones de las tareas</strong>: Al seleccionar esta opción, las fechas planificadas de las tareas se ajustan según el tiempo de espera del Destinatario Principal de la tarea, si el tiempo de espera se produce durante la duración de la tarea. </p><p>Por ejemplo, si una tarea con una restricción de Tan pronto como sea posible está programada para empezar el 1 de junio y para completarse el 3 de junio, y el usuario asignado principal tiene marcado el 2 de junio como Tiempo de espera, cuando esta selección está habilitada, las fechas planificadas de la tarea son del 1 al 4 de junio. Según la restricción de tareas, existen los siguientes escenarios: </p> 
       <ul> 
       <li>En el caso de restricciones de tareas relacionadas con la planificación desde una fecha de inicio (tan pronto como sea posible, la hora más temprana disponible, el inicio no antes de, el inicio no después de, el inicio debe comenzar el), la fecha de inicio planeada no cambia, pero la fecha de finalización planeada cambia.</li> 
       <li>En el caso de restricciones de tarea relacionadas con la planificación desde una fecha de finalización (lo más tarde posible, la hora de finalización más reciente disponible, el fin no antes de, el fin no después de, el fin debe terminar el), la fecha de finalización planeada no cambia, pero la fecha de inicio planeada cambia.</li> 
       <li>Para las tareas con una restricción de Fechas fijas, ni el Inicio planificado ni la Fecha de Finalización cambian. </li> 
       </ul><p>La duración de la tarea no cambia al seleccionar esta configuración. Solo cambian las fechas planificadas, dependiendo de la restricción de tareas. Para obtener información sobre la restricción de tareas, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Información general sobre la restricción de tareas</a>. </p><p>- <strong>Ignorar el tiempo de espera del usuario en duraciones de tareas</strong>: Al seleccionar esta opción, las fechas planificadas de las tareas del proyecto se mantienen como estaba planificado originalmente, incluso si el Destinatario Principal de la tarea tiene tiempo de espera durante la duración de la tarea. </p><p>Tenga en cuenta lo siguiente al seleccionar opciones para esta configuración:</p> 
       <ul> 
       <li><p>La opción predeterminada para esta configuración para un nuevo proyecto es la misma que la preferencia de proyecto a nivel de sistema. </p><p>Para obtener información sobre las preferencias del proyecto en el nivel de sistema, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar las preferencias de proyecto de todo el sistema</a>. </p></li> 
       <li>Cuando se adjunta una plantilla a un proyecto existente, la configuración del proyecto se actualiza para que coincida con la de la plantilla. </li> 
       <li><p>Workfront decide qué fechas de tareas planificadas se ajustan según el valor de Restricción de tareas de la tarea. Dependiendo de lo que sea, ya sea el Inicio planificado o la Fecha de Finalización planificada, o ambos podrían verse afectados, o incluso seguir siendo iguales. Por ejemplo, si una tarea tiene una Restricción de Fechas Fijas, las fechas no se ajustan cuando el Destinatario Principal tiene tiempo de espera, incluso cuando <strong>Considere el tiempo de espera del usuario en las duraciones de las tareas</strong> está seleccionado. </p></li> 
       </ul></td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>Modo de nivelación de recursos</strong> </td> 
       <td> <p> <p>Seleccione entre las siguientes opciones:</p> <p>- <strong>Manual</strong>: debe nivelar manualmente los recursos (esta es la configuración predeterminada)</p> <p>- <strong>Automático</strong>: Workfront nivela sus recursos.</p> <p>Para obtener más información sobre la redistribución de recursos, consulte <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md" class="MCXref xref">Recursos de nivel en el diagrama de Gantt </a>.</p> </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>Riesgo</strong> </td> 
       <td> <p> <p>Defina el nivel de riesgo del proyecto. El riesgo es sólo un indicador de lo riesgoso que puede ser un proyecto. Puede priorizar la ejecución de sus proyectos en función del nivel de riesgo.</p> <p> <p>Considere la posibilidad de seleccionar entre los siguientes niveles de riesgo:</p> <p>- Muy bajo</p> <p>- Bajo</p> <p>- Medio</p> <p>- Alto</p> <p>- Muy alto</p> <p>Los niveles de riesgos que indica aquí no se pueden personalizar.</p> <p>Estas no están relacionadas con los riesgos potenciales que podrían producirse durante la vida de un proyecto y que debería registrar en la pestaña Riesgos del proyecto o en el caso de negocio. Para obtener información sobre posibles riesgos del proyecto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md" class="MCXref xref">Editar y crear tipos de riesgo</a>. </p> </p> </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>Conjuntos de recursos</strong> </td> 
       <td> <p> <p>Especifique los grupos de recursos asociados al proyecto. Los grupos de recursos son colecciones de usuarios que se necesitan al mismo tiempo para la finalización de un proyecto y permiten la presupuestación de proyectos en el Planificador de recursos. Para obtener más información sobre los grupos de recursos, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resumen de los grupos de recursos </a>. </p> <p>Cuando edita proyectos de forma masiva, solo aparecen en este campo los grupos de recursos comunes a todos los proyectos seleccionados. Si los proyectos seleccionados no tienen grupos de recursos compartidos, este campo estará vacío. Los grupos de recursos que especifique aquí sobrescribirán los grupos de recursos individuales de los proyectos.</p> </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <strong>Permitir que las tarifas de facturación a nivel de compañía anulen las tarifas a nivel de proyecto</strong></td> 
       <td>Seleccione esta opción para permitir que las tasas de facturación a nivel de empresa anulen las tasas de rol de trabajo históricas a menos que dichas tasas estén marcadas como facturadas. Al habilitar esta opción, se anulan las tasas de rol del trabajo histórico a menos que se marquen como facturadas. <br>Para obtener más información, consulte <a href="../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md" class="MCXref xref">Anular tasas de facturación a nivel de proyecto con tasas de facturación a nivel de empresa</a>.</td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>Requerir tiempo de aprobación de este proyecto</strong></td> 
       <td> <p> Seleccione esta opción para requerir que el propietario del proyecto apruebe el tiempo de registro en el proyecto. Si utiliza Registros de facturación y selecciona esta opción, solo las horas aprobadas del proyecto aparecerán como horas facturables disponibles para los Registros de facturación. El tiempo de aprobación del proyecto es independiente de la aprobación de las hojas de horas. </p> <p>Para obtener más información sobre la necesidad de aprobar un proyecto con tiempo, consulte <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" class="MCXref xref">Requerir tiempo para ser aprobado para un proyecto</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>Filtrar tipos de hora</strong> y</span> <strong>Tipos de hora</strong></td> 
       <td> <p> <p>Seleccione entre las siguientes opciones:</p> 
       <ul> 
       <li> <p>Select <strong>No</strong> para que todos los tipos de hora específicos del proyecto estén disponibles en el proyecto. (Esta es la selección predeterminada)</p> <p>O</p> </li> 
       <li>Select <strong>Sí</strong> para que solo un subconjunto de los tipos de hora específicos del proyecto esté disponible en el proyecto, seleccione los tipos de hora que desee poner a disposición. (Mantenga pulsada la tecla Mayús para seleccionar varios tipos de hora).</li> 
       <p>Si selecciona esta opción, solo los tipos de hora que seleccione estarán disponibles para seleccionarlos al iniciar sesión en el proyecto (o en las tareas y problemas dentro del proyecto). Debe seleccionar al menos un tipo de hora; si selecciona esta opción y no selecciona ningún tipo de hora, todos los tipos de hora estarán disponibles en el proyecto.</p> </ul>

   <p>Se deben realizar las mismas selecciones de hora a nivel de usuario individual para que el usuario vea estas opciones de tipo de hora en el proyecto. Para obtener más información sobre la definición de tipos de hora en el nivel de usuario, consulte <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Tiempo de registro</a>. </p> </p> </td> 
      </tr> 
      <tr data-mc-conditions=""> 
       <td role="rowheader"><strong>Notificación de recordatorio</strong> </td> 
       <td> <p> <p>Seleccione la notificación recordatoria que debe asociarse al proyecto. Debe configurar las Notificaciones de recordatorio para proyectos de este campo para que aparezcan durante la edición de un proyecto. Para obtener más información sobre la configuración de las notificaciones de recordatorio, consulte <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md"><a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configuración de notificaciones de recordatorio</a> .</a></p> </p> </td> 
      </tr> 
      <tr data-mc-conditions=""> 
       <td role="rowheader"><strong>Proceso de aprobación</strong></td> 
       <td> <p>Seleccione el proceso de aprobación que desea asociar al proyecto. El administrador de Workfront debe definir los procesos de aprobación a nivel de sistema para poder asociarlos a los proyectos. <span>Un usuario con acceso administrativo a procesos de aprobación también puede crear procesos de aprobación específicos del grupo.</span> Para obtener más información sobre la creación de procesos de aprobación, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Creación de un proceso de aprobación para elementos de trabajo</a>.</p> <p>Tenga en cuenta lo siguiente al agregar procesos de aprobación: </p> 
       <ul> 
       <li>En la lista solo se muestran los procesos de aprobación activos. </li> 
       <li> <p>En la lista se muestran los procesos de aprobación de todo el sistema y de grupos específicos. Un proceso de aprobación asociado a un grupo que no sea el del proyecto no se muestra en la lista.</p> <p>Si el grupo asociado con el proyecto cambia, el proceso de aprobación específico del grupo se convierte en un proceso de aprobación de un solo uso. Para obtener más información sobre cómo los cambios en el grupo del proyecto o en el proceso de aprobación afectan a la configuración de aprobación, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Efecto de los cambios en el grupo y el proceso de aprobación en los procesos de aprobación asignados</a>. </p> </li> <!--(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)-->
       <p>Cuando se editan proyectos de forma masiva, existen los siguientes escenarios:</p> 
       <ul> 
       <li> <p>Cuando se seleccionan proyectos del mismo grupo, en este campo se muestran tanto los procesos de aprobación de nivel de sistema como de grupo.</p> </li> 
       <li> <p>Cuando selecciona proyectos de diferentes grupos, en este campo solo se muestran los procesos de aprobación a nivel de sistema.</p> </li> 
       <li> <p>Cuando alguno de los proyectos tiene un proceso de aprobación de un solo uso adjunto, se reemplaza por el proceso de aprobación de nivel de sistema o de grupo que seleccione. </p> </li> 
      </ul> </td> 
      </tr> 
      <tr> 
      </tr> 
      </tbody> 
      </table>

1. (Opcional) Continúe editando las secciones siguientes, según la información que desee modificar.

   O

   Haga clic en **Guardar**.

### Configuración de tarea {#task-settings}

Puede definir los valores predeterminados que se asociarán a todas las tareas nuevas cuando las añada al proyecto.

Para obtener información sobre cómo afecta esta configuración a la creación de nuevas tareas, consulte la sección [Valores predeterminados de tarea al agregar tareas a un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-overview.md#understa) en el artículo [Información general sobre la creación de tareas](../../../manage-work/tasks/create-tasks/create-tasks-overview.md).

1. Comience a editar el proyecto como se describe anteriormente.
1. Haga clic en **Configuración de tareas** en el panel izquierdo.

   ![](assets/nwe-task-settings-in-edit-project-box-350x211.png)

1. En el **Proceso de aprobación predeterminado de tarea** , seleccione la tarea Proceso de aprobación que desea asociar con todas las tareas nuevas cuando las agregue al proyecto.

   El administrador de Workfront (o un usuario con acceso administrativo a procesos de aprobación) debe crear un proceso de aprobación de nivel de sistema para una tarea antes de poder asociarlo a un proyecto. En la lista solo se muestran los procesos de aprobación activos. Para obtener información sobre la creación de procesos de aprobación, consulte [Creación de un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md). Para obtener información sobre cómo los cambios en el grupo del proyecto o en el proceso de aprobación afectan a la configuración de aprobación, consulte [Efecto de los cambios en el grupo y el proceso de aprobación en los procesos de aprobación asignados](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

   Cuando se editan proyectos de forma masiva, existen los siguientes escenarios:

   * Cuando se seleccionan varios proyectos del mismo grupo, en este campo se muestran tanto los procesos de aprobación de tareas de nivel de sistema como los específicos de grupo.
   * Cuando selecciona varios proyectos de diferentes grupos, en este campo solo se muestran los procesos de aprobación de tareas a nivel de sistema.

1. En el **Forms personalizado predeterminado de tarea** , seleccione el formulario personalizado o los formularios que desea asociar a todas las tareas nuevas cuando los agregue al proyecto. Debe crear los formularios personalizados antes de que estén disponibles para seleccionarlos en este campo. En la lista solo aparecen los formularios personalizados activos. Para obtener más información sobre la creación de formularios personalizados, consulte [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). Puede asociar hasta diez formularios personalizados con una tarea.
1. (Opcional) Seleccione **Utilizar el esfuerzo de trabajo para calcular automáticamente las horas planificadas de la tarea** si desea habilitar la administración del esfuerzo de tareas utilizando Esfuerzo de trabajo en lugar de Horario planificado.

   ![](assets/nwe-work-effort-on-projects-350x182.png)

1. (Condicional y opcional) Si ha seleccionado Utilizar esfuerzo de trabajo para calcular automáticamente las horas planificadas de la tarea, haga clic en el menú desplegable de cada nivel de esfuerzo y seleccione un porcentaje para cada nivel. Los siguientes valores de porcentaje son valores predeterminados:

   | Tamaño | Porcentaje |
   |---|---|
   | Pequeño | 25% |
   | Medio | 50% |
   | Grande | 75% |

   >[!TIP]
   >
   >Cuando el tipo de actualización del proyecto está establecido en Automático y selecciona esta configuración, las horas planificadas de las tareas se actualizan según la duración de la tarea y el porcentaje del esfuerzo de trabajo, si están establecidos en cero. Para obtener más información sobre el uso de Esfuerzo de Trabajo para planificar el esfuerzo de una tarea, consulte [Información general sobre el esfuerzo de trabajo](../../../manage-work/tasks/task-information/work-effort.md).

1. (Opcional) Continúe editando las secciones siguientes, según la información que desee modificar.

   O

   Haga clic en **Guardar**.

### Configuración de problema {#issue-settings}

1. Comience a editar el proyecto como se describe anteriormente.
1. Haga clic en **Configuración de problemas** en el panel izquierdo.

   ![](assets/nwe-issue-settings-in-edit-project-box-350x306.png)

1. (Opcional) Anule la selección de **Permitir que los usuarios agreguen problemas en línea** . Se selecciona de forma predeterminada.

   Al anular la selección de esta opción, los usuarios no pueden añadir problemas en línea al proyecto o a las tareas de la sección Problemas .

   >[!TIP]
   >
   >Anule la selección de esta opción si desea obligar a los usuarios a completar los Nuevos campos de problema o los formularios personalizados asociados con nuevos problemas. Al permitir que los usuarios introduzcan problemas en línea, pueden evitar los campos Nuevo problema y los formularios personalizados al crear problemas. Para obtener información sobre la configuración de campos y formularios personalizados para problemas nuevos, consulte [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Al anular la selección de esta opción, los usuarios con permisos para agregar problemas al proyecto o las tareas pueden hacerlo de las siguientes maneras:

   * Haga clic en Nuevo problema en la parte superior de la lista de problemas en la sección Problemas del proyecto o de las tareas.
   * Cuando el proyecto se configura como una cola de solicitudes, pueden introducir una nueva solicitud en el área Solicitudes .

   >[!NOTE]
   >
   >Al editar proyectos de forma masiva, esta configuración se habilita si al menos un proyecto lo tiene habilitado y se deshabilita si todos los proyectos seleccionados lo tienen deshabilitado.

   <!--drafted for bulk edit projects: the statement above needs to be corrected when the new UI for bulk edit projects is updated; not sure if we'll need to describe this at all or we can cover this in  a "Considerations" mini section inside the Editing in bulk section below- ??? -->

1. (Opcional) Continúe editando las secciones siguientes, según la información que desee modificar.

   O

   Haga clic en **Guardar**.

### Acceso {#access}

1. Comience a editar el proyecto como se describe anteriormente.
1. Haga clic en **Acceso** en el panel izquierdo.

   ![](assets/nwe-access-in-edit-project-box-350x262.png)

1. Especifique lo siguiente **Acceso** información del proyecto:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Cuando alguien está asignado a una tarea</strong></td> 
      <td><p>Seleccionar de <strong>Ver</strong>, <strong>Contribute,</strong> o <strong>Administrar</strong> acceso a una tarea. Al usuario asignado a una tarea se le concede automáticamente este acceso a la tarea.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>También conceder acceso al proyecto</strong></td> 
      <td><p>Seleccionar de <strong>Ver</strong>, <strong>Contribute</strong>o <strong>Administrar</strong> acceso al proyecto. Al usuario asignado a una tarea también se le concede automáticamente este acceso al proyecto.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Cuando alguien está asignado a un problema</strong></td> 
      <td><p>Seleccionar de <strong>Ver</strong>, <strong>Contribute,</strong> o <strong>Administrar</strong> acceso a un problema. Al usuario asignado a un problema se le concede automáticamente este acceso al problema. Para obtener más información, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema </a>.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>También conceder acceso al proyecto</strong></td> 
      <td><p>Seleccionar de <strong>Ver</strong>, <strong>Contribute</strong>o <strong>Administrar</strong> acceso al proyecto. Al usuario asignado a un problema también se le concede automáticamente este acceso al proyecto.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Cuando alguien envía una solicitud: Proporcionarles acceso</strong></td> 
      <td><p>Seleccionar de <strong>Ver</strong>, <strong>Contribute</strong>o <strong>Administrar</strong> acceso a la solicitud. Cuando el proyecto también es una cola de solicitudes y un usuario envía una solicitud al proyecto, se le concede este acceso a la solicitud que presentó. Para obtener información sobre la configuración de un proyecto como cola de solicitudes, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Crear una cola de solicitud</a>.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Las personas de la misma compañía heredarán los mismos permisos en todas las solicitudes</strong></td> 
      <td><p>Seleccione este campo si desea que las personas de la misma empresa tengan el mismo acceso a todas las solicitudes del proyecto, tanto si las enviaron como si no.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Cuando alguien tiene acceso a este proyecto: Darles acceso a ...</strong></td> 
      <td><p>Seleccione las opciones de acceso que desea que tengan los usuarios en el proyecto si este se comparte con ellos. Seleccione las opciones específicas para su acceso si están designadas como <strong>Visualizadores</strong>, <strong>Colaboradores</strong>o <strong>Administradores</strong> al compartir el proyecto con ellos. </p><p>La variable <strong>Eliminar</strong> en la <strong>Administrar</strong> el nivel de permiso determina si los usuarios pueden eliminar el proyecto en sí. Usuarios con <strong>Administrar</strong> el acceso al proyecto puede eliminar tareas y problemas dentro del proyecto, independientemente de si esta opción está seleccionada o no, si tienen <strong>Administrar</strong> permisos para las tareas y los problemas. </p></td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.

## Editar un proyecto en el encabezado del proyecto (limitado)

Puede editar una cantidad limitada de información en el encabezado del proyecto.

El administrador del sistema o del grupo puede personalizar los campos que se ven en el encabezado del proyecto.

![](assets/project-header-350x18.png)

De forma predeterminada, los campos siguientes se incluyen en el encabezado del proyecto.

* Nombre de proyecto
* Propietario del proyecto
* Fecha y hora de finalización planificadas

   >[!NOTE]
   >
   >Este campo solo se puede editar si el proyecto está programado desde la Fecha de finalización. Cuando el proyecto está programado desde la fecha de inicio, Workfront calcula la fecha y hora de finalización planeada en función de la duración de las tareas.

* Condición

   >[!NOTE]
   >
   >Este campo solo se puede editar si el tipo de condición del proyecto es manual. Cuando el tipo de condición se establece en Estado de progreso, Workfront calcula la condición en función del progreso de las tareas. Para obtener más información, consulte [Descripción general de la condición y el tipo de condición del proyecto](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

* Estado
* Tome decisiones de aprobación si está configurado como aprobador en un proceso de aprobación actual

## Editar proyectos de forma masiva

Puede editar proyectos de forma masiva y actualizar la información de todos los proyectos seleccionados al mismo tiempo.


La información que está cambiando en todos los proyectos seleccionados sobrescribe la información existente en proyectos individuales, excepto en el campo Administrador de recursos .

Al agregar un nuevo administrador de recursos al editar proyectos de forma masiva, se agrega ese administrador a todos los proyectos seleccionados. Si otros administradores de recursos están asociados con los proyectos seleccionados, permanecen en los proyectos además del que se agregó mediante la edición masiva.

La edición de proyectos de forma masiva varía en función del entorno en el que elija actualizarlos.

### Editar proyectos de forma masiva en el entorno de producción

Para editar proyectos de forma masiva:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en **Proyectos**.
1. Seleccione varios proyectos de la lista.
1. Haga clic en **Editar**.

   La variable **Editar proyectos** se abre.

   ![](assets/edit-projects-in-bulk-nwe-350x303.png)

1. Especifique la información de todos los proyectos seleccionados en las secciones siguientes:

   * **Información general**

      Para obtener más información, consulte la [Información general](#overview) en este artículo.

   * **Finanzas**

      Para obtener más información, consulte la [Finanzas](#finance) en este artículo.

   * **Portafolio**

      Para obtener más información, consulte la sección &quot;Asociación de proyectos&quot; en la sección [Información general](#overview) en este artículo.

   * **Configuración**

      Para obtener más información, consulte la [Configuración del proyecto](#project-settings) en este artículo.

   * **Acceso**

      Para obtener más información, consulte la [Acceso](#access) en este artículo.

   * **Formularios personalizados**

      Para obtener más información, continúe con el paso 7 a continuación.

      <!--   
     <p>(NOTE:&nbsp;make sure this stays accurate)</p>   
     -->

   * **Tareas**

      Para obtener más información, consulte la [Configuración de tareas](#task-settings) en este artículo.

   * **Problemas**

      Para obtener más información, consulte la   [Configuración de problemas](#issue-settings) en este artículo.

   * **Comentario**

      Para obtener más información, continúe con el paso 9 a continuación.

      <!--   
     <p>(NOTE: ensure this step stays accurate)</p>   
     -->


1. (Opcional) En el área Configuración, seleccione cualquiera de las siguientes opciones:

   * **Volver a calcular costos e ingresos**: Seleccione esta opción para volver a calcular Costes e Ingresos en todos los proyectos seleccionados.
   * **Volver a calcular las líneas de tiempo**: Seleccione esta opción para volver a calcular las líneas de tiempo de todos los proyectos seleccionados.
   * **Volver a calcular los informes de valoración**: Seleccione esta opción para volver a calcular los valores del informe de valoración de todos los proyectos seleccionados.

   ![recalculate_cost_scorecards__etc_in_bulk_edit_for_projects.PNG](assets/recalculate-costs--scorecards--etc-in-bulk-edit-for-projects-350x225.png)

1. Haga clic en **Forms personalizado** para editar los formularios personalizados adjuntos a todos los proyectos seleccionados.

   Si los proyectos seleccionados no tienen formularios personalizados comunes, no se muestra ningún formulario en esta sección.

   Solo se pueden editar los campos de los formularios adjuntos a todos los proyectos seleccionados y que tienen permisos para editar.

1. (Opcional) En la sección Forms personalizado , seleccione el **Volver a calcular expresiones personalizadas** para asegurarse de que todos los campos personalizados calculados que se encuentran en la Forms personalizada adjunta a los proyectos seleccionados estén actualizados.

   >[!IMPORTANT]
   >
   >Se recomienda no seleccionar más de 500 proyectos al mismo tiempo que se vuelven a calcular las expresiones personalizadas.

1. (Opcional) Haga clic en **Comentario**, luego seleccione el cuadro Publicar una actualización en cada proyecto , especifique un comentario que desee mostrar en el flujo de actualizaciones del proyecto en el campo disponible y realice una de las siguientes acciones:

   * Haga clic en el **People** icono ![](assets/people-icon-updates-classic.png) para etiquetar a un usuario al que se notificará de su comentario.
   * Haga clic en el **Bloqueo** icono ![](assets/lock-icon-open-updates-classic.png) para restringir el comentario solo a personas de su empresa.

   Este comentario es visible para todas las personas con acceso de Vista al proyecto y con acceso para ver Notas.

1. Haga clic en **Guardar cambios**.

   Todos los cambios realizados ahora están visibles en todos los proyectos seleccionados.

<div class="preview">

### Editar proyectos en bloque en el entorno de vista previa

Tenga en cuenta lo siguiente al editar proyectos de forma masiva en el entorno de vista previa :

* Cuando se seleccionan proyectos que tienen diferentes valores para el mismo campo, el campo muestra un indicador &quot;Varios valores&quot; en el cuadro Editar proyectos. Los campos que son casillas de verificación, botones de opción y toggles tienen un indicador de &quot;Varios valores&quot; junto a ellos.

   ![](assets/multiple-values-indicator-dates-bulk-edit-projects.png)

* Además del indicador &quot;Varios valores&quot;, cuando las opciones seleccionadas son diferentes en al menos uno de los proyectos seleccionados, los campos con varias opciones se muestran de una de las siguientes maneras:

   * Los campos de casilla de verificación tienen una línea en lugar de una casilla de verificación para la opción que está activada para algunos pero no para todos los proyectos seleccionados.

      ![](assets/multiple-values-indicator-check-boxes-bulk-edit-projects.png)

   * Los campos de tipo de alternancia se muestran atenuados, con el botón de alternancia en el centro de la opción que está activada para algunos pero no para todos los proyectos seleccionados.

   ![](assets/multiple-values-highlighted-bulk-edit-projects.png)

   * Los campos de tipo botón de opción que tengan algunas opciones seleccionadas pero no todas, muestran todos los botones de opción como vacíos.

      ![](assets/multiple-values-indicator-radio-buttons-bulk-edit-projects.png)


* Al actualizar una opción en un campo de varias opciones (como un campo que se muestra como un conjunto de toggles o casillas de verificación), todas las demás opciones deben coincidir entre los proyectos seleccionados.

   >[!IMPORTANT]
   >
   >Por ejemplo, puede tener un campo de casilla de verificación con tres casillas de verificación (Opción 1, Opción 2 y Opción 3) y la Opción 1 está desmarcada para todos los proyectos, y la Opción 2 y 3 están seleccionadas para algunos proyectos y no están seleccionadas para otros que haya seleccionado. Si desea comprobar la opción 1 para todos los proyectos, también debe hacer que las opciones 2 y 3 coincidan para todos los proyectos seleccionados antes de poder guardar los cambios, por lo que debe seleccionarlos o desmarcarlos para que puedan coincidir en todos los proyectos seleccionados. Si no cambia ninguna de las opciones, puede guardar el campo tal cual y los proyectos mantienen su selección actual para todas las opciones.

* Cuando selecciona varios proyectos que pertenecen a grupos diferentes, los estados que aparecen en el campo Estado son estados de nivel de sistema y no estados de nivel de grupo.

Para editar proyectos en el entorno de vista previa:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.
1. Haga clic en **Proyectos**.
1. Seleccione varios proyectos de la lista.
1. Haga clic en el **Editar** icono ![](assets/edit-icon.png) en la parte superior de la lista.
La variable **Editar proyectos** se abre.

   ![](assets/edit-projects-in-bulk-modal-unshimmed.png)

Según la forma en que el administrador de Workfront o el administrador de grupo hayan modificado la plantilla de diseño, las áreas del panel izquierdo del cuadro Editar proyecto o cualquier campo enumerado en estas áreas se pueden reorganizar o no mostrar. Para obtener más información, consulte [Personalización de la vista Detalles mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Haga clic en **Información general** para editar información general sobre los proyectos seleccionados.  Para obtener más información sobre la edición del área Información general, consulte la sección [Información general](#overview) en este artículo.

   >[!TIP]
   >
   >Los campos que edite se muestran con un fondo morado claro.

1. Haga clic en **Forms personalizado** para editar, agregar o reemplazar formularios personalizados asociados a los proyectos seleccionados.

   Los formularios personalizados adjuntos a todos los proyectos seleccionados se muestran en la **Formularios personalizados en común** en la sección **Forms personalizado** .

   ![](assets/custom-forms-in-common-unshimmed.png)

   >[!TIP]
   >
   >   Los nombres de los formularios que son comunes a todos los proyectos seleccionados se muestran en el panel izquierdo del cuadro Editar proyectos .

1. Comience a escribir el nombre de un formulario personalizado en la sección **Agregar formulario personalizado** campo .


   ![](assets/forms-already-attached-indication-in-bulk-editing-projects-unshimmed.png)

   Los formularios personalizados que ya están adjuntos a los proyectos seleccionados se muestran en la **Formularios adjuntos** en la sección **Agregar formulario personalizado** campo .

   Los formularios personalizados adicionales que se pueden asociar a proyectos pero que no están adjuntos a ninguno de los proyectos seleccionados se muestran en la **Forms para agregar** en la sección **Agregar formulario personalizado** campo .

1. Haga clic en para seleccionar el formulario personalizado adicional en el **Agregar formulario personalizado** o **Forms para agregar** subsecciones cuando aparecen en la lista.

   Cuando un formulario personalizado ya está adjunto a algunos de los proyectos seleccionados, al agregar un formulario aparece una indicación junto al nombre del formulario, cuántos proyectos ya tienen seleccionado el formulario.

1. (Opcional) Haga clic en el **x** a la derecha del nombre de un formulario personalizado y haga clic en **Eliminar** para eliminarlo de todos los proyectos seleccionados.

   >[!CAUTION]
   >
   >La eliminación de formularios personalizados hace que se pierda toda la información de campo personalizado existente en los formularios. Esto no se puede recuperar.

   Para obtener más información sobre la edición de formularios personalizados, consulte la sección [Forms personalizado](#custom-forms) en este artículo.

1. Haga clic en **Finanzas** para editar la información financiera de todos los proyectos seleccionados.
Para obtener más información sobre la edición del área de finanzas, consulte la sección [Finanzas](#finance) en este artículo.
1. Haga clic en **Configuración del proyecto** para editar la configuración de todos los proyectos seleccionados.
Para obtener más información sobre la edición del área Configuración del proyecto , consulte la sección [Configuración del proyecto](#project-settings) en este artículo.
1. Haga clic en **Configuración de tareas** para editar la configuración de tareas de todos los proyectos seleccionados.
Para obtener más información sobre la edición del área Configuración de tareas , consulte la sección [Configuración de tareas](#task-settings) en este artículo.
1. Haga clic en **Configuración de problemas** para editar la configuración de problemas de todos los proyectos seleccionados.
Para obtener más información sobre la edición del área Configuración de problemas , consulte la sección [Configuración de problemas](#issue-settings) en este artículo.
1. Haga clic en **Acceso** para editar la configuración de acceso de todos los proyectos seleccionados.
Para obtener más información sobre la edición del área de acceso, consulte la sección [Acceso](#access) en este artículo.
1. (Opcional) Para eliminar cualquier información agregada en el cuadro Editar proyectos , pase el ratón sobre un campo editado y haga clic en el botón **x** deseche el icono situado en la parte superior derecha del campo .

   ![](assets/discard-icon-for-field-edit-projects-in-bulk-unshimmed.png)

1. (Opcional) Haga clic en **Cancelar** en la parte inferior del **Editar proyectos** para eliminar todos los cambios realizados en todos los proyectos.
1. Haga clic en **Guardar**.

</div>

