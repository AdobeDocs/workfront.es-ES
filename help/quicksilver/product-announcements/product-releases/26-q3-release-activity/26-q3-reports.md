---
title: Mejoras en los informes del tercer trimestre de 2026
description: Mejoras en los informes del tercer trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: f465ac03e0ff91216d1ef934a1696127796645ba
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 1%

---

# Mejoras en los informes del tercer trimestre de 2026

Esta página describe las mejoras de los informes realizadas con la versión del tercer trimestre de 2026 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del tercer trimestre de 2026, consulte [Información general de la versión del tercer trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Valores predeterminados de solicitud de panel de lienzo y persistencia de preferencias de usuario

>[!NOTE]
>
>Vista previa: 25 de junio de 2026>Versión rápida de producción: 15 de julio de 2026>Producción para todos: 16 de julio de 2026

Para mejorar la eficacia de los usuarios que se desplazan entre paneles y registros preservando su estado de filtro de trabajo, los administradores de paneles ahora pueden definir valores de solicitud predeterminados para los paneles de lienzo. Estos valores predeterminados se aplican automáticamente a todos los visualizadores de tableros.

Cuando un usuario actualiza las solicitudes, sus selecciones se guardan y se restauran al actualizar, volver a abrir o después de navegar a un registro y volver.

Los administradores pueden restablecer el estado predeterminado del tablero en cualquier momento. Los usuarios también pueden volver rápidamente a los valores predeterminados mediante el menú de tres puntos.

Antes de esta mejora, las solicitudes del panel no tenían una preferencia de usuario predeterminada configurable o guardada para el estado de la solicitud.

Para obtener más información, consulte [Filtrar un panel de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/filter-canvas-dashboard.md).

## Añadir varios intervalos de direcciones IP de Power BI a la lista de permitidos de Data Connect a la vez

>[!NOTE]
>
>Vista previa: N/D>Versión rápida de producción: 11 de junio de 2026>Producción para todos: 16 de julio de 2026

Los administradores de Workfront que conectan Microsoft Power BI a Workfront Data Connect ahora pueden añadir un conjunto completo de intervalos de direcciones IP de Azure a la lista de permitidos en un solo paso. En la ficha **Lista de permitidos IP** de **Conexión de datos**, el botón **Nueva dirección IP** incluye ahora una opción **Agregar bloques de direcciones IP de Power BI** que abre un cuadro de diálogo en el que puede pegar las entradas de la etiqueta de servicio Power BI desde el archivo JSON de intervalos de IP de Azure y etiquetas de servicio de Microsoft publicado.

Esto reemplaza el flujo de trabajo anterior de agregar cada bloque CIDR de Power BI de uno en uno, lo que resultaba lento para las regiones que publican decenas de prefijos de dirección.

Para obtener más información, consulte [Establecer una conexión con Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).


## Ordenar la lista de paneles de lienzo

>[!NOTE]
>
>Vista previa: 11 de junio de 2026>Versión rápida de producción: 15 de julio de 2026>Producción para todos: 16 de julio de 2026
>
>Paneles de lienzo se encuentra en la versión beta.

Ahora puede ordenar la lista Paneles de lienzo por cualquiera de las siguientes columnas: **Nombre**, **Descripción**, **Creado por** o **Fecha de creación**. Haga clic en un encabezado de columna para ordenar la lista por esa columna y, a continuación, haga clic de nuevo en el mismo encabezado para invertir la dirección de ordenación. De manera predeterminada, la lista está ordenada por **Nombre** de la A a la Z. El criterio de ordenación se conserva al cambiar entre pestañas en la lista Paneles de lienzo.

Para obtener más información, consulte [Usar paneles de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md).

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

