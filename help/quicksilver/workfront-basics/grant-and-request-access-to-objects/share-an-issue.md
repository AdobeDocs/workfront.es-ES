---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Compartir un problema
description: El administrador de Adobe Workfront concede a los usuarios acceso para ver o editar problemas cuando asignan niveles de acceso. Para obtener más información sobre la concesión de acceso a los problemas, consulte Conceder acceso a los problemas.
author: Alina
feature: Get Started with Workfront
exl-id: 91ee72e0-20a9-4b06-9f80-a343dd4fbe06
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 2%

---

# Compartir un problema

El administrador de Adobe Workfront concede a los usuarios acceso para ver o editar problemas cuando asignan niveles de acceso. Para obtener más información sobre la concesión de acceso a los problemas, consulte [Conceder acceso a los problemas](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md).

Junto con el nivel de acceso que se concede a los usuarios, también puede concederles permisos para Ver, Contribute o Administrar problemas específicos que tiene acceso para compartir. Para obtener más información sobre los niveles de acceso y los permisos, vea [Cómo funcionan juntos los niveles de acceso y los permisos](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Los permisos son específicos de un elemento en Workfront y definen qué acciones se pueden realizar sobre ese elemento.

## Consideraciones acerca de problemas de uso compartido

Además de las consideraciones siguientes, consulte [Información general sobre los permisos de uso compartido en objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Un administrador de Workfront puede agregar o quitar permisos a cualquier elemento del sistema, para todos los usuarios, sin ser el propietario de esos elementos.

* El creador de un problema tiene permisos de administración de forma predeterminada.
* Puede compartir problemas individualmente o puede compartir varios de ellos a la vez. Compartir problemas es idéntico a compartir otros elementos en Workfront. Para obtener más información sobre cómo compartir elementos en Workfront, vea [Compartir un objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Puede conceder los siguientes permisos a un problema: 

   * Ver

     ![vista_en_problema.png](assets/view-on-issue-221x216.png)

   * Administrar

     ![administrar_en_problemas.png](assets/manage-on-issues-179x199.png)

   * Aportar\
     ![Contribute_on_issue.png](assets/contribute-on-issue-156x205.png)

* Cuando comparte un problema, todos los documentos adjuntos al problema heredan los mismos permisos.

  El administrador de Workfront puede especificar si los documentos deben heredar permisos de objetos superiores en el nivel de acceso del usuario. Para obtener más información acerca de cómo restringir permisos heredados en documentos, vea [Crear o modificar niveles de acceso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Puede eliminar los permisos heredados de un problema. Para obtener más información, vea [Quitar permisos de objetos](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Formas de compartir un problema

* Manualmente, lo que es similar a compartir cualquier otro objeto en Workfront. Para obtener más información sobre cómo compartir objetos en Workfront, vea [Compartir un objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Automáticamente, mediante una de las siguientes acciones:

   * Especifique los permisos en cualquiera de los objetos principales del problema: proyecto, programa o portafolio. Los problemas heredan los permisos de sus objetos principales. Para obtener información acerca de cómo ver permisos heredados en objetos, vea [Ver permisos heredados en objetos](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * Agregue entidades al Uso compartido de proyectos en una plantilla utilizada para crear el proyecto en el que se encuentra el problema. Para obtener información sobre cómo compartir proyectos desde plantillas, vea [Compartir una plantilla](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * Especifique los permisos sobre todos los problemas de un proyecto al editarlo. Para obtener información sobre cómo administrar el acceso a problemas o solicitudes en el proyecto en función de los permisos de un usuario para el proyecto, consulte la sección [](../../manage-work/projects/manage-projects/edit-projects.md#access) en el artículo [Editar proyectos](../../manage-work/projects/manage-projects/edit-projects.md).

     >[!TIP]
     >
     >Si no especifica los permisos de problema que desea que tengan los usuarios cuando se les asignen los problemas del proyecto, recibirán los mismos permisos que tienen en el proyecto de forma predeterminada.

   * Especifique los permisos que reciben los usuarios en los problemas que envían en una cola de solicitudes al crear una cola de solicitudes. Para obtener más información, vea [Crear una cola de solicitudes](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

     >[!IMPORTANT]
     >
     >Los permisos se conceden de forma diferente en función de si el proyecto se publica o no como cola de solicitudes:
     >
     >   
     >   
     >   * Cuando un usuario envía una solicitud a un proyecto publicado como cola de solicitudes, los usuarios que son el Contacto principal y el Introducido por obtienen el permiso especificado.
     >   * Cuando un usuario envía una solicitud a un proyecto que no se ha publicado como cola de solicitudes, el contacto principal (si es diferente al usuario introducido por) obtiene el permiso especificado y el usuario introducido por obtiene permisos de administración para el problema.
     >   
     >

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Automatically share an issue at the project level</h2>
<p>(NOTE: this info duplicates in Edit projects - linked there instead (above).)&nbsp;</p>
<p>As the Project Owner, you can grant permissions automatically to users as the issues are added to a project.</p>
<ol>
<li value="1">Go to the project whose issues you want to share automatically.</li>
<li value="2"> Click the More menu <img src="assets/more-icon.png">, then click <strong>Edit</strong>. </li>
<li value="3">In the <strong>Edit Project</strong> box that displays, click <strong>Access</strong>.</li>
<li value="4">In the <strong>When someone is assigned to an ISSUE</strong> field, select from the following permissions levels:
<ul>
<li><strong>View</strong></li>
<li><strong>Contribute</strong></li>
<li><strong>Manage</strong><br>Now, when someone is assigned to an issue on the selected project, they are granted the specified permissions to the issue.&nbsp;</li>
</ul></li>
<li value="5">(Optional) Select the <strong>Also grant ... access to the project</strong> field to also grant View, Contribute, or Manage permissions to the projects to the user assigned to the issue</li>
<li value="6">In the <strong>When someone submits a REQUEST ...</strong> field, select from the following permissions levels:
<ul>
<li><strong>View</strong></li>
<li><strong>Contribute</strong></li>
<li><p><strong>Manage</strong></p><note type="important">
<p>Permissions are granted differently depending on whether or not the project is published as a request queue:</p>
<ul>
<li>When a user submits a request to a project published as a request queue, the Primary Contact and Entered By users are granted the permission specified.</li>
<li>When a user submits a request to a project not published as a request queue, the Primary Contact (if different from Entered By user) is granted the permission specified, and the Entered By user is granted Manage permissions to the issue.</li>
</ul>
</note></li>
</ul></li>
<li value="7"> <p>(Optional) Select the <strong>People from the same company will inherit the same permissions for all requests</strong> field.</p> <p>People from the same company as the user submitting the request are granted the same permissions on the requests as the user.&nbsp;</p> </li>
<li value="8">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Automatically share an issue in request queues</h2>
<p>(NOTE: drafted because it's duplicated from Create a Request Queue which is linked above)&nbsp;</p>
<p>As the Project Owner, you can grant permissions automatically to users as the issues are submitted to a request queue.</p>
<ol>
<li value="1">Go to the project whose issues you want to share automatically.</li>
<li value="2">Click <strong>Edit Project</strong>.</li>
<li value="3">Click <strong>More</strong> then click <strong>Queue Setup</strong>. </li>
<li value="4"> <p>On the <strong>Queue Details</strong> sub-tab, in the drop-down menu under <strong>When someone makes a request, automatically grant</strong>, select from the following permissions levels:</p>
<ul>
<li><strong>View Access</strong> </li>
<li><strong>Contribute Access</strong> </li>
<li> <p><strong>Manage Access</strong> </p> </li>
</ul> <p>Now, when someone submits a request to the selected project, they are granted the specified permissions to the request.</p> </li>
<li value="5"> <p>(Optional) Select the <strong>People from the same company will inherit the same permissions for all requests</strong>.</p> <p>People from the same company as the user submitting the request are granted the same permissions on the requests as the user.&nbsp;</p> </li>
<li value="6">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Permisos de problemas

La siguiente tabla muestra qué permisos puede otorgar a los usuarios cuando les permite Ver, Contribute o Administrar un problema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Acciones</strong> </td> 
   <td><strong>Administrar</strong> </td> 
   <td><strong>Contribute</strong> </td> 
   <td><strong>Vista</strong> </td> 
  </tr> 
  <tr> 
   <td> <p>Añadir problemas</p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Eliminar </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Adjuntar formulario personalizado</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar campos personalizados</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aprobar problema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Agregar Un Proceso De Aprobación</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Agregar documentos</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Copiar problema*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Mover problema</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Registrar horas</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Convertir a proyecto*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aceptar asignación</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Actualizaciones/ comentarios</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Modificar fechas planificadas</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Hacer asignaciones</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Compartir</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Compartir en todo el sistema</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;Controlado por los niveles de acceso y los permisos del proyecto.
