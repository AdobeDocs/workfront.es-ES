---
content-type: release-notes
keywords: notas,trimestral,actualizar,versión
navigation-topic: 2021-2-release-activity
title: 21. 2 Mejoras en los informes
description: Esta página describe todas las mejoras de creación de informes realizadas con la versión 21.2 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción la semana del 10 de mayo de 2021. Para obtener una lista de todos los cambios disponibles con la versión 21.2, consulte Información general sobre la versión 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1d5f76ef-bea7-4630-8051-454b0d109341
source-git-commit: 158af1f48fba264b98108b5f0a573b7904eb875e
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 95%

---

# 21. 2 Mejoras en los informes

Esta página describe todas las mejoras de creación de informes realizadas con la versión 21.2 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción la semana del 10 de mayo de 2021. Para obtener una lista de todos los cambios disponibles con la versión 21.2, consulte [Información general sobre la versión 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Restringir la edición de horas en proyectos e informes

Para proporcionar un mayor control sobre la edición de horas en la pestaña Horas de un proyecto y en los informes de horas, hemos añadido una configuración que permite a los administradores de Workfront restringir la edición de horas a los propietarios de horas y a los administradores del sistema.

Anteriormente, los usuarios con plantillas de horas y horas habilitadas en su nivel de acceso podían editar las horas.

Para obtener más información, consulte [Configurar preferencias de horas y hojas de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Nueva apariencia para el campo Asignaciones en listas e informes actualizados

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Para que coincida con el aspecto moderno de otras áreas en la nueva experiencia de Workfront, se ha modificado el estilo del campo Asignaciones en listas e informes actualizados. Este rediseño incluye:

* Un avatar redondeado para las imágenes de perfil de usuario, los roles y los equipos
* Se muestran las iniciales de los usuarios sin imágenes de perfil
* Un nuevo icono de función de trabajo
* Un nuevo icono Personas para asignaciones avanzadas
* Un nuevo icono de acceso restringido
* Otros cambios menores de diseño

Para obtener más información sobre las asignaciones en las listas, consulte [Asignar tareas](../../../manage-work/tasks/assign-tasks/assign-tasks.md) o [Asignar problemas](../../../manage-work/issues/manage-issues/assign-issues.md).

![](assets/assignments-updates-350x193.png)

## Nueva apariencia para los campos de escritura anticipada en listas e informes actualizados

>[!NOTE]
>
>Se eliminó temporalmente del entorno de producción el 20 de mayo de 2021.

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Para adaptarse al aspecto moderno de otras áreas en la nueva experiencia de Workfront, el estilo ha cambiado para los campos de escritura anticipada en las listas e informes actualizados. Estos cambios incluyen los siguientes:

* El icono de escritura anticipada se ha eliminado del campo.
* Al hacer clic en un campo de escritura anticipada, el menú de sugerencias ahora se muestra antes de introducir el texto.
* El menú de sugerencias es ahora más sensible a la longitud de los valores y estos valores se truncan al final cuando se alcanza el límite de caracteres, en lugar de en el medio del valor.

Para obtener información sobre las listas actualizadas, consulte la sección [La diferencia entre las listas actualizadas y las listas heredadas](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) en el artículo [Comenzar con las listas en Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

![](assets/typeahead-updates-350x336.png)

## Informar sobre actualizaciones del sistema

El nuevo informe de Entrada de cuaderno ofrece una mayor capacidad de auditoría al permitir profundizar en las actualizaciones del sistema, incluyendo:

* Cambios de estado en un proyecto, tarea o problema
* Tareas o problemas eliminados
* Valores en campos personalizados
* Fechas planificadas de finalización
* Cambios del propietario del proyecto

Por ejemplo, puede configurar este informe para mostrar la actividad en torno a un campo personalizado específico, incluyendo el proyecto del campo personalizado, cuándo se ingresó un valor por primera vez, cuál fue ese valor, cuándo se actualizó el campo, cuál era el valor anterior, cuál fue el nuevo valor ingresado, qué usuarios completaron estas acciones, etc.

Anteriormente, solo se podía informar sobre las actualizaciones del sistema a través de la API de Workfront.

Para obtener más información sobre este informe y para qué puede usarlo, consulte [Informe sobre el área de actualizaciones con un informe de entrada de diario](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

