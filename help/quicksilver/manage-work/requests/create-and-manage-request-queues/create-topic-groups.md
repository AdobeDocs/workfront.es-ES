---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Crear grupos de temas
description: Los grupos de temas están asociados con las colas de solicitud. Permiten clasificar las colas de solicitud en varias categorías, según la naturaleza de las solicitudes.
author: Alina
feature: Work Management
exl-id: 7c5959f4-f33f-4f5e-b031-748dbe1a24a5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# Crear grupos de temas

Los grupos de temas están asociados con las colas de solicitud. Permiten clasificar las colas de solicitud en varias categorías, según la naturaleza de las solicitudes.

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
   <td role="rowheader"> <p role="rowheader">Licencia de Adobe Workfront*</p> </td> 
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

## Descripción general de los grupos de temas

Por ejemplo, si tiene una cola de solicitud para solicitudes de marketing, puede tener un grupo de temas de &quot;Campaña del día de la madre&quot;, con un grupo de temas de segundo nivel de &quot;Medios digitales&quot; y un grupo de temas de segundo nivel adicional de &quot;Medios impresos&quot;. A continuación, puede tener varios temas de cola dentro de cada grupo de temas. Por ejemplo, &quot;Anuncio de banner&quot; y &quot;Blog&quot; pueden ser temas de cola para el grupo de temas &quot;Medios digitales&quot;.

Para obtener más información sobre cómo crear colas de solicitud, consulte [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!TIP]
>
>* Puede crear hasta 10 niveles de grupos de temas dentro de una cola de solicitud.
>* No hay límite en el número de temas de cola que se pueden asociar con un grupo de temas.
>* Los grupos de temas son un objeto que se puede informar.
>


## Crear grupos de temas

Se recomienda crear Grupos de temas antes de crear un Tema de cola. Sin embargo, se puede crear un grupo de temas dentro del generador de temas de cola. Para obtener más información sobre la creación de temas de cola, consulte [Crear temas de cola](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

Para crear un grupo de temas:

1. Vaya al proyecto que ha publicado como cola de solicitud de ayuda.\
   Para obtener más información sobre la publicación de un proyecto como cola de solicitud de ayuda, consulte [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Haga clic en **Grupos de temas** en el panel izquierdo. Es posible que tenga que hacer clic en **Mostrar más**, luego **Grupos de temas**.
1. Haga clic en **Nuevo grupo de temas**.

   ![](assets/new-topic-group-box-nwe-350x306.png)

1. Especifique la siguiente información:

   * **Nombre**: El nombre es visible para los usuarios que envían solicitudes a esta cola de solicitudes.
   * **Descripción**: La descripción se muestra cuando los usuarios seleccionan el grupo de temas en el proceso de envío de una nueva solicitud.
   * **Agregar al grupo de temas**: Puede agregar el nuevo grupo de temas a un grupo de temas existente o agregarlo directamente al proyecto publicado como cola de solicitud de ayuda.

1. Haga clic en **Guardar**.\
   Esto crea un nuevo grupo de temas en la cola de solicitud. Ahora puede seleccionar categorías adicionales en el primer menú desplegable de una cola de solicitud.\
   Para obtener más información sobre el envío de solicitudes, consulte [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
