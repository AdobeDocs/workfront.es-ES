---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión 2017.3 de Beta 3
description: La versión 2017.3 estará disponible en el entorno de producción a principios de noviembre de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: dc0cada8-4b9e-40cb-89a5-16f15268b513
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 6%

---

# Actividad de la versión 2017.3 de Beta 3

La versión 2017.3 estará disponible en el entorno de producción a principios de noviembre de 2017.

>[!IMPORTANT]
>
> La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción de.

Para ver una lista de todos los cambios realizados en 2017.3, consulte  [Resumen de la actividad de la versión 2017.3](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md).

La versión 2017.3 de Beta 3 contiene mejoras para todos los usuarios:

* [Personalizar colores para gráficos](#customize-chart-colors)
* [Opciones Adicionales Al Copiar Proyectos](#additional-options-when-copying-projects)
* [Mejora del Planificador de recursos: Filtros](#resource-planner-improvement-filters)
* [Mejora del Planificador de recursos: mostrar las horas del problema en el área de &quot;configuración&quot;](#resource-planner-improvement-show-issue-hours-in-the-settings-area)
* [La información de SSO para las zonas protegidas de actualización y vista previa personalizadas no se actualiza](#sso-information-for-the-custom-refresh-and-preview-sandboxes-do-not-refresh)
* [Requisitos actualizados de compatibilidad del explorador para Workfront Proof](#updated-browser-support-requirements-for-workfront-proof)

## Personalizar colores de gráfico {#customize-chart-colors}

Ahora puede personalizar los colores de los elementos de los gráficos. Esto se aplica a todos los tipos de gráficos de los informes. Esto no se aplica al gráfico Gantt.

Antes de este cambio, los colores de los elementos de todos los gráficos se seleccionaban de forma predeterminada en Workfront. Para obtener más información sobre cómo personalizar los colores del gráfico, vea las secciones &quot;Personalizar colores del gráfico&quot; en [Agregar un gráfico a un informe](../../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

## Opciones Adicionales Al Copiar Proyectos {#additional-options-when-copying-projects}

Ahora, al copiar un proyecto, las opciones ahora coinciden con las que están disponibles al copiar tareas o problemas. También puede cambiar el estado del proyecto copiado mientras lo está copiando.

Antes de esta actualización, no se podía cambiar el estado del proyecto copiado durante su copia y solo había dos opciones disponibles al copiar un proyecto:

* Para conservar asignaciones en tareas y el proyecto
* Para conservar el progreso de las tareas y proyectos

Con la nueva funcionalidad, se han eliminado las opciones anteriores y se han añadido las siguientes opciones al copiar un proyecto:

* Borrar asignaciones
* Borrar información financiera
* Borrar progreso
* Borrar aprobaciones
* Borrar datos personalizados
* Borrar notificaciones de recordatorio
* Borrar documentos
* Borrar los gastos
* Borrar todas las predecesoras
* Borrar permisos
* Seleccionar todo

Para obtener más información sobre la nueva funcionalidad relacionada con la copia de proyectos, consulte la sección &quot;Copia de un proyecto en el entorno de vista previa&quot; en   [Copiar un proyecto](../../../../manage-work/projects/manage-projects/copy-project.md).

## Mejora del Planificador de recursos: Filtros {#resource-planner-improvement-filters}

Ahora puede filtrar la información que ve en el Planificador de recursos por los siguientes objetos:

* Portafolio
* Estado del proyecto
* Equipo
* Función
* Conjunto de recursos

También puede agregar un filtro personalizado basado en estos objetos.

Para obtener más información sobre el uso del Planificador de recursos, consulte [Resumen del Planificador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md). 

## Mejora del Planificador de recursos: mostrar las horas del problema en el área de &quot;Configuración&quot; {#resource-planner-improvement-show-issue-hours-in-the-settings-area}

Hay una nueva área de Configuración en el Planificador de recursos que muestra varias opciones para personalizar el Planificador de recursos. Con esta versión, hemos añadido la primera opción, incluir las horas planificadas de los problemas en las columnas Horas planificadas del Planificador de recursos.

Para obtener más información sobre el uso del Planificador de recursos, consulte [Resumen del Planificador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## La información de SSO para las zonas protegidas de actualización y vista previa personalizadas no se actualiza {#sso-information-for-the-custom-refresh-and-preview-sandboxes-do-not-refresh}

A partir de esta versión, cuando actualice los entornos limitados de actualización y vista previa personalizadas, la información de SSO no se copia del entorno de producción ni se desactiva. Antes de este cambio, la información de SSO de las zonas protegidas de actualización y vista previa personalizadas se deshabilitaba y se establecía en &quot;Ninguno&quot;.

Para obtener más información sobre el entorno de espacio aislado de actualización personalizado, consulte [El entorno de espacio aislado de actualización personalizado de Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

Para obtener más información sobre el entorno de vista previa de espacio aislado, consulte [El entorno de espacio aislado de vista previa de Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

## Requisitos actualizados de compatibilidad del explorador para Workfront Proof {#updated-browser-support-requirements-for-workfront-proof}

Se han actualizado los requisitos de compatibilidad del explorador para Workfront Proof. Para obtener más información, consulte [Requisitos del explorador Adobe Workfront](../../../../workfront-basics/workfront-browser-requirements.md).
