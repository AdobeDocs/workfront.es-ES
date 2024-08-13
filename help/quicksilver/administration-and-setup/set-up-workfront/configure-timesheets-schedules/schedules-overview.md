---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: usuario, programación
navigation-topic: configure-timesheets-and-schedules
title: Resumen de horarios
description: Puede definir la semana laboral utilizando los horarios. Puede asociar una programación a un usuario o proyecto. Esto permite a [!DNL Adobe Workfront] calcular las escalas de tiempo y la disponibilidad del usuario. Para obtener instrucciones, consulte Creación de una programación.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# Información general sobre horarios

<!-- Audited: 1/2024 -->

Puede definir la semana laboral mediante los horarios y asociar un horario a un usuario o proyecto. Esto permite que [!DNL Adobe Workfront] calcule las escalas de tiempo y la disponibilidad del usuario. Para obtener instrucciones, vea [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Tenga en cuenta lo siguiente al trabajar con programaciones en Workfront:

* El administrador [!DNL Workfront] identifica las horas de operación de la organización en una programación.

  Del mismo modo, un administrador de grupo puede identificar las horas de funcionamiento de una programación administrada por un grupo que administra. Para obtener más información sobre los administradores de grupos, consulte [Administradores de grupos](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

  Por ejemplo, una programación se puede definir como: de lunes a viernes, de 8 a. m. a 5 p. m., con una pausa horaria para el almuerzo.

* [!DNL Workfront] usa la programación para determinar cuándo comienza y finaliza el día laborable.

  Esto no impide que un usuario trabaje o complete su trabajo en [!DNL Workfront] fuera del horario laboral normal. Por lo general, no es necesario crear una nueva programación o una excepción de programación para centrarse en el trabajo planificado por la noche.

  Del mismo modo, su organización puede tener horarios de llegada flexibles para su día de trabajo. Puede tener un conjunto de empleados que llega a las 8 a. m. y otro conjunto que llega a las 9 a. m. No es necesario crear programaciones únicas para cada grupo, si los grupos tienen programaciones similares o idénticas. Pero si los grupos tienen programaciones drásticamente diferentes, sus usuarios deben asociarse con programaciones únicas. Un empleado entiende si una asignación debe completarse a las 5 p.m., significa que el trabajo debe realizarse antes del final del día hábil, independientemente de la hora en que ingresen al trabajo.

* Le recomendamos que cree programaciones independientes para cada zona horaria asociada a la organización.

  Puede asignar una zona horaria específica para cada programación a fin de asegurarse de que el trabajo esté programado correctamente para los usuarios que trabajan en diferentes zonas horarias.

* El horario predeterminado [!DNL Workfront] se usa en los cálculos de escala de tiempo cuando los usuarios o proyectos no están asociados a un horario.

  El Horario predeterminado viene con su sistema [!DNL Workfront] y no se puede eliminar a menos que se reemplace por un nuevo horario que usted cree.

* Además de calcular escalas de tiempo, [!DNL Workfront] usa programaciones para calcular la disponibilidad del usuario.

  >[!IMPORTANT]
  >
  >[!DNL Workfront] utiliza el usuario o la programación del proyecto para determinar la disponibilidad de recursos en el Planificador de recursos. La programación que se use depende de lo que haya seleccionado el administrador de [!DNL Workfront] para la opción [!UICONTROL Calcular disponibilidad de recursos mediante]. Para obtener información acerca de la configuración de Administración de recursos, vea [Configurar las preferencias de Administración de recursos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Jerarquía de horarios

Si una tarea se asigna a un usuario asociado a una programación y reside en un proyecto asociado a una segunda programación, tiene al menos dos programaciones que podrían aplicarse a los cálculos de escala de tiempo.

>[!IMPORTANT]
>
>[!DNL Workfront] usa la programación de un usuario solo cuando la opción [!UICONTROL Calcular disponibilidad de recursos usando] está establecida en [!UICONTROL La programación del usuario] en el área de [!UICONTROL Administración de recursos] de [!UICONTROL Configuración]. Para obtener información sobre cómo la configuración [!UICONTROL Calcular disponibilidad de recursos mediante] afecta a la programación que se usa para la administración de recursos, consulte [Configurar las preferencias de administración de recursos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

El orden en el que el sistema utiliza las programaciones cuando existe más de una es el siguiente:

* Cuando se asigna un usuario a una tarea, [!DNL Workfront] utiliza la programación del usuario para calcular la escala de tiempo de la tarea. Esto también incluye la hora personal del usuario. Se ignora la programación del proyecto.

  Para obtener más información sobre el tiempo personal, consulte [Configurar el tiempo libre personal](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* Cuando se asignan varios usuarios a una tarea y los usuarios tienen programaciones diferentes durante el lapso de tiempo de la tarea, [!DNL Workfront] usa una de las siguientes programaciones, tal como se define en el área de [!UICONTROL Preferencias del proyecto] de [!UICONTROL Configuración]:

   * El horario del usuario designado como la persona asignada principal
   * La programación asociada con el proyecto.

     Para obtener más información acerca de las preferencias del proyecto, vea [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Si el usuario asignado a la tarea no tiene ninguna programación, o si la tarea está asignada solamente a un rol de trabajo, a un equipo o no está asignada, [!DNL Workfront] usa la programación del proyecto para los cálculos de escala de tiempo.
* Si el usuario asignado a la tarea no tiene ninguna programación, o si la tarea está asignada solamente a un rol de trabajo, a un equipo o no está asignada, y el proyecto no tiene ninguna programación, [!DNL Workfront] usa la programación en el sistema designado como la Programación predeterminada para los cálculos de escala de tiempo.

  ![](assets/default-schedule.png)

## Collaboration en [!DNL Workfront] entre zonas horarias

Para obtener información acerca del uso de programaciones para ayudar a los usuarios a colaborar en [!DNL Workfront] en diferentes zonas horarias, vea [Trabajar en diferentes zonas horarias](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
