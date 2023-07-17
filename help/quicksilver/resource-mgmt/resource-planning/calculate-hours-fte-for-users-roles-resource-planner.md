---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Información general sobre el cálculo de horas y FTE para usuarios y roles en el Planificador de recursos
description: Información general sobre el cálculo de horas y FTE para usuarios y roles en el Planificador de recursos
author: Alina
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
source-git-commit: 4331917d133c52cf727f148b75a213853c1e5679
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 1%

---

# Información general sobre el cálculo de horas y FTE para usuarios y roles en el Planificador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina:KEEP THIS:***Linked to: Configuring My Settings, Editing User Accounts, Planning in the Resource Planner -- *** Some of this documentation is also duplicated in this article (Scheduling): https://support.workfront.com/hc/en-us/articles/360000557174)</p>
-->

Puede mostrar la asignación y disponibilidad de los recursos en el Planificador de recursos por horas, ETC o costo.\
Para obtener más información sobre el cálculo de costos en el Planificador de recursos, consulte [Calcular costos en el Planificador de recursos](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

&quot;FTE&quot; significa Equivalente a Tiempo Completo. Es una medida del tiempo que representa la cantidad de horas dedicadas al trabajo real durante un día o una semana para un usuario o rol.

Los siguientes conjuntos de información de recursos se calculan de forma diferente en el Planificador de recursos:

* Los valores de Horas disponibles o ETC se calculan según la forma en que el administrador del sistema configure las preferencias de Administración de recursos en el sistema.\
  Para obtener más información sobre cómo se calculan los valores de Horas disponibles y FTE, consulte [Calcular horas disponibles o ETC para usuarios y roles en el Planificador de recursos](#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner).\
  Para obtener más información sobre la definición de las preferencias de gestión de recursos para el sistema de Adobe Workfront, consulte [Configurar preferencias de administración de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* Todos los demás valores de FTE se calculan según la programación por defecto del sistema.\
  Para obtener más información sobre cómo se muestran los demás valores en el Planificador de recursos al utilizar FTE, vea la sección [Calcule el resto de los valores de horas y horas trabajadas para los usuarios y las funciones del puesto en el Planificador de recursos](#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner) en este artículo.

Es importante comprender qué es el valor de FTE para cada uno de los usuarios y sus funciones de trabajo para administrar con precisión los recursos a medida que los asigna al trabajo.

## Calcular horas disponibles o ETC para usuarios y roles en el Planificador de recursos {#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner}

* [Calcular las horas disponibles y el tiempo de espera completo de un usuario en el Planificador de recursos](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner)
* [Calcular las horas disponibles y el tiempo de espera completo de un rol en el Planificador de recursos](#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner)
* [Calcular las horas disponibles y el tiempo de espera completo de un usuario en el Planificador de recursos (ejemplo)](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example)

### Calcular las horas disponibles y el tiempo de espera completo de un usuario en el Planificador de recursos {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner}

El administrador de Workfront determina cómo se calcula el tiempo disponible para un usuario seleccionando la opción de usar una de las siguientes opciones en el área Administración de recursos de Configuración:

* El horario predeterminado del sistema y el FTE del usuario.
* La programación del usuario.

Para obtener más información, consulte [Configurar preferencias de administración de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><br></p>
<p> <img src="assets/nwe-resource-management-system-setting-user's-schedule-350x157.png" style="width: 350;height: 157;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p>
<p>(NOTE: The determines how to calculate resource availability at the system level.For more information about defining the Resource Management preferences for the system, see Configure Resource Management preferences.)</p>
<p>Based on how this setting is configured, the availability of the users in the Resource Planner (hours as well as FTE availability) is calculated by using the following methods: </p>
<ul>
<li><strong>The Default Schedule</strong>: The Default Schedule of the system and the user FTE are used to determine the Available Hours and FTE value for the user in the Resource Planner. The Schedule of the user is ignored. In this case:
<ul>
<li> The <strong>Available Hours</strong> in the<strong>Resource Planner</strong> are calculated using the following formula:<br><code>User Available Hours = Default Schedule Hours * User FTE value</code> <span style="color: #dc143c;">( NOTE: this is the correct value. If this shows as a division in other articles, that is wrong. It's a multiplication between these 2 values).</span><br>For example, if the Default Schedule has 40 hours a week available for work, and the user FTE is 0.5, the user is available to work for 20 hours a week in the Resource Planner.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a></li>
<li style="font-weight: normal;"> The <strong>Available FTE</strong> for the user in the<strong>Resource Planner</strong> is the same as the user FTE specified in the user settings. <br>For example, if the user FTE is 0.5 in the user settings, the available FTE of the user is 0.5 in the Resource Planner. For more information about the value of the user FTE as it displays in the user settings, see <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.<br></li>
</ul></li>
<li><strong>The User's Schedule</strong>: The Schedule of the user is used to determine the availability of the user in the Resource Planner. The value of the user FTE is ignored. In this case:
<ul>
<li> The <strong>Available Hours</strong> in the<strong>Resource Planner</strong> are the same as the Hours from the Schedule of the user.<br>For example, if the Schedule of the user has 40 hours a week available for work, the user is available to work for 40 hours a week in the Resource Planner. </li>
<li> The <strong>Available FTE</strong> in the<strong>Resource Planner</strong> is calculated by the following formula:<br><em><code>User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code><br></em>For example, if the Schedule of the user has 20 hours available to work, and the Default Schedule in Workfront has 40 hours available to work, the user's FTE is 0.5.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</li>
</ul></li>
</ul> <note type="note">
If the user is not associated with a schedule, the Available Hours for the user are calculated using the Default Schedule.
</note>
</div>
-->

### Calcular las horas disponibles y el tiempo de espera completo de un rol en el Planificador de recursos {#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner}

Primero debe calcular la disponibilidad del usuario y, a continuación, puede calcular la disponibilidad de cada uno de sus roles.

La disponibilidad de los roles en el Planificador de recursos tiene en cuenta la disponibilidad total del usuario y la variable **Porcentaje de disponibilidad de FTE** asociadas a cada función del usuario.\
![percent_of_fte_availability_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)

Para obtener más información sobre cómo asociar una **Porcentaje de disponibilidad de FTE** con una función de trabajo para un usuario, consulte [Edición del perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Por ejemplo, si el valor de Horas disponibles para un usuario es 40 y puede desempeñar una función principal durante el 75 % de ese tiempo y otra función durante el 25 % de ese tiempo, el Planificador de recursos muestra que la variable **Horas disponibles** para la Función principal durante una semana es de 30 horas y que la variable **Horas disponibles** El valor de Otro rol es 10 horas. En este caso, el valor de FTE para la función principal es 0,75 y el valor de FTE para la otra función es 0,25.

>[!NOTE]
>
>El tiempo total disponible para el usuario se calcula mediante uno de los dos métodos descritos en la sección [Calcular las horas disponibles y el tiempo de espera completo de un usuario en el Planificador de recursos](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner) de este artículo.

Al ver el Planificador de recursos en la vista de rol, la disponibilidad de un rol es un total de la disponibilidad de todos los usuarios que pueden cumplir ese rol.\
Para obtener más información sobre la disponibilidad de los recursos en el Planificador de recursos, consulte la [Resumen del Planificador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Calcular las horas disponibles y el tiempo de espera completo de un usuario en el Planificador de recursos (ejemplo) {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example}

La siguiente tabla ilustra cómo se calculan las horas disponibles y el tiempo de ejecución completo disponible para el usuario en el Planificador de recursos, en función del método que utilice el administrador del sistema para el cálculo de tiempo de ejecución completo en las Preferencias de administración de recursos.

Para este ejemplo, se utilizan los números siguientes:

* Un horario predeterminado de 40 horas
* Horario de 20 horas de un usuario
* Un ETC de usuario de 0,75

| Método para el cálculo de FTE (configuración del sistema) | **Horas desde el horario del usuario** | **Horas desde el horario predeterminado** | **Campo FTE de usuario** | **Horas disponibles en el Planificador de recursos** | **ETC disponibles en el Planificador de recursos** |
|---|---|---|---|---|---|
| **El horario predeterminado** | Ignorado | 40 | 0.75 | **30** (calculado) | **0.75** |
| **El horario del usuario** | 20 | 40 | Ignorado | **20** | **0,5** (calculado) |

Las excepciones de horario y los días libres pueden afectar a la cantidad de horas planificadas o ETC. Para obtener más información, consulte [Configurar preferencias de administración de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Calcule el resto de los valores de horas y horas trabajadas para los usuarios y las funciones del puesto en el Planificador de recursos {#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner}

Además de las horas disponibles o FTE, en el Planificador de recursos también se muestra la siguiente información horaria:

* Horas planificadas
* Horas presupuestadas
* Desviación de hora
* Horas netas\
  Para obtener más información sobre estos valores, consulte [Información general sobre horas, ETC y costos en las vistas Proyecto y Rol del Planificador de recursos](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

* Diferencia de horas\
  Para obtener más información sobre lo que representa este valor, consulte [Información general sobre horas, ETC y costos en las vistas Proyecto y Rol del Planificador de recursos](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

Puede mostrar la misma información en el Planificador de recursos como FTE o como horas.

Workfront utiliza la fórmula siguiente para mostrar todos los demás valores como FTE en el Planificador de recursos:

`FTE = Resource Planner Hours/ Default Schedule Hours`

>[!NOTE]
>
>AVL La programación del usuario se ignora al calcular el valor de FTE para todos los valores excepto para los valores de FTE disponibles (en el caso de los valores de FTE disponibles, en el Planificador de recursos). Para el cálculo solo se tiene en cuenta el Horario predeterminado.

Este cálculo se aplica a los siguientes valores:

* ETC planificado (PLN)
* ETC presupuestado (BDG)
* Desviación de FTE (VAR)
* NET FTE
* Diferencia de FTE (DIF)
