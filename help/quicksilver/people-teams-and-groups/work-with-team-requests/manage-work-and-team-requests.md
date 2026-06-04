---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Administrar solicitudes de trabajo y equipo
description: Una solicitud representa una asignación de tarea o problema pendiente. Las solicitudes de trabajo se realizan a individuos y las solicitudes de equipo se realizan a equipos.
author: Courtney
feature: People Teams and Groups, Work Management
exl-id: ef96e520-0d5f-4180-a27a-1fbbffff8f2b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/h9ebMyu8AQNPQTzfYkEMbEbHtghIj-wegaml3cM3RMY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: be65ef36-43e4-48e1-a062-caa3778e15beid: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 488
ht-degree: 96%

---

# Administrar solicitudes de trabajo y equipo

Una solicitud representa una asignación de tarea o problema pendiente. Las solicitudes de trabajo se realizan a individuos y las solicitudes de equipo se realizan a equipos.

>[!NOTE]
>
>Los equipos de Agile no tienen solicitudes de equipo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Para asignar o trabajar en una solicitud:
   <p>Ligero o superior</p>
  <p>Revisión o superior</p>
   <p>Para reasignar una solicitud:
   <p>Estándar</p>
   <p>Trabajo o superior</p></td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Asignar una solicitud a un equipo {#assign-a-request-to-a-team}

Los gestores de proyecto y los solicitantes de problemas pueden asignar trabajo a los equipos cuando no saben qué recurso es adecuado para realizar el trabajo o cuando no importa quién lo complete.

Las tareas asignadas al equipo permanecen en la pestaña [!UICONTROL Team Requests] hasta que un usuario del equipo se ofrezca voluntario para trabajar en la solicitud.

Cuando se asigna una solicitud a un equipo y a un usuario que no es miembro del equipo, esta se puede ver tanto en la pestaña [!UICONTROL Team Requests] como en el área de solicitudes de trabajo del usuario. Si el usuario que no está en el equipo se ofrece como voluntario para trabajar en la tarea, esta permanecerá en la pestaña [!UICONTROL Team Requests] hasta que un usuario del equipo se ofrezca como voluntario para trabajar en ella.

Los equipos pueden asignarse a tareas y problemas de cualquiera de las siguientes maneras:

* A través del [!UICONTROL Gantt Chart]
* Desde una lista de tareas o problemas (individual o en de forma masiva)
* Cuando se crea o modifica una tarea o un problema
* Mediante reglas de enrutamiento en una solicitud (solo problemas)

Puede asignar manualmente una solicitud a un equipo desde la página de equipos, tal como se describe en esta sección.

Para asignar manualmente una solicitud a un equipo desde la página de equipos:

{{step1-to-team}}

1. Haga clic en el icono **[!UICONTROL Switch team]** ![Cambiar icono de equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Haga clic en el icono **[!UICONTROL More]** ![](assets/more-icon.png) y, a continuación, seleccione **[!UICONTROL Send work request]**.

   ![](assets/edit-team-settings-350x205.png)

1. Rellene la información del cuadro que se abre.
1. Haga clic en **[!UICONTROL Send Request]**.\
   Ahora se asigna al equipo una nueva tarea que se muestra en la pestaña Solicitudes de equipo. Esta tarea no está asociada actualmente a un proyecto, pero se puede mover, tal como se describe en [Mover tareas](../../manage-work/tasks/manage-tasks/move-tasks.md).

## Solicitudes de reasignación {#reassign-requests}

Puede reasignar solicitudes que se hayan asignado a su equipo:

{{step1-to-team}}

1. Haga clic en el icono **[!UICONTROL Switch team]** ![Cambiar icono de equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.
1. En el panel de navegación izquierdo, seleccione **[!UICONTROL Team Requests]**.
1. Haga clic en el icono **[!UICONTROL Reassign]**.

1. Empiece a escribir el nombre del usuario, grupo o equipo al que desea reasignar la solicitud y, a continuación, haga clic en **[!UICONTROL Assign]**.\
   Se reasigna la solicitud.
