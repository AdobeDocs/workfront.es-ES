---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión final de Beta 2018.1
description: Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión final de Beta 2018.1. La funcionalidad estaba disponible en el entorno de vista previa el 31 de enero de 2018. Estará disponible en el entorno de producción en marzo de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 35bd3604-5452-4b46-afb1-78bc2fbb48ec
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# Actividad de la versión final de Beta 2018.1

Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión final de Beta 2018.1. La funcionalidad estaba disponible en el entorno de vista previa el 31 de enero de 2018. Estará disponible en el entorno de producción en marzo de 2018.

>[!IMPORTANT]
>
> La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción de.

Para ver una lista de todos los cambios realizados en 2018.1, consulte  [resumen de la actividad de la versión 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

La versión final de Beta 2018.1 incluye mejoras para administradores de Workfront y otros usuarios:

**Para Administradores**

* [Configurar disponibilidad de recursos y asignaciones de usuarios para calcular según el horario de usuario](#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule)

**Para Todos Los Usuarios**

* [Mejoras móviles](#mobile-enhancements)
* [Integración de Jira](#jira-integration)
* [Actualización de los nombres de los visualizadores de revisión](#update-to-proofing-viewer-names)
* [Cambio en la cadencia de sincronización al sincronizar desde el entorno de producción de revisión a vista previa](#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview)
* [El mensaje de advertencia aparece cuando se alcanza el límite de 2000 elementos en el Planificador de recursos](#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner)

## Mejoras de Mobile {#mobile-enhancements}

Las siguientes funciones llegarán a las tiendas de aplicaciones móviles a principios de marzo de 2018:

* Nueva navegación: Se ha rediseñado la página de inicio de nuestras aplicaciones móviles.
* Inicio en móvil: Nuestra nueva funcionalidad de Inicio ahora también se ha actualizado en nuestras aplicaciones móviles.

La nueva funcionalidad es compatible tanto con las plataformas iOS como con las Android.

## Integración de Jira {#jira-integration}

Ahora puede vincular problemas de Jira a tareas o problemas de Workfront instalando y configurando el complemento de Workfront para Jira. Con esta integración, los administradores de proyectos pueden seguir trabajando en Workfront, mientras que los ingenieros de desarrollo pueden seguir trabajando en Jira, mientras que sus elementos individuales se vinculan mediante la integración de Workfront con Jira.

Puede configurar lo siguiente mediante esta integración:

* Establezca déclencheur para que las asignaciones de Workfront creen automáticamente problemas de Jira cuando se produzcan.
* Vincule manualmente los problemas de Jira a las tareas o problemas de Workfront que se hayan creado anteriormente.
* Especifique los campos que deben sincronizarse en los elementos vinculados en cuanto uno de los elementos se actualice en una de las aplicaciones.

El complemento de Workfront estará disponible tanto para las versiones On-Premise como On-Demand de Jira. El complemento es gratuito y estará disponible para descargar en el Atlassian Marketplace a principios de marzo de 2018.

Para obtener más información sobre el complemento de Workfront para Jira, incluido un vínculo para descargarlo, consulte [Uso de Workfront con Jira.](https://support.workfront.com/hc/en-us/sections/115001130053)

## Actualización de los nombres de visualizador de revisión {#update-to-proofing-viewer-names}

Se ha cambiado el nombre del visualizador de pruebas basado en HTML 5 y del visualizador de pruebas basado en Flash en todo el sistema de Workfront. Los nombres anteriores y actualizados son los siguientes: 

| **Nombre anterior** | **Nombre actualizado** |
|---|---|
| Visor de pruebas de HTML5 | Nuevo visor de revisión |
| visor de revisión de Flash | Visualizador de revisiones heredadas |

{style="table-layout:auto"}

 Para obtener más información acerca del uso del nuevo visor de revisión, vea [Revisión de pruebas en el visor de revisión.](https://support.workfront.com/hc/en-us/sections/115000275214)

## Configurar disponibilidad de recursos y asignaciones de usuarios para calcular según el horario de usuario {#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule}

>[!NOTE]
>
>Las herramientas de programación de recursos han quedado obsoletas y se han eliminado de Workfront con la versión 23.1. Para obtener información sobre la programación de recursos mediante el Distribuidor de cargas de trabajo, consulte [Información general del Distribuidor de cargas de trabajo](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

El administrador de Workfront ahora puede determinar cómo calcula Workfront la disponibilidad de recursos y la asignación de usuarios en el nivel del sistema (teniendo en cuenta las horas y la disponibilidad de FTE). El administrador de Workfront puede configurar la disponibilidad de recursos y la asignación de usuarios para que se calculen mediante la programación predeterminada o la del usuario.

Esta configuración afecta a la disponibilidad del usuario en las siguientes circunstancias al programar recursos:

* Al permitir que Workfront asigne recursos automáticamente, como se describe en &quot;Asignar manualmente tareas y problemas no asignados en las áreas de programación&quot;.

* Al mostrar los indicadores de asignación, como se describe en &quot;Administrar asignaciones de usuarios en las áreas de programación&quot;.

Para obtener más información, consulte &quot;Configuración del modo en que Workfront calcula la disponibilidad de horas de recursos y FTE para el área de Programación&quot;.

>[!NOTE]
>
>Las herramientas de programación de recursos han quedado obsoletas y se han eliminado de Workfront con la versión 23.1. Para obtener información sobre la programación de recursos mediante el Distribuidor de cargas de trabajo, consulte [Información general del Distribuidor de cargas de trabajo](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).


## Cambio en la cadencia de sincronización al sincronizar desde el entorno de producción de revisión a vista previa {#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview}

>[!NOTE]
>
>Este cambio entra en vigor el 11 de febrero de 2018.

Los datos del entorno de producción de Workfront Proof ahora se sincronizan con el entorno de vista previa de Workfront Proof cada semana.

Antes de este cambio, los datos se sincronizaban mensualmente desde el entorno de producción de Workfront Proof al entorno de vista previa, mientras que los datos del entorno de producción de Workfront se sincronizaban semanalmente con el entorno de vista previa de Workfront. Esta discrepancia provocaba algunos errores de sincronización al utilizar la funcionalidad de revisión en el entorno de vista previa de Workfront. 

Para obtener más información, consulte [Vista previa del entorno de prueba de espacio aislado- Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md). 

## El mensaje de advertencia aparece cuando se alcanza el límite de 2000 elementos en el Planificador de recursos {#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner}

Como actualmente estamos trabajando en una solución más permanente para mejorar el rendimiento en el Planificador de recursos, hemos introducido un límite de 2000 elementos para cada vista que pueda aplicar al Planificador de recursos:

* La Vista de usuario muestra sólo 2.000 asignaciones
* La vista de proyecto muestra sólo 2.000 proyectos
* La Vista de roles muestra sólo 2.000 roles

Cuando el Planificador de recursos intenta cargar más de 2.000 elementos, aparece una notificación avisándole de que solo se pueden mostrar 2.000 elementos.

Para obtener más información sobre estos límites y cómo afectan al Planificador de recursos, consulte [Limitaciones de visualización del Planificador de recursos](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our beta program for the Resource Planner performance, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a>.</p>
-->
