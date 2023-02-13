---
filename: migrate-resource-scheduling-to-workload-balancer
product-area: resource-management
navigation-topic: resource-management-overview
title: Migración de la programación de recursos a [!UICONTROL Equilibrador de carga de trabajo]
description: Queremos que experimente la menor interrupción posible del trabajo ayudándole a diseñar un plan de migración. Los pasos siguientes le ayudarán a capacitar a su equipo y a determinar el mejor momento para cambiar al equilibrador de carga de trabajo.
author: Alina
exl-id: 4bc08d5f-99c7-40e2-85d6-1de0b585aef8
source-git-commit: d2a8380e3383b97b8245bd2b6d3cb9ff75306e4f
workflow-type: tm+mt
source-wordcount: '1304'
ht-degree: 0%

---

# Migrar desde recurso [!UICONTROL Programación] a [!UICONTROL Equilibrador de carga de trabajo]

<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa.</span>

<!-- drafted for res scheduling deprecation blurb for PREVIEW release - Oct 2022 - CHANGE THIS BLURB TO SOMETHING ELSE AT PRODUCTION:-->

>[!CAUTION]
>  
>  
> <span class="preview">Las áreas de programación se han eliminado del entorno de vista previa y se eliminarán del entorno de producción en **Enero de 2023**. </span>\
> <span class="preview"> Después de enero de 2023, debe programar los recursos en el equilibrador de carga de trabajo. </span>
>  
><span class="preview"> Para obtener información sobre la programación de recursos mediante el equilibrador de carga de trabajo, consulte la sección [El equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/workload-balancer.md).</span>

La información de este artículo se aplica solo si ha gestionado la programación de sus recursos en el recurso [!UICONTROL Programación] áreas de Adobe Workfront. Workfront ha comenzado a dejar de utilizar la variable [!UICONTROL Programación] herramientas en noviembre de 2020 y las ha sustituido por el [!UICONTROL Equilibrador de carga de trabajo].

Para obtener información sobre el plan de desuso para la variable [!UICONTROL Programación de recursos] herramientas y la cronología para su reemplazo con la variable [!UICONTROL Equilibrador de carga de trabajo], consulte [Obsolescencia de las herramientas de programación de recursos en Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

Queremos que experimente la menor interrupción posible del trabajo ayudándole a diseñar un plan de migración. Los pasos siguientes le ayudarán a capacitar a su equipo y a determinar el mejor momento para cambiar al [!UICONTROL Equilibrador de carga de trabajo].

## Localización de las herramientas de programación de recursos

Es posible que usted y sus equipos estén utilizando parte del recurso [!UICONTROL Programación] herramientas en las siguientes áreas de Workfront:

* La variable [!UICONTROL Programación] en la sección [!UICONTROL Recurso] area
* La variable [!UICONTROL Programación] sección de un proyecto
* La variable [!UICONTROL Programación] sección de un equipo

Con esta desaprobación, la variable [!UICONTROL Equilibrador de carga de trabajo] reemplaza todas las variables  [!UICONTROL Programación de recursos] herramientas en todas las áreas enumeradas anteriormente.

## Paso 1: Capacite a sus equipos

Tome la formación [Programa de Gestión de Recursos para la nueva experiencia de Adobe Workfront](https://one.workfront.com/s/resource-management-program-nwe) (75 minutos) en Workfront One.

Si tiene dificultades para iniciar sesión o acceder al curso, póngase en contacto con el servicio de atención al cliente. Para obtener más información, consulte [Contactar con el servicio de atención al cliente](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

## Paso 2: Determine el mejor momento para migrar {#step-2-determine-the-best-time-to-migrate}

Siga los pasos a continuación para determinar cuándo es el mejor momento para migrar:

1. Determinar qué características del recurso [!UICONTROL Programación] herramientas que su equipo utiliza con mayor frecuencia y asegúrese de que dichas funciones están disponibles en la [!UICONTROL Equilibrador de carga de trabajo]. Para obtener información sobre qué características están disponibles actualmente en la variable [!UICONTROL Equilibrador de carga de trabajo], consulte la sección &quot;Disponibilidad de funciones&quot; en el artículo [Obsolescencia de las herramientas de programación de recursos en Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

   >[!IMPORTANT]
   >
   >Casi todas las capacidades de las herramientas de programación están ahora en Workload Balancer.

1. Determine si su equipo administra asignaciones de usuario en asignaciones. Ajustar o modificar las asignaciones de usuario significa modificar las horas programadas por día para cada usuario a lo largo de la duración de un elemento de trabajo.

   Las asignaciones editadas en las herramientas de programación no se transfieren al equilibrador de carga de trabajo. De forma predeterminada, el sistema distribuye por igual el total de horas planificadas de un elemento de trabajo durante toda la duración del elemento.

   Debe administrar las asignaciones manualmente en el equilibrador de carga de trabajo para asegurarse de que las asignaciones coinciden con las que tiene en las herramientas de programación. Para obtener más información, consulte [Administrar asignaciones de usuario en el equilibrador de carga de trabajo](../workload-balancer/manage-user-allocations-workload-balancer.md).

1. Los filtros guardados en el área Programación no se transferirán automáticamente al equilibrador de carga de trabajo. Tómese tiempo para crear los filtros que pueda necesitar en el equilibrador de carga de trabajo. Para obtener información sobre la creación de filtros en el equilibrador de carga de trabajo, consulte [Filtrar información en el equilibrador de carga de trabajo](../workload-balancer/filter-information-workload-balancer.md).

<!--
1. Using the information gathered from Steps 1 and Step 2, decide which version of Step 3 you should continue with based on the needs of your organization.
-->

## Paso 3: Migrar a [!UICONTROL Equilibrador de carga de trabajo]{#step-3-migrate-to-the-workload-balancer}

Hemos identificado las siguientes versiones para este paso, según sus conclusiones en el paso 2:

* [Paso 3a: Usted o sus equipos utilizan la variable [!UICONTROL Programación] , pero no modifique la asignación de usuarios](#step-3a-you-or-your-teams-use-the-scheudling-tools-but-do-not-modify-user-allocation)
* [Paso 3b: Usted o sus equipos administran las asignaciones de usuario en la variable [!UICONTROL Programación] herramientas](#step-3b-you-or-your-teams-manage-user-allocations-in-the-scheduling-tools)

### Paso 3a: Usted o sus equipos utilizan la variable [!UICONTROL Programación] , pero no modifique la asignación de usuarios

Si usted o sus equipos no modifican las asignaciones de horas diarias en las asignaciones de trabajo, entonces está listo para cambiar los recursos de programación a la [!UICONTROL Equilibrador de carga de trabajo].

![](assets/nwe-workload-balancer-global-350x125.png)

Haga lo siguiente:

* Elija una fecha de transición.

   >[!TIP]
   >
   >Proporcione a su equipo un poco de tiempo para realizar la formación sobre el uso del equilibrador de carga de trabajo antes de la fecha de transición. Para obtener información sobre formación, consulte la sección [Migración de la programación de recursos al equilibrador de carga de trabajo](#migrate-from-resource-uicontrol-scheduling-to-the-uicontrol-workload-balancer) en este artículo.

* Siga estas directrices para ayudar a sus equipos:

   * Animar a sus equipos a visitar el [Información general sobre [!UICONTROL Equilibrador de carga de trabajo]](../../resource-mgmt/workload-balancer/overview-workload-balancer.md) y todas las páginas vinculadas desde allí para profundizar en cómo [!UICONTROL Equilibrador de carga de trabajo] funciona.
   * Aloje reuniones de preguntas frecuentes para que sus equipos respondan preguntas la semana anterior a la transición, realicen el cambio y luego celebren otra reunión de preguntas frecuentes para responder a preguntas de seguimiento.
   * Envíe comentarios a Workfront mediante el botón Comentarios de la barra de herramientas superior. Nuestros desarrolladores de productos siempre están interesados en conocer sus casos de uso para saber cómo podemos crear la variable [!UICONTROL Equilibrador de carga de trabajo] proporcione más valor.

### Paso 3b: Usted o sus equipos administran las asignaciones de usuario en la variable [!UICONTROL Programación] herramientas

Si el flujo de trabajo coincide con este escenario, debe ser más estratégico en su plan de transición. Las asignaciones diarias que se muestran en la variable [!UICONTROL Programación] las herramientas se almacenan en una base de datos diferente a las asignaciones diarias que se muestran en la variable [!UICONTROL Equilibrador de carga de trabajo]. Esto significa que los ajustes de las asignaciones diarias que realiza en el recurso [!UICONTROL Programación] las herramientas no se transfieren a las asignaciones diarias en la variable [!UICONTROL Equilibrador de carga de trabajo].

>[!CAUTION]
>
>Tiene hasta **Enero de 2023** para asegurarse de que la asignación de usuarios desde las áreas de programación coincide con la del equilibrador de carga de trabajo en el entorno de producción. En ese momento, se eliminan las herramientas de programación del entorno Producción. Debe ajustar manualmente las asignaciones del equilibrador de carga de trabajo para que coincidan con las de las herramientas de programación. <span class="preview">Las herramientas de programación ya se han eliminado del entorno de vista previa.</span>


Tenga en cuenta lo siguiente al realizar la transición a [!UICONTROL Equilibrador de carga de trabajo] cuando utilice [!UICONTROL Programación] funcionalidad:

* Ponga en espera la gestión de las asignaciones en el [!UICONTROL Programación] herramientas a medida que los gestores de recursos realizan el cambio. Para ello:

   * Averigüe la duración promedio de las tareas en sus proyectos actuales y tenga esto en cuenta a la hora de determinar cuánto tiempo necesita poner en espera la administración de las asignaciones de usuario.

      >[!TIP]
      >
      >Solo debe mirar los proyectos actuales o de planificación, que son aquellos para los que sus equipos están realizando asignaciones de forma activa y administrando asignaciones diarias.

   * Cree un informe de tarea y añada el campo Duración de la tarea en la vista y agrúpelo por Nombre del proyecto. Resuma la columna Duración en la opción Ver por Promedio y, a continuación, guarde el informe.

      Para obtener información sobre cómo crear un informe, consulte [Crear un informe personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) .

   * Analice el informe de tareas. Por ejemplo, si la duración promedio de la tarea es de 3 días, puede que sea mejor una transición de una semana. Haga que el equipo deje de administrar asignaciones de usuarios durante una semana. La semana siguiente, cambie el equipo a [!UICONTROL Equilibrador de carga de trabajo] y comenzar a administrar asignaciones de usuarios la semana siguiente.
   >[!NOTE]
   >
   >Esta sugerencia podría no funcionar si la duración promedio de la tarea es mayor que el tiempo restante hasta la eliminación de las herramientas de programación.


   ![](assets/timeline-stop-using-resource-scheduler-callouts-350x178.png)

   >[!TIP]
   >
   >Puede seguir realizando tareas y asignando tareas durante el período de transición. Las asignaciones realizadas se reflejarán tanto en el Programador de recursos como en [!UICONTROL Equilibrador de carga de trabajo].

* Si es una organización más grande con equipos que administran recursos para cientos de proyectos, puede considerar la posibilidad de realizar la transición desde el [!UICONTROL Programación] para [!UICONTROL Equilibrador de carga de trabajo] un portafolio a la vez. Tenga en cuenta un despliegue gradual mediante la creación de filtros personalizados en la variable [!UICONTROL Equilibrador de carga de trabajo] para ver un portafolio específico a la vez.

* Permita que los administradores de recursos se asocien: tener asignaciones de revisión de persona realizadas en la variable  [!UICONTROL Programación de recursos] herramientas y una que realice los ajustes adecuados en la [!UICONTROL Equilibrador de carga de trabajo]. Una vez que ese equipo de dos reconcilie ambas herramientas, haga que transfieran sus flujos de trabajo a la variable [!UICONTROL Equilibrador de carga de trabajo].

## Necesita más asistencia

Si necesita información adicional con esta migración, póngase en contacto con el soporte técnico personalizado. Para obtener información sobre cómo ponerse en contacto con la asistencia técnica, consulte [Contactar con el servicio de atención al cliente](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
