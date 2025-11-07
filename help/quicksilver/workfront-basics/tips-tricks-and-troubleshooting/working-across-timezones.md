---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Trabajar en diferentes zonas horarias
description: Puede resultar útil entender cómo  [!DNL Adobe Workfront]  usa las zonas horarias para calcular los campos de tiempo para objetos y la hora en otras áreas, como los correos electrónicos.
feature: Get Started with Workfront
author: Becky
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '1249'
ht-degree: 71%

---

# Trabajar en diferentes zonas horarias

<!-- Audited: 2/2024 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Puede resultar útil comprender cómo [!DNL Adobe Workfront] utiliza las zonas horarias para calcular lo siguiente:

* Campos de tiempo para objetos
* La hora en otras áreas de [!DNL Workfront], como los correos electrónicos automatizados de Workfront

>[!WARNING]
>
>Si no encuentra su zona horaria exacta en la lista proporcionada, busque la zona horaria más cercana a la suya y actualícela para su instancia.
>
>Además, tenga en cuenta que una zona horaria similar podría no coincidir completamente con la suya.
>
>Por ejemplo, puede que algunos países o territorios tengan horario de verano y el suyo no. Es posible que deba ajustar los husos horarios del sistema según estos cambios si fuera necesario.


## Husos horarios en [!DNL Workfront]

Las horas que se ven en [!DNL Workfront] se basan en configuraciones de zona horaria para la instancia de [!DNL Workfront] de la organización y para el perfil de usuario. Si estas dos zonas horarias fueran diferentes, es posible que se vean discrepancias horarias en diferentes áreas y características que se usan en [!DNL Workfront].

>[!NOTE]
>
>En un formulario personalizado adjunto a un objeto, las instrucciones de fecha y hora de los campos personalizados calculados se calculan y guardan a partir de la hora universal coordinada (UTC), no mediante las configuraciones de zona horaria establecidas para la instancia de su organización y el perfil de usuario. Los cálculos de un formulario personalizado se generan y muestran en función de las zonas horarias individuales de cada usuario.

* [Instancia de  [!DNL Workfront]  de su organización](#your-organization-s-workfront-instance)
* [El perfil de usuario](#your-user-profile)

### Instancia de [!DNL Workfront] de su organización {#your-organization-s-workfront-instance}

La zona horaria de la instancia de [!DNL Workfront] de su organización suele estar establecida según la ubicación de la oficina principal. Esto determina lo siguiente:

* La hora mostrada en los correos electrónicos generados por [!DNL Workfront]
* La zona horaria de los usuarios añadidos recientemente (antes de que el administrador de [!DNL Workfront] configure una zona horaria diferente para ellos según su lugar de trabajo)

  Para obtener más información sobre estos dos ejemplos, consulte [Configuración de la información básica para el sistema](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* El inicio o final de una tarifa de facturación anulada para un proyecto. Para obtener más información, consulte [Anulación de tarifas de facturación de funciones en el nivel de proyecto](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### El perfil de usuario {#your-user-profile}

El campo Zona horaria del perfil del usuario controla la hora que se muestra en los mensajes de correo electrónico salientes.

La zona horaria también afecta a lo que se muestra en un informe de calendario de PTO.

Para obtener información sobre la configuración de la zona horaria en el perfil de usuario, consulte [Configuración de mis opciones](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

Para obtener información sobre cómo un administrador de [!DNL Workfront] (o alguien con acceso de [!UICONTROL Edición] de usuarios) puede configurar la zona horaria de un perfil de usuario, consulte [Editar el perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

### Zona horaria del explorador

La zona horaria del navegador debe configurarse para la ubicación en la que trabaje. Esto determina lo siguiente:

<!--
* The time shown in your outgoing [!DNL Workfront] email messages
[NOTE FROM LISA: Saeid that dates/times shown in emails are more complicated than how it is described in the article so we decided to comment out this line.]
-->
* Horas de un objeto en el que trabaje, como las horas de inicio y finalización.

  Si los usuarios de varias zonas horarias están asignados a un objeto, [!DNL Workfront] convierte las horas del objeto para todos los implicados, utilizando la zona horaria configurada en el explorador de cada usuario.

  **EJEMPLO**
En la zona horaria estándar del Este (EST) en la que trabaja, establece una tarea para que comience a las 4:00 p.m. y la asigna a los usuarios que trabajan en la zona horaria estándar del Pacífico (PST). Para esos usuarios, la hora de inicio se muestra a las 1:00 p.m. Si se mostrara como las 4:00 p.m., empezarían a trabajar en él con tres horas de retraso.

  Si el creador del objeto no conoce la diferencia entre las zonas horarias de los usuarios asignados y no realiza los ajustes necesarios al establecer las horas del objeto, o si los usuarios asignados no conocen esa diferencia, puede ser difícil ajustar el tiempo correctamente mientras todos colaboran en el objeto.

  **EJEMPLO**

  Configura una tarea de un día para que comience a las 9:00 AM EST, olvidando que algunos usuarios de la tarea trabajan en la zona PST. Para ellos, la hora de inicio es 6:00 AM. Debido a que no comenzarán a trabajar en él hasta las 9:00 de su hora (mediodía de su hora), la tarea comienza y finaliza con tres horas de retraso.

La configuración de la zona horaria difiere entre los exploradores. Para obtener más información, consulte la documentación de cada explorador o la información de ayuda.

## Cómo se puede facilitar el trabajo de los usuarios entre zonas horarias

Ayude a los usuarios a trabajar con mayor facilidad entre varias zonas horarias de varias formas:

* [Uso de horarios](#use-schedules)
* [Uso de campos de tiempo calculado en un formulario personalizado](#use-calculated-time-fields-in-a-custom-form)
* [Utilice campos de texto en lugar de campos de fecha en un formulario personalizado](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### Uso de horarios {#use-schedules}

Los administradores de [!DNL Workfront] crean horarios separados para cada zona horaria dentro de la organización a fin de asegurarse de que el trabajo esté programado adecuadamente para todos, independientemente de dónde se encuentren. Una vez que el administrador crea el horario, se puede asociar con determinados proyectos y usuarios:

* **[!UICONTROL Proyectos]**: el creador de un proyecto puede seleccionar una programación para un proyecto individual. Esto determinará la programación de las tareas del proyecto, en función de las horas de trabajo establecidas para las zonas horarias de los usuarios asignados.
* **[!UICONTROL Usuarios]**: un administrador de [!DNL Workfront] (o alguien con acceso para [!UICONTROL Editar] usuarios) puede seleccionar una programación para cada usuario en el perfil del usuario.

  Esta programación podría ser diferente de una programación de proyecto. Por ejemplo, cuando alguien crea una tarea en el proyecto y aún no le ha asignado a nadie, la tarea utiliza la programación del proyecto. Cuando se asigna un usuario a la tarea, esta utiliza la programación de ese usuario.

  Si se asignan varios usuarios a una tarea, el sistema utiliza una de las siguientes opciones, según la configuración de las preferencias de proyecto de todo el sistema o del grupo:

   * Zona horaria de la programación del propietario principal de la tarea
   * Zona horaria de la programación del proyecto.

  Si se asigna un usuario a una tarea, el sistema utiliza una de las siguientes opciones, según la configuración de las preferencias de proyecto de todo el sistema o del grupo:

   * Zona horaria de la programación de la persona asignada a la tarea
   * Zona horaria de la programación del proyecto.

  Esto puede hacer que las fechas de las tareas cambien.

>[!BEGINSHADEBOX]

**EJEMPLO:**
Se asigna a un usuario de EST una tarea de un día programada para iniciarse a las 9:00 AM PST, que es mediodía EST. Como al usuario de EST le quedan solo 2 horas laborables por día, la fecha de finalización de la tarea se extiende unas 6 horas hasta el siguiente día laborable.


>[!ENDSHADEBOX]

Para obtener información sobre el área de [!UICONTROL Preferencias del proyecto] de [!UICONTROL Configuración], consulte [Configurar las preferencias de proyecto de todo el sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para obtener instrucciones sobre cómo asignar una programación a un proyecto o a un usuario, consulte [Crear programación](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Para obtener información sobre cómo afecta la zona horaria configurada en su programación a la distribución de [!UICONTROL Horas planificadas] en el [!UICONTROL Distribuidor de cargas de trabajo], consulte [Administrar asignaciones de usuarios en el [!UICONTROL Distribuidor de cargas de trabajo]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).


### Uso de campos de tiempo calculado en un formulario personalizado {#use-calculated-time-fields-in-a-custom-form}

Puede utilizar una serie de campos personalizados calculados en un formulario personalizado para mostrar la hora actual de los usuarios de su organización, como una fila de relojes de aeropuerto que muestran la hora en varias ciudades. Puede crear un campo para cada una de las zonas horarias en las que trabajen los usuarios, cada una de las cuales calculará la hora de su zona horaria.

Para obtener más información, consulte [Añadir campos calculados a un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md), así como la sección [Campos personalizados calculados por fecha y hora](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) en el artículo [Información general sobre las expresiones de datos calculados](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### Utilice campos de texto en lugar de campos de fecha en un formulario personalizado {#use-text-fields-instead-of-date-fields-in-a-custom-form}

Si no desea que [!DNL Workfront] convierta las horas configuradas en un objeto para usuarios de diferentes zonas horarias, puede utilizar un campo de texto en un formulario personalizado que adjunte a un objeto, en lugar de un campo de fecha. De este modo, la hora muestra la hora a la que escribe para todos los integrantes del proyecto.

Si lo hace, le recomendamos que recuerde a los usuarios del formulario que calculen la diferencia entre su zona horaria y el suyo para que puedan determinar cuándo debe comenzar y finalizar el trabajo. Puede incluirlo en las instrucciones que escriba para el formulario personalizado o en la información del objeto de ese campo. Para obtener más información, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
