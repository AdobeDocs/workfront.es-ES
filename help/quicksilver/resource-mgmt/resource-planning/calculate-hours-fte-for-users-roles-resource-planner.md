---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Información general sobre el cálculo de horas y FTE para usuarios y roles en el Planificador de recursos
description: Información general sobre el cálculo de horas y FTE para usuarios y roles en el Planificador de recursos.
author: Lisa
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
source-git-commit: 7f0aac7c8519b1e570e29fedf1492918e8120ad2
workflow-type: tm+mt
source-wordcount: '1323'
ht-degree: 67%

---

# Información general sobre el cálculo de horas y EJC para usuarios y funciones en el Planificador de recursos

<!-- Audited: 5/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina:KEEP THIS:***Linked to: Configuring My Settings, Editing User Accounts, Planning in the Resource Planner -- *** Some of this documentation is also duplicated in this article (Scheduling): https://support.workfront.com/hc/en-us/articles/360000557174)</p>
-->

Puede mostrar la asignación y disponibilidad de los recursos en el Planificador de recursos por horas, EJC o coste.\
Para obtener más información sobre el cálculo de costes en el Planificador de recursos, consulte [Calcular costes en el Planificador de recursos](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

Equivalente a tiempo completo (ETC) es una medida del tiempo que representa la cantidad de horas dedicadas al trabajo real durante un día o una semana para un usuario o rol.

Los siguientes conjuntos de información de recursos se calculan de forma diferente en el Planificador de recursos:

* Los valores de Horas disponibles o EJC se calculan según la forma en que el administrador del sistema configure las preferencias de Administración de recursos en el sistema.\
  Para obtener más información sobre cómo se calculan los valores de horas disponibles y de tiempo completo, consulte [Calcular horas disponibles o EJC para usuarios y funciones en el Planificador de recursos](#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner).\
  Para obtener más información sobre la definición de las preferencias de Administración de recursos para el sistema de Adobe Workfront, consulte [Configurar preferencias de administración de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* Todos los demás valores de EJC se calculan según el horario predeterminado del sistema.\
  Para obtener más información sobre cómo se muestran todos los demás valores en el Planificador de recursos al utilizar EJC, consulte la sección [Calcular todos los demás valores de horas y EJC para usuarios y funciones el Planificador de recursos](#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner) en este artículo.

Es importante comprender cuál es el EJC para cada uno de los usuarios y sus funciones para administrar con precisión los recursos a medida que los asigna al trabajo.

## Calcular horas disponibles o EJC para usuarios y funciones en el Planificador de recursos {#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner}

### Calcular las horas disponibles y EJC para un usuario en el Planificador de recursos {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner}

El administrador de Workfront determina cómo se calcula el tiempo disponible para un usuario seleccionando una de las siguientes opciones en el área Administración de recursos de Configuración:

* El horario predeterminado del sistema y el EJC del usuario.
* El horario del usuario.

![Configuración del sistema para los horarios de los usuarios](assets/setup-resource-mgmt.png)

>[!NOTE]
>
>Determina cómo calcular la disponibilidad de los recursos a nivel del sistema. Para obtener más información sobre la definición de las preferencias de administración de recursos para el sistema, consulte [Configurar preferencias de administración de recursos](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

En función de cómo se configure esta opción, la disponibilidad de los usuarios en el Planificador de recursos (horas y disponibilidad de EJC) se calcula mediante los siguientes métodos:

* **El horario predeterminado**: el horario predeterminado del sistema y EJC del usuario se utilizan para determinar las horas disponibles y el valor de EJC para el usuario en el Planificador de recursos. Se ignora la programación del usuario. En este caso:

   * Las horas disponibles en el Planificador de recursos se calculan mediante la siguiente fórmula:

     `User Available Hours = Default Schedule Hours * User FTE value`

     Por ejemplo, si el horario predeterminado tiene 40 horas a la semana disponibles para trabajar y el EJC del usuario es 0,5, el usuario estará disponible para trabajar 20 horas a la semana en el Planificador de recursos.

     Para obtener más información sobre las programaciones, incluido el horario predeterminado, consulte [Crear programación](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   * El valor de FTE disponible para el usuario en el Planificador de recursos es el mismo que el valor de FTE del usuario especificado en la configuración del usuario.

     Por ejemplo, si el EJC del usuario es 0,5 en la configuración de usuario, el EJC disponible del usuario es 0,5 en el Planificador de recursos. Para obtener más información sobre el valor de EJC del usuario tal como se muestra en la configuración del usuario, consulte [Editar el perfil de un usuario](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* **El horario del usuario**: El horario del usuario se usa para determinar la disponibilidad del usuario en el Planificador de recursos. Se ignora el valor de FTE del usuario. En este caso:

   * Las horas disponibles en el Planificador de recursos son las mismas que las horas de la programación del usuario.

     Por ejemplo, si la programación del usuario tiene 40 horas a la semana disponibles para trabajar, el usuario puede trabajar durante 40 horas a la semana en el Planificador de recursos.

   * El valor de FTE disponible en el Planificador de recursos se calcula mediante la siguiente fórmula:

     `User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours`

     Por ejemplo, si el horario del usuario tiene 20 horas disponibles para trabajar y el Horario predeterminado de Workfront tiene 40 horas disponibles para trabajar, el valor de FTE del usuario es 0,5.

     Para obtener más información sobre las programaciones, incluido el horario predeterminado, consulte [Crear programación](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

>[!NOTE]
>
>Si el usuario no está asociado a un horario, las horas disponibles para el usuario se calculan mediante el horario predeterminado.

### Calcular las horas disponibles y el EJC de una función en el Planificador de recursos {#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner}

Primero, debe calcular la disponibilidad del usuario y, a continuación, puede calcular la disponibilidad de cada una de sus funciones.

La disponibilidad de los roles en el Planificador de recursos tiene en cuenta la disponibilidad total del usuario y el porcentaje de disponibilidad de FTE asociado a cada rol del usuario.\
![percent_of_fte_availability_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)

Para obtener más información acerca de cómo asociar un valor de Porcentaje de disponibilidad de FTE con un rol de usuario, vea [Editar el perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Por ejemplo, si el valor de Horas disponibles para un usuario es 40 y puede desempeñar un rol principal durante el 75 % de ese tiempo y otro rol durante el 25 % de ese tiempo, el Planificador de recursos muestra que el valor de Horas disponibles para el rol principal durante una semana es 30 horas y que el valor de Horas disponibles para el otro rol es 10 horas. En este caso, el valor de FTE para la función principal es 0,75 y el valor de FTE para la otra función es 0,25.

>[!NOTE]
>
>El tiempo total disponible para el usuario se calcula mediante uno de los dos métodos descritos en [Calcular las horas disponibles y FTE para un usuario en el Planificador de recursos](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner) de este artículo.

Al ver el Planificador de recursos en la vista de función, la disponibilidad de una función es un total de la disponibilidad de todos los usuarios que pueden cumplir dicha función.

Para obtener más información sobre la disponibilidad de recursos en el Planificador de recursos, consulte [Información general sobre el Planificador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Calcular las horas disponibles y EJC para un usuario en el Planificador de recursos (ejemplo) {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example}

La siguiente tabla ilustra cómo se calculan las horas disponibles y el tiempo de ejecución completo disponible para el usuario en el Planificador de recursos, en función del método que utilice el administrador del sistema para el cálculo de tiempo de ejecución completo en las Preferencias de administración de recursos.

Para este ejemplo, se utilizan los números siguientes:

* Un horario predeterminado de 40 horas
* Horario de usuario de 20 horas
* Un FTE de usuario de 0,8

| Método para el cálculo del FTE (configuración del sistema) | **Horas a partir del horario del usuario** | **Horas a partir del horario predeterminado** | **Campo FTE del usuario** | **Horas disponibles en el Planificador de recursos** | **FTE disponible en el Planificador de recursos** |
|---|---|---|---|---|---|
| **El horario predeterminado** | Ignorado | 40 | 0,8 | **32** (calculado) | **0,8** |
| **El horario del usuario** | 20 | 40 | Ignorado | **20** | **0,5** (calculado) |

Las excepciones de horario y los días libres pueden afectar a la cantidad de horas planificadas o FTE. Para obtener más información, consulte [Configurar preferencias de administración de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

Ejemplo de vista del Planificador de recursos por usuario y horas:

![Vista del Planificador de recursos por usuario y horas](assets/resource-planner-by-user-by-hours.png)

Ejemplo de vista del Planificador de recursos por usuario y FTE:

![Vista del Planificador de recursos por usuario y ETC](assets/resource-planner-by-user-by-fte.png)

## Calcular todos los demás valores de horas y FTE para usuarios y funciones en el Planificador de recursos {#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner}

Además de las horas disponibles o FTE, en el Planificador de recursos también se muestra la siguiente información horaria:

* Horas planificadas
* Horas presupuestadas
* Variación de horas
* Horas netas\
  Para obtener más información, vea [Información general sobre horas, FTE y costes en las vistas Proyecto y Función del Planificador de recursos](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

* Diferencia de horas\
  Para obtener más información, vea [Información general sobre horas, FTE y costes en las vistas Proyecto y Función del Planificador de recursos](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

Puede mostrar la misma información en el Planificador de recursos que ETC u horas.

Workfront utiliza la fórmula siguiente para mostrar todos los demás valores como FTE en el Planificador de recursos:

`FTE = Resource Planner Hours/ Default Schedule Hours`

>[!NOTE]
>
>La programación del usuario se omite al calcular el valor de FTE para todos los valores excepto para los valores de FTE disponibles (AVL) en el Planificador de recursos. Para el cálculo solo se tiene en cuenta el Horario predeterminado.

Este cálculo se aplica a los siguientes valores:

* FTE planificado (PLN)
* FTE presupuestado (BDG)
* Variación de ETC (VAR)
* ETC NETO
* Diferencia de ETC (DIF)
