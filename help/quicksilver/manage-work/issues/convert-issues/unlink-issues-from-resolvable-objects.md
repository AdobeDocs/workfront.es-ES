---
product-area: projects
navigation-topic: convert-issues
title: Desvincular problemas de sus objetos de resolución
description: Cuando crea un proyecto o una tarea, al convertir un problema en el proyecto o la tarea, tiene la opción de mantener el problema original. El administrador de Adobe Workfront debe habilitar esta preferencia para que pueda tener esta opción durante la conversión del problema. Para obtener más información sobre la conversión de problemas en proyectos y tareas, consulte Información general sobre la conversión de problemas en Adobe Workfront.
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 95%

---

# Desvincular problemas de sus objetos de resolución

<!--Audited: 08/2025-->

Cuando crea un proyecto o una tarea, al convertir un problema en el proyecto o la tarea, tiene la opción de mantener el problema original. El administrador de Adobe Workfront debe habilitar esta preferencia para que pueda tener esta opción durante la conversión del problema.\
Para obtener más información sobre la conversión de problemas en proyectos y tareas, consulte [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Cuando decide mantener el problema que se convirtió en el proyecto o en la tarea, la resolución del problema está vinculada al proyecto o a la tarea. El problema se convierte en el objeto que se puede resolver en el proyecto o la tarea. El proyecto o la tarea son los objetos que se pueden resolver del problema.

También puede vincular manualmente un problema a otro. El segundo problema se convierte en el objeto que se puede resolver del primer problema, en este caso.\
Para obtener más información sobre la objetos que se pueden resolver, consulte [Información general sobre resolución y objetos que se pueden resolver](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

>[!TIP]
>
>El estado del problema no se puede cambiar, ya que cambia automáticamente con el estado del objeto que se puede resolver.

Puede desvincular la resolución de un problema de la de un proyecto, tarea o problema eliminando el proyecto, la tarea o el problema del problema.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Colaborador o superior</p>
   <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuración de nivel de acceso</td> 
   <td> <p>Editar acceso a Problemas</p> <p>Ver acceso a tareas y proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración del problema</p> <p>Permisos de vista para la tarea o el proyecto</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
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
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Issues</p> <p>View access to Tasks and&nbsp;Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the issue</p> <p>View permissions on the task or project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Desvincular un problema de un proyecto, tarea o problema

1. Vaya al problema que está vinculado a un proyecto, tarea o problema.
1. Haga clic en la sección **Detalles del problema**.
1. Vaya al área de **Información general** de la sección **Detalles del problema**.
1. En el campo **Resuelto por**, quite el tipo de objeto que se puede resolver.\
   Un problema puede resolverse mediante un proyecto, una tarea o un problema.

   Esto qutia el objeto que se puede resolver del problema.

1. Haga clic en **Guardar** **cambios**.\
   El problema ya no está vinculado a un proyecto, tarea o problema y ahora puede resolverlo de forma independiente.
