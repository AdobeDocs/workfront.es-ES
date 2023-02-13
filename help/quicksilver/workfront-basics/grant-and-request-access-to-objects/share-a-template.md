---
title: Uso compartido de una plantilla
product-area: templates
navigation-topic: grant-and-request-access-to-objects
description: Como administrador de Adobe Workfront, puede otorgar a los usuarios acceso para ver o editar plantillas cuando asigne su nivel de acceso. Un usuario debe tener una licencia Plan para tener acceso a Editar plantillas.
author: Alina
feature: Get Started with Workfront
exl-id: 19fb0de5-7db5-42a9-9f33-a4570acfeef8
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 2%

---

# Compartir una plantilla

Como administrador de Adobe Workfront, puede otorgar a los usuarios acceso para ver o editar plantillas cuando asigne su nivel de acceso. Un usuario debe tener una licencia Plan para tener acceso a Editar plantillas.

Para obtener más información sobre la concesión de acceso a plantillas, consulte [Concesión de acceso a plantillas](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

Junto con el nivel de acceso que concede, un usuario también puede recibir permisos para Ver o Administrar plantillas específicas de otros usuarios que las compartan.

>[!NOTE]
>
>Los niveles de permisos funcionan dentro de los niveles de Access. Por ejemplo, un usuario no puede recibir permisos para Administrar una plantilla si su nivel de acceso solo les permite Ver plantillas.

Los permisos son específicos para un elemento de Workfront y definen qué acciones se pueden realizar en ese elemento.

## Consideraciones al compartir una plantilla

* Además de las consideraciones siguientes, consulte [Información general sobre cómo compartir permisos en objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
* De forma predeterminada, el creador de una plantilla y el propietario de la plantilla tienen permisos de administración para la plantilla. Para obtener información sobre la designación de un usuario como propietario de plantilla, consulte [Editar plantillas de proyecto](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* Puede compartir lo siguiente al compartir una plantilla:

   * La plantilla

      Para obtener más información sobre cómo compartir una plantilla, consulte [Compartir plantillas de proyecto](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

      Puede conceder los siguientes permisos a una plantilla:

      * Vista

         ![](assets/view-on-template-262x221.png)

      * Administrar

         ![](assets/manage-on-template-225x280.png)
   * Los proyectos futuros que se crean con la plantilla . Puede conceder los mismos niveles de permisos a los proyectos creados a partir de una plantilla que a un proyecto individual. 

      Para obtener información sobre cómo compartir un proyecto desde una plantilla a nivel de plantilla, consulte [Compartir plantillas de proyecto](../../manage-work/projects/create-and-manage-templates/share-project-template.md).


* Al compartir una plantilla o un proyecto creado a partir de la plantilla, los usuarios heredan los mismos permisos de forma predeterminada a todos los objetos secundarios asociados con la plantilla o el proyecto.

   Para obtener más información sobre la jerarquía de objetos en Workfront, consulte  [Explicación de los objetos en Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* Cuando comparte una plantilla, todas las tareas y los documentos de la plantilla, así como los problemas del proyecto futuro creado a partir de la plantilla, heredan los mismos permisos, a menos que se especifique lo contrario.

   Para obtener información sobre la administración del acceso a las tareas de plantilla y los problemas del proyecto en función de los permisos de un usuario en el proyecto, consulte la [Acceso](../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) sección del artículo [Editar plantillas de proyecto](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* El administrador de Workfront puede especificar si los documentos deben heredar permisos de objetos superiores en el nivel de acceso del usuario. Para obtener más información sobre la restricción de permisos heredados en documentos, consulte [Crear o modificar niveles de acceso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Share a template</h2>
<p>(NOTE: drafted because this is also linked above: Share project templates >> which is an article in the Manage Work section>> Templates)&nbsp;</p>
<ol>
<li value="1"> <p>Go to the template you want to share with other entities, click <strong>Template Actions</strong>, then <strong>Template Sharing</strong>.<br>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <strong>Share Template</strong>.</p> <note type="note">
If you select multiple templates, you cannot view who already has permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing the name of a user, group, team, job role, or company that you want to share the template with in the <strong>Give template access to</strong> or <strong>Edit template access for</strong> fields.</p> <p>Select them when they appear in the list.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant:<br>
<ul>
<li><p><strong>View it</strong>: Users with these permissions are able to view the template and create a project using it, or attach it to an existing project.</p><p><img src="assets/template-permissions-350x197.png" alt="template_permissions.png" style="width: 350;height: 197;"></p></li>
<li><strong>Manage it</strong>: Users with these permissions are able to edit or delete the template.</li>
</ul></li>
<li value="4">(Optional) Click <strong>Advanced Settings</strong> to fine-tune your settings for each level of permissions.</li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<h2>Share a project at the template level</h2>
<p>You can share the future projects that are created using a template with users at the template level.</p>
<ol>
<li value="1"> <p>Go to the template whose future projects you want to share with other entities, click <strong>Template Actions</strong>, then <strong>Project Sharing</strong>.</p> <p>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <strong>Share Project</strong>.</p> <note type="note">
If you select multiple templates, you cannot view who already has project permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing and then select the name of a user, group, team, job role, or company with whom you want to share future projects created from the template in the <strong>Give project access to</strong> or <strong>Edit template access for</strong> fields.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant.<br>Select from the following:<br>
<ul>
<li><strong>No access</strong>: You can specify which users will not have any access to the template.<br>This option is available only when bulk sharing projects from templates.&nbsp;</li>
<li><strong>View</strong>: Users with these permissions can view projects created from the template.</li>
<li><strong>Contribute</strong>: Users with these permissions can contribute to projects created from the template&nbsp;</li>
<li><strong>Manage</strong>: Users with these permissions can manage or delete projects created from this template.<br><img src="assets/share-project-from-template-350x268.png" alt="share_project_from_template.png" style="width: 350;height: 268;"></li>
</ul></li>
<li value="4">(Optional) Click <strong>Advanced Settings</strong> to fine-tune your settings for each level of permissions. </li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Configuración avanzada para compartir plantillas

En la tabla siguiente se muestran los permisos que puede conceder a los usuarios al permitirles ver o administrar una plantilla. Para obtener instrucciones sobre cómo compartir una plantilla, consulte la sección [Compartir una plantilla](../../manage-work/projects/create-and-manage-templates/share-project-template.md#share) en el artículo [Compartir plantillas de proyecto](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Acciones</th> 
   <th>Administrar</th> 
   <th>Vista</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Copiar</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Eliminar</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar detalles de plantilla</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ver plantilla</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Compartir</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Compartir en todo el sistema</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Agregar documentos</p> <p>Sugerencia: A veces, las personas agregan documentos a una plantilla de proyecto pensando que los están agregando a un proyecto. Puede evitarlo en sus destinatarios desactivando esta configuración.</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

Para comprender los permisos que concede a los usuarios de los proyectos creados a partir de una plantilla, consulte [Uso compartido de un proyecto en Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
