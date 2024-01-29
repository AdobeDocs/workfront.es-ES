---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: usuario, programación
navigation-topic: configure-timesheets-and-schedules
title: Información general sobre horarios
description: Puede definir la semana laboral utilizando los horarios. Puede asociar una programación a un usuario o proyecto. Esto permite [!DNL Adobe Workfront] para calcular las escalas de tiempo y la disponibilidad del usuario. Para obtener instrucciones, consulte Creación de una programación.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: 32da139d7385e05436a669bdc6f36b71ad83c8d2
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# Información general sobre horarios

<!-- Audited: 1/2024 -->

Puede definir la semana laboral mediante los horarios y asociar un horario a un usuario o proyecto. Esto permite [!DNL Adobe Workfront] para calcular las escalas de tiempo y la disponibilidad del usuario. Para obtener instrucciones, consulte [Creación de una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Tenga en cuenta lo siguiente al trabajar con programaciones en Workfront:

* El [!DNL Workfront] El administrador identifica las horas de funcionamiento de la organización en una programación.

  Del mismo modo, un administrador de grupo puede identificar las horas de funcionamiento de una programación administrada por un grupo que administra. Para obtener más información sobre los administradores de grupo, consulte [Administradores de grupo](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

  Por ejemplo, una programación se puede definir como: de lunes a viernes, de 8 a. m. a 5 p. m., con una pausa horaria para el almuerzo.

* [!DNL Workfront] utiliza la programación para determinar cuándo comienza y finaliza el día laborable.

  Esto no impide que un usuario trabaje o complete su trabajo en [!DNL Workfront] fuera del horario laboral normal. Por lo general, no es necesario crear una nueva programación o una excepción de programación para centrarse en el trabajo planificado por la noche.

  Del mismo modo, su organización puede tener horarios de llegada flexibles para su día de trabajo. Puede tener un conjunto de empleados que llega a las 8 a. m. y otro conjunto que llega a las 9 a. m. No es necesario crear programaciones únicas para cada grupo, si los grupos tienen programaciones similares o idénticas. Pero si los grupos tienen programaciones drásticamente diferentes, sus usuarios deben asociarse con programaciones únicas. Un empleado entiende si una asignación debe completarse a las 5 p.m., significa que el trabajo debe realizarse antes del final del día hábil, independientemente de la hora en que ingresen al trabajo.

* Le recomendamos que cree programaciones independientes para cada zona horaria asociada a la organización.

  Puede asignar una zona horaria específica para cada programación a fin de asegurarse de que el trabajo esté programado correctamente para los usuarios que trabajan en diferentes zonas horarias.

* El [!DNL Workfront] Horario predeterminado se utiliza en los cálculos de escala de tiempo cuando los usuarios o proyectos no están asociados a una programación.

  El Horario predeterminado viene con su [!DNL Workfront] El sistema y no se pueden eliminar a menos que se reemplacen por una nueva programación que cree.

* Además de calcular los plazos, [!DNL Workfront] utiliza programaciones para calcular la disponibilidad del usuario.

  >[!IMPORTANT]
  >
  >[!DNL Workfront] utiliza el usuario o la programación del proyecto para determinar la disponibilidad de los recursos en el Planificador de recursos. La programación que se use depende de lo que [!DNL Workfront] administrador seleccionado para [!UICONTROL Calcular disponibilidad de recursos mediante] configuración. Para obtener información acerca de la configuración de Administración de recursos, consulte [Configurar preferencias de administración de recursos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Jerarquía de horarios

Si una tarea se asigna a un usuario asociado a una programación y reside en un proyecto asociado a una segunda programación, tiene al menos dos programaciones que podrían aplicarse a los cálculos de escala de tiempo.

>[!IMPORTANT]
>
>[!DNL Workfront] utiliza la programación de un usuario solo cuando la variable [!UICONTROL Calcular disponibilidad de recursos mediante] se establece en [!UICONTROL El horario del usuario] en el [!UICONTROL Administración de recursos] área de [!UICONTROL Configurar]. Para obtener información acerca de cómo [!UICONTROL Calcular disponibilidad de recursos mediante] afecta a la programación que se utiliza para la gestión de recursos, consulte [Configurar preferencias de administración de recursos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

El orden en el que el sistema utiliza las programaciones cuando existe más de una es el siguiente:

* Cuando se asigna a un usuario una tarea, [!DNL Workfront] utiliza la programación del usuario para calcular la escala de tiempo de la tarea. Esto también incluye la hora personal del usuario. Se ignora la programación del proyecto.

  Para obtener más información sobre el tiempo personal, consulte [Configuración del tiempo libre personal](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* Cuando se asignan varios usuarios a una tarea y los usuarios tienen programaciones diferentes durante el lapso de tiempo de la tarea, [!DNL Workfront] utiliza una de las siguientes programaciones, tal como se define en la [!UICONTROL Preferencias de proyecto] área de [!UICONTROL Configurar]:

   * El horario del usuario designado como la persona asignada principal
   * La programación asociada con el proyecto.

     Para obtener más información sobre las preferencias de proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Si el usuario asignado a la tarea no tiene ninguna programación o si la tarea está asignada solo a un rol, a un equipo o no está asignada, [!DNL Workfront] utiliza la programación del proyecto para los cálculos de escala de tiempo.
* Si el usuario asignado a la tarea no tiene ninguna programación, o si la tarea está asignada solo a un rol, un equipo o no está asignada, y el proyecto no tiene ninguna programación, [!DNL Workfront] utiliza la programación del sistema designada como predeterminada para los cálculos de escala de tiempo.

  ![](assets/default-schedule.png)

## Colaboración en [!DNL Workfront] entre zonas horarias

Para obtener información sobre cómo usar las programaciones para ayudar a los usuarios a colaborar en [!DNL Workfront] para zonas horarias, consulte [Trabajo entre zonas horarias](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
