---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión beta 2 de 2018.2
description: Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión beta 2 de 2018.2. La funcionalidad se publicó en el entorno de vista previa el 5 de abril de 2018. Estará disponible en el entorno de producción en junio de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: c8ef68f5-53db-4c3c-af0f-e1c98521ec27
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Actividad de la versión beta 2 de 2018.2

Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión beta 2 de 2018.2. La funcionalidad se publicó en el entorno de vista previa el 5 de abril de 2018. Estará disponible en el entorno de producción en junio de 2018.

>[!IMPORTANT]
>
> La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción de.

Para ver una lista de todos los cambios realizados en 2018.2, consulte  [información general sobre la actividad de la versión 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

La versión beta 2 de 2018.2 incluye las siguientes mejoras:

* [Editar campos directamente desde el área de inicio](#edit-fields-directly-from-the-home-area)
* [Registrar tiempo en días](#log-time-in-days)
* [Ver relaciones de predecesoras entre proyectos en el gráfico Gantt en una lista de proyectos](#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects)
* [Uso de Costes Presupuestados en Portfolio Optimizer para Calcular Finanzas de Portfolio](#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances)
* [Informe Utilización: Rellena las horas presupuestadas desde el nuevo área de presupuesto de recursos](#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area) (Solo vista previa)

* [Informe Utilización: Ver Horas Presupuestadas por Usuario en un Proyecto](#utilization-report-view-budgeted-hours-by-user-on-a-project) (Solo vista previa)

* [Progreso de revisión de la lista de documentos disponible para usuarios sin revisión](#proof-progress-from-the-document-list-available-to-non-proofing-users)
* [Mejoras de Mobile](#mobile-improvements)

## Editar campos directamente desde el área de inicio {#edit-fields-directly-from-the-home-area}

Ahora, al seleccionar un objeto en el área de Inicio, puede editar los campos asociados a ese objeto directamente desde el panel derecho del área de Inicio. 

Antes de este cambio, la información solo se podía ver en el área de Inicio, no editarse.

Para obtener más información, consulte la [Actualizar o editar un elemento de trabajo en el área de Inicio](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md) en el artículo  [Actualizar o editar un elemento de trabajo en el área de Inicio](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).

## Registrar tiempo en días {#log-time-in-days}

Los administradores de Workfront ahora pueden configurar si los usuarios de su organización registran el tiempo en días u horas. Los usuarios con una licencia de Planner pueden configurar esta opción por sí mismos.

Antes de este cambio, los usuarios solo podían registrar las horas en horas.

Puede configurar esta opción editando el perfil de usuario. Para obtener más información, consulte [Configurar si se registran horas y días](../../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

Para obtener información sobre cómo los usuarios pueden registrar el tiempo en días después de actualizar esta configuración, consulte [Registrar tiempo](../../../../timesheets/create-and-manage-timesheets/log-time.md).

## Ver relaciones de predecesoras entre proyectos en el gráfico Gantt en una lista de proyectos {#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects}

Ahora puede ver las relaciones de predecesoras entre proyectos en el diagrama de Gantt en las siguientes listas de proyectos:

* La pestaña Proyectos dentro de un portafolio o programa
* En un informe de proyecto

Antes de este cambio, las relaciones predecesoras entre proyectos solo se podían ver para tareas individuales en el nivel de proyecto.

Para obtener más información, consulte [Configurar cómo se muestra la información en el gráfico Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 

## Uso de Costes Presupuestados en Portfolio Optimizer para Calcular Finanzas de Portfolio {#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances}

El nuevo Optimizador de Portfolio ahora utiliza el Coste Presupuestado de la nueva área de Presupuestación de Recursos del Caso Comercial o del Planificador de Recursos para calcular los siguientes campos:

* Valor neto
* Retorno de la inversión (ROI)
* Costo

Anteriormente, tanto el Optimizador de Portfolio nuevo como el anterior utilizaban el Coste presupuestado de legado. El Optimizador de Portfolio heredados sigue utilizando el coste presupuestado heredado para calcular el valor neto, el rendimiento de la inversión y el coste.

También hemos añadido dos nuevos campos a los campos financieros de Portfolio: ROI heredado y Valor neto heredado para capturar los nuevos valores de las nuevas herramientas de administración de recursos.

Para obtener más información, consulte [Información general de Portfolio Optimizer](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md) en el artículo  [Información general de Portfolio Optimizer](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## Informe Utilización: Rellena las horas presupuestadas desde el nuevo área de presupuesto de recursos {#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area}

>[!NOTE]
>
>Esta funcionalidad no se incluirá en la versión oficial del entorno de vista previa con la versión 2018.2. Se volverá a introducir durante el período beta para la versión 2018.3 y se lanzará al entorno de producción con la versión 2018.3. 

Las horas presupuestadas en el informe de utilización ahora se rellenan a partir de la información disponible en la nueva área de Presupuestación de recursos del caso comercial.

Antes de este cambio, se utilizaba la información del área Estimaciones de recursos de legado.

Para obtener más información, consulte [Descripción general del informe Utilización de los recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) en el artículo  [Descripción general del informe Utilización de los recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Informe Utilización: Ver Horas Presupuestadas por Usuario en un Proyecto {#utilization-report-view-budgeted-hours-by-user-on-a-project}

>[!NOTE]
>
>Esta funcionalidad no se incluirá en la versión oficial del entorno de vista previa con la versión 2018.2. Se volverá a introducir durante el período beta para la versión 2018.3 y se lanzará al entorno de producción con la versión 2018.3. 

El informe Utilización de un proyecto ahora muestra las horas presupuestadas por usuario.

Antes de este cambio, el informe Utilización mostraba solo las horas presupuestadas por rol. 

Para obtener más información, consulte [Descripción general del informe Utilización de los recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) en el artículo [Descripción general del informe Utilización de los recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Progreso de revisión de la lista de documentos disponible para usuarios sin revisión {#proof-progress-from-the-document-list-available-to-non-proofing-users}

Los indicadores de progreso de prueba (Enviado, Abierto, Comentarios realizados y Decisión) ahora se muestran para todos los usuarios al ver la lista de documentos. Esto incluye a los usuarios que no pueden generar pruebas (para obtener más información sobre cómo permitir que los usuarios generen pruebas, consulte la sección .

Antes de este cambio, los indicadores de progreso de prueba solo estaban disponibles para los usuarios que podían generar pruebas.

Para obtener más información, consulte [Progreso de prueba e información general de estado](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md).

## Mejoras de Mobile {#mobile-improvements}

La aplicación móvil incluye las siguientes mejoras:

* Los vínculos compartidos con usted en otras aplicaciones móviles ahora se abren en la aplicación móvil de Workfront.

  Para obtener más información sobre cómo compartir vínculos, consulte .

  Esta actualización ya está disponible en iOS y Android.

* Hemos actualizado nuestros requisitos de soporte para la plataforma iOS para admitir iPhone X.

  Para obtener más información acerca de los dispositivos móviles y sistemas operativos compatibles, consulte . 
