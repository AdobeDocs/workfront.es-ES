---
content-type: overview
product-area: projects
navigation-topic: financials
title: Visión General de Jerarquía de Ingresos y Costes
description: Este artículo describe el proceso paso a paso para determinar las tarifas de facturación y de costo adecuadas para los roles de trabajo y los usuarios para el tipo de ingresos y de costo por hora de usuario y rol.
author: Lisa
feature: Work Management
source-git-commit: dfc6344303f33a9c3c89837b759235612e54904e
workflow-type: tm+mt
source-wordcount: '3519'
ht-degree: 0%

---

# Resumen de la jerarquía de ingresos y costes

{{highlighted-preview-article-level}}

{{ultimate-package}}

Para proporcionar cálculos financieros precisos, Workfront utiliza las tarifas de facturación adecuadas al calcular los ingresos de una tarea o proyecto. La función y las tasas de usuario deben estar bien definidas a todos los niveles para lograr cálculos financieros precisos.

Las secciones de este artículo describen el proceso paso a paso para determinar las tarifas de facturación y de costo adecuadas para los roles de trabajo y los usuarios para el tipo de ingresos y de costo por hora de usuario y rol.

Para obtener más información sobre tarifas de facturación, tipos de ingresos y cómo se calculan los ingresos, consulte [Información general sobre facturación e ingresos](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Resumen de las fechas de entrada en vigor

Los administradores de Workfront pueden, opcionalmente, establecer fechas en vigor que determinen cuándo se aplican en el sistema las tarifas de facturación, las tarifas de coste y otros atributos financieros. Por ejemplo, un rol o usuario puede tener una tasa de facturación predeterminada de 50 $. Con las fechas efectivas aplicadas, esa tasa de $50 podría establecerse para que caduque el 31 de marzo, y una nueva tasa de $55 comenzaría automáticamente el 1 de abril.

Para los cálculos de ingresos planificados, las tarifas de facturación se basan en la fecha de las horas planificadas. Las horas planificadas se distribuyen de forma uniforme a lo largo de la duración de la tarea. En el ejemplo anterior, las horas planificadas para el 31 de marzo o una fecha anterior utilizan la tasa de 50 $, y las horas planificadas para el 1 de abril o una fecha posterior utilizan la tasa de 55 $.

Para los cálculos de ingresos reales, las tarifas de facturación se basan en la fecha de las horas registradas. En el ejemplo anterior, las horas registradas el 31 de marzo o en una fecha anterior utilizan la tasa de 50 $, y las horas registradas el 1 de abril o en una fecha posterior utilizan la tasa de 55 $.

>[!NOTE]
>
>Las asignaciones de tareas no están definidas con fechas en vigor. En su lugar, las asignaciones extraen las tasas aplicables del sistema, ya sea de una tarjeta de tasas, un perfil de usuario o una sustitución de nivel de asignación. Las fechas en vigor garantizan que la tasa correcta se aplique en función del tiempo de trabajo, pero no definen directamente las asignaciones.

## Resumen del rol de facturación

Se ha establecido una **función del puesto para la facturación** para un usuario en el nivel de asignación o de proyecto. Solo se aplica a los usuarios y no se puede utilizar en otros roles. Por ejemplo, la función de trabajo principal de un usuario es Designer, pero en una tarea o proyecto actúa como Designer sénior y la tasa debe reflejarlo.

Un rol de nivel de asignación para facturación es sólo para esa asignación específica y no se aplica automáticamente a las demás asignaciones del usuario. Un rol de nivel de proyecto para facturación se aplica a todas las asignaciones del usuario en ese proyecto. Puede anularlo en el nivel de asignación individual si es necesario.

Cuando se aplica una función de trabajo para la facturación en el nivel de asignación de usuario o de proyecto, se puede utilizar la tarifa adjunta a la función de trabajo para la facturación en lugar de las tarifas de usuario o función de trabajo en los cálculos de ingresos. El rol de facturación solo está disponible cuando se utiliza el tipo de ingresos por hora Usuario y Rol.

>[!NOTE]
>
>Aunque un usuario puede actuar con una función diferente a efectos de facturación, los cálculos de costes siguen utilizando su función de trabajo principal. La función del puesto de facturación solo afecta a los cálculos de facturación.

Para obtener más información, consulte [Configurar un rol para la facturación](/help/quicksilver/manage-work/projects/project-finances/set-up-job-role-for-billing.md).

## Resumen de las tarifas conservadas

El indicador **Conservar información de tarifas de facturación del proyecto** en un proyecto controla si el sistema usa la información de facturación para las asignaciones en el momento en que se finaliza la tarjeta de tarifas, o si permite modificaciones basadas en cambios durante el transcurso del proyecto. Cualquier cambio en el rol de trabajo, el salario, la tarjeta de tarifas u otra información relacionada con la facturación del usuario no afectará las tarifas de facturación para las asignaciones. Las tarifas se conservan de acuerdo con la tarjeta de tarifas final en el momento en que se activó el indicador del proyecto. Estas propiedades de asignación (como el rol y el salario) se siguen actualizando, lo que garantiza que el coste real de la asignación sea preciso.

Cuando el indicador está activado, el sistema bloquea las tarifas de facturación con fecha efectiva (establecidas en la tarjeta de tarifas finalizada adjunta al proyecto) durante la duración del proyecto.

El indicador se puede activar en un proyecto cuando el trabajo ha comenzado y ya existen asignaciones y horas. En ese momento:

* La tarifa final aprobada para la tarjeta de tarifas se convierte en la fuente de tarifas de facturación para todas las asignaciones del proyecto.
* Todas las asignaciones pasadas, actuales y futuras se recalcularán utilizando las tasas aprobadas finales.
* Se vuelven a calcular los valores reales y planificados.

>[!NOTE]
>
>Una vez activado el indicador para conservar las tarifas de facturación, no se puede desactivar a menos que el proyecto no tenga asignaciones ni horas. Esto garantiza que todos los informes financieros reflejen las verdaderas tasas contractuales.
>Cuando el indicador está desactivado, el sistema permite volver a calcular o ajustar dinámicamente las tarifas de facturación. Cualquier actualización de la función, el salario o la tarifa de facturación del usuario se reflejará inmediatamente en la tarifa de facturación de la asignación.

Para obtener más información, consulte [Editar proyectos](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md) y [Administrar tarjetas de tarifas](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

## Ingresos planificados - Usuario y rol por hora

Cuando el tipo de ingresos de la tarea es Usuario y Rol por hora, Workfront utiliza jerarquías de tasas de usuarios y de roles para determinar la tasa de facturación de los ingresos planificados.

Esta imagen muestra el flujo de la jerarquía de ingresos planificada:

![Ingresos planificados para el tipo de ingresos por hora de usuario y rol](assets/planned-revenue-chart.png)

Cuando se asigna un usuario a la tarea, Workfront busca según esta jerarquía:

1. El sistema busca primero una tasa conservada en la asignación para el usuario.

   Una tasa conservada sigue la jerarquía, pero la tasa se bloquea cuando se conserva el proyecto. Para obtener más información, vea [Información general sobre las tarifas conservadas](#overview-of-preserved-rates).

1. A continuación, el sistema busca la tasa de facturación en una tarjeta de tarifas, para la función de trabajo principal o la función de trabajo para la facturación del usuario asignado a la tarea. Si existe una tasa y está bloqueada, esa tasa se utiliza en el cálculo de ingresos.

   Si existe una tasa en la tarjeta de tasas y está desbloqueada, el sistema no utiliza esa tasa y busca la siguiente tasa en la jerarquía.

1. A continuación, el sistema busca la tasa de anulación en el nivel de asignación para el usuario. Se trata de una tasa agregada manualmente vinculada a la asignación específica y reemplaza todas las demás tasas para el usuario de esta asignación (excepto una tasa bloqueada en la tarjeta de tasas). Si se encuentra una tasa, esta se utiliza en el cálculo de ingresos.
1. A continuación, el sistema busca una función de trabajo para la facturación en el nivel de asignación de tareas.

   La función de trabajo para la facturación es solo para una asignación específica y se aplica a la asignación en lugar de la tasa de función de trabajo principal del usuario. Por ejemplo, la función de trabajo principal de un usuario es Designer, pero en una tarea actúa como Designer sénior con una tasa de facturación más alta.

   Workfront busca la función para la tasa de facturación:

   * El sistema busca primero la tasa de facturación de la función de trabajo para la facturación de la asignación (Designer sénior en el ejemplo), teniendo en cuenta las fechas en vigor. Verá esto en el área Tasas > Facturación del proyecto, en una agrupación **Tasa Source: invalidaciones > Tipo de recurso: Rol**. Se trata de una tasa de anulación del proyecto.
   * A continuación, el sistema busca la función del puesto de tarifa de facturación en una tarjeta de tarifa, teniendo en cuenta las fechas de entrada en vigor. Verá esto en el área Tasas > Facturación del proyecto, en una agrupación **Tasa Source: Tasa adjunta > Tipo de recurso: Rol**.
   * Si la tarifa de la función de facturación no está en el proyecto ni en la tarjeta de tarifas, el sistema busca la tarifa de función de nivel de sistema (Designer sénior en el ejemplo), teniendo en cuenta las fechas en vigor.
   * Si se asigna una función de trabajo para facturación y no se encuentra ninguna de las tarifas de los pasos anteriores, la tarifa de facturación es 0.

     >[!NOTE]
     >
     >Cuando se asigna una función de trabajo para facturación, pero la tasa de facturación es 0, este es un indicador para volver a configurar la tasa. Una tasa de 0 significa que no se configuraron tasas para ese rol (Designer sénior en el ejemplo) en Workfront. Debe agregar tarifas para el rol o eliminar el rol para facturación de la asignación.
     >
     >Dado que las tareas heredan las tarifas de rol del proyecto cuando están disponibles en el nivel de proyecto, las tarifas de búsqueda de la función de trabajo para facturación en el proyecto ya se habrían encontrado cuando Workfront buscó en la función de trabajo para facturación en el nivel de asignación de tarea. La búsqueda en el nivel de proyecto de un rol de facturación sigue estando en la jerarquía de búsqueda.

1. Si una función de trabajo para facturación no estaba disponible en el nivel de asignación de tarea, el sistema busca la tasa de facturación en el proyecto, para el usuario específico asignado a la tarea, teniendo en cuenta las fechas en vigor. Verá esto en el área Tasas > Facturación del proyecto, en una agrupación **Tarifa Source: invalidaciones > Tipo de recurso: usuario**. Se trata de una tasa de anulación del proyecto.
1. A continuación, el sistema busca la tasa de facturación en el nivel del sistema en el perfil del usuario, teniendo en cuenta las fechas de entrada en vigor.
1. A continuación, el sistema busca la tasa de facturación de la función de trabajo principal del usuario (Designer en el ejemplo).

   * El sistema busca primero la tasa de facturación del proyecto, para el rol principal del usuario, teniendo en cuenta las fechas de vigencia. Verá esto en el área Tasas > Facturación del proyecto, en una agrupación **Tasa Source: invalidaciones > Tipo de recurso: Rol**. Se trata de una tasa de anulación del proyecto.
   * A continuación, el sistema busca la tasa de función del puesto en una tarjeta de tasa, teniendo en cuenta las fechas en vigor. Verá esto en el área Tasas > Facturación del proyecto, en una agrupación **Tasa Source: Tasa adjunta > Tipo de recurso: Rol**.
   * A continuación, el sistema busca la tasa de funciones a nivel del sistema, teniendo en cuenta las fechas de entrada en vigor.

1. Si no se encuentra ninguna de estas tarifas, la tarifa de facturación es 0.

Cuando un usuario no está asignado a la tarea, Workfront busca las tasas de rol según esta jerarquía:

1. En primer lugar, el sistema busca una tasa conservada en la asignación del rol.
1. El sistema busca la tasa de facturación en una tarjeta de tarifas, para el rol asignado a la tarea. Si existe una tasa y está bloqueada, esa tasa se utiliza en el cálculo de ingresos.

   Si existe una tasa en la tarjeta de tasas y está desbloqueada, el sistema no utiliza esa tasa y busca la siguiente tasa en la jerarquía.

1. A continuación, el sistema busca la tasa de anulación de la tarea de asignación para el rol. Se trata de una tasa añadida manualmente para el rol en la asignación específica y anula todas las demás tasas para el rol en esta tarea. Si se encuentra una tasa, esta se utiliza en el cálculo de ingresos.
1. A continuación, el sistema busca la tasa de facturación para el rol asignado a la tarea.

   * El sistema busca primero la tasa de facturación del proyecto para el rol, teniendo en cuenta las fechas de vigencia. Verá esto en el área Tasas > Facturación del proyecto, en una agrupación **Tasa Source: invalidaciones > Tipo de recurso: Rol**. Se trata de una tasa de anulación del proyecto.
   * A continuación, el sistema busca la tasa de función del puesto en una tarjeta de tasa, teniendo en cuenta las fechas en vigor. Verá esto en el área Tasas > Facturación del proyecto, en una agrupación **Tasa Source: Tasa adjunta > Tipo de recurso: Rol**.
   * A continuación, el sistema busca la tasa de funciones a nivel del sistema, teniendo en cuenta las fechas de entrada en vigor.

1. Si no se encuentra ninguna de estas tarifas, la tarifa de facturación es 0.

## Ingresos reales - Usuario y rol por hora

Cuando el tipo de ingresos de la tarea es Usuario y Rol por hora, Workfront utiliza dos jerarquías para determinar la tasa de facturación de los ingresos reales. La tasa de facturación se basa en las horas de registro del usuario en una tarea.

El &quot;usuario&quot; en las jerarquías es la persona asignada a la tarea. El &quot;propietario&quot; es la persona cuyo tiempo se registra en la tarea, incluso si no está asignada a la tarea. Por ejemplo, a Michael se le asigna una tarea, pero Joanna completa el trabajo porque Michael estaba enfermo. El administrador puede registrar la hora con la tarea y establecer el propietario de las horas registradas en Joanna. Los valores de ingresos planificados se basan en la asignación y tasa de Michael en la jerarquía, pero los valores de ingresos reales se basan en la tasa de Joanna.

Esta imagen muestra el flujo de la jerarquía de ingresos real:

![Ingresos reales por tipo de costo por hora de usuario y rol](assets/actual-revenue-chart.png)

### Cuando el propietario de las horas registradas y el usuario asignado en la tarea son el mismo

Workfront busca primero una tarifa de facturación por la asignación del usuario. Si un usuario no está asignado a la tarea, busca una tasa de facturación por la asignación de rol.

La jerarquía para este escenario es la misma que la jerarquía de ingresos planificada. Ver [Ingresos planificados - Usuario y rol por hora](#planned-revenue--user-and-role-hourly) para este flujo de trabajo.

### Cuando el propietario de las horas registradas no es el usuario asignado a la tarea

Workfront busca en las propiedades de usuario del propietario según esta jerarquía:

1. El sistema busca primero una tasa conservada en la asignación para el propietario.
1. A continuación, el sistema busca la tasa de facturación en una tarjeta de tarifas, para la función de trabajo principal del propietario. Si existe una tasa y está bloqueada, esa tasa se utiliza en el cálculo de ingresos.

   Si existe una tasa en la tarjeta de tasas y está desbloqueada, el sistema no utiliza esa tasa y busca la siguiente tasa en la jerarquía.

1. A continuación, el sistema busca la tasa de facturación del proyecto, para el propietario, teniendo en cuenta las fechas de entrada en vigor. Verá esto en el área Tasas > Facturación del proyecto, en una Tasa Source: Anulaciones > Tipo de recurso: Agrupación de usuarios. Se trata de una tasa de anulación del proyecto.
1. A continuación, el sistema busca una función de trabajo para la facturación en el nivel de proyecto.

   La función de trabajo para la facturación es solo para un proyecto específico y se aplica al proyecto en lugar de la tasa de función de trabajo principal del propietario. Por ejemplo, la función principal del propietario es Designer, pero en un proyecto actúa como Designer sénior con una tasa de facturación más alta.

   Workfront busca la función para la tasa de facturación:

   * El sistema busca primero la función del puesto para la tarifa de facturación desde una tarjeta de tarifas, teniendo en cuenta las fechas de entrada en vigor. Verá esto en el área Tasas > Facturación del proyecto, en una agrupación **Tasa Source: Tasa adjunta > Tipo de recurso: Rol**.
   * Si la tarifa de la función de facturación no está en la tarjeta de tarifas, el sistema busca la tarifa de función de nivel de sistema (Designer sénior en el ejemplo), teniendo en cuenta las fechas en vigor.
   * Si se asigna una función de trabajo para facturación y no se encuentra ninguna de las tarifas de los pasos anteriores, la tarifa de facturación es 0.

     >[!NOTE]
     >
     >Cuando se asigna una función de trabajo para facturación, pero la tasa de facturación es 0, este es un indicador para volver a configurar la tasa. Una tasa de 0 significa que no se configuraron tasas para ese rol (Designer sénior en el ejemplo) en Workfront. Debe agregar tarifas para el rol o eliminar el rol para facturación del proyecto.

1. A continuación, el sistema busca la tasa de facturación en el nivel del sistema en el perfil de usuario del propietario, teniendo en cuenta las fechas de entrada en vigor.
1. A continuación, el sistema busca la tasa de facturación de la función de trabajo principal del propietario (Designer en el ejemplo).

   * El sistema busca primero la tasa de facturación del proyecto, para el rol principal del propietario, teniendo en cuenta las fechas de vigencia. Verá esto en el área Tasas > Facturación del proyecto, en una agrupación **Tasa Source: invalidaciones > Tipo de recurso: Rol**. Se trata de una tasa de anulación del proyecto.
   * A continuación, el sistema busca la tasa de función del puesto en una tarjeta de tasa, teniendo en cuenta las fechas en vigor. Verá esto en el área Tasas > Facturación del proyecto, en una agrupación **Tasa Source: Tasa adjunta > Tipo de recurso: Rol**.
   * A continuación, el sistema busca la tasa de funciones a nivel del sistema, teniendo en cuenta las fechas de entrada en vigor.

1. Si no se encuentra ninguna de estas tarifas, la tarifa de facturación es 0.

## Coste planificado - Usuario y rol por hora

Cuando el tipo de coste de la tarea es Usuario y Rol por hora, Workfront utiliza jerarquías de tasa de usuarios y de roles para determinar la tasa del coste planificado.

Esta imagen muestra el flujo de la jerarquía de costes planificada:

![Costo planificado para el tipo de costo por hora de usuario y rol](assets/planned-cost-chart.png)

Cuando se asigna un usuario a la tarea, Workfront busca según esta jerarquía:

1. El sistema busca la tasa de anulación de la tarea de asignación para el usuario. Se trata de una tasa agregada manualmente para el usuario en la asignación específica y anula todas las demás tasas para el usuario en esta tarea. Si se encuentra una tasa, esta se utiliza en el cálculo de costes.
1. A continuación, el sistema busca la tasa de coste del proyecto para el usuario específico asignado a la tarea, teniendo en cuenta las fechas en vigor. Verá esto en el área Tasas > Costo del proyecto, en una agrupación de **Tasa Source: invalidaciones > Tipo de recurso: usuario**. Se trata de una tasa de anulación del proyecto.
1. A continuación, el sistema busca la tasa de coste a nivel del sistema en el perfil del usuario, teniendo en cuenta las fechas de entrada en vigor.
1. A continuación, el sistema busca la tasa de coste de la función de trabajo principal del usuario con la combinación de atributos asignados, en función de la puntuación del atributo.
1. Si no se encuentra ninguna de estas tasas, la tasa de coste es 0.

Cuando un usuario no está asignado a la tarea, Workfront busca las tasas de coste de la función del trabajo según esta jerarquía:

1. El sistema busca la tasa de anulación de la tarea de asignación para el rol. Se trata de una tasa añadida manualmente para el rol en la asignación específica y anula todas las demás tasas para el rol en esta tarea. Si se encuentra una tasa, esta se utiliza en el cálculo de costes.
1. A continuación, el sistema busca la tasa de coste de funciones a nivel del sistema con la combinación de atributos asignados, basándose en la puntuación de atributos, teniendo en cuenta las fechas en vigor.
1. Si no se encuentra ninguna de estas tasas, la tasa de coste es 0.

## Coste real: usuario y rol por hora

Cuando el tipo de coste de la tarea es Usuario y Rol por hora, Workfront utiliza dos jerarquías para determinar la tasa de facturación del coste real. La tasa de facturación se basa en las horas de registro del usuario en una tarea.

El &quot;usuario&quot; en las jerarquías es la persona asignada a la tarea. El &quot;propietario&quot; es la persona cuyo tiempo se registra en la tarea, incluso si no está asignada a la tarea. Por ejemplo, a Michael se le asigna una tarea, pero Joanna completa el trabajo porque Michael estaba enfermo. El administrador puede registrar la hora con la tarea y establecer el propietario de las horas registradas en Joanna. Los valores de ingresos planificados se basan en la asignación y tasa de Michael en la jerarquía, pero los valores de ingresos reales se basan en la tasa de Joanna.

Esta imagen muestra el flujo de la jerarquía de coste real:

![Costo real por tipo de costo por hora de usuario y rol](assets/actual-cost-chart.png)

### Cuando el propietario de las horas registradas y el usuario asignado en la tarea son el mismo

Workfront busca primero una tasa de coste por la asignación del usuario. Si un usuario no está asignado a la tarea, busca una tasa de coste por la asignación de rol.

La jerarquía para este escenario es la misma que la jerarquía de coste planificada. Consulte [Coste planificado - Usuario y rol por hora](#planned-cost--user-and-role-hourly) para este flujo de trabajo.

### Cuando el propietario de las horas registradas no es el usuario asignado a la tarea

Workfront busca en las propiedades de usuario del propietario según esta jerarquía:

1. El sistema busca la tasa de costo en el proyecto, para el propietario, teniendo en cuenta las fechas efectivas. Verá esto en el área Tasas > Costo del proyecto, en una agrupación de **Tasa Source: invalidaciones > Tipo de recurso: usuario**. Se trata de una tasa de anulación del proyecto.
1. A continuación, el sistema busca la tasa de coste a nivel del sistema en el perfil de usuario del propietario, teniendo en cuenta las fechas de entrada en vigor.
1. A continuación, el sistema busca la tasa de coste de la función de trabajo principal del propietario (Designer en el ejemplo).

   * El sistema busca primero la tasa de coste del proyecto, para el rol principal del propietario, teniendo en cuenta las fechas de entrada en vigor. Verá esto en el área Tasas > Costo del proyecto, en una agrupación de **Tasa Source: invalidaciones > Tipo de recurso: Rol**. Se trata de una tasa de anulación del proyecto.
   * A continuación, el sistema busca la tasa de función del puesto en una tarjeta de tasa, teniendo en cuenta las fechas en vigor. Verá esto en el área Tasas > Costo del proyecto, en una agrupación de **Tasa Source: Tasa adjunta > Tipo de recurso: Rol**.
   * A continuación, el sistema busca la tasa de funciones a nivel del sistema, teniendo en cuenta las fechas de entrada en vigor.

1. Si no se encuentra ninguna de estas tarifas, la tarifa de facturación es 0.

