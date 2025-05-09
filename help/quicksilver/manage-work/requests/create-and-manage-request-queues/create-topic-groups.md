---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Crear grupos de temas
description: Los grupos de temas están asociados a las colas de solicitudes. Permiten clasificar las colas de solicitudes en varias categorías según la naturaleza de las solicitudes.
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 7c5959f4-f33f-4f5e-b031-748dbe1a24a5
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 90%

---

# Crear grupos de temas

<!-- Audited: 2/2024 -->

Los grupos de temas están asociados a las colas de solicitudes. Las colas de solicitudes se pueden clasificar en varias categorías, según la naturaleza de las solicitudes, mediante grupos de temas.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Licencia de Adobe Workfront</p> </td> 
   <td>   
      <p>Nuevo: estándar</p>
      <p>O</p> 
      <p>Actual: plan</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p> Administrar permisos del proyecto</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Información general sobre los grupos de temas

Por ejemplo, si tiene una cola de solicitudes para solicitudes de marketing, puede tener un grupo de temas de “Campaña del día de la madre”, con uno de segundo nivel de “Medios digitales” y otro de segundo nivel de “Medios impresos”. Entonces, puede tener varios temas de la cola dentro de cada grupo de temas. Por ejemplo, “Publicidad tipo titular” y “Blog” pueden ser temas de la cola para el grupo de temas “Medios digitales”.

Para obtener más información sobre cómo crear colas de solicitudes, consulte [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Tenga en cuenta lo siguiente al trabajar con grupos de temas:

* Puede crear hasta 10 niveles de grupos de temas dentro de una cola de solicitudes.
* No hay límite en el número de temas de cola que se pueden asociar a un grupo de temas.
* Los grupos de temas son un objeto notificable.
* No se pueden mover grupos de temas de un proyecto a otro.

## Crear grupos de temas

Se recomienda crear grupos de temas antes de crear un tema de cola. Sin embargo, se puede crear un grupo de temas dentro en el generador de temas de cola. Para obtener más información sobre cómo crear temas de colas, consulte [Crear temas de cola](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

Para crear un grupo de temas:

1. Vaya al proyecto que ha publicado como Cola de solicitudes de ayuda.\
   Para obtener más información sobre cómo publicar un proyecto como cola de solicitud de ayuda, consulte [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Haga clic en **Grupos de temas** en el panel izquierdo.
1. Crear **Nuevo grupo de temas**

   ![](assets/new-topic-group-box-nwe-350x306.png)

1. Especifique la siguiente información:

   * **Nombre**: el nombre es visible para los usuarios que envían solicitudes a esta cola de solicitudes.
   * **Descripción**: la descripción se muestra cuando los usuarios seleccionan el grupo de temas en el proceso de envío de una nueva solicitud.
   * **Añadir al grupo de temas**: puede añadir el nuevo grupo de temas a uno existente o directamente al proyecto publicado como Cola de solicitudes de ayuda.

1. Haga clic en **Guardar**.\
   Esto crea un nuevo grupo de temas en la cola de solicitudes. Ahora puede seleccionar categorías adicionales en el primer menú desplegable debajo de una cola de solicitudes.\
   Para obtener más información sobre cómo enviar solicitudes, consulte [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
