---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: usuario, horario
navigation-topic: configure-timesheets-and-schedules
title: Información general sobre los horarios
description: Puede definir la semana laboral mediante el uso de horarios. Puede asociar un horario a un usuario o proyecto. Esto permite a [!DNL Adobe Workfront]  calcular las líneas de tiempo y la disponibilidad del usuario. Para obtener instrucciones, consulte Crear un horario.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: 325334010d5f1206931cc9ace67f9511d614ffca
workflow-type: tm+mt
source-wordcount: '761'
ht-degree: 95%

---

# Información general sobre los horarios

<!-- Audited: 1/2024 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Puede definir la semana laboral mediante el uso de horarios y asociar un horario a un usuario o proyecto. Esto permite a [!DNL Adobe Workfront] calcular las líneas de tiempo y la disponibilidad del usuario. Para obtener instrucciones, consulte [Crear un horario](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Tenga en cuenta lo siguiente al trabajar con horarios en Workfront:

* La persona con la función de administrador de [!DNL Workfront] identifica las horas operativas de la organización en un horario.

  Del mismo modo, una persona con la función de administrador de grupo puede identificar las horas operativas de un horario administrado por un grupo que administra. Para obtener más información sobre los administradores de grupos, consulte [Administradores de grupos](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

  Por ejemplo, un horario se puede definir como: de lunes a viernes, de 8 h a 17 h, con una pausa de una hora para el almuerzo.

* [!DNL Workfront] usa el horario para determinar cuándo comienza y finaliza el día laborable.

  Esto no impide que un usuario trabaje o complete su trabajo en [!DNL Workfront] fuera del horario laboral normal. Por lo general, no es necesario crear un nuevo horario o una excepción de horario para centrarse en el trabajo planificado por la noche.

  Del mismo modo, su organización puede tener horas de llegada flexibles para su día laborable. Puede tener un conjunto de empleados que llegue a las 8 h y otro que llegue a las 9 h. No es necesario crear horarios únicos para cada grupo, si los grupos tienen horarios similares o idénticos. Pero si los grupos tienen horarios drásticamente diferentes, sus usuarios deben asociarse a horarios únicos. El empleado entiende que, si una asignación debe completarse a las 17 h, significa que el trabajo debe realizarse antes del final del día laborable, independientemente de la hora en que entre al trabajo.

* Le recomendamos que cree horarios independientes para cada zona horaria asociada a la organización.

  Puede asignar una zona horaria específica para cada horario a fin de asegurarse de que el trabajo se programe correctamente para los usuarios que trabajan en diferentes zonas horarias.

* Cuando los usuarios o proyectos no están asociados a un horario, se usa el horario predeterminado de [!DNL Workfront] en los cálculos de línea de tiempo. 

  El horario predeterminado viene con el sistema de [!DNL Workfront] y no se puede eliminar a menos que se reemplace por uno nuevo que se cree.

* Además de calcular líneas de tiempo, [!DNL Workfront] usa horarios para calcular la disponibilidad del usuario.

  >[!IMPORTANT]
  >
  >[!DNL Workfront] utiliza el horario del usuario o del proyecto para determinar la disponibilidad de recursos en el Planificador de recursos. El horario que se use depende de lo que haya seleccionado la persona con la función de administrador de [!DNL Workfront] para la opción [!UICONTROL Calculate Resource Availability Using] Para obtener información acerca de la configuración de administración de recursos, vea [Configurar las preferencias de administración de recursos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Jerarquía de horarios

Si una tarea se asigna a un usuario asociado a un horario y reside en un proyecto asociado a un segundo horario, tiene al menos dos horarios que podrían aplicarse a los cálculos de línea de tiempo.

>[!IMPORTANT]
>
>[!DNL Workfront] usa el horario del usuario solo cuando la opción [!UICONTROL Calculate Resource Availability Using] está establecida en [!UICONTROL The User&#39;s Schedule] en el área [!UICONTROL Resource Management] de [!UICONTROL Setup]. Para obtener información sobre cómo la opción [!UICONTROL Calculate Resource Availability Using] afecta al horario utilizado para la administración de recursos, consulte [Configurar las preferencias de administración de recursos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

El orden en el que el sistema utiliza los horarios cuando existe más de uno es el siguiente:


* Cuando se asigna un usuario a una tarea, [!DNL Workfront] usa cualquiera de las siguientes programaciones, tal como se definen en el área de [!UICONTROL Preferencias del proyecto] de [!UICONTROL Configuración]:

   * La programación del usuario asignado a la tarea
   * Horario asociado al proyecto.

     Para obtener más información sobre los días libres personales, consulte [Configurar los días libres personales](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* Cuando se asignan varios usuarios a una tarea y los usuarios tienen horarios diferentes durante el lapso de tiempo de la tarea, [!DNL Workfront] usa uno de los siguientes horarios, tal como se define en el área [!UICONTROL Project Preferences] de [!UICONTROL Setup]:

   * Horario del usuario designado como usuario asignado principal
   * Horario asociado al proyecto.

     Para obtener más información acerca de las preferencias de proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Si el usuario asignado a la tarea no tiene horario, o si la tarea se ha asignado solo a una función o un equipo, o no se ha asignado, [!DNL Workfront] usa el horario del proyecto para los cálculos de línea de tiempo.
* Si el usuario asignado a la tarea no tiene horario, o si la tarea se ha asignado solo a un equipo o no se ha asignado, y el proyecto no tiene horario, [!DNL Workfront] usa el horario del sistema designado como horario predeterminado para los cálculos de línea de tiempo.

  ![Programación predeterminada](assets/default-schedule.png)

## Colaboración en [!DNL Workfront] entre zonas horarias

Para obtener información acerca del uso de horarios para ayudar a los usuarios a colaborar en [!DNL Workfront] en diferentes zonas horarias, consulte [Trabajo en diferentes zonas horarias](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
