---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Trabajo en zonas horarias
description: 'Puede ser útil comprender cómo [!DNL Adobe Workfront] utiliza husos horarios para calcular lo siguiente: EDITAR ME.'
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: ecb6928c946203b03a93cf5687fd53abf8e6a8f3
workflow-type: tm+mt
source-wordcount: '1086'
ht-degree: 0%

---

# Trabajo en zonas horarias

Puede ser útil comprender cómo [!DNL Adobe Workfront] utiliza zonas horarias para calcular lo siguiente:

* Campos de tiempo para objetos
* Tiempos en otros [!DNL Workfront] áreas, como correos electrónicos automatizados de Workfront

## Husos horarios en [!DNL Workfront]

Veces que se ven en [!DNL Workfront] se basan en las configuraciones de zona horaria de la organización [!DNL Workfront] y para su perfil de usuario. Si estos dos husos horarios son diferentes, es posible que vea discrepancias horarias en diferentes áreas y características que use en [!DNL Workfront].

>[!NOTE]
>
><div class="preview">En un formulario personalizado adjunto a un objeto, las instrucciones de fecha y hora de los campos personalizados calculados se calculan y se guardan en la Hora universal coordinada (UTC), no en las configuraciones de zona horaria establecidas para la instancia de su organización y su perfil de usuario. Los cálculos en un formulario personalizado se generan y muestran en función de los husos horarios individuales de cada usuario.</div>




* [La [!DNL Workfront] instancia](#your-organization-s-workfront-instance)
* [Su perfil de usuario](#your-user-profile)

### La [!DNL Workfront] instancia {#your-organization-s-workfront-instance}

Zona horaria de la organización [!DNL Workfront] generalmente se configura para la ubicación de la oficina principal. Esto determina lo siguiente:

* El tiempo que se muestra en los correos electrónicos generados por [!DNL Workfront]
* El huso horario para los usuarios recién agregados (antes del [!DNL Workfront] el administrador configura una zona horaria diferente en función de su lugar de trabajo)

   Para obtener más información sobre estos dos ejemplos, consulte [Configurar información básica para el sistema](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Inicio o final de una tasa de facturación sobrescrita para un proyecto. Para obtener más información, consulte [Anular tasas de facturación de rol de trabajo en el nivel de proyecto](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### Su perfil de usuario {#your-user-profile}

La zona horaria del perfil de usuario debe configurarse para la ubicación en la que trabaje. Esto determina lo siguiente:

* El tiempo que se muestra en la salida [!DNL Workfront] mensajes de correo electrónico
* Tiempos para un objeto en el que trabaje, como las horas de inicio y finalización

   Si se asignan a un objeto usuarios de varias zonas horarias, [!DNL Workfront] convierte las horas del objeto para todos los implicados, utilizando la zona horaria configurada en cada perfil de usuario.

   **Ejemplo:** En la zona horaria estándar oriental (EST) donde trabaja, configure una tarea para que comience a las 4 de la tarde y asígnela a los usuarios que trabajen en la zona horaria estándar del Pacífico (PST). Para esos usuarios, la hora de inicio es la 1:00 PM. Si fuera a mostrarlo a las 4:00 pm, empezarían a trabajar en ello tres horas después.

   Si el creador del objeto no nota la diferencia entre las zonas horarias de los asignadores y realiza los ajustes necesarios al establecer las horas de los objetos, o si los asignadores no tienen en cuenta esa diferencia, puede ser difícil obtener la sincronización correcta mientras todos colaboran con el objeto.

   **Ejemplo:** Puede configurar una tarea de un día para que comience a las 9:00 AM EST, olvidando que algunos usuarios de la tarea trabajan en la zona PST. Para ellos, la hora de inicio es 6:00 AM. Como no empezarán a trabajar en ello hasta las 9:00 de su hora (mediodía de su hora), la tarea comienza y finaliza con tres horas de retraso.

Para obtener información sobre la configuración de la zona horaria en el perfil de usuario, consulte [Configurar mis ajustes](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

Para obtener información sobre cómo [!DNL Workfront] administrador (o alguien con [!UICONTROL Editar] acceso a los usuarios) puede configurar la zona horaria en un perfil de usuario; consulte [Edición del perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Cómo facilitar el trabajo de los usuarios entre zonas horarias

Puede ayudar a los usuarios a trabajar más fácilmente en varios husos horarios de varias maneras:

* [Usar programaciones](#use-schedules)
* [Usar campos de hora calculados en un formulario personalizado](#use-calculated-time-fields-in-a-custom-form)
* [Utilizar campos de texto en lugar de campos de fecha en un formulario personalizado](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### Usar programaciones {#use-schedules}

[!DNL Workfront] los administradores crean programaciones independientes para cada zona horaria dentro de su organización a fin de garantizar que el trabajo esté programado de manera adecuada para todos, independientemente del lugar donde esté. Una vez que el administrador crea las programaciones, se pueden asociar a ciertos proyectos y usuarios:

* **[!UICONTROL Proyectos]**: Un creador de proyectos puede seleccionar una programación para un proyecto individual. Esto determina la programación de las tareas del proyecto, en función de las horas de trabajo establecidas para las zonas horarias de los usuarios asignados.
* **[!UICONTROL Usuarios]**: A [!DNL Workfront] administrador (o alguien con [!UICONTROL Editar] acceso a los usuarios) puede seleccionar una programación para cada usuario en el perfil del usuario.

   Esta programación puede diferir de una programación de proyecto. Por ejemplo, cuando alguien crea una tarea en el proyecto y aún no le ha asignado nadie, la tarea utiliza la programación del proyecto. Cuando se asigna un usuario a la tarea, la tarea utiliza la programación de ese usuario.

   Si se asignan varios usuarios a una tarea, el sistema utiliza una de las siguientes opciones, tal como se configuran en las preferencias de proyecto de todo el sistema:

   * Zona horaria de la programación del propietario principal de la tarea
   * Zona horaria de la programación del proyecto.

   Esto puede hacer que cambien las fechas de las tareas.

   **Ejemplo:** Un usuario EST se asigna a una tarea de un día programada para empezar a las 9:00 AM PST, que es el mediodía EST. Dado que el usuario EST solo tiene 2 horas laborables para el día, la fecha de finalización de la tarea se extiende unas 6 horas hasta el siguiente día laborable.

   Para obtener información sobre la variable [!UICONTROL Preferencias de proyecto] área de [!UICONTROL Configuración], consulte [Configurar las preferencias de proyecto de todo el sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   Para obtener instrucciones sobre la asignación de una programación a un proyecto o a un usuario, consulte [Crear una programación](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   Para obtener información sobre cómo la zona horaria configurada en la programación afecta a la distribución de [!UICONTROL Horas planificadas] en el [!UICONTROL Programación] y [!DNL Workload Balancer], consulte lo siguiente:

   * [Administrar asignaciones de usuario en la variable [!UICONTROL Programación] áreas](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md)
   * [Administrar asignaciones de usuario en la variable [!DNL Workload Balancer]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)



### Usar campos de hora calculados en un formulario personalizado {#use-calculated-time-fields-in-a-custom-form}

Puede utilizar una serie de campos personalizados calculados en un formulario personalizado para mostrar la hora actual para los usuarios de su organización, como una fila de relojes de aeropuerto que muestre la hora en varias ciudades. Puede crear un campo para cada una de las zonas horarias en las que trabajan los usuarios, calculando cada una la hora de su zona horaria.

Para obtener más información, consulte [Agregar datos calculados a un formulario personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md), así como la sección [Campos personalizados calculados por fecha y hora](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) en el artículo [Expresiones de datos calculadas](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### Utilizar campos de texto en lugar de campos de fecha en un formulario personalizado {#use-text-fields-instead-of-date-fields-in-a-custom-form}

Si no quieres [!DNL Workfront] para convertir las horas configuradas para en un objeto para usuarios de diferentes zonas horarias, puede utilizar un campo de texto en un formulario personalizado que adjunte a un objeto en lugar de un campo de fecha. De este modo, la hora muestra la hora que escriba para todos los integrantes del proyecto.

Si lo hace, le recomendamos que recuerde a los usuarios del formulario que calculen la diferencia entre su zona horaria y la suya para que puedan determinar cuándo debe comenzar y finalizar el trabajo. Puede incluirlo en las instrucciones que escriba para el formulario personalizado o en una información del objeto para ese campo. Para obtener más información, consulte [Añadir un campo personalizado a un formulario personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
