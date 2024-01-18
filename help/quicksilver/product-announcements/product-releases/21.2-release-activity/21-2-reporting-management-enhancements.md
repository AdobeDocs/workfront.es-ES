---
content-type: release-notes
keywords: notas, trimestral, actualizar, versión
navigation-topic: 2021-2-release-activity
title: 21. 2 Mejoras en los informes
description: Esta página describe todas las mejoras de creación de informes realizadas con la versión 21.2 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción el 10 de mayo de 2021. Para obtener una lista de todos los cambios disponibles con la versión 21.2, consulte Información general de la versión 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1d5f76ef-bea7-4630-8051-454b0d109341
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# 21. 2 Mejoras en los informes

Esta página describe todas las mejoras de creación de informes realizadas con la versión 21.2 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción el 10 de mayo de 2021. Para obtener una lista de todos los cambios disponibles con la versión 21.2, consulte [21.2 Información general de la versión](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Restringir la edición de horas en proyectos e informes

Para proporcionar más control sobre la edición de horas en la pestaña Horas de un proyecto e informes de Horas, hemos agregado una configuración que permite a los administradores de Workfront restringir la edición de horas a los propietarios de horas y a los administradores del sistema.

Anteriormente, los usuarios con hojas de horas y horas habilitadas en su nivel de acceso podían editar las horas.

Para obtener más información, consulte [Configurar preferencias de horas y hojas de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Nueva apariencia para el campo Asignaciones en listas e informes actualizados

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Para que coincida con el aspecto moderno de otras áreas en la nueva experiencia de Workfront, el estilo ha cambiado para el campo Asignaciones en listas e informes actualizados. Este rediseño incluye:

* Un avatar redondeado para las imágenes de perfil de usuario, los roles y los equipos
* Se muestran las iniciales de los usuarios sin imágenes de perfil
* Un nuevo icono de rol
* Un nuevo icono Personas para asignaciones avanzadas
* Un nuevo icono de acceso restringido
* Otros cambios menores de diseño

Para obtener más información sobre las asignaciones en listas, consulte [Asignar tareas](../../../manage-work/tasks/assign-tasks/assign-tasks.md) o [Asignar problemas](../../../manage-work/issues/manage-issues/assign-issues.md).

![](assets/assignments-updates-350x193.png)

## Nueva apariencia para los campos de escritura anticipada en listas e informes actualizados

>[!NOTE]
>
>Se eliminó temporalmente del entorno de producción el 20 de mayo de 2021.

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Para adaptarse al aspecto moderno de otras áreas en la nueva experiencia de Workfront, el estilo ha cambiado para los campos de escritura anticipada en las listas e informes actualizados. Estos cambios incluyen:

* El icono de escritura anticipada se ha eliminado del campo.
* Al hacer clic en un campo de escritura anticipada, el menú de sugerencias ahora se muestra antes de introducir el texto.
* El menú de sugerencias responde mejor a la longitud de los valores, que ahora se truncan al final cuando se alcanza el límite de caracteres en lugar de en medio del valor.

Para obtener información sobre las listas actualizadas, consulte [La diferencia entre las listas actualizadas y las heredadas](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) en el artículo [Introducción a las listas en Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

![](assets/typeahead-updates-350x336.png)

## Informar sobre actualizaciones del sistema

El nuevo informe Entrada de cuaderno ofrece una mayor capacidad de auditoría al permitirle explorar en profundidad las actualizaciones del sistema, entre las que se incluyen las siguientes:

* Cambios de estado en un proyecto, tarea o problema
* Tareas o problemas eliminados
* Valores en campos personalizados
* Fechas planificadas de finalización
* Cambios del propietario del proyecto

Por ejemplo, puede configurar este informe para mostrar la actividad en torno a un campo personalizado específico, incluido el proyecto del campo personalizado, cuándo se introdujo un valor por primera vez, cuál era ese valor, cuándo se actualizó el campo, cuál era el valor anterior, cuál era el valor introducido recientemente, qué usuarios completaron estas acciones, etc.

Anteriormente, solo se podía informar sobre las actualizaciones del sistema a través de la API de Workfront.

Para obtener más información sobre este informe y para qué puede utilizarlo, consulte [Informe sobre el área de Actualizaciones](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

