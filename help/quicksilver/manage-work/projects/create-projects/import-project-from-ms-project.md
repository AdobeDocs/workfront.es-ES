---
product-area: projects
navigation-topic: create-projects
title: Importar un proyecto desde Microsoft Project
description: Puede importar proyectos de Microsoft Project a Adobe Workfront y administrar todos los proyectos en una aplicación. Cada vez que se importa un proyecto desde un proyecto de Microsoft, se crea un nuevo proyecto en Workfront.
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 1%

---

# Importar un proyecto desde Microsoft Project

Puede importar proyectos de Microsoft Project a Adobe Workfront y administrar todos los proyectos en una aplicación. Cada vez que se importa un proyecto desde un proyecto de Microsoft, se crea un nuevo proyecto en Workfront.

>[!IMPORTANT]
>
>No todos los campos de Microsoft Project se transfieren a Workfront.
>
>Para obtener más información sobre la compatibilidad de campos entre Workfront y Microsoft Project, consulte [Asignar campos de proyecto de Microsoft a proyectos de Adobe Workfront](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

## Requisitos de acceso

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
   <td> <p>Nueva licencia: Standard </p> 
   O
   <p>Licencia actual: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre el acceso a los proyectos, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Concesión de acceso a proyectos</a>. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Al crear un proyecto, recibe automáticamente permisos de administración en el proyecto </p> <p> Para obtener información sobre los permisos del proyecto, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Uso compartido de un proyecto en Adobe Workfront</a>.</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

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

Puede crear un proyecto desde el área Proyectos del menú principal o desde el área Proyectos de un portafolio o programa.

1. Vaya a Proyecto de Microsoft y abra un proyecto que desee importar en Workfront.
1. Clic **Archivo**, entonces **Guardar como** para guardar el proyecto como un archivo .xml.

1. Inicie sesión en Workfront.
1. Realice una de las siguientes acciones:

   * Haga clic en **Menú principal** ![](assets/main-menu-icon.png), haga clic en **Proyectos** y, a continuación, expanda **Nuevo proyecto**.
   * Vaya a un portafolio y amplíe **Nuevo proyecto**.
   * Vaya a un programa y expanda **Nuevo proyecto**.
   * Si es administrador de un grupo, también puede crear un proyecto en la sección Proyectos de un grupo que administre. Para obtener más información, consulte [Crear y modificar proyectos de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. Elija la **Importar MS Project** opción.

   ![](assets/new-project-dropdown-nwe-350x358.png)

1. Clic **Seleccionar archivo**, a continuación, busque el archivo .xml en el equipo que exportó desde Microsoft Project.
1. Importe el archivo seleccionado.

   Workfront inicia el proceso de importación y crea un nuevo proyecto basado en el archivo exportado desde Microsoft Project.

   Una vez completado el proceso de importación, se le dirigirá a la nueva página del proyecto que mostrará una confirmación de que la importación se ha completado correctamente.

   >[!NOTE]
   >
   >Workfront tiene una limitación de tiempo de 15 minutos en las cargas de archivos. Si la carga del archivo tarda más, le recomendamos que divida el proyecto en proyectos más pequeños e impórtelos por separado. Una vez importadas en Workfront, mueva las tareas de un proyecto a otro para combinarlas en un proyecto. Para obtener información sobre cómo mover tareas, consulte [Mover tareas](../../../manage-work/tasks/manage-tasks/move-tasks.md).

1. (Opcional) Continúe editando el proyecto en Workfront. Para obtener información sobre la edición de proyectos, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

   El estado de un nuevo proyecto creado a partir de una plantilla corresponde al estado definido por el administrador de Workfront en el área Preferencias del proyecto o por un administrador de grupo en el área Preferencias del proyecto de grupo. Para obtener información sobre cómo configurar las preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
