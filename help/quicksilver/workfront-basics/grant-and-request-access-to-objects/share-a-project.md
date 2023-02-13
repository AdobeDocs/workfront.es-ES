---
title: Uso compartido de un proyecto en Adobe Workfront
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: El administrador de Adobe Workfront puede concederle acceso para ver o editar proyectos al asignar su nivel de acceso. Para obtener más información, consulte Concesión de acceso a proyectos.
author: Alina
feature: Get Started with Workfront
exl-id: eaeedff8-9114-40d9-8cd4-56996edc7dad
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 3%

---

# Uso compartido de un proyecto en Adobe Workfront

El administrador de Adobe Workfront puede concederle acceso para ver o editar proyectos al asignar su nivel de acceso. Para obtener más información, consulte [Concesión de acceso a proyectos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Junto con el nivel de acceso que se concede a los usuarios, también puede otorgarles permisos para ver, contribuir o administrar proyectos específicos a los que tenga acceso para compartir.

Los permisos son específicos para un elemento de Workfront y definen qué acciones se pueden realizar en ese elemento.

## Consideraciones sobre cómo compartir proyectos

Además de las consideraciones siguientes, consulte [Información general sobre cómo compartir permisos en objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* De forma predeterminada, el creador de un proyecto tiene permisos para administrar el proyecto y también está designado como Propietario del proyecto. Si el proyecto está asignado a otro propietario, ese usuario también tiene permisos para administrar el proyecto. Cuando el creador (o propietario) del proyecto comparte el proyecto con otros usuarios, conceden a estos permisos para controlar lo que pueden hacer mientras trabajan en el proyecto.

   Sin embargo, si el propietario de un proyecto no tiene una licencia de Planificador, no tiene acceso completo para administrar el proyecto. Solo los usuarios con una licencia de Plan pueden tener permisos para administrar un proyecto. Para obtener más información, consulte [Cómo funcionan juntos los niveles de acceso y los permisos](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

* Puede compartir proyectos individualmente o varios de ellos a la vez. Compartir proyectos es idéntico al uso compartido de otros objetos. Para obtener más información sobre cómo compartir elementos en Workfront, consulte [Compartir un objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Puede conceder los siguientes permisos a un proyecto: 

   * Vista
   * Administrar
   * Aportar

      ![](assets/view-on-projects-190x207.png) ![](assets/contribute-on-projects-159x243.png) ![](assets/manage-on-projects-178x230.png)

* Cuando comparte un proyecto, todas las tareas, problemas y documentos heredan los mismos permisos, a menos que se especifique lo contrario.

   Para obtener información sobre la administración del acceso a las tareas y los problemas del proyecto en función de los permisos de un usuario en el proyecto, consulte la [](../../manage-work/projects/manage-projects/edit-projects.md#access) sección del artículo [Editar proyectos](../../manage-work/projects/manage-projects/edit-projects.md).

   El administrador de Workfront puede especificar si los documentos deben heredar permisos de objetos superiores en el nivel de acceso del usuario. Para obtener más información sobre la restricción de permisos heredados en documentos, consulte [Crear o modificar niveles de acceso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Puede quitar permisos heredados de un proyecto para que los objetos secundarios no los hereden. Para obtener más información sobre cómo quitar permisos heredados de objetos, consulte  [Eliminación de permisos de objetos](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Formas de compartir un proyecto {#ways-to-share-a-project}

Puede compartir un proyecto de las siguientes maneras:

* Manualmente realizando una de las siguientes acciones:

   * Agregar usuarios al equipo del proyecto. Cuando agrega usuarios al equipo del proyecto, automáticamente obtienen permisos de visualización del proyecto.\
      Para obtener más información sobre cómo agregar usuarios a un equipo de proyecto, consulte la sección &quot;Agregar usuarios a un equipo de proyecto&quot; en [Información general del equipo del proyecto](../../manage-work/projects/planning-a-project/project-team-overview.md).
   * Uso compartido individual o masivo de los proyectos al usar la variable **Uso compartido** .

      Compartir un proyecto es similar a compartir todos los demás objetos en Adobe Workfront.

      Para obtener información sobre cómo compartir objetos en Workfront, consulte [Compartir un objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Automáticamente, realizando una de las siguientes acciones:

   * Coloque un proyecto en un **Portfolio** o **Programa** que ya se ha compartido con otros usuarios. Los usuarios obtienen los mismos permisos para el proyecto que tienen para el portafolio o el programa.\
      Para obtener información sobre cómo agregar un proyecto a un **Portfolio**, consulte [Agregar proyectos a un portafolio](../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md).\
      Para obtener información sobre cómo agregar un proyecto a un **Programa**, consulte [Agregar un proyecto a un programa](../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md).

      Para obtener información sobre la visualización de permisos heredados en un objeto, consulte [Ver permisos heredados en objetos](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

   * Agregue entidades al uso compartido de proyectos en una plantilla utilizada para crear el proyecto. Para obtener información sobre cómo compartir proyectos desde plantillas, consulte [Compartir una plantilla](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).
   * Defina la plantilla de acceso al proyecto.

      Para definir la plantilla de acceso al proyecto, consulte [Compartir un objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

      >[!TIP]
      >
      >Al adjuntar o guardar una plantilla, puede borrar las reglas de Uso compartido de proyectos de plantilla.

   * Editar un proyecto y definir la variable **Cuando alguien tiene acceso a este proyecto** configuración. Para obtener más información, consulte [Editar proyectos](../../manage-work/projects/manage-projects/edit-projects.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because I created new article and linked it above) </p>
<p>To view what users have inherited the access on the project from a portfolio or a program, do the following:</p>
<ol style="list-style-type: lower-alpha;">
<li value="1">Go to a project whose sharing permissions you want to view. </li>
<li value="2"> Click the <strong>More</strong> menu <img src="assets/more-icon.png">, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>Expand the <strong>Inherited Permissions</strong> list. </p> <p>This list displays the names of users that have access to either the portfolio or the program that the project belongs to and also have permissions to the project. </p> <p> <img src="assets/screen-shot-2014-01-22-at-10.13.10-am-350x284.png" style="width: 350;height: 284;"> </p> </li>
</ol>
</div>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a project whose sharing permissions you want for all projects you create from scratch. (NOTE: drafted because linked above)&nbsp;</li>
<li value="2"> Click the More menu, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>In the Project Access box that displays, near the upper-right corner, click the gear icon <img src="assets/gear-icon-settings.png">, then click <strong>Set as my project access template</strong>.</p> <p>The entities that are granted permissions on the selected project have the same permissions for all the projects you create from scratch in the future.</p> <p> The project access template overrides the sharing defaults granted to you by the Workfront administrator in your Access Level.<br>For more information about specifying sharing defaults for projects in the Access Level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>.</p> </li>
<li value="4">Click <strong>Save</strong>.</li>
</ol>
-->

## Limitaciones para diferentes tipos de licencias

* Los usuarios con una licencia de trabajador no tienen permisos para administrar proyectos. Para los trabajadores, el permiso de uso compartido más alto es Contribute.
* Los usuarios con una licencia de Solicitud pueden ver información del proyecto, pero tienen acceso limitado al proyecto.
* La excepción a cambiar el estado de un proyecto se produce cuando un usuario con permisos de Vista o Contribute también se incluye en un proceso de aprobación. Pueden aprobar el proyecto, que cambia el estado del proyecto, pero el estado es el estado predefinido para aprobación o rechazo.
* Para poder copiar un proyecto, un usuario también debe tener acceso para crear proyectos en su nivel de acceso.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Configure default permissions for a project</h2>
<p>(NOTE: drafted because I added one more way to automatically share the project above in the bullet list and linked it to Edit Projects) </p>
<p>As a project owner, you can configure the default permissions for View, Manage, and Contribute access that are used when sharing&nbsp;the project with others. When users share a project, the default permissions are used. Users can then adjust the default permissions when sharing the project, as described in <a title="Project Permissions" href="#ways-to-share-a-project" class="MCXref xref">Ways to share a project</a>. </p>
<p>To configure the default permissions that are included with each access level:</p>
<ol>
<li value="1">Go to the project where you want to set the default permissions.</li>
<li value="2"> <p>Click the More menu <img src="assets/more-icon.png">, then click <strong>Edit</strong>. <img src="assets/edit-icon.png"></p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/edit-projnwe-350x155.png" style="width: 350;height: 155;"> </p> </li>
<li value="3">Click <strong>Access</strong> in the list on the left.</li>
<li value="4"> <p>In the <strong>When someone is given access to this PROJECT</strong> section, select permissions that you want to be available when users are given access to the project via sharing.</p> <p>Ensure that any permissions that you want to include in the selected access level are selected and deselect any permissions that you do not want to include in the selected permissions level.</p> <p>To view which permissions are available for each level, see&nbsp;<a title="Project Permissions" href="#Understanding_Project_Permissions" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <note type="note">
The
<strong>Delete</strong> access in the
<strong>Manage</strong> permission level determines whether users can&nbsp;delete the project itself. Users with
<strong>Manage</strong> access to the project can delete tasks and issues within the project regardless of whether this option is selected, if they have
<strong>Manage</strong> permissions to the tasks and issues.&nbsp;
</note> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## Opciones de permiso del proyecto

La tabla siguiente muestra los permisos que los usuarios pueden conceder al compartir un proyecto. Para obtener más información sobre el acceso que los usuarios obtienen en función de su licencia, consulte [Concesión de acceso a proyectos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Acciones</strong> </p> </th> 
   <th> <p><strong>Administrar</strong> </p> </th> 
   <th> <p><strong>Aportar</strong> </p> </th> 
   <th> <p><strong>Vista</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Agregar formulario personalizado</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Actualizar campos personalizados</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Agregar Un Proceso De Aprobación</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aprobar un proyecto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aprobar horas</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓ </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Crear Un Proyecto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Agregar documentos</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Agregar problemas</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Agregar tareas</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Copiar proyecto</p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Eliminar proyecto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Modificar fechas planificadas</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Compartir proyecto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Compartir en todo el sistema</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ver proyecto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Actualizaciones/ comentarios</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Cambiar estado</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Registrar horas</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Editar asignaciones</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Administrar línea de base</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Administrar riesgos*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Administrar finanzas*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Agregar/Editar gastos*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ver finanzas*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Adjuntar plantilla</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Guardar como plantilla</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Agregar o editar caso empresarial</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Editar detalles del proyecto</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Editar plantilla</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Exportar a MS Project</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Volver a calcular finanzas/línea de tiempo*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Definir propiedades de cola</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Editar proyecto de forma masiva en una lista</p> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Los usuarios sin acceso a datos financieros no pueden administrar los riesgos y las finanzas de los proyectos, aunque tengan acceso de edición a los proyectos. Para obtener información sobre el acceso a los datos financieros, consulte [Concesión de acceso a datos financieros](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
