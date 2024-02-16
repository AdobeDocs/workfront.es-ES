---
content-type: overview
navigation-topic: grant-and-request-access-to-objects
title: Información general sobre los permisos de uso compartido en objetos
description: Puede compartir o quitar permisos a un objeto que haya creado o a un objeto que se haya compartido con usted.
author: Alina
feature: Get Started with Workfront
exl-id: 7c14702e-ac55-4266-88a7-f31618f84218
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 0%

---

# Información general sobre los permisos de uso compartido en objetos

<!-- Audited: 12/2023 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Redundancy here with the article Permissions for shared objects?</p>
-->
Al compartir un objeto con alguien en el sistema, puede conceder al destinatario cualquiera de los siguientes permisos: ver, contribuir y administrar.

No es necesario ser administrador de Adobe Workfront para compartir permisos en objetos a los que tiene acceso, pero los permisos en los objetos funcionan dentro de los niveles de acceso establecidos por el administrador de Workfront.

Puede compartir o quitar permisos a un objeto que haya creado o a un objeto que se haya compartido con usted. Si no es el creador del objeto, debe tener acceso de uso compartido en el objeto que desea compartir en su nivel de acceso, además de permisos de uso compartido en el objeto. Para obtener información sobre los niveles de acceso, consulte [Información general sobre nuevos niveles de acceso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md) o [Información general sobre niveles de acceso](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

>[!NOTE]
>
>Un administrador de Workfront puede agregar o quitar permisos a cualquier elemento del sistema, para todos los usuarios, sin ser el propietario de esos elementos.

## Objetos que se pueden compartir en Workfront

Puede compartir los siguientes objetos en Workfront con otros usuarios:

* **Proyectos**: para obtener más información, consulte [Uso compartido de un proyecto en Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* **Plantillas**: para obtener más información, consulte [Compartir plantillas de proyecto](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

* **Portfolio**: para obtener más información, consulte [Compartir un portafolio](../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio.md).

* **Programas**: para obtener más información, consulte [Compartir un programa](../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md) .

* **Tareas**: para obtener más información, consulte [Compartir una tarea](../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

* **Problemas**: para obtener más información, consulte [Compartir un problema](../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

* **Documentos**: para obtener más información, consulte [Compartir un documento](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

* **Carpetas de documentos**: para obtener más información, consulte [Compartir una carpeta de documentos](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

* **Pruebas**: para obtener más información, consulte [Compartir una revisión en Workfront](/help/quicksilver/review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* **Informes, tableros y calendarios**: para obtener más información, consulte [Uso compartido de informes, tableros y calendarios](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md). Además, consulte los siguientes artículos:

   * [Uso compartido de informes en Adobe Workfront](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [Compartir un tablero](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [Compartir un informe de calendario](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* **Filtros, vistas y agrupaciones**: para obtener más información, consulte [Compartir un filtro, una vista o una agrupación](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

* **Planes**: para obtener más información, consulte [Compartir un plan en el Scenario Planner](../../scenario-planner/share-a-plan.md).

  Esto requiere una licencia adicional.

* **Metas**: para obtener más información, consulte [Compartir una meta en Workfront Goals](../../workfront-goals/workfront-goals-settings/share-a-goal.md).

  Esto requiere una licencia adicional.

## Consideraciones acerca de compartir objetos

* Solo puede compartir el mismo nivel o un nivel inferior de permisos que tenga sobre el objeto.

  Por ejemplo, si tiene permisos de contribución sobre el objeto, no puede conceder a otro usuario permisos de administración sobre ese objeto.

* No se puede compartir un objeto con un nivel de permiso superior al nivel de acceso de un usuario.

  Por ejemplo, si un usuario tiene acceso de Vista a Proyectos en su nivel de acceso, no puede otorgarle permisos de Administración en un proyecto.
* Un usuario con permisos para ver al menos un objeto puede compartir ese objeto con otra persona.
* Puede compartir objetos con usuarios activos, roles, equipos, grupos o empresas.

  >[!NOTE]
  >
  >Solo puede compartir un plan o una meta con otros usuarios activos. Esto requiere licencias adicionales.
  >
  >
  >Para obtener más información, consulte:
  >
  >* [Compartir un plan en el Scenario Planner](../../scenario-planner/share-a-plan.md)
  >* [Compartir una meta en Workfront Goals](../../workfront-goals/workfront-goals-settings/share-a-goal.md)

## Limitaciones de uso compartido

Puede compartir un objeto con hasta 100 entidades (usuarios, equipos, grupos, roles, empresas). Se recomienda compartir objetos con grupos, equipos o empresas en lugar de con usuarios individuales para evitar esta limitación.

## Permisos de uso compartido para objetos

La siguiente tabla ilustra el nivel de permisos que puede seleccionar al compartir un objeto. No todos los objetos tienen todos estos ajustes disponibles. Puede conceder a otra entidad permisos para Ver o Administrar un objeto. Si comparte un proyecto, tarea o problema, también puede conceder permisos para contribuir a él.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Ver</strong></td> 
   <td> <p>Puede realizar las siguientes acciones en el objeto:</p> 
    <ul> 
     <li><p>Ver el objeto</p></li> 
     <li><p>Agregar documentos al objeto</p></li> 
     <li><p>Ver información de finanzas sobre el objeto</p></li> 
     <li> <p>Compartir el objeto<br></p> <p>Cuando comparte el objeto, puede conceder a otros usuarios el mismo nivel de permiso que sólo tiene en el objeto, no un nivel superior.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Contribuir</strong></td> 
   <td> <p>Puede realizar las siguientes acciones en el objeto:</p> 
    <ul> 
     <li>Todas las acciones incluidas con el permiso Ver.</li> 
     <li>Agregar gastos a él</li> 
     <li>Agregar problemas a él (si es una tarea o un proyecto)</li> 
     <li>Agregar tareas (si es un proyecto)</li> 
     <li>Editar Forms personalizado en él</li> 
     <li>Registrar horas en el objeto</li> 
     <li>Realizar asignaciones en él</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Administrar</strong></td> 
   <td> <p>Puede realizar las siguientes acciones en el objeto:</p> 
    <ul> 
     <li>Todas las acciones incluidas con los permisos Ver y Contribuir</li> 
     <li>Eliminarla</li> 
     <li>Administrar la información de finanzas en él</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Convertir esto en público para los usuarios externos</strong></td> 
   <td> <p>Cualquier persona que no tenga una cuenta de Workfront puede ver el objeto haciendo clic en un vínculo a él. Esto no está disponible para todos los objetos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Convertirlo en visible en todo el sistema.</strong></td> 
   <td> <p>El objeto se puede encontrar en búsquedas y lo puede ver cualquier persona que tenga una cuenta de Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Comprender los permisos heredados y la jerarquía de objetos

### Permisos heredados de objetos principales {#permissions-inherited-from-parent-objects}

Los permisos en Workfront se heredan jerárquicamente. Esto significa que, si concede permisos a un usuario sobre un objeto principal, obtiene los mismos permisos sobre los objetos secundarios asociados a él de forma predeterminada.

Por ejemplo, si otorga permisos de contribución a un usuario para un proyecto, el usuario tiene permisos de contribución para todas las tareas y problemas (objetos secundarios) asociados a ese proyecto.

Siguiendo con el ejemplo anterior, no se pueden restringir los permisos a objetos secundarios. Si no desea que el usuario tenga permisos de contribución para objetos secundarios asociados con el proyecto, debe quitar manualmente los permisos heredados de los objetos y, a continuación, ajustar los permisos para el usuario individual, incluida la configuración avanzada. 

Para obtener más información sobre la jerarquía y la interdependencia de objetos en Workfront, consulte la sección [Interdependencia y jerarquía de objetos](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#interdependency-and-hierarchy-of-objects) en el artículo [Información general sobre objetos Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>El administrador de Workfront puede deshabilitar los permisos heredados para documentos de su nivel de acceso. Para obtener más información sobre cómo deshabilitar los permisos heredados para documentos en el nivel de acceso, consulte [Crear o modificar niveles de acceso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### Permisos adquiridos mediante suscripciones a la organización  {#permissions-acquired-through-organizational-memberships}

Si concede permisos de Administración a un Grupo de usuarios de un objeto y concede permisos de Vista a un usuario individual de ese Grupo en el mismo objeto, el usuario tendrá el nivel más alto de permisos (Administrar) concedido a través de la pertenencia al Grupo en el objeto. 

Si desea conceder permisos inferiores a un usuario que ya forma parte de una unidad organizativa (Grupo, Equipo, Función del puesto o Empresa) con un nivel de permisos superior, debe quitar los permisos de la unidad organizativa y agregar usuarios individuales con un nivel inferior de permisos.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Remove permissions from objects</h2>
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">AL: draft/ hide this div when Becky makes Remove permissions from objects live and replace with the drafted content with the link at the top of this section</p>
<p>You can remove permissions from objects you have access to Share. Removing permissions from objects is identical for all objects that can be shared.&nbsp;</p> <note type="note">
&nbsp;You cannot remove permissions when you share items in bulk. You can remove permissions only when selecting individual items.&nbsp;
</note>
<p>To remove permissions from objects consider the following:&nbsp;</p>
<ul>
<li><a href="#remove-entities-from-the-sharing-list-of-an-object" class="MCXref xref">Remove entities from the sharing list of an object</a> </li>
<li><a href="#remove-inherited-permissions" class="MCXref xref">Remove inherited permissions</a> </li>
<li><a href="#make-an-object-private" class="MCXref xref">Make an object private</a> </li>
</ul>
<p><strong>Remove entities from the sharing list of an object</strong></p>
<p>You can remove entities from the sharing list of an object to remove their permissions from the object.</p>
<p>To remove permissions from objects:&nbsp;</p>
<ol>
<li value="1">Navigate to an object on which you want to modify the permissions.</li>
<li value="2">Click the <strong>Actions</strong> menu, then click <strong>Sharing</strong>.<br>For example, on a project, click <strong>Project Actions</strong>, then <strong>Sharing</strong>.&nbsp;</li>
<li value="3">Click the <strong>x</strong> next to the name of a user, team, group, company, job role to remove them.<br></li>
<li value="4">In the <strong><User Name>'s Workfront access will be removed from this</strong> drop-down menu, select whether you want their access to be removed just from the object you have selected, or from all children objects associated with it.<br>The following scenarios exist:
<ul>
<li>If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they are granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.&nbsp;</li>
<li>If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they have been given individual permission on each child object.&nbsp;</li>
</ul></li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<p> <p><strong>Remove inherited permissions</strong></p> </p>
<p>Inherited permissions can be removed from objects allowing for owners to specifically&nbsp;identify who will get access to children objects regardless of the access of a user to a parent object. Only users with Manage permission are able to remove inherited permissions.</p>
<p>To remove inherited permissions:</p>
<ol>
<li value="1">Navigate to an object to which you have Manage permissions. <br>For example, navigate to a task.</li>
<li value="2">Go to the sharing list as described in the <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> section in this article. </li>
<li value="3">Select the <strong>X</strong>&nbsp;mark next to <strong>Inherited Permission</strong>&nbsp;on the sharing box to remove&nbsp;anyone listed there.<br><br>This ensures that no one who is granted permissions to the parent object (for example, the project) has permissions to this task by default. You must list&nbsp; individual entities in the sharing list of the task to grant permissions on the task.<br><note type="note">
You cannot remove individual entities from the Inherited Permissions list. You can only disable the Inherited Permissions for all entities listed.
</note></li>
<li value="4">Click <strong>Save</strong>.&nbsp;</li>
</ol>
<p><strong>Make an object private</strong></p>
<p>If you have shared an object system-wide, or you have shared it with external uses by making it public, you can make it private again by removing the system-wide or public permissions.&nbsp;</p>
<p>For more information about making an object available system-wide, or publicly, see the section <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> in this article.</p>
<p>To make an object private:</p>
<ol>
<li value="1">Go to the object you want to make private.<br>For example, navigate to a report.</li>
<li value="2">Click <strong>Report Actions</strong>, then <strong>Sharing</strong>.<br><br></li>
<li value="3">Click <strong>Remove public access</strong> to remove the access of external users to viewing the report.</li>
<li value="4">Click <strong>Remove system-wide access</strong> to stop sharing it with all Workfront users.&nbsp;</li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Compartir un objeto

Para obtener información sobre cómo compartir objetos, consulte [Compartir un objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

## Eliminación de permisos de objetos

Para obtener información sobre cómo quitar permisos de objetos, consulte [Eliminación de permisos de objetos](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Solicitar permisos a objetos

Cuando alguien le envía un vínculo a un objeto para el que no tiene permisos de visualización, o cuando tiene permisos inferiores en un objeto y desea solicitar un nivel superior de permisos, puede solicitar permisos en el objeto. 

Puede solicitar acceso a un objeto a cualquier persona que tenga permiso para compartir el objeto. 

Para obtener más información sobre la solicitud de permisos a objetos, consulte [Solicitud de acceso a objetos](../../workfront-basics/grant-and-request-access-to-objects/request-access.md).
