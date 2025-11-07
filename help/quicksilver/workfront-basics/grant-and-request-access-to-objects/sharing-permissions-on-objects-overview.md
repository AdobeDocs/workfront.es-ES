---
content-type: overview
navigation-topic: grant-and-request-access-to-objects
title: Información general sobre los permisos de uso compartido en objetos
description: Es posible compartir o quitar permisos de un objeto que creó o de un objeto compartido con usted.
author: Courtney
feature: Get Started with Workfront
exl-id: 7c14702e-ac55-4266-88a7-f31618f84218
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '1289'
ht-degree: 89%

---

# Información general sobre los permisos de uso compartido en objetos

<!-- Audited: 12/2023 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Redundancy here with the article Permissions for shared objects?</p>
-->
Al compartir un objeto con alguien en el sistema, es posible conceder al destinatario cualquiera de los siguientes permisos: ver, contribuir y administrar.

No es necesario ser administrador de Adobe Workfront para compartir permisos en objetos a los que tenga acceso, pero los permisos de los objetos funcionan dentro de los niveles de acceso establecidos por el administrador de Workfront.

Es posible compartir o quitar permisos de un objeto que creó o de un objeto compartido con usted. Si no se trata del creador del objeto, será necesario tener acceso de uso compartido sobre el objeto que quiera compartir en su nivel de acceso, además de permisos de uso compartido sobre el objeto. Para obtener información acerca de los niveles de acceso, consulte [Información general sobre los nuevos niveles de acceso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md) o [Información general sobre los niveles de acceso](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

>[!NOTE]
>
>Un administrador de Workfront puede añadir o quitar permisos a cualquier elemento del sistema, para todos los usuarios, sin que tengan que ser el propietario de esos elementos.

## Objetos que se pueden compartir en Workfront

Es posible compartir los siguientes objetos en Workfront con otros usuarios:

* **Proyectos**: para obtener más información, consulte [Compartir proyectos en Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* **Plantillas**: para obtener más información, consulte [Compartir plantillas de proyecto](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

* **Portafolios**: para obtener más información, consulte [Compartir portafolios](../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio.md).

* **Programas**: para obtener más información, consulte [Compartir programas](../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md) .

* **Tareas**: para obtener más información, consulte [Compartir tareas](../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

* **Problemas**: para obtener más información, consulte [Compartir problemas](../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

* **Documentos**: para obtener más información, consulte [Compartir documentos](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

* **Carpetas de documentos**: para obtener más información, consulte [Compartir carpetas de documentos](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

* **Pruebas**: para obtener más información, consulte [Compartir pruebas en Workfront](/help/quicksilver/review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* **Informes, tableros y calendarios**: para obtener más información, consulte [Compartir informes, tableros y calendarios](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md). Además, consulte los siguientes artículos:

   * [Uso compartido de informes en Adobe Workfront](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [Compartir un panel de control](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [Compartir un informe de calendario](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* **Filtros, vistas y agrupaciones**: para obtener más información, consulte [Compartir filtros, vistas o agrupaciones](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

* **Planes**: para obtener más información, consulte [Compartir planes en el Planificador de escenarios](../../scenario-planner/share-a-plan.md).

  Se requiere una licencia adicional.

* **Metas**: para obtener más información, consulte [Compartir metas en Workfront Goals](../../workfront-goals/workfront-goals-settings/share-a-goal.md).

  Se requiere una licencia adicional.

## Consideraciones acerca del uso compartido de objetos

* Solo es posible compartir el mismo nivel o un nivel inferior de permisos que tenga sobre el objeto.

  Por ejemplo, si tuviera permisos de contribución sobre el objeto, no podría conceder a otro usuario permisos de administración sobre ese objeto.

* No es posible compartir un objeto con un nivel de permisos superior al nivel de acceso de un usuario.

  Por ejemplo, si un usuario tuviera acceso de vista a los proyectos de su nivel de acceso, no podría otorgarle permisos de administración en un proyecto.
* Un usuario que tenga permiso para ver al menos un objeto podrá compartir ese objeto con otra persona.
* Es posible compartir objetos con usuarios activos, funciones, equipos, grupos o empresas.

  >[!NOTE]
  >
  >Solo es posible compartir un plan o una meta con otros usuarios activos. Esto requiere licencias adicionales.
  >
  >
  >Para obtener más información, consulte lo siguiente:
  >
  >* [Compartir planes en el Planificador de escenarios](../../scenario-planner/share-a-plan.md)
  >* [Compartir metas en Workfront Goals](../../workfront-goals/workfront-goals-settings/share-a-goal.md)

* Workfront envía notificaciones a los usuarios cuando comparte un objeto con ellos. Las notificaciones se emiten cuando ambas configuraciones están habilitadas:

   * Las notificaciones por correo electrónico de **Uso compartido de objetos con el usuario** y **Uso compartido de objetos con el equipo** están habilitadas en el área de configuración por un administrador del sistema o del grupo. Para obtener más información, consulte [Configurar notificaciones de los eventos para todos los usuarios del sistema](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
   * **Alguien comparte un objeto conmigo** y **Alguien comparte un objeto con mi equipo** notificaciones habilitadas en la página de perfil del usuario. Para obtener más información, consulte [Modificar sus propias notificaciones por correo electrónico](/help/quicksilver/workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  La configuración de nivel de sistema o de grupo debe habilitarse primero para poder habilitar la configuración de notificación para el usuario.

## Limitaciones de uso compartido

Es posible compartir un objeto con hasta 100 entidades (usuarios, equipos, grupos, roles o empresas). Se recomienda compartir objetos con grupos, equipos o empresas en lugar de con usuarios individuales para evitar esta limitación.

## Permisos de uso compartido para objetos

En la siguiente tabla se muestra el nivel de permisos que se pueden seleccionar al compartir objetos. No todos los objetos disponen de toda esta configuración. Es posible conceder a otra entidad permisos para ver o administrar objetos. Al compartir proyectos, tareas o problemas, también es posible otorgar permisos de contribución.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Ver</strong></td> 
   <td> <p>Puede realizar las siguientes acciones en el objeto:</p> 
    <ul> 
     <li><p>Ver el objeto</p></li> 
     <li><p>Añadir documentos al objeto</p></li> 
     <li><p>Agregar problemas al objeto (si es una tarea o un proyecto)</p></li> 
     <li><p>Ver información financiera sobre el objeto</p></li> 
     <li> <p>Compartir el objeto<br></p> <p>Cuando comparte el objeto, puede conceder a otros usuarios el mismo nivel de permiso que solo tiene en el objeto, no en un nivel superior.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Aportar</strong></td> 
   <td> <p>Puede realizar las siguientes acciones en el objeto:</p> 
    <ul> 
     <li>Todas las acciones incluidas con el permiso de visualización.</li> 
     <li>Añadirle gastos</li> 
     <li>Añadirle tareas (si se trata de un proyecto)</li> 
     <li>Editar en él formularios personalizados</li> 
     <li>Registrar horas en el objeto</li> 
     <li>Realizar asignaciones en él</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Administrar</strong></td> 
   <td> <p>Puede realizar las siguientes acciones en el objeto:</p> 
    <ul> 
     <li>Todas las acciones incluidas con los permisos de visualización y aportación</li> 
     <li>Eliminarlo</li> 
     <li>Administrar información financiera en él</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Lo convierte en público para los usuarios externos</strong></td> 
   <td> <p>Cualquier persona que no tenga una cuenta de Workfront puede ver el objeto haciendo clic en un vínculo a él. Esto no está disponible para todos los objetos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Convertirlo en visible en todo el sistema.</strong></td> 
   <td> <p>El objeto se puede encontrar en búsquedas y ser visto por usuarios con una cuenta de Workfront.</p><p><b>Nota</b>: los usuarios con licencias de colaborador o solicitante no pueden ver proyectos, aunque esta configuración esté habilitada. </td> 
  </tr> 
 </tbody> 
</table>

## Comprender los permisos heredados y la jerarquía de objetos

### Permisos heredados de objetos principales {#permissions-inherited-from-parent-objects}

Los permisos en Workfront se heredan jerárquicamente. Esto significa que, si concede permisos a un usuario sobre un objeto principal, obtiene los mismos permisos sobre los objetos secundarios asociados a él de forma predeterminada.

Por ejemplo, si concede permisos de aportación a un usuario para un proyecto, el usuario tendrá permisos de aportación para todas las tareas y problemas (objetos secundarios) asociados a ese proyecto.

Siguiendo con el ejemplo anterior, no se pueden restringir los permisos en los objetos secundarios. Si no desea que el usuario tenga permisos de aportación para los objetos secundarios asociados al proyecto, debe quitar manualmente los permisos heredados de los objetos y, a continuación, ajustar los permisos para el usuario individual, incluida cualquier configuración avanzada. 

Para obtener más información sobre la jerarquía y la interdependencia de objetos en Workfront, consulte la sección [Interdependencia y jerarquía de objetos](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#interdependency-and-hierarchy-of-objects) en el artículo [Información general sobre los objetos de Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Su administrador de Workfront puede deshabilitar los permisos heredados para los documentos de su nivel de acceso.Para obtener más información sobre la deshabilitación de los permisos heredados de los documentos en el nivel de acceso, consulte [Crear o modificar niveles de acceso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### Permisos adquiridos mediante suscripciones a la organización  {#permissions-acquired-through-organizational-memberships}

Si concede permisos de administración a un grupo de usuarios de un objeto y concede permisos de visualización a un usuario individual de ese grupo en el mismo objeto, el usuario tendrá el nivel más alto de permisos (Administrar) concedido a través de los miembros del grupo en el objeto. 

Si desea conceder permisos inferiores a un usuario que ya forma parte de una unidad organizativa (Grupo, Equipo, Función o Compañía) con un nivel de permiso superior, debe quitar los permisos de la unidad organizativa y añadir usuarios individuales con un nivel inferior de permisos.


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

## Quitar permisos de objetos

Para obtener información sobre cómo quitar permisos de objetos, consulte [Quitar permisos de objetos](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Solicitar permisos para objetos

Cuando una persona le envía un vínculo a un objeto para el que no tiene permisos de visualización, o cuando tiene permisos inferiores en un objeto y desea solicitar un nivel superior de permisos, puede solicitar permisos en el objeto. 

Puede solicitar acceso a un objeto de cualquier persona que tenga permiso para compartir el objeto. 

Para obtener más información acerca de cómo solicitar permisos para objetos, consulte [Solicitar acceso a objetos](../../workfront-basics/grant-and-request-access-to-objects/request-access.md).
