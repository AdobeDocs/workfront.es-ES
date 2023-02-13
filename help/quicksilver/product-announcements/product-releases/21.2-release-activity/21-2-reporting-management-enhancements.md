---
content-type: release-notes
keywords: notas,trimestral,actualizar,versión
navigation-topic: 2021-2-release-activity
title: 21. 2 Mejoras en los informes
description: Esta página describe todas las mejoras de Informes realizadas con la versión 21.2 en el entorno de Vista previa. Estas mejoras estarán disponibles en el entorno de producción en la semana del 10 de mayo de 2021. Para obtener una lista de todos los cambios disponibles con la versión 21.2, consulte Información general sobre la versión 21.2.
author: Luke
feature: Product Announcements
exl-id: 1d5f76ef-bea7-4630-8051-454b0d109341
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---

# 21. 2 Mejoras en los informes

Esta página describe todas las mejoras de Informes realizadas con la versión 21.2 en el entorno de Vista previa. Estas mejoras estarán disponibles en el entorno de producción en la semana del 10 de mayo de 2021. Para obtener una lista de todos los cambios disponibles con la versión 21.2, consulte [Resumen de la versión 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Restringir la edición de horas en proyectos e informes

Para proporcionar más control sobre la edición de horas en la ficha Horas de un proyecto y de los informes de horas, hemos añadido una configuración que permite a los administradores de Workfront restringir la edición de horas a los propietarios de horas y a los administradores de sistemas.

Anteriormente, los usuarios con hojas de hora y horas habilitadas en su nivel de acceso podían editar horas.

Para obtener más información, consulte [Configuración de las preferencias de horas y horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Nuevo aspecto del campo Asignaciones en listas e informes actualizados

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Para que coincida con el aspecto moderno de otras áreas en la nueva experiencia de Workfront, el estilo ha cambiado para el campo Asignaciones en listas e informes actualizados. Este rediseño incluye:

* Un avatar redondeado para imágenes de perfil de usuario, roles de trabajo y equipos
* Se muestran las iniciales de los usuarios sin imágenes de perfil
* Un nuevo icono de función de trabajo
* Un nuevo icono Personas para asignaciones avanzadas
* Un nuevo icono de acceso restringido
* Otros cambios menores en el diseño

Para obtener más información sobre las asignaciones en listas, consulte [Asignación de tareas](../../../manage-work/tasks/assign-tasks/assign-tasks.md) o [Asignación de problemas](../../../manage-work/issues/manage-issues/assign-issues.md).

![](assets/assignments-updates-350x193.png)

## Nuevo aspecto y presentación de los campos typeforward en listas e informes actualizados

>[!NOTE]
>
>Eliminado temporalmente del entorno de producción el 20 de mayo de 2021.

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Para que coincida con el aspecto moderno de otras áreas en la nueva experiencia de Workfront, el estilo ha cambiado para los campos de tipo de avance en las listas e informes actualizados. Estos cambios incluyen:

* El icono Typeforward se ha eliminado del campo .
* Al hacer clic en un campo de tipo &quot;delante&quot;, ahora se muestra el menú de sugerencias antes de escribir texto.
* El menú de sugerencias es más adaptable a la longitud de los valores y estos valores ahora se truncan al final cuando se alcanza el límite de caracteres en lugar de en medio del valor.

Para obtener información sobre listas actualizadas, consulte la [La diferencia entre las listas actualizadas y las listas heredadas](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) sección del artículo [Introducción a las listas en Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

![](assets/typeahead-updates-350x336.png)

## Informar sobre actualizaciones del sistema

El nuevo informe Entrada de diario le ofrece una buena auditabilidad al permitirle explorar en profundidad las actualizaciones del sistema, entre las que se incluyen:

* Cambios de estado en un proyecto, tarea o problema
* Tareas o problemas eliminados
* Valores de campos personalizados
* Fechas de finalización previstas
* Cambios en el propietario del proyecto

Por ejemplo, puede configurar este informe para que muestre la actividad alrededor de un campo personalizado específico, incluido el proyecto para el campo personalizado, cuándo se introdujo por primera vez un valor, qué era ese valor, cuándo se actualizó el campo, cuál era el valor anterior, cuál era el valor recién introducido, qué usuarios completaron estas acciones, etc.

Anteriormente, solo se podía informar sobre las actualizaciones del sistema a través de la API de Workfront.

Para obtener más información sobre este informe y para qué puede utilizarlo, consulte [Informe del área Actualizaciones](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

