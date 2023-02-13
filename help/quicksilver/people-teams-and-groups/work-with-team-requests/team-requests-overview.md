---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Información general sobre solicitudes de equipo
description: Las solicitudes del equipo se encuentran en el área Equipos del menú principal.
author: Lisa
feature: People Teams and Groups
exl-id: c131c021-8bc0-4a48-a873-9ee0e189bcab
source-git-commit: 9693ac3792fec3eca6218a228f2067519ed433ac
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Información general sobre solicitudes de equipo

## Comprender las solicitudes del equipo

Las solicitudes del equipo se encuentran en la [!UICONTROL Equipos] en el [!UICONTROL Menú principal]. Haga clic en el [!UICONTROL Solicitudes del equipo] icono ![Icono de solicitud](assets/request-icon.png) en el panel izquierdo para ver las solicitudes del equipo.

>[!NOTE]
>
>Los equipos móviles no tienen solicitudes de equipo.

La variable [!UICONTROL Solicitudes del equipo] muestra las solicitudes en espera de asignación para el equipo que está seleccionado actualmente en la lista desplegable. El número entre paréntesis indica cuántos artículos están listos para trabajar.

Una solicitud de equipo representa un elemento de trabajo pendiente que no está asignado a un usuario específico. En su lugar, se asigna a un equipo, y cualquier miembro de ese equipo puede voluntariamente aceptar la responsabilidad por el artículo. Si un usuario se ofrece a trabajar en una solicitud de equipo, el usuario acepta la asignación de trabajo como propia. La tarea se asigna al usuario individual además del equipo.

>[!NOTE]
>
>Una solicitud de equipo no debe utilizarse para asignaciones de tareas colaborativas. Si necesita asignar varios usuarios para que trabajen juntos en una tarea, siga este procedimiento [!UICONTROL Asignaciones avanzadas] y no a través de solicitudes del equipo. Para obtener más información, consulte [Crear asignaciones avanzadas](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

## Comprender el [!UICONTROL Listo para empezar] y [!UICONTROL Todo] opciones

Hay dos opciones en la parte superior de la sección Solicitudes de equipo : [!UICONTROL Listo para empezar] y [!UICONTROL Todo].

La variable [!UICONTROL Listo para empezar] solo muestra las tareas y los problemas que cumplen todos los criterios siguientes:

* Todos los predecesores han cumplido las condiciones para sus tipos de dependencias predecesores.\
   Por ejemplo, si el tipo de relación de predecesor es [!UICONTROL Finish-Start] (la tarea predecesora debe finalizar antes de que pueda iniciarse la tarea dependiente), el predecesor debe marcarse como [!UICONTROL Completar]. (Para obtener más información sobre los tipos de dependencias predecesores, consulte [Descripción general de los tipos de dependencia de tareas](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).)

* El usuario que ha iniciado sesión es la persona asignada a estas tareas y problemas (para solicitudes de trabajo), o el equipo seleccionado se asigna a estas tareas y problemas (para solicitudes de equipo).
* El estado del proyecto es [!UICONTROL Actual].
* La variable [!UICONTROL Fecha inicial prevista] o [!UICONTROL Fecha de inicio planeada] ha pasado o está programado que comience dentro de las dos semanas siguientes a la fecha de hoy (o no [!UICONTROL Fecha inicial prevista] o [!UICONTROL Fecha de inicio planeada] se ha definido).
* La variable [!UICONTROL Fecha de entrega] ya se ha producido o se producirá en un plazo de dos semanas a partir de la fecha actual.

>[!NOTE]
>
>Si la tarea cumple los tres primeros criterios y tiene una fecha de entrega en un plazo de dos semanas a partir de la fecha actual, se mostrará como [!UICONTROL Listo para empezar] incluso si las fechas previstas/proyectadas están por encima de dos semanas. Si la tarea no tiene una fecha de entrega, las fechas Planificadas/Proyectadas deben estar dentro de las dos semanas de la fecha actual.

La variable [!UICONTROL Todo] muestra todas las tareas y problemas de los proyectos actuales asignados al usuario que ha iniciado sesión o todas las tareas o problemas asignados al equipo.
