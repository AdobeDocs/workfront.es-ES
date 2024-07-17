---
product-area: projects
navigation-topic: convert-issues
title: Desvincular problemas de sus objetos de resolución
description: Cuando crea un proyecto o una tarea al convertir un problema en el proyecto o la tarea, tiene la opción de mantener el problema original. El administrador de Adobe Workfront debe habilitar esta preferencia para que pueda tener esta opción durante la conversión del problema. Para obtener más información sobre la conversión de problemas a proyectos y tareas, consulte Información general sobre la conversión de problemas en Adobe Workfront.
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Desvincular problemas de sus objetos de resolución

Cuando crea un proyecto o una tarea al convertir un problema en el proyecto o la tarea, tiene la opción de mantener el problema original. El administrador de Adobe Workfront debe habilitar esta preferencia para que pueda tener esta opción durante la conversión del problema.\
Para obtener más información acerca de la conversión de problemas en proyectos y tareas, vea [Información general sobre la conversión de problemas en Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Cuando decide mantener el problema que se convirtió en el proyecto o en la tarea, la resolución del problema está vinculada al proyecto o a la tarea. El problema se convierte en el objeto solucionable del proyecto o de la tarea. El proyecto o la tarea son los objetos de resolución del problema.

También puede vincular manualmente un problema a otro. El segundo problema se convierte en el objeto de resolución del primer problema, en este caso.\
Para obtener más información sobre la resolución de objetos, vea [Información general sobre la resolución y los objetos solucionables](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

>[!TIP]
>
>El estado del problema no se puede cambiar, ya que cambia automáticamente con el estado del objeto de resolución.

Puede desvincular la resolución de un problema de la de un proyecto, tarea o problema eliminando el proyecto, la tarea o el problema del problema.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

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
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas</p> <p>Ver acceso a tareas y proyectos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos sobre el problema</p> <p>Ver permisos en la tarea o el proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Desvincular un problema de un proyecto, tarea o problema

1. Vaya al problema que está vinculado a un proyecto, tarea o problema.
1. Haga clic en la sección **Detalles del problema**.
1. Vaya al área de **Información general** de la sección **Detalles del problema**.
1. En el campo **Resuelto por**, quite el tipo de objeto solucionable.\
   Un problema puede resolverse mediante un proyecto, una tarea o un problema.

   Esto elimina el objeto de resolución del problema.

1. Haga clic en **Guardar** **Cambios**.\
   El problema ya no está vinculado a un proyecto, tarea o problema y ahora puede resolverlo de forma independiente.
