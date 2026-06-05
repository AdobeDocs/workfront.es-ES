---
title: Mejoras en los informes del tercer trimestre de 2026
description: Mejoras en los informes del tercer trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: b9c63e1ca4b2b301ee104ee84151a2d0148a8cea
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 3%

---

# Mejoras en los informes del tercer trimestre de 2026

Esta página describe las mejoras de los informes realizadas con la versión del tercer trimestre de 2026 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del tercer trimestre de 2026, consulte [Información general de la versión del tercer trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Cambios en las horas reales en fórmulas personalizadas

>[!NOTE]
>
>Vista previa: 1 de junio de 2026>Versión rápida de producción: 1 de junio de 2026>Producción para todos: 1 de junio de 2026

En 2025, se agregó un nuevo campo Horas reales a la base de datos de Workfront como `actualWorkRequiredDouble`, y el campo Horas reales existente (`actualWorkRequired` en la base de datos) cambió el nombre de Horas reales heredadas. Consulte la [nota de la versión](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-project-enhancements.md) para obtener más información.

En junio de 2026, las fórmulas personalizadas existentes que usaban `actualWorkRequired` (Horas reales heredadas) se migraron para usar `actualWorkRequiredDouble` (Horas reales) en su lugar. `actualWorkRequired` ya no se puede usar en cálculos y fórmulas.

Además, se recomienda encarecidamente usar `actualWorkRequiredDouble` en todos los informes.

Al reemplazar el campo, tenga en cuenta que `actualWorkRequired` almacena valores en minutos, mientras que `actualWorkRequiredDouble` almacena valores en horas con precisión decimal.

Para obtener más información sobre las horas reales, vea [Ver horas reales](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md).

## Campos de datos de moneda personalizados en informes de Panel de lienzo

>[!NOTE]
>
>Vista previa: 28 de mayo de 2026>Versión rápida de producción: 11 de junio de 2026>Producción para todos: 16 de julio de 2026

Los informes del panel de lienzo ahora admiten campos de datos de moneda personalizados como columnas, filtros, agrupaciones y agregaciones, incluso cuando se configuran varias tasas de cambio en Configuración del sistema. Cuando un campo de datos de moneda personalizado se muestra como una columna o agregación, los valores se convierten a la moneda seleccionada en la opción de tasa de cambio del panel, a menos que el campo esté bloqueado en el nivel de informe.

Ahora se procesan los informes que anteriormente fallaban con un mensaje de &quot;campo restringido&quot; después de agregar una segunda moneda de tipo de cambio. Los campos de moneda de planificación permanecen restringidos cuando se definen varios tipos de cambio.

Para obtener más información, consulte [Usar campos monetarios en paneles de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/switch-currencies.md).

## Precisión de datos mejorada en los informes del panel de lienzo

>[!NOTE]
>
>Vista previa: 14 de mayo de 2026>Versión rápida de producción: 11 de junio de 2026>Producción para todos: 16 de julio de 2026
>
>Paneles de lienzo se encuentra en la versión beta.

Los paneles de lienzo ahora estructuran las consultas de informes para evitar filas duplicadas cuando los filtros o campos cruzan registros relacionados, de modo que los recuentos, las sumas y otros agregados devuelven valores precisos.

Anteriormente, una unión entre registros relacionados podía repetir los registros principales una vez para cada registro relacionado. Por ejemplo, en un informe de proyecto filtrado a tareas asignadas a un usuario específico, cada proyecto se repite una vez por cada tarea coincidente. Un KPI que sumara el presupuesto del proyecto podría mostrar 6000 $ en lugar de los 1250 $ correctos.

No hay cambios en la interfaz del panel Lienzo. Los informes existentes devuelven automáticamente datos precisos después de esta versión.