---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Resumen de solicitudes de equipo
description: Las solicitudes de equipo se encuentran en el área Equipos del menú principal.
author: Lisa
feature: People Teams and Groups
exl-id: c131c021-8bc0-4a48-a873-9ee0e189bcab
source-git-commit: 9693ac3792fec3eca6218a228f2067519ed433ac
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Resumen de solicitudes de equipo

## Comprender las solicitudes de equipo

Las solicitudes de equipo se encuentran en el área [!UICONTROL Equipos] del [!UICONTROL Menú principal]. Haga clic en el icono [!UICONTROL Solicitudes de equipo] ![Icono de solicitud](assets/request-icon.png) en el panel izquierdo para ver las solicitudes de equipo.

>[!NOTE]
>
>Los equipos de Agile no tienen solicitudes de equipo.

La ficha [!UICONTROL Solicitudes de equipo] muestra las solicitudes en espera de asignación para el equipo seleccionado actualmente en la lista desplegable. El número entre paréntesis indica cuántos elementos están listos para trabajar.

Una solicitud de equipo representa un elemento de trabajo pendiente que no está asignado a un usuario específico. En su lugar, se le asigna a un equipo y cualquier miembro de ese equipo puede ofrecerse como voluntario para aceptar la responsabilidad del artículo. Si un usuario se ofrece voluntario para trabajar en una solicitud de equipo, el usuario acepta la asignación de trabajo como propia. La tarea se asigna al usuario individual además del equipo.

>[!NOTE]
>
>No se debe utilizar una solicitud de equipo para asignaciones de tareas de colaboración. Si necesita asignar varios usuarios para que trabajen juntos en una tarea, hágalo a través de [!UICONTROL Asignaciones avanzadas] y no a través de Solicitudes de equipo. Para obtener más información, consulte [Crear asignaciones avanzadas](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

## Comprenda las opciones [!UICONTROL Listo para comenzar] y [!UICONTROL Todos]

Hay dos opciones en la parte superior de la sección de solicitudes de equipo: [!UICONTROL Listo para comenzar] y [!UICONTROL Todo].

La opción [!UICONTROL Listo para comenzar] solo muestra las tareas y los problemas que cumplen todos los criterios siguientes:

* Todas las predecesoras han cumplido las condiciones de los tipos de dependencia de predecesoras.\
  Por ejemplo, si el tipo de relación de predecesora es [!UICONTROL Finalizar-Iniciar] (la tarea de predecesora debe finalizar antes de que pueda comenzar la tarea dependiente), la predecesora debe marcarse como [!UICONTROL Completada]. (Para obtener más información acerca de los tipos de dependencia de predecesoras, vea [Información general sobre los tipos de dependencia de tareas](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).)

* El usuario que ha iniciado sesión es la persona asignada a estas tareas y problemas (para solicitudes de trabajo), o el equipo seleccionado está asignado a estas tareas y problemas (para solicitudes de equipo).
* El estado del proyecto es [!UICONTROL Actual].
* La [!UICONTROL fecha proyectada de inicio] o la [!UICONTROL fecha planificada de inicio] han pasado o están programadas para comenzar en un plazo de dos semanas a partir de la fecha de hoy (o no se ha definido una [!UICONTROL fecha proyectada de inicio] o una [!UICONTROL fecha planificada de inicio]).
* La [!UICONTROL fecha de transferencia] ya se ha producido o se producirá en un plazo de dos semanas a partir de la fecha actual.

>[!NOTE]
>
>Si la tarea cumple los tres primeros criterios y tiene una fecha de transferencia dentro de las dos semanas siguientes a la fecha actual, se mostrará como [!UICONTROL Lista para comenzar] aunque las fechas planificadas/proyectadas superen las dos semanas. Si la tarea no tiene una fecha de transferencia, las fechas planificadas/proyectadas deben estar dentro de las dos semanas de la fecha actual.

La opción [!UICONTROL Todos] muestra todas las tareas y problemas de los proyectos actuales que están asignados al usuario que ha iniciado sesión o todas las tareas o problemas asignados al equipo.
