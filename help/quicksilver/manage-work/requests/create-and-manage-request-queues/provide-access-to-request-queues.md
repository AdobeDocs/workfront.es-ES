---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Proporcionar acceso a colas de solicitud
description: Cuando se proporciona acceso a una cola de solicitudes, se determina quién en la organización puede ver la cola de solicitudes en el área Solicitudes de Adobe Workfront.
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Proporcionar acceso a colas de solicitud

Cuando se proporciona acceso a una cola de solicitudes, se determina quién en la organización puede ver la cola de solicitudes en el área Solicitudes de Adobe Workfront.

Puede proporcionar a distintos usuarios acceso a una cola de solicitud, en función de si forman parte del equipo del proyecto, del grupo del proyecto o de la empresa del proyecto. También puede proporcionar acceso a todos los miembros del sistema a una cola de solicitudes. 

Esto resulta útil en organizaciones que invitan a partes interesadas externas a Workfront y desean limitar el acceso de los usuarios a áreas específicas; en este caso, una cola de solicitudes abierta únicamente a los usuarios asociados con la empresa o el grupo del proyecto limita la visibilidad a las partes interesadas externas. Al permitir el acceso a cualquier persona, la solicitud es visible tanto para las partes interesadas internas como para las externas.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p> Administrar permisos para el proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront

## Requisitos previos

Antes de que la cola de solicitudes esté disponible para los usuarios del área Solicitudes , debe crear un proyecto con la siguiente configuración:

* Designarla como una cola de solicitudes. Para obtener más información sobre la creación de una cola de solicitud, consulte [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* Actualice el estado del proyecto a Actual.

## Proporcionar acceso a una cola de solicitud

1. Vaya al proyecto en el que desea proporcionar acceso a las colas de solicitud.

   >[!NOTE]
   >
   >En el área Solicitudes solo están visibles los proyectos con el estado Actual.

1. Haga clic en **Detalles de cola** en el panel izquierdo. Es posible que tenga que hacer clic en **Mostrar más**, luego **Detalles de cola**.
1. Select **Publicar como cola de solicitud de ayuda** para designar el proyecto como cola de solicitud.
1. Seleccione entre las siguientes opciones:

   * **Cualquiera**: Cualquier usuario puede ver y agregar solicitudes a la cola de solicitudes.
   * **Personas con acceso a la vista de este proyecto**: Los usuarios que tienen permisos de Vista en el proyecto pueden ver y agregar solicitudes a la cola de solicitudes. 
   * **Personas en la compañía de este proyecto**: Los usuarios asociados con la empresa del proyecto pueden ver y agregar solicitudes. La empresa asociada al proyecto se muestra entre paréntesis junto a esta opción. 
   * **Personas del grupo de este proyecto**: Los usuarios asociados con el grupo del proyecto pueden ver y agregar solicitudes. El grupo asociado al proyecto se muestra entre paréntesis junto a esta opción.

      Las colas de grupo son útiles cuando varios departamentos comparten una cuenta de Workfront para lograr objetivos organizativos únicos. Cada departamento puede tener sus propias colas que los miembros de otros grupos no deberían poder ver.

      Para obtener información sobre quién tiene permisos en un proyecto, consulte [Uso compartido de un proyecto en Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).\
      Los grupos y las empresas pueden asociarse con el proyecto al editarlo. Para obtener más información sobre la edición de proyectos, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Haga clic en **Guardar**.
