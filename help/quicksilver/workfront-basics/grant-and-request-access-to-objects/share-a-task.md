---
title: Compartir una tarea
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: El administrador de Adobe Workfront puede concederle acceso para ver o editar tareas cuando asignen niveles de acceso. Para obtener más información sobre la concesión de acceso a tareas, consulte Concesión de acceso a tareas.
author: Alina
feature: Get Started with Workfront
exl-id: 45da15cb-8880-41f7-a0de-939882c1f154
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 4%

---

# Compartir una tarea

El administrador de Adobe Workfront puede concederle acceso para ver o editar tareas cuando asignen niveles de acceso. Para obtener más información sobre la concesión de acceso a tareas, consulte [Concesión de acceso a tareas](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

Junto con el nivel de acceso que se concede a los usuarios, también puede otorgarles permisos para Ver, Contribuir o Administrar tareas específicas a las que tenga acceso para compartir.

Los permisos son específicos para un elemento de Workfront y definen qué acciones se pueden realizar en ese elemento.

## Consideraciones al compartir una tarea

Además de las consideraciones siguientes, consulte [Información general sobre cómo compartir permisos en objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* El creador de una tarea tiene permisos de administración de forma predeterminada.
* Puede compartir tareas de forma individual o varias de ellas a la vez, de forma masiva.\
   Compartir tareas es idéntico al uso compartido de otros objetos. Para obtener más información sobre cómo compartir elementos en Workfront, consulte [Compartir un objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Puede conceder los siguientes permisos a una tarea: 

   * Vista
   * Administrar
   * Aportar\
      ![](assets/screen-shot-2014-05-30-at-11.37.24-am-175x192.png) ![](assets/screen-shot-2014-01-23-at-1.12.40-pm-154x258.png) ![](assets/screen-shot-2014-01-22-at-10.53.00-am-182x252.png)

* Al compartir una tarea, los usuarios heredan los mismos permisos de forma predeterminada en todos los objetos secundarios asociados a la tarea. Por ejemplo, heredan los mismos permisos sobre las tareas secundarias, los problemas y los documentos adjuntos a la tarea.\
   Para obtener más información sobre la jerarquía de objetos en Workfront, consulte  [Explicación de los objetos en Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   El administrador de Workfront puede especificar si los documentos deben heredar permisos de objetos superiores en el nivel de acceso del usuario. Para obtener más información sobre la restricción de permisos heredados en documentos, consulte [Crear o modificar niveles de acceso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Puede quitar permisos heredados de una tarea.\
   Para obtener más información sobre cómo quitar permisos heredados de objetos, consulte  [Eliminación de permisos de objetos](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Formas de compartir una tarea

Puede compartir una tarea de las siguientes maneras:

* Manualmente, ya sea de forma individual o en masa. Compartir manualmente tareas es similar a compartir cualquier otro objeto en Workfront.

   Para obtener más información sobre cómo compartir objetos en Workfront, consulte  [Compartir un objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Automáticamente, haciendo lo siguiente:

   * Especifique los permisos en cualquiera de los objetos principales de la tarea: proyecto, programa o portafolio. Las tareas heredan los permisos de sus objetos principales. Para obtener información sobre la visualización de permisos heredados en objetos, consulte [Ver permisos heredados en objetos](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * Agregue entidades a Uso compartido de proyectos en una plantilla utilizada para crear el proyecto en el que se encuentra la tarea. Para obtener información sobre cómo compartir proyectos desde plantillas, consulte [Compartir una plantilla](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * Especifique los permisos de todas las tareas de un proyecto al editarlo. Para obtener información sobre la administración del acceso a las tareas del proyecto en función de los permisos de un usuario para el proyecto, consulte la [](../../manage-work/projects/manage-projects/edit-projects.md#access) sección del artículo [Editar proyectos](../../manage-work/projects/manage-projects/edit-projects.md).
   >[!TIP]
   >
   >Si no especifica qué permisos de tareas desea que tengan los usuarios cuando estén asignados a las tareas del proyecto, reciben los mismos permisos que tienen en el proyecto de forma predeterminada.

## Permisos de tareas

La tabla siguiente muestra los permisos que puede conceder a los usuarios cuando les permite ver, Contribute o administrar una tarea:

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Acción</strong> </th> 
   <th><strong>Administrar</strong> </th> 
   <th><strong>Aportar</strong> </th> 
   <th><strong>Vista</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">Agregar tareas</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Agregar Predecesores</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Agregar problemas</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Eliminar tarea</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row"> <p>Edición general de tareas<br></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Cambiar estado de tarea</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Editar restricción de tarea</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Ver tarea</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Agregar documentos</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Copiar tarea*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Mover tarea*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Registrar horas</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Modificar fechas planificadas</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aceptar asignación</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Realizar una asignación</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Adjuntar formulario personalizado</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Editar campos personalizados</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Crear un proceso de aprobación</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aprobar Una Tarea</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Editar finanzas*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Agregar/Editar gastos</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Ver finanzas</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Actualizaciones/comentarios</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Compartir</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Compartir en todo el sistema</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;Se controla mediante el nivel de acceso y los permisos del proyecto.
