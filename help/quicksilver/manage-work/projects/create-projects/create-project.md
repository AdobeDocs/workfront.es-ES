---
product-area: projects
navigation-topic: create-projects
title: Crear un proyecto
description: Un proyecto es una gran unidad de trabajo en Adobe Workfront. Puede crear proyectos desde cero, utilizar una plantilla o convertir problemas o tareas en proyectos.
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '1390'
ht-degree: 85%

---

# Crear un proyecto

<!--remove Preview and Production references-->

<!-- Audited: 12/2023 -->

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

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
+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nuevo: estándar</p>
        <p>o</p>
        <p>Actual: plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Al crear un proyecto, recibirá automáticamente permisos de Administración en el proyecto.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Formas de crear proyectos

Puede crear un proyecto en Workfront mediante uno de los métodos siguientes:

* Cree un proyecto desde cero sin usar una plantilla. Este artículo describe cómo crear un proyecto desde cero.

* Copie un proyecto existente.\
  Para obtener más información sobre cómo copiar un proyecto, consulte [Copiar un proyecto](../../../manage-work/projects/manage-projects/copy-project.md).

* Utlice una plantilla.\
  Para obtener más información sobre cómo usar una plantilla para crear un nuevo proyecto, consulte [Crear un proyecto a partir de una plantilla](../../../manage-work/projects/create-projects/create-project-from-template.md).

* Importe un proyecto desde Microsoft Project.\
  Para obtener más información sobre cómo importar un proyecto desde MS Project, consulte [Importar un proyecto desde Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* Importe un proyecto mediante kick-starts.

  Como administrador de Workfront, puede importar proyectos mediante kick-start.

  Para obtener información acerca de cómo importar datos mediante kick-starts en Workfront, consulte [Importar datos en Adobe Workfront a través de una plantilla de Kick-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

  Para obtener información sobre la importación de proyectos mediante los puntapiés inicial, consulte [Escenario de Kick-Starts: preparación sencilla de importación de proyectos y tareas](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md).

* Publique una iniciativa desde un escenario en Adobe Workfront Scenario Planner.

  El planificador de escenarios requiere una de las siguientes opciones:

   * Licencia adicional para la estructura de licencias actual de Workfront.
   * Licencia de Ultimate para la nueva estructura de licencias de Workfront.

  Para obtener información sobre el Planificador de escenarios de Workfront, consulte [Información general sobre el Planificador de escenarios](../../../scenario-planner/scenario-planner-overview.md). Para obtener información acerca de cómo crear proyectos a partir de iniciativas de publicación, consulte [Actualizar o crear proyectos mediante la publicación de iniciativas en el Planificador de escenarios](../../../scenario-planner/publish-scenarios-update-projects.md).

* Agregue proyectos a medida que los conecte desde un tipo de registro en Workfront Planning. En el entorno Producción, solo se pueden crear proyectos sin plantillas desde Workfront Planning. <span class="preview">Puede crear proyectos utilizando una plantilla en el entorno de vista previa.</span>

  Debe tener una nueva licencia de Workfront y una licencia adicional de Workfront Planning para Workfront Planning.

  Para obtener información sobre el acceso a Workfront Planning, consulte [Información general sobre el acceso](/help/quicksilver/planning/access/access-overview.md).

  Para obtener información acerca de cómo crear proyectos agregándolos a registros, vea la sección &quot;Crear proyectos al conectarlos con registros de Workfront Planning&quot; en el artículo [Crear objetos de Workfront desde Workfront Planning al conectarlos a registros](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)

## Requisitos previos

Antes de empezar, debe asegurarse de que:

* El administrador del sistema o del grupo ha habilitado la preferencia “Permitir que los usuarios creen proyectos sin usar una plantilla” en el área de Configuración.

  Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Nueva configuración predeterminada del proyecto

Al crear un proyecto, Workfront le aplica un conjunto de configuraciones predeterminadas. Por ejemplo, Estado, Grupo y Modo de programación están preestablecidos al crear un proyecto.

Tenga en cuenta lo siguiente:

* Como administrador de Workfront o de un grupo, puede establecer la configuración predeterminada para un nuevo proyecto al configurar las Preferencias del proyecto para toda la instancia de Workfront o para un grupo.
* Workfront aplica la configuración del grupo, si la hay, antes de aplicar las establecidas por el administrador de Workfront.
* El estado predeterminado de un nuevo proyecto corresponde al estado definido por el administrador de Workfront en el área principal Preferencias del proyecto o por un administrador de grupos (o administrador de Workfront) en el área Preferencias del proyecto para un grupo.

  >[!NOTE]
  >
  >Se recomienda que el estado predeterminado de un nuevo proyecto sea Planificando. A medida que realiza cambios en el nuevo proyecto, esto garantiza que no se envíen notificaciones a los usuarios asignados al proyecto.
  >
  >Para obtener más información acerca de cómo configurar el estado predeterminado y otras opciones predeterminadas para un nuevo proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) o [Configurar las preferencias de proyecto para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

* Existen los siguientes escenarios para la forma en que Workfront define el grupo y el estado de un nuevo proyecto:

   * Si crea un proyecto desde cero, el grupo del proyecto es su Grupo de inicio.

     El estado del proyecto es el estado predeterminado en las Preferencias del proyecto de su Grupo de inicio, si hay uno, o de su instancia de Workfront. Puede cambiar el estado predeterminado al crear el proyecto a cualquier estado disponible para el Grupo del proyecto.

   * Si crea un proyecto a partir de una plantilla, la configuración de la plantilla tiene prioridad sobre la configuración establecida por el administrador de Workfront o del grupo.

     El Grupo del nuevo proyecto es el Grupo de la plantilla. Si la plantilla no está asociada a un Grupo, el Grupo del proyecto es el Grupo de inicio del usuario que crea el proyecto.

     El estado predeterminado de un nuevo proyecto creado a partir de una plantilla corresponde al estado definido por el administrador de Workfront en el área principal Preferencias de proyecto o por un administrador de grupos (o administrador de Workfront) en el área Preferencias de proyecto para el grupo. Puede cambiar el estado predeterminado al crear un proyecto a partir de una plantilla, a cualquiera de los estados del Grupo del proyecto que es el Grupo de la plantilla o el Grupo de inicio del usuario que crea el proyecto.

   * Si crea un proyecto convirtiendo un problema, el grupo de un nuevo proyecto es el Grupo del proyecto existente del problema. Si el usuario que convierte el problema no tiene acceso al proyecto del problema o si el proyecto del problema no tiene un grupo, el grupo del nuevo proyecto es el Grupo de inicio del usuario que convierte el problema.

     Los estados del nuevo proyecto coinciden con los estados de grupo del grupo asociado con el proyecto, que es el Grupo del proyecto original o el Grupo de inicio del usuario que convierte el problema.

     Si está utilizando una plantilla al crear el proyecto mediante la conversión del problema, consulte el segundo escenario anterior para comprender qué grupo y qué estado aplica Workfront al nuevo proyecto.

## Creación de un proyecto desde cero

>[!NOTE]
>
>Si está creando un proyecto a partir de una plantilla, le recomendamos que también consulte el artículo [Crear un proyecto a partir de una plantilla](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).


1. Realice una de las siguientes acciones:

   * Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) de la esquina superior derecha de Adobe Workfront o (si está disponible), en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) de la esquina superior izquierda. Haga clic en **Proyectos** y, a continuación, expanda **Nuevo proyecto**.
   * Vaya a un portafolio y expanda **Nuevo proyecto**.
   * Vaya a un programa y expanda **Nuevo proyecto**.
   * Si es administrador de un grupo, también puede crear un proyecto en la sección Proyectos de un grupo que administre. Para obtener más información, consulte [Crear y modificar proyectos de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

   ![Menú de Nuevo proyecto](assets/new-project-dropdown-nwe-350x358.png)

1. Haga clic en **Nuevo proyecto** en el menú para crear un proyecto desde cero.
1. Escriba un nombre diferente para el proyecto. Pulse Intro para guardar el nombre.

   ![Introducir un nombre para el proyecto](assets/rename-untitled-project.png). 

   El encabezado de la página del proyecto muestra una descripción general rápida del estado y el progreso actuales de un proyecto. La información del encabezado del proyecto cambia a medida que se actualiza la información del proyecto.

1. Pulse **Añadir la adición de tareas**.

   O

   Haga clic en **Nueva tarea** para añadir tareas al proyecto y asignarles recursos.

   Para obtener más información sobre cómo añadir tareas a un proyecto, consulte [Crear tareas en un proyecto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Edite los detalles del proyecto haciendo clic en el menú **Más** y, a continuación, **Editar** ![Editar icono](assets/qs-edit-icon.png) junto al nombre del proyecto.

   Se abre el cuadro de diálogo **Editar proyecto**.

   Para obtener más información sobre cómo editar un proyecto, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

1. (Opcional) Después de configurar el proyecto y añadir las tareas, puede cambiar el estado del proyecto a **Al día**.

   Esto indica que el proyecto está listo para iniciarse y que los usuarios asignados a las tareas pueden empezar a trabajar en él.

   Para obtener más información acerca de los estados de los proyectos, consulte [Acceso a la lista de estados de proyectos del sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).
