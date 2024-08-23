---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Crear grupos de temas
description: Los grupos de temas están asociados a las colas de solicitudes. Permiten clasificar las colas de solicitudes en varias categorías, según la naturaleza de las solicitudes.
author: Lisa
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 7c5959f4-f33f-4f5e-b031-748dbe1a24a5
source-git-commit: 067a5bd54f794574f5f2d1ad98ad29b6e02ab297
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# Crear grupos de temas

<!-- Audited: 2/2024 -->

Los grupos de temas están asociados a las colas de solicitudes. Permiten clasificar las colas de solicitudes en varias categorías, según la naturaleza de las solicitudes.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
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
   <td> <p>Editar acceso a Proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p> Administración de permisos del proyecto</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Información general sobre los grupos de temas

Por ejemplo, si tiene una cola de solicitudes para solicitudes de marketing, puede tener un grupo de temas de &quot;Campaña del día de la madre&quot;, con un grupo de temas de segundo nivel de &quot;Medios digitales&quot; y un grupo de temas de segundo nivel adicional de &quot;Medios impresos&quot;. A continuación, puede tener varios temas de la cola dentro de cada grupo de temas. Por ejemplo, &quot;Anuncio de banner&quot; y &quot;Blog&quot; pueden ser temas de cola para el grupo de temas &quot;Medios digitales&quot;.

Para obtener más información acerca de cómo crear colas de solicitudes, vea [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!TIP]
>
>* Puede crear hasta 10 niveles de grupos de temas dentro de una cola de solicitudes.
>* No hay límite en el número de temas de la cola que se pueden asociar a un grupo de temas.
>* Los grupos de temas son un objeto del que se puede informar.
>

## Crear grupos de temas

Se recomienda crear Grupos de temas antes de crear un Tema de la cola. Sin embargo, se puede crear un grupo de temas dentro de en el Generador de temas de colas. Para obtener más información acerca de cómo crear temas de colas, vea [Crear temas de colas](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

Para crear un grupo de temas:

1. Vaya al proyecto que ha publicado como Cola de solicitudes de ayuda.\
   Para obtener más información sobre cómo publicar un proyecto como cola de solicitud de ayuda, vea [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Haga clic en **Grupos de temas** en el panel izquierdo. Es posible que tengas que hacer clic en **Mostrar más** y luego en **Grupos de temas**.
1. Haga clic en **Nuevo grupo de temas**.

   ![](assets/new-topic-group-box-nwe-350x306.png)

1. Especifique la siguiente información:

   * **Nombre**: el nombre es visible para los usuarios que envían solicitudes a esta cola de solicitudes.
   * **Descripción**: la descripción se muestra cuando los usuarios seleccionan el grupo de temas en el proceso de envío de una nueva solicitud.
   * **Agregar al grupo de temas**: puede agregar el nuevo grupo de temas a un grupo de temas existente o puede agregarlo directamente al proyecto publicado como cola de solicitudes de ayuda.

1. Haga clic en **Guardar**.\
   Esto crea un nuevo grupo de temas en la cola de solicitudes. Ahora puede seleccionar categorías adicionales en el primer menú desplegable debajo de una Cola de solicitudes.\
   Para obtener más información sobre cómo enviar solicitudes, consulte [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
