---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Administrar solicitudes de trabajo y equipo
description: Una solicitud representa una asignación de tarea o problema pendiente. Las solicitudes de trabajo se realizan a individuos y las solicitudes de equipo se realizan a equipos.
author: Lisa
feature: People Teams and Groups, Work Management
exl-id: ef96e520-0d5f-4180-a27a-1fbbffff8f2b
source-git-commit: dfd5c7423b65e6065ab9c2094578443b81189abd
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---

# Administrar solicitudes de trabajo y equipo

Una solicitud representa una asignación de tarea o problema pendiente. Las solicitudes de trabajo se realizan a individuos y las solicitudes de equipo se realizan a equipos.

>[!NOTE]
>
>Los equipos de Agile no tienen solicitudes de equipo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Para asignar o trabajar en una solicitud:
   <p>Nuevo: Claro o superior</br>
    o</br>
   Actual: revisar o superior</p>
   <p>Para reasignar una solicitud:
   <p>Nuevo: Estándar</br>
    o</br>
   Actual: Trabajo o superior</p></td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Asignar una solicitud a un equipo {#assign-a-request-to-a-team}

Los jefes de proyecto y los solicitantes de problemas pueden asignar trabajo a los equipos cuando no saben qué recurso es adecuado para realizar el trabajo o cuando no importa quién lo complete.

Las tareas asignadas al equipo permanecen en la ficha [!UICONTROL Solicitudes de equipo] hasta que un usuario del equipo se ofrezca voluntario para trabajar en la solicitud.

Cuando se asigna una solicitud a un equipo y a un usuario que no es miembro del equipo, esta se puede ver tanto en la ficha [!UICONTROL Solicitudes de equipo] como en el área de solicitudes de trabajo del usuario. Si el usuario que no está en el equipo se ofrece como voluntario para trabajar en la tarea, esta permanecerá en la ficha [!UICONTROL Solicitudes de equipo] hasta que un usuario del equipo se ofrezca como voluntario para trabajar en ella.

Los equipos pueden asignarse a tareas y problemas de cualquiera de las siguientes maneras:

* A través del [!UICONTROL gráfico Gantt]
* Desde una lista de tareas o problemas (individual o en bloque)
* Cuando se crea o modifica una tarea o un problema
* Mediante reglas de enrutamiento en una solicitud (solo problemas)

Puede asignar manualmente una solicitud a un equipo desde la página de equipo, tal como se describe en esta sección.

Para asignar manualmente una solicitud a un equipo desde la página de equipo:

{{step1-to-team}}

1. Haga clic en el icono **[!UICONTROL Cambiar equipo]** ![Cambiar icono de equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Haga clic en el icono **[!UICONTROL Más]** ![](assets/more-icon.png) y, a continuación, seleccione **[!UICONTROL Enviar solicitud de trabajo]**.

   ![](assets/edit-team-settings-350x205.png)

1. Rellene la información del cuadro que se abre.
1. Haga clic en **[!UICONTROL Enviar solicitud]**.\
   Ahora se asigna al equipo una nueva tarea que se muestra en la pestaña Solicitudes de equipo. Esta tarea no está asociada actualmente a un proyecto, pero se puede mover, como se describe en [Mover tareas](../../manage-work/tasks/manage-tasks/move-tasks.md).

## Solicitudes de reasignación {#reassign-requests}

Puede reasignar solicitudes que se hayan asignado a su equipo:

{{step1-to-team}}

1. Haga clic en el icono **[!UICONTROL Cambiar equipo]** ![Cambiar icono de equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.
1. En el panel de navegación izquierdo, seleccione **[!UICONTROL Solicitudes de equipo]**.
1. Haga clic en el icono **[!UICONTROL Reasignar]**.

1. Empiece a escribir el nombre del usuario, grupo o equipo al que desea reasignar la solicitud y, a continuación, haga clic en **[!UICONTROL Asignar]**.\
   Se reasigna la solicitud.
