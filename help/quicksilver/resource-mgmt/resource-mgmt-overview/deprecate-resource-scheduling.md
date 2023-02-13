---
content-type: reference
product-area: resource-management
keywords: carga de trabajo,equilibrador
navigation-topic: resource-management-overview
title: Obsolescencia de las herramientas de programación de recursos en Adobe Workfront
description: Actualmente estamos en proceso de desaprobar todas las herramientas de programación de Adobe Workfront y sustituirlas por el equilibrador de carga de trabajo.
author: Alina
feature: Resource Management
exl-id: 7fa644cd-cf6a-40f8-ae28-bf222bb45d3f
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# Obsolescencia de las herramientas de programación de recursos en Adobe Workfront

>[!IMPORTANT]
>  
><span class="preview">La funcionalidad Programación descrita en este artículo se ha desaprobado y eliminado de Adobe Workfront a partir de la versión 23.1 de enero de 2023.   </span>
>  
> <span class="preview"> Este artículo también se eliminará poco después de la versión 23.1, a principios de 2023. En este momento, le recomendamos que actualice los marcadores según corresponda. </span>
> 
><span class="preview"> Ahora puede utilizar el equilibrador de carga de trabajo para programar el trabajo para sus recursos. </span>
>  
> <span class="preview">Para obtener información sobre la programación de recursos mediante el equilibrador de carga de trabajo, consulte la sección [El equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!--
We are currently in the process of removing all Scheduling tools from Adobe Workfront and replacing them with the Workload Balancer.

>[!IMPORTANT]
>
>We are no longer implementing new feature functionality for the current Scheduling solution and we no longer consider nor prioritize defects for a fix in this area of Adobe Workfront.

This article describes the timeline for this deprecation and it compares the functionality of the Scheduling tools and that of the Workload Balancer to indicate which Scheduling capabilities are already supported in the Workload Balancer. 

We have been announcing a more exact timeline through the Announcement Center at key milestones during the deprecation process and this article has been updated as this process continues.

>[!NOTE]
>
>The changes described in this article do not affect any other resource management tools. For example, they do not affect the [!UICONTROL Resource Planner] or the [!UICONTROL Utilization] report.
-->

## Cómo debe prepararse

Para obtener información detallada sobre cómo debe prepararse para la transición entre Programación y Equilibrador de carga de trabajo, consulte [Migración de la programación de recursos al equilibrador de carga de trabajo](../../resource-mgmt/resource-mgmt-overview/migrate-resource-scheduling-to-workload-balancer.md).

Si actualmente utiliza herramientas de programación, le recomendamos que las interrumpa y empiece a usar el equilibrador de carga de trabajo.

![Área de programación de recursos global](assets/resource-scheduler-global-350x127.png)

Casi todas las funciones disponibles anteriormente en las áreas de programación están ahora disponibles en el equilibrador de carga de trabajo. Para obtener más información, consulte la sección [Disponibilidad de funcionalidades](#feature-availability) en este artículo. Puede continuar programando los recursos para trabajar exclusivamente en el equilibrador de carga de trabajo.

![Área del equilibrador de carga de trabajo global](assets/workload-balancer-pti-350x111.png)

## Información que no se transferirá al equilibrador de carga de trabajo

La siguiente información no se transfiere de las herramientas de programación al equilibrador de carga de trabajo:

* **Asignaciones diarias para usuarios**: No debe utilizar Programación y Equilibrador de carga de trabajo al mismo tiempo para ajustar las mismas asignaciones de usuario. Si ha gestionado las asignaciones de usuario en las herramientas de programación, las asignaciones diarias ajustadas no se transfieren al equilibrador de carga de trabajo. Del mismo modo, si ha ajustado las asignaciones de usuario en el equilibrador de carga de trabajo, no se transfieren a las herramientas de programación. Le recomendamos encarecidamente que se asegure de que las asignaciones diarias sean precisas en el equilibrador de carga de trabajo para prepararse para esta transición. Para obtener más información, consulte [Administrar asignaciones de usuario en el equilibrador de carga de trabajo](../workload-balancer/manage-user-allocations-workload-balancer.md).
* **Filtros**: Si ha guardado filtros en las áreas de programación, no se transfieren al equilibrador de carga de trabajo. Debe volver a crear los filtros en el equilibrador de carga de trabajo. Para obtener más información, consulte [Filtrar información en el equilibrador de carga de trabajo](../workload-balancer/filter-information-workload-balancer.md).

## Elementos destacados de la cronología de obsolescencia

>[!IMPORTANT]
>
>Utilice este artículo para comprender la cronología más reciente para la desaprobación de las herramientas de programación. Cualquier actualización a esta línea de tiempo se comunicará en este artículo y en los mensajes del Centro de anuncios.

A continuación se muestra una cronología del proceso de desaprobación de las herramientas de programación de recursos:

* [Versión 2020.4 (noviembre de 2020)](#2020-4-release-november-2020)
* [Versión 2021.4 (octubre de 2021)](#2021-4-release-october-2021)
* [Versiones de 2022.4 y 2023.1 (de octubre de 2022 a enero de 2023)](#2022-4-2023-1-releases)

### Versión 2020.4 (noviembre de 2020) {#2020-4-release-november-2020}

* La nueva funcionalidad de funciones ya no está implementada para la solución de programación
* Solo se priorizarán los defectos de gravedad altos y críticos para una corrección
* Nuevas funciones del equilibrador de carga de trabajo agregadas a Workfront

### Versión 2021.4 (octubre de 2021) {#2021-4-release-october-2021}

* El equilibrador de carga de trabajo está establecido como predeterminado para cualquier usuario nuevo de Workfront
* Filtros mejorados que se pueden compartir e incluir campos adicionales

### Versiones de 2022.4 y 2023.1 (de octubre de 2022 a enero de 2023) {#2022-4-2023-1-releases}

* No se priorizará ningún defecto para una corrección durante y después de las versiones 2022.4 o 2023.1
* Todas las áreas de programación se eliminan del entorno de vista previa (**20 de octubre de 2022**)
* Todas las áreas de programación se eliminan del entorno de producción (**Enero de 2023**)
* Workload Balancer es la única herramienta de programación de recursos disponible en Workfront (después de **Enero de 2023**)

## Disponibilidad de funcionalidades {#feature-availability}

A menos que se especifique lo contrario, todas las funciones de Programación de recursos han estado o estarán disponibles en el equilibrador de carga de trabajo. Para obtener información sobre el equilibrador de carga de trabajo, consulte [Información general del equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Además de las funciones existentes, el equilibrador de carga de trabajo tiene o tendrá nuevas funciones que no existían en las herramientas de programación de recursos, como se muestra en la siguiente tabla:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td rowspan="2"><span style="font-weight: normal;"><b>Funciones</b></span> </td> 
   <td rowspan="2"> <b>Disponibilidad de funcionalidades de las herramientas de programación de recursos</b></td> 
   <td colspan="3"><b>Disponibilidad de las funciones del equilibrador de carga de trabajo</b></td> 
  </tr> 
  <tr> 
   <td><b>Disponible ahora</b></td> 
   <td><b>Disponible próximamente</b></td> 
   <td><b>No planificado</b></td> 
  </tr> 
  <tr> 
   <td> <p>Herramienta de acceso desde el área Recursos</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Áreas separadas para trabajo no asignado y asignado</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aplicar y crear filtros para trabajo sin asignar y asignado</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Acceder a elementos de trabajo directamente desde la herramienta</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Asignación o desasignación manual de tareas y problemas</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ajustar asignaciones individuales</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Incluir tiempo de problema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Mostrar fechas proyectadas </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Mostrar trabajo completado</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Mostrar el tiempo libre del usuario, los fines de semana y las excepciones de programación</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Asignación rápida de usuarios en función de las funciones*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Reemplazar rápidamente usuarios*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Anular la asignación de usuarios rápidamente*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>Acceso a la herramienta desde un equipo</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>Acceso a la herramienta desde un proyecto</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr>
   <td>Los usuarios con licencia de trabajo pueden ajustar las asignaciones de usuario al acceder al equilibrador de carga de trabajo desde un proyecto </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <td>Mostrar problemas en el área de trabajo sin asignar</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <td><span>Asignación y desasignación de tareas y problemas arrastrando y soltando*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visible para todos los usuarios del Plan, sin que se le designe un Administrador de recursos en el proyecto.</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Agrupar información por proyecto</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Compartir el equilibrador de carga de trabajo con usuarios sin acceso al área de recursos</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Mostrar y ajustar asignaciones por semana</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Acceder a los usuarios directamente desde la herramienta</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Acceda a más información sobre los elementos de trabajo sin salir del panel Resumen*</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Mostrar y ajustar la asignación como valor de porcentaje </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Mostrar la diferencia entre el tiempo disponible y el tiempo asignado</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Mostrar la disponibilidad del usuario en un gráfico</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Elementos de trabajo y proyectos de código de color por estado del proyecto</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Actualizar automáticamente las horas planificadas a medida que ajusta la asignación de usuarios (para tareas con un tipo de duración simple)</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>Sugerir asignaciones basadas en el patrón de asignación del usuario, las asignaciones existentes de Roles o Equipos</span> </td> 
   <td> </td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Filtros mejorados que se pueden compartir e incluir campos adicionales</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>Realizar asignaciones avanzadas</span> </td> 
   <td> </td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr>

<tr> 
   <td><span>Elementos de trabajo de código de color por proyectos y estado del proyecto</span> </td> 
   <td> </td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td>

<tr> 
   <td>Agregar usuarios al equipo del proyecto (reubicado en el <b>People</b> pestaña del proyecto) </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td> </td>

</tr>
   <tr> 
   <td>Asignación automática de tareas y problemas</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr>

</tbody> 
</table>

*Estas funciones solo están disponibles en la nueva experiencia de Adobe Workfront.
