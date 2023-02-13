---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: usuario,programación
navigation-topic: configure-timesheets-and-schedules
title: Información general sobre las programaciones
description: Puede definir la semana laboral mediante programas. Puede asociar una programación con un usuario o un proyecto. Esto permite que [!DNL Adobe Workfront] para calcular las cronologías y la disponibilidad del usuario. Para obtener instrucciones, consulte Crear una programación.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---

# Información general sobre las programaciones

Puede definir la semana laboral mediante programaciones y asociar una programación a un usuario o proyecto. Esto permite que [!DNL Adobe Workfront] para calcular las cronologías y la disponibilidad del usuario. Para obtener instrucciones, consulte [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Tenga en cuenta lo siguiente cuando trabaje con programaciones en Workfront:

* La variable [!DNL Workfront] el administrador identifica las horas de funcionamiento de la organización en una programación.

   Del mismo modo, un administrador de grupo puede identificar las horas de funcionamiento de una programación administrada por un grupo que administra.

   Para obtener más información sobre los administradores de grupos, consulte [Administradores de grupo](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

   Por ejemplo, una programación se puede definir como: De lunes a viernes, de 8:00 a 17:00, con una hora de descanso para el almuerzo.

* [!DNL Workfront] utiliza la programación para determinar cuándo comienza y finaliza la jornada laboral.

   Esto no impide que un usuario trabaje o complete el trabajo en [!DNL Workfront] fuera del horario laboral normal. Por lo general, no es necesario crear un nuevo programa o una excepción de programación para centrarse en el trabajo planificado por la noche.

   Del mismo modo, es posible que su organización tenga horarios de llegada flexibles para su jornada laboral. Puede tener un conjunto de empleados que llega a las 8 a. m. y otro conjunto que llega a las 9 a. m. No es necesario crear programaciones únicas para cada grupo, si los grupos tienen programaciones similares o idénticas. Pero si los grupos tienen programaciones drásticamente diferentes, sus usuarios deben estar asociados con programaciones únicas. Un empleado entiende que si una asignación se debe completar a las 5 p. m., significa que el trabajo debe realizarse al final del día hábil, independientemente de la hora en que entre al trabajo.

* Se recomienda crear programas independientes para cada zona horaria asociada a la organización.

   Puede asignar una zona horaria específica a cada programación para asegurarse de que el trabajo esté programado correctamente para los usuarios que trabajan en diferentes zonas horarias.

* La variable [!DNL Workfront] La programación predeterminada se utiliza en los cálculos de cronología cuando los usuarios o proyectos no están asociados a una programación.

   La programación predeterminada viene con su [!DNL Workfront] y no se pueden eliminar a menos que se reemplacen por una nueva programación que cree.

* Además de calcular las cronologías, [!DNL Workfront] utiliza programas para calcular la disponibilidad del usuario.

   >[!IMPORTANT]
   >
   >[!DNL Workfront] utiliza el usuario o la programación del proyecto para determinar la disponibilidad de recursos en el Planificador de recursos. La programación utilizada depende de la [!DNL Workfront] administrador seleccionado para el [!UICONTROL Calcular la disponibilidad de los recursos utilizando] configuración. Para obtener información sobre la configuración de Administración de recursos, consulte [Configurar las preferencias de Administración de recursos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Jerarquía de programaciones

Si se asigna una tarea a un usuario que está asociado con una programación y reside en un proyecto que está asociado con una segunda programación, tiene al menos 2 programaciones que podrían aplicarse a los cálculos de cronología.

>[!IMPORTANT]
>
>[!DNL Workfront] utiliza la programación de un usuario solo cuando la variable [!UICONTROL Calcular la disponibilidad de los recursos utilizando] está configurada en [!UICONTROL Programación del usuario] en el [!UICONTROL Gestión de recursos] área de [!UICONTROL Configuración]. Para obtener información sobre cómo se usa la variable [!UICONTROL Calcular la disponibilidad de los recursos utilizando] afecta a la programación que se usa para la administración de recursos, consulte [Configurar las preferencias de Administración de recursos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

El orden en que el sistema utiliza las programaciones cuando existe más de una es:

* Cuando se asigna un usuario a una tarea, [!DNL Workfront] utiliza la programación del usuario para calcular la cronología de la tarea. Esto también incluye la hora personal del usuario. Se ignora la programación del proyecto.

   Para obtener más información sobre el tiempo personal, consulte [Configure el tiempo de espera personal en [!DNL Adobe Workfront]](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* Cuando se asignan varios usuarios a una tarea y los usuarios tienen diferentes programaciones durante el lapso de tiempo de la tarea, [!DNL Workfront] utiliza cualquiera de las siguientes programaciones, tal como se definen en la variable [!UICONTROL Preferencias de proyecto] área de [!UICONTROL Configuración]:

   * La programación del usuario designado como usuario asignado principal
   * La programación asociada al proyecto.

      Para obtener más información sobre las preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Si el usuario asignado a la tarea no tiene programación o la tarea está asignada únicamente a una función de trabajo, un equipo o está sin asignar, [!DNL Workfront] utiliza la programación del proyecto para los cálculos de línea de tiempo.
* Si el usuario asignado a la tarea no tiene programación o la tarea está asignada únicamente a una función de trabajo, a un equipo o no está asignada y el proyecto no tiene programación, entonces [!DNL Workfront] utiliza la programación del sistema designado como Programa predeterminado para los cálculos de cronología.

   ![](assets/default-schedule.png)

## Colaboración en [!DNL Workfront] en zonas horarias

Para obtener información sobre el uso de programaciones para ayudar a los usuarios a colaborar en [!DNL Workfront] en zonas horarias, consulte [Trabajo en zonas horarias](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
