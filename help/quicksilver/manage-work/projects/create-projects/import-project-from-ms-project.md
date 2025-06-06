---
product-area: projects
navigation-topic: create-projects
title: Importar un proyecto desde Microsoft Project
description: Puede importar proyectos de Microsoft Project a Adobe Workfront y administrar todos los proyectos en una aplicación. Cada vez que se importa un proyecto desde Microsoft Project, se crea un nuevo proyecto en Workfront.
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: b38c98ec79617a78c76510bcb109da2ff83247af
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 67%

---

# Importar un proyecto desde Microsoft Project

<!-- Audited: 4/2025 -->

Puede importar proyectos de Microsoft Project a Adobe Workfront y administrar todos los proyectos en una aplicación. Cada vez que se importa un proyecto desde Microsoft Project, se crea un nuevo proyecto en Workfront.

>[!IMPORTANT]
>
>No todos los campos de Microsoft Project se transfieren a Workfront.
>
>Para obtener más información sobre la compatibilidad de campos entre Workfront y Microsoft Project, vea [Asignar campos de Microsoft Project a proyectos de Adobe Workfront](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Nuevo: estándar </p> 
   O
   <p>Actual: plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso</td> 
   <td> <p>Acceso de edición a proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Al crear un proyecto, se reciben automáticamente permisos de administración para ese proyecto </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--old permissions model: 

You must have the following access to perform the steps in this article:

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
   <td> <p>Plan </p> </td> 
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

## Creación de un proyecto a partir de un MS Project

Puede crear un proyecto a partir del área de **Proyectos** en el **Menú principal**, o a partir del área de **Proyectos** de un portafolio o programa.

1. Inicie sesión en el proyecto de Microsoft y abra un proyecto que desee importar en Workfront.
1. Haga clic en **Archivo** y, a continuación, en **Guardar como** para guardar el proyecto como un archivo .xml.

1. Inicie sesión en Workfront.
1. Realice una de las siguientes acciones:

   * Haga clic en el **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Workfront o haga clic en **Menú principal** ![Líneas del menú principal](assets/lines-main-menu.png) en la esquina superior izquierda, si está disponible, haga clic en **Proyectos** y expanda **Nuevo proyecto**.
   * Vaya a un portafolio y expanda **Nuevo proyecto**.
   * Vaya a un programa y expanda **Nuevo proyecto**.
   * Si es administrador de grupo, puede crear un proyecto en la sección **Proyectos** de un grupo que administre. Para obtener más información, vea [Crear y modificar proyectos de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. Haga clic en **Importar MS Project**. Aparece el cuadro de diálogo **Importar archivo de MS**.

   ![Nuevo menú desplegable de proyecto](assets/import-ms-project-option.png)

1. Haga clic en **Seleccionar archivo** y, a continuación, busque el archivo .xml en el equipo que exportó desde Microsoft Project.
1. Importe el archivo seleccionado. Workfront inicia el proceso de importación y crea un nuevo proyecto basado en el archivo exportado desde Microsoft Project.

   Una vez completado el proceso de importación, se le dirigirá a la nueva página del proyecto, en la que se muestra la confirmación de que la importación se ha completado correctamente.

   >[!NOTE]
   >
   >Workfront tiene una limitación de tiempo de 15 minutos en las cargas de archivos. Si la carga del archivo tarda más, le recomendamos que divida el proyecto en proyectos más pequeños y que los importe por separado. Una vez importados en Workfront, mueva las tareas de un proyecto a otro para combinarlas en un solo proyecto. Para obtener más información sobre cómo mover tareas, vea [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

1. (Opcional) Continúe editando el proyecto en Workfront. Para obtener información sobre cómo editar proyectos, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).


   >[!NOTE]
   >
   >El estado de un nuevo proyecto creado a partir de una plantilla corresponde al estado definido por el administrador de Workfront en el área de **Preferencias del proyecto** o por un administrador de grupo en el área de **Preferencias del proyecto de grupo**. Para obtener información sobre cómo configurar las preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
