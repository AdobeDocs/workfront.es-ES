---
product-area: projects
navigation-topic: create-projects
title: Crear un proyecto
description: Un proyecto es una gran unidad de trabajo en Adobe Workfront. Puede crear proyectos desde cero, utilizar una plantilla o convertir problemas o tareas a proyectos.
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
source-git-commit: 9125e2f7dbff41625166dcd358bab44d7c1b971b
workflow-type: tm+mt
source-wordcount: '1371'
ht-degree: 1%

---

# Crear un proyecto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is linked from the UI from the Projects global nav section in classic. Do not change/ remove)</p>
-->

Los proyectos representan una gran cantidad de trabajo que debe realizarse en Adobe Workfront.

## Requisitos de acceso

<!--drafted for P&P - replace table below with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td role="rowheader">plan de Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre el acceso a los proyectos, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Concesión de acceso a proyectos</a>. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Cuando crea un proyecto, automáticamente recibe permisos de administración para el proyecto </p> <p> Para obtener información sobre los permisos del proyecto, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Uso compartido de un proyecto en Adobe Workfront</a>.</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Formas de crear proyectos

Puede crear un proyecto en Workfront mediante uno de los métodos siguientes:

* Cree un proyecto desde cero sin usar una plantilla. En este artículo se describe cómo crear un proyecto desde cero.

* Copie un proyecto existente.\
   Para obtener más información sobre cómo copiar un proyecto, consulte [Copiar un proyecto](../../../manage-work/projects/manage-projects/copy-project.md).

* Utilice una plantilla.\
   Para obtener más información sobre el uso de una plantilla para crear un nuevo proyecto, consulte [Creación de un proyecto mediante una plantilla](../../../manage-work/projects/create-projects/create-project-from-template.md).

* Importar un proyecto desde Microsoft Project.\
   Para obtener más información sobre la importación de un proyecto desde MS Project, consulte [Importar un proyecto desde un proyecto de Microsoft](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* Importar un proyecto mediante los primeros pasos.

   Como administrador de Workfront, puede importar proyectos mediante un inicio.

   Para obtener información sobre la importación de datos mediante el inicio en Workfront, consulte [Importar datos en Adobe Workfront mediante una plantilla de inicio rápido](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md) .

   Para obtener información sobre la importación de proyectos mediante la introducción, consulte [Caso Kick-Starts : preparación sencilla de importación de proyectos y tareas](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md) .

* Publique una iniciativa desde un escenario en el planificador de escenarios de Adobe Workfront. El planificador de escenarios requiere una licencia adicional. Para obtener información sobre el planificador de escenarios de Workfront, consulte [Información general del planificador de escenarios](../../../scenario-planner/scenario-planner-overview.md). Para obtener información sobre la creación de proyectos a partir de iniciativas de publicación, consulte  [Actualizar o crear proyectos publicando iniciativas en el Planificador de escenarios](../../../scenario-planner/publish-scenarios-update-projects.md).

## Requisitos previos

Antes de empezar, debe asegurarse de que

* El administrador del sistema o del grupo habilitó la preferencia &quot;Permitir a los usuarios crear proyectos sin usar una plantilla&quot; en el área Configuración.

   Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Nueva configuración predeterminada del proyecto

Al crear un proyecto, Workfront le aplica un conjunto de ajustes predeterminados. Por ejemplo, el estado, el grupo o el modo de programación están predefinidos al crear un proyecto.

Tenga en cuenta lo siguiente:

* Como administrador de Workfront o de un grupo, puede configurar las opciones predeterminadas de un nuevo proyecto al configurar las preferencias de proyecto para la instancia de Workfront o para un grupo.
* Workfront aplica la configuración del grupo, si la hay, antes de aplicar las establecidas por el administrador de Workfront.
* El estado predeterminado de un nuevo proyecto corresponde al estado definido por el administrador de Workfront en el área principal Preferencias del proyecto o por un administrador de grupo (o administrador de Workfront) en el área Preferencias del proyecto de un grupo.

   >[!NOTE]
   >
   >Se recomienda que el estado predeterminado de un nuevo proyecto sea Planning. A medida que realiza cambios en el nuevo proyecto, esto garantiza que las notificaciones no tengan déclencheur con los usuarios asignados al proyecto.
   >
   >Para obtener más información sobre la configuración del estado predeterminado y otros ajustes predeterminados de un nuevo proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) o [Configuración de las preferencias de un proyecto para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

* Existen los siguientes escenarios para la forma en que Workfront define el grupo y el estado de un nuevo proyecto:

   * Si crea un proyecto desde cero, el grupo del proyecto es su grupo de inicio.

      El estado del proyecto es el estado predeterminado en las preferencias de proyecto de su grupo principal, si existe, o de su instancia de Workfront. Puede cambiar el estado predeterminado al crear el proyecto a cualquier estado disponible para el Grupo del proyecto.

   * Si crea un proyecto con una plantilla, la configuración de la plantilla tiene prioridad sobre la configuración establecida por el administrador de Workfront o del grupo.

      El Grupo del nuevo proyecto es el Grupo de la plantilla. Si la plantilla no está asociada a un grupo, el grupo del proyecto es el grupo de inicio del usuario que crea el proyecto.

      El estado predeterminado de un nuevo proyecto creado a partir de una plantilla se corresponde con el estado definido por el administrador de Workfront en el área principal Preferencias del proyecto o por un administrador de grupo (o administrador de Workfront) en el área Preferencias del proyecto del grupo. Puede cambiar el estado predeterminado al crear un proyecto de una plantilla a cualquiera de los estados del Grupo del proyecto que sea el Grupo de la plantilla o el Grupo Principal del usuario que crea el proyecto.

   * Si crea un proyecto convirtiendo un problema, el grupo de un nuevo proyecto es el grupo del proyecto existente del problema. Si el usuario que convierte el problema no tiene acceso al proyecto del problema o si el proyecto del problema no tiene un grupo, el grupo del nuevo proyecto es el grupo principal del usuario que está convirtiendo el problema.

      Los estados del nuevo proyecto coinciden con los estados de grupo del grupo asociado al proyecto que es el Grupo del proyecto original o el Grupo Principal del usuario que está convirtiendo el problema.

      Si utiliza una plantilla cuando esté creando el proyecto convirtiendo el problema, consulte el segundo escenario anterior para comprender qué grupo y qué estado Workfront aplica al nuevo proyecto.

## Crear un proyecto desde cero

1. Realice una de las siguientes acciones:

   * Haga clic en el **Menú principal** ![](assets/main-menu-icon.png), haga clic en **Proyectos** y, a continuación, expanda **Nuevo proyecto**.
   * Vaya a un portafolio y, a continuación, expanda **Nuevo proyecto**.

      >[!TIP]
      >
      >Cuando crea un proyecto utilizando una plantilla de un portafolio, el campo Portfolio del nuevo proyecto se actualiza para mostrar el portafolio desde el que eligió crear el proyecto. Esto sobrescribe el campo Portfolio de la plantilla, si se especifica.

   * Vaya a un programa y, a continuación, expanda **Nuevo proyecto**.

      >[!TIP]
      >
      >Cuando crea un proyecto utilizando una plantilla de un programa, se actualiza el campo Program de los nuevos proyectos para mostrar el Programa que ha elegido para crear el proyecto. El campo Portfolio de la plantilla se actualiza para mostrar el portafolio del programa desde el que ha elegido crear el proyecto. Esto sobrescribe los campos Programa y Portfolio de la plantilla, si se especifican.

   * Si es administrador de un grupo, también puede crear un proyecto en la sección Proyectos de un grupo que administre. Para obtener más información, consulte [Creación y modificación de los proyectos de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

      >[!TIP]
      >
      >Cuando se crea un proyecto con una plantilla de un grupo, el grupo desde el que se crea el proyecto se muestra en el campo Grupo del nuevo proyecto solo cuando no se especifica el campo Grupo de la plantilla. Si se especifica el campo Grupo de plantilla, el campo Grupo del nuevo proyecto es el de la plantilla.
   ![](assets/new-project-dropdown-nwe-350x358.png)

1. Haga clic en **Nuevo proyecto** si desea crear un proyecto desde cero.
1. Escriba un nombre para el proyecto. Pulse Intro para guardar el nombre.

   ![](assets/untitled-project-rename-new-project-nwe-350x127.png)

   El encabezado de la página del proyecto muestra información general rápida sobre el estado actual y el progreso de un proyecto. La información del encabezado del proyecto cambia a medida que se actualiza la información del proyecto.

1. Haga clic en **Empezar a añadir** **Tareas**.

   O

   Haga clic en **Nueva tarea** para agregar tareas al proyecto y asignarles recursos.\
   Para obtener más información sobre cómo agregar tareas a un proyecto, consulte [Crear tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Edite los detalles del proyecto haciendo clic en el botón **Más menú** y luego **Editar** ![](assets/qs-edit-icon.png) junto al nombre del proyecto.

   La variable **Editar proyecto** se abre.

   Para obtener más información sobre cómo editar un proyecto, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

1. (Opcional) Después de configurar los ajustes del proyecto y agregar las tareas, puede cambiar el estado del proyecto a **Actual**.

   Esto indica que el proyecto ya está listo para iniciarse y que los usuarios asignados a las tareas ahora pueden empezar a trabajar en ellos.

   Para obtener más información sobre los estados de los proyectos, consulte [Acceso a la lista de estados de proyectos del sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).
