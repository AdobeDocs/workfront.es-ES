---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Proporcionar acceso a las colas de solicitudes
description: Al proporcionar acceso a una cola de solicitudes, se determina quién de la organización puede ver la cola en el área Solicitudes de Adobe Workfront.
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Proporcionar acceso a las colas de solicitudes

Al proporcionar acceso a una cola de solicitudes, se determina quién de la organización puede ver la cola en el área Solicitudes de Adobe Workfront.

Puede proporcionar a distintos usuarios acceso a una cola de solicitudes, en función de si forman parte del equipo del proyecto, del grupo de proyectos o de la compañía del proyecto. También puede proporcionar acceso a todos los usuarios del sistema a una cola de solicitudes. 

Esto resulta útil en organizaciones que invitan a partes interesadas externas a Workfront y desean limitar el acceso de los usuarios a áreas específicas; en este caso, una cola de solicitudes abierta solo a los usuarios asociados con la compañía o el grupo del proyecto limita la visibilidad a las partes interesadas externas. Al permitir el acceso a cualquier persona, la solicitud se hace visible tanto para las partes interesadas internas como externas.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p> Administración de permisos del proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront

## Requisitos previos

Antes de que la cola de solicitudes esté disponible para los usuarios en el área de Solicitudes, debe crear un proyecto con la siguiente configuración:

* Designarlo como cola de solicitudes. Para obtener más información acerca de cómo crear una cola de solicitudes, vea [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* Actualice el estado del proyecto a Actual.

## Proporcionar acceso a una cola de solicitudes

1. Vaya al proyecto en el que desea proporcionar acceso a las colas de solicitudes.

   >[!NOTE]
   >
   >En el área de solicitudes solo están visibles los proyectos con el estado Actual.

1. Haga clic en **Detalles de cola** en el panel izquierdo. Es posible que tengas que hacer clic en **Mostrar más** y luego en **Detalles de la cola**.
1. Seleccione **Publish como cola de solicitud de ayuda** para designar el proyecto como cola de solicitud.
1. Seleccione entre las siguientes opciones:

   * **Cualquiera**: cualquier usuario puede ver y agregar solicitudes a la cola de solicitudes.
   * **Personas con acceso de visualización en este proyecto**: Los usuarios que tienen permisos de visualización en el proyecto pueden ver y agregar solicitudes a la cola de solicitudes. 
   * **Personas en la compañía de este proyecto**: Los usuarios asociados con la compañía del proyecto pueden ver y agregar solicitudes. La compañía asociada con el proyecto se enumera entre paréntesis junto a esta opción. 
   * **Las personas en el grupo de este proyecto**:Los usuarios asociados con el grupo del proyecto pueden ver y agregar solicitudes. El grupo asociado con el proyecto se muestra entre paréntesis junto a esta opción.

     Las colas de grupo son útiles cuando varios departamentos comparten una cuenta de Workfront para lograr objetivos organizativos únicos. Cada departamento puede tener sus propias colas que los miembros de otros grupos no deberían poder ver.

     Para obtener información sobre quién tiene permisos en un proyecto, consulte [Compartir un proyecto en Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).\
     Los grupos y empresas pueden asociarse con el proyecto al editarlo. Para obtener más información sobre cómo editar proyectos, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Haga clic en **Guardar**.
