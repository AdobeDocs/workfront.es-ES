---
title: Mejoras en los informes del cuarto trimestre de 2026
description: Mejoras en los informes del cuarto trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
source-git-commit: 3599b27bb1b838ebe7d0a2648e6c67333da83dc8
workflow-type: tm+mt
source-wordcount: '1434'
ht-degree: 5%
---
# Mejoras en los informes del cuarto trimestre de 2026

Esta página describe las mejoras de los informes realizadas con la versión del cuarto trimestre de 2026 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del cuarto trimestre de 2026, consulte [Información general de la versión del cuarto trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

## Los paneles de lienzo ya están disponibles en Google Cloud Platform y Microsoft Azure

>[!NOTE]
>
>Vista previa: N/D
>Versión rápida de producción: 14 de octubre de 2026
>Producción para todos: 15 de octubre de 2026

Las instancias de Workfront en Google Cloud Platform (GCP) y Azure ahora pueden adherirse a la versión beta abierta de paneles de lienzo. Para obtener más información, consulte [Usar paneles de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md).

## Registre un anuncio privado de Snowflake para Workfront Data Connect

>[!NOTE]
>
>Vista previa: N/D
>Versión rápida de producción: 14 de octubre de 2026
>Producción para todos: 15 de octubre de 2026

Ahora puede compartir los datos de Workfront Data Connect directamente con la cuenta de Snowflake de su organización registrando un anuncio privado. Este método de conexión utiliza la capacidad de listado privado de Snowflake para compartir datos de forma segura entre organizaciones sin exponerlos públicamente, y funciona en varias regiones y plataformas de alojamiento.

Un anuncio privado resulta útil cuando desea unir los datos de Workfront con otros datos del almacén de datos empresarial. Como los datos aterrizan en su propia cuenta de Snowflake, puede consultarlos junto con el resto de los datos.

Para obtener más información, consulte [Registrar un anuncio privado para Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/register-a-private-listing.md).

## Herramientas de MCP de creación de informes ahora disponibles para paneles de lienzo

>[!NOTE]
>
>Vista previa: 1 de octubre de 2026
>Versión rápida de producción: 14 de octubre de 2026
>Producción para todos: 15 de octubre de 2026

Para facilitar el uso de paneles de lienzo, hemos agregado herramientas al MCP de Workfront. Ahora puede crear y administrar paneles de lienzo a través del chat y el panel y los widgets se crean para usted con sus datos de Workfront. Esto funciona con clientes de MCP como Claude y Cursor.

Por ejemplo, puede realizar lo siguiente:

* Cree informes preguntando. Describa un tablero o un gráfico en lenguaje natural en lugar de crearlo manualmente.
* Edite en su lugar. Pida que se cambie el nombre de un widget, cambie un filtro, cambie un tipo de gráfico o cambie el tamaño, y los cambios se aplican al tablero activo.
* Reutilice lo que tiene. Duplique un tablero o widget existente como punto de partida en lugar de volver a compilar desde cero.

### Funciones compatibles

**Paneles de control**

* Crear un nuevo tablero
* Enumere sus tableros (los suyos, compartidos con usted, todos o favoritos) y busque por título
* Abrir o ver la estructura de un panel
* Actualizar título, descripción, moneda, filtros y peticiones de datos
* Duplique un tablero (con o sin sus widgets, indicadores y filtros)
* Eliminación de un panel de control

**Widgets**

* KPI: un solo número agregado (suma, promedio, recuento, mínimo, máximo, etc.)
* Gráfico: gráfico de barras, columnas, líneas y circulares; admite gráficos simples, de varias series y apilados
* Tabla: tablas de varias columnas con agrupación de filas
* Ver la configuración de un widget y actualizarla, copiarla, cambiarla de tamaño, cambiarla de posición o eliminarla

**Opciones de informes**

* Filtrado de datos con condiciones y grupos AND/OR
* Agrupar y agregar por cualquier campo
* Profundizar desde un KPI o gráfico en los registros subyacentes
* Etiquetas de columna personalizadas, formato de número, fecha y moneda y estilo de celda condicional
* Mensajes y filtros de nivel de panel

Para obtener más información, consulte [Usar paneles de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md).

## Copiar o mover widgets entre paneles de lienzo

>[!NOTE]
>
>Vista previa: 1 de octubre de 2026
>Versión rápida de producción: 14 de octubre de 2026
>Producción para todos: 15 de octubre de 2026

Ahora puede copiar un widget en el mismo tablero, en otro tablero al que tenga acceso de edición o en un tablero nuevo. También puede mover un widget a otro tablero al que tenga acceso de edición o a un tablero nuevo.

Al copiar un widget, ahora se abre un cuadro de diálogo en el que se selecciona el panel de destino y se especifica si se copia o se mueve el widget. Anteriormente, el Report Builder se abría de inmediato.

## Filtrar por relaciones de colección en paneles de lienzo

>[!NOTE]
>
>Vista previa: 1 de octubre de 2026
>Versión rápida de producción: 14 de octubre de 2026
>Producción para todos: 15 de octubre de 2026

Cuando se crea un filtro en un panel de lienzo, ahora se puede filtrar por relaciones de colección, que son campos que se vinculan a un grupo de registros relacionados en lugar de a un único registro. Por ejemplo, puede filtrar el estado de las tareas que pertenecen a un proyecto para mostrar una lista de proyectos que tienen tareas en el estado &quot;Nuevo&quot;.

Anteriormente, el filtrado en relaciones de colección requería un modo de texto.

Para obtener más información, consulte [Referencia del filtro de informes para paneles de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/filter-reference.md).

## Copia de paneles en paneles de lienzo

>[!NOTE]
>
>Vista previa: 3 de septiembre de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

Ahora puede copiar un panel de lienzo usando la nueva acción **Copiar panel**. Esta acción está disponible para cualquier usuario cuyo nivel de acceso conceda derechos de edición o creación a los paneles, aunque solo tenga acceso de visualización al panel específico que se está copiando. Los usuarios sin derechos de edición o creación en los paneles no ven esta acción.

Al copiar un tablero, puede cambiarle el nombre, actualizar su descripción y su moneda y elegir qué widgets, filtros de tablero y peticiones de datos de tablero desea transferir a la copia.

Las configuraciones de Ejecutar como usuario en widgets solo se conservan si es el usuario designado o un administrador del sistema. Las preferencias de uso compartido no se copian en el nuevo tablero, y se muestra un mensaje de confirmación con un vínculo al nuevo tablero una vez completada la copia.

Anteriormente, no había forma de copiar un tablero; los usuarios tenían que reconstruir los tableros desde cero para crear variaciones específicas para la audiencia.

## Campo Tipo de aprobación en paneles de lienzo

>[!NOTE]
>
>Producción para todos: 28 de agosto de 2026
>[!BADGE Fuera del horario]{type=Neutral}

La entidad Approval ahora incluye un campo **Tipo de aprobación**, que permite a los usuarios distinguir entre aprobaciones de prueba, aprobaciones de versión de documento, aprobaciones de admisión y otros tipos de aprobación.

## Actualización de terminología de aprobación en paneles de lienzo

>[!NOTE]
>
>Producción para todos: 28 de agosto de 2026
>[!BADGE Fuera del horario]{type=Neutral}

Se ha cambiado el nombre de los siguientes campos utilizados en paneles de lienzo para aprobaciones de documentos y trabajos para una mayor claridad:

| Nombre anterior | Nuevo nombre |
| --- | --- |
| Aprobación de documento | Aprobación |
| Fase de aprobación del documento | Fase de aprobación |
| Participante de la fase de aprobación del documento | Participante de fase de aprobación |
| Proceso de aprobación | Proceso de aprobación de trabajo |
| Fase de aprobación | Fase de aprobación de trabajo |
| Estado de la aprobación | Estado del aprobador del trabajo |
| Esperando aprobación | Esperando aprobación de trabajo |

Este cambio no afecta al funcionamiento de los informes actuales.

## Informes de tabla dinámica en paneles de lienzo

>[!NOTE]
>
>Vista previa: 27 de agosto de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

El nuevo tipo de informe de tabla dinámica de los paneles de lienzo agrega datos con resúmenes precisos y completos. Puede crear métricas como recuentos, sumas y promedios directamente en el panel y, a continuación, explorar en profundidad los registros subyacentes detrás de cualquier total.

Para obtener más información, consulte [Crear un informe de tabla dinámica en un panel de lienzo](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-pivot-table-report.md).

## Aplicar fechas de finalización a los informes programados

>[!NOTE]
>
>Vista previa: 13 de agosto de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

Los informes programados ahora requieren una fecha de finalización para evitar una entrega indefinida. Las programaciones que pasan su fecha de finalización se desactivan automáticamente.

Las programaciones existentes se han actualizado con fechas de finalización para mejorar la fiabilidad y reducir el uso innecesario del sistema. Workfront también proporciona visibilidad y advertencias agregadas para ayudarle a administrar los ciclos de vida de las programaciones de informes a medida que se aproximan a su fecha de finalización.

Para obtener más información, consulte [Programar una entrega automática de informes](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

## Los campos de referencia nativos están disponibles para listas e informes

>[!NOTE]
>
>Vista previa: 30 de julio de 2026
>Versión rápida de producción: 13 de agosto de 2026
>Producción para todos: 15 de octubre de 2026

Ahora puede agregar campos de referencia nativos a listas e informes en Workfront.

Un campo de referencia nativo es un campo personalizado. Cuando el campo se encuentra en un formulario personalizado adjunto a un objeto, el campo se rellena a partir de los datos del objeto. Por ejemplo, si el campo hace referencia al campo Descripción y se encuentra en un formulario personalizado adjunto a un proyecto, extrae la descripción del proyecto. (Puede que el campo muestre &quot;N/D&quot; si no hay datos disponibles).

Para obtener información sobre cómo crear campos de referencia nativos, incluida la lista de campos nativos admitidos, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
Para obtener información sobre cómo agregar campos a los informes, consulte [Crear un informe personalizado](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Ordenación coherente de los valores de campos de selección múltiple en listas e informes heredados

>[!NOTE]
>
>Vista previa: 30 de julio de 2026
>Versión rápida de producción: 13 de agosto de 2026
>Producción para todos: 15 de octubre de 2026

Ahora verá las opciones seleccionadas para campos personalizados de selección múltiple en un orden coherente y predecible en listas e informes heredados. El orden de los campos viene determinado por la forma en que se organizan los campos en el formulario personalizado.

![El orden de los campos de formulario personalizados coincide con el orden de los valores seleccionados en una lista o informe](assets/new-field-order-multi-select.png)

Anteriormente, las opciones seleccionadas se mostraban en el orden en el que se elegían o en un orden incoherente, lo que dificultaba el análisis y la comparación de filas.

Nota: La nueva ordenación no se aplica si el campo utiliza el modo de texto.
