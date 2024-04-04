---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Trabajo entre zonas horarias
description: Puede resultar útil comprender cómo [!DNL Adobe Workfront] utiliza zonas horarias para calcular campos de hora para objetos y horas en otras áreas, como correos electrónicos.
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: 0483230c5d8b7d33f420c6c5f09c4a5aafe37f37
workflow-type: tm+mt
source-wordcount: '1152'
ht-degree: 0%

---

# Trabajo entre zonas horarias

<!-- Audited: 2/2024 -->

Puede resultar útil comprender cómo [!DNL Adobe Workfront] utiliza zonas horarias para calcular lo siguiente:

* Campos de tiempo para objetos
* Horas en otros [!DNL Workfront] áreas, como correos electrónicos automatizados de Workfront

>[!WARNING]
>
>Si no encuentra su zona horaria exacta en la lista que proporcionamos, busque la zona horaria más cercana a la suya y actualícela para su instancia.
>
>Además, tenga en cuenta que una zona horaria similar podría no coincidir perfectamente con la suya.
>
>Por ejemplo, algunos países o territorios pueden observar el horario de verano, pero es posible que su país no lo haga. Es posible que deba ajustar los husos horarios del sistema según estos cambios, si es necesario.


## Husos horarios en [!DNL Workfront]

Horas que ves en [!DNL Workfront] se basan en configuraciones de zona horaria para las [!DNL Workfront] y para su perfil de usuario. Si estas dos zonas horarias son diferentes, es posible que vea discrepancias horarias en diferentes áreas y características que usa en [!DNL Workfront].

>[!NOTE]
>
>En un formulario personalizado adjunto a un objeto, las instrucciones de fecha y hora de los campos personalizados calculados se calculan y guardan mediante la hora universal coordinada (UTC), no mediante las configuraciones de zona horaria establecidas para la instancia de su organización y el perfil de usuario. Los cálculos de un formulario personalizado se generan y se muestran en función de las zonas horarias individuales de cada usuario.

* [El de su organización [!DNL Workfront] instancia](#your-organization-s-workfront-instance)
* [Su perfil de usuario](#your-user-profile)

### El de su organización [!DNL Workfront] instancia {#your-organization-s-workfront-instance}

Zona horaria de la actividad de su organización [!DNL Workfront] La instancia de suele configurarse para la ubicación de la oficina principal. Esto determina lo siguiente:

* Tiempo mostrado en los correos electrónicos generados por [!DNL Workfront]
* La zona horaria de los usuarios recién añadidos (antes del [!DNL Workfront] configure un huso horario diferente para ellos (en función de dónde trabajen)

  Para obtener más información sobre estos dos ejemplos, consulte [Configurar la información básica del sistema](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Inicio o final de una tarifa de facturación anulada para un proyecto. Para obtener más información, consulte [Anular tarifas de facturación de rol en el nivel de proyecto](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### Su perfil de usuario {#your-user-profile}

La zona horaria del perfil de usuario debe configurarse para la ubicación donde trabaje. Esto determina lo siguiente:

<!--
* The time shown in your outgoing [!DNL Workfront] email messages
[NOTE FROM LISA: Saeid that dates/times shown in emails are more complicated than how it is described in the article so we decided to comment out this line.]
-->
* Horas de un objeto en el que trabaje, como las horas de inicio y finalización

  Si los usuarios de varias zonas horarias están asignados a un objeto, [!DNL Workfront] convierte las horas del objeto para todos los implicados, utilizando la zona horaria configurada en cada perfil de usuario.

  **Ejemplo:** En la zona horaria estándar del Este (EST) en la que trabaja, establece una tarea para que comience a las 4:00 p.m. y la asigna a los usuarios que trabajan en la zona horaria estándar del Pacífico (PST). Para estos usuarios, la hora de inicio se muestra como 1:00 p.m. Si se mostrara a las 4:00 p.m., empezarían a trabajar con tres horas de retraso.

  Si el creador del objeto no observa la diferencia entre las zonas horarias de los usuarios asignados y realiza los ajustes necesarios al establecer las horas del objeto, o si los usuarios asignados no notan esa diferencia, puede ser difícil ajustar la temporización correctamente mientras todos colaboran en el objeto.

  **Ejemplo:** Configura una tarea de un día para que comience a las 9:00 AM EST, olvidando que algunos usuarios de la tarea trabajan en la zona PST. Para ellos, la hora de inicio es a las 6:00 AM. Debido a que no empezarán a trabajar en él hasta las 9:00 su hora (mediodía su hora), la tarea comienza y finaliza con tres horas de retraso.

Para obtener información sobre la configuración de la zona horaria en el perfil de usuario, consulte [Configurar mis ajustes](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

Para obtener información acerca de cómo [!DNL Workfront] administrador (o alguien con [!UICONTROL Editar] acceso a los usuarios) puede configurar la zona horaria en un perfil de usuario, consulte [Edición del perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Cómo puede facilitar el trabajo de los usuarios entre zonas horarias

Puede ayudar a los usuarios a trabajar con mayor facilidad en varias zonas horarias de varias formas:

* [Usar horarios](#use-schedules)
* [Uso de campos de tiempo calculado en un formulario personalizado](#use-calculated-time-fields-in-a-custom-form)
* [Utilice campos de texto en lugar de campos de fecha en un formulario personalizado](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### Usar horarios {#use-schedules}

[!DNL Workfront] los administradores crean horarios diferentes para cada zona horaria dentro de la organización a fin de garantizar que el trabajo esté programado adecuadamente para todos, independientemente de dónde se encuentren. Una vez que el administrador crea las programaciones, se pueden asociar con determinados proyectos y usuarios:

* **[!UICONTROL Proyectos]**: el creador de un proyecto puede seleccionar una programación para un proyecto individual. Esto determina la programación de las tareas del proyecto, en función de las horas de trabajo establecidas para las zonas horarias de los usuarios asignados.
* **[!UICONTROL Usuarios]**: A [!DNL Workfront] administrador (o alguien con [!UICONTROL Editar] acceso a los usuarios) puede seleccionar una programación para cada usuario en el perfil del usuario.

  Esta programación puede ser diferente de una programación de proyecto. Por ejemplo, cuando alguien crea una tarea en el proyecto y aún no le ha asignado a nadie, la tarea utiliza la programación del proyecto. Cuando se asigna un usuario a la tarea, esta utiliza la programación de ese usuario.

  Si se asignan varios usuarios a una tarea, el sistema utiliza una de las siguientes opciones, según se ha configurado en las preferencias de proyecto para todo el sistema:

   * Zona horaria de la programación del propietario principal de la tarea
   * Zona horaria de la programación del proyecto.

  Esto puede hacer que las fechas de las tareas cambien.

  **Ejemplo:** Se asigna a un usuario de EST una tarea de un día programada para comenzar a las 9:00 AM PST, que es el mediodía EST. Como al usuario de EST le quedan sólo 2 horas laborables por día, la fecha de finalización de la tarea se extiende unas 6 horas hasta el siguiente día laborable.

  Para obtener más información sobre [!UICONTROL Preferencias de proyecto] área de [!UICONTROL Configurar], consulte [Configurar las preferencias de proyecto de todo el sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  Para obtener instrucciones sobre cómo asignar una programación a un proyecto o a un usuario, consulte [Creación de una programación](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

  Para obtener información sobre cómo la zona horaria configurada en la programación afecta a la distribución de [!UICONTROL Horas planificadas] en el [!UICONTROL Distribuidor de cargas de trabajo], consulte [Administrar asignaciones de usuarios en [!UICONTROL Distribuidor de cargas de trabajo]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).


### Uso de campos de tiempo calculado en un formulario personalizado {#use-calculated-time-fields-in-a-custom-form}

Puede utilizar una serie de campos personalizados calculados en un formulario personalizado para mostrar la hora actual de los usuarios de su organización, como una fila de relojes de aeropuerto que muestran la hora en varias ciudades. Puede crear un campo para cada una de las zonas horarias en las que trabajen los usuarios, cada una de las cuales calculará la hora de su zona horaria.

Para obtener más información, consulte [Añadir datos calculados a un formulario personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md), así como la sección [Campos personalizados calculados por fecha y hora](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) en el artículo [Resumen de las expresiones de datos calculados](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### Utilice campos de texto en lugar de campos de fecha en un formulario personalizado {#use-text-fields-instead-of-date-fields-in-a-custom-form}

Si no quieres... [!DNL Workfront] para convertir las horas configuradas en un objeto para los usuarios de diferentes zonas horarias, puede utilizar un campo de texto en un formulario personalizado que adjunte a un objeto, en lugar de un campo de fecha. De este modo, la hora muestra la hora a la que escribe para todos los integrantes del proyecto.

Si lo hace, le recomendamos que recuerde a los usuarios del formulario que calculen la diferencia entre su huso horario y el suyo para que puedan determinar cuándo debe comenzar y finalizar el trabajo. Puede incluirlo en las instrucciones que escriba para el formulario personalizado o en la información del objeto de ese campo. Para obtener más información, consulte [Agregar un campo personalizado a un formulario personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
