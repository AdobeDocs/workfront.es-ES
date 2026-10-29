---
content-type: release-notes
title: Actividad de la versión del primer trimestre de 2027 para Adobe Workfront Planning
description: Esta es la actividad de lanzamiento del producto Adobe Workfront Planning para el primer trimestre de 2027.
author: Becky
feature: Product Announcements
role: Admin
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
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 949503fecba92a7b8536b4af0b9c684e7f9e3300
workflow-type: tm+mt
source-wordcount: '1082'
ht-degree: 3%
---
# Actividad de la versión del primer trimestre de 2027 para Adobe Workfront Planning

Este artículo describe las funciones que se lanzarán para Workfront Planning durante la versión del primer trimestre de 2027.

Para obtener una lista de todas las características publicadas para Adobe Workfront Planning, consulte [Actividad de la versión de Adobe Workfront Planning: índice de artículo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Mejor visibilidad de los resultados de búsqueda rápida en la vista de tabla

>[!NOTE]
>
>Vista previa: 29 de octubre de 2026
>Versión rápida de producción: 12 de noviembre de 2026
>Producción para todos: 21 de enero de 2027

Cuando se utiliza la búsqueda rápida en la vista de tabla para encontrar un elemento, la vista elimina todos los registros que no coinciden con la búsqueda y muestra sólo los elementos que coinciden.

Antes de esta mejora, todos los registros se mostraban con los que coincidían con los resultados de búsqueda resaltados.

Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

<!--

## Record-level permissions - restricted access to records

PLACEHOLDER: The release note field on the Workfront task points to an anchor story that no longer exists, so there is no description yet. Add the description and help link before unhiding.

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

-->

## Permitir la conexión de registros de tipos de registros globales conectados en espacios de trabajo secundarios cuando la conectividad entre espacios de trabajo está desactivada

>[!NOTE]
>
>Vista previa: 29 de octubre de 2026
>Versión rápida de producción: 12 de noviembre de 2026
>Producción para todos: 21 de enero de 2027

Cuando se agregan dos tipos de registros globales conectados a un espacio de trabajo secundario, ahora puede desactivar la conectividad entre espacios de trabajo y seguir vinculando registros localmente. Cada espacio de trabajo secundario sólo ve sus propios registros para ambos tipos de registro y puede conectarlos entre sí. Ya no se muestran los registros del espacio de trabajo global ni de otros espacios de trabajo secundarios.

Antes de esta mejora, si la conectividad entre espacios de trabajo se desactivaba para los tipos de registros globales conectados, los espacios de trabajo secundarios no podían vincular sus propios registros entre sí. Si estaba activado, los usuarios podían ver y vincular registros del espacio de trabajo global y de todos los demás espacios de trabajo secundarios.

Para obtener más información, vea [Información general sobre el tipo de registro entre espacios de trabajo](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

## Ver el recuento total de registros en las vistas de tabla

>[!NOTE]
>
>Vista previa: 29 de octubre de 2026
>Versión rápida de producción: 12 de noviembre de 2026
>Producción para todos: 21 de enero de 2027

La vista de tabla ahora muestra el número total de registros y el recuento se actualiza automáticamente al aplicar filtros, buscar o cambiar la vista. El recuento de registros siempre refleja los resultados filtrados completos y respeta los permisos.

Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

<!--

## Field aggregators available for groupings in the table view

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

Grouped records in the table views now show a summary row for each grouping, plus a grand total for the full table. Groupings and the grand total use the same summary functions, and nested groupings get their own summaries that include all child records. Aggregators update automatically as you filter, search, regroup, or edit records.

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).

## Add sections to organize Planning views

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

You can now create sections in the Workfront Planning View dropdown menu to organize related views as your list grows. You can name each section when you create it, then move views from My Views and Shared with Me into your custom sections. System views stay fixed in the System section.

For information, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md).

-->

<!--

## Filters for Workfront objects connected record fields

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

You can now filter for certain Workfront object types that meet a filter criteria when you add them as a connected field in Planning.

Only those Workfront objects that meet your filtering criteria will display as options in connected fields when editing a record.

For this feature, we added a new Record filtering rules option in the New connection tab when connecting the following Workfront object types: projects, portfolios, programs, groups, companies. Prior to this enhancement, filters were available only when connecting two record types.

For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

-->

## Limitaciones de número de campo de búsqueda

>[!NOTE]
>
>Vista previa: 29 de octubre de 2026
>Versión rápida de producción: 12 de noviembre de 2026
>Producción para todos: 21 de enero de 2027

Se están introduciendo límites en cuanto a la cantidad de campos de búsqueda que se pueden agregar a un tipo de registro:

* Hasta 40 campos de búsqueda por tipo de registro
* Hasta 5 campos de búsqueda de texto largo por tipo de registro. Los campos de búsqueda conectados se contabilizan en el límite de su campo original.
* Hasta 50 000 caracteres en el valor de una sola celda de búsqueda de texto largo. Si el contenido combinado de los valores de búsqueda supera este límite, los valores se muestran en orden de conexión hasta que se alcanza el límite. Se omiten el primer valor que lo excedería y todos los valores posteriores. El campo de objeto conectado original nunca cambia.

Recibirá un error cuando intente crear o editar un campo de búsqueda más allá de los dos primeros límites. Los tipos de registros que ya superan estos límites no se ven afectados por este cambio. Puede editarlos, pero no puede agregar más campos de búsqueda o valores hasta que esté por debajo del límite.

Para obtener más información, consulte [Información general sobre limitaciones de objetos de Planificación de Workfront de Adobe](/help/quicksilver/planning/general/limitations-overview.md).

## Los nuevos campos ahora aparecen únicamente en la vista donde los crea

>[!NOTE]
>
>Vista previa: 29 de octubre de 2026
>Versión rápida de producción: 12 de noviembre de 2026
>Producción para todos: 21 de enero de 2027

Al agregar un nuevo campo a un tipo de registro, ahora sólo se muestra en la vista en la que está trabajando y se oculta en todas las demás vistas existentes. Otras vistas permanecen como están configuradas y puede mostrar el nuevo campo en ellas, si es necesario.

Antes de esta mejora, se añadían nuevos campos que se mostraban en todas las vistas, lo que a veces causaba confusión a los usuarios que no estaban familiarizados con los nuevos campos.

Para obtener más información, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

## Exportar detalles de registro desde cualquier vista

>[!NOTE]
>
>Vista previa: 29 de octubre de 2026
>Versión rápida de producción: 12 de noviembre de 2026
>Producción para todos: 21 de enero de 2027

Ahora puede exportar los detalles de un registro desde cualquier vista de detalles, sin tener que cambiar a la vista Todos los campos.

Anteriormente, la opción de exportación solo estaba disponible cuando se seleccionaba la vista Todos los campos.

Para obtener más información, vea [Exportar los detalles de un registro](/help/quicksilver/planning/records/export-the-record-page.md).

<!--

## Cancel and revert changes when editing records when business rules are violated

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

To ensure data integrity, when a business rule is violated while you edit a record, the change is blocked, the value reverts, and a toast notification explains why the edit is not allowed. The warning is visible in all areas where you are editing records, including the table view or details page.

If multiple rules are violated, each violation issues its own toast notification.

For more information, see [Configure business rules](/help/quicksilver/planning/architecture/configure-business-rules.md).

-->

## Rendimiento mejorado con la carga de datos incremental en las vistas de tabla y cronología

<!-- NOTE FROM CSV: Must check with Lilit whether this will come to the timeline view in addition to the table (Lilit said yes; this was messaged before but pulled). The second bullet will change; check with Lilit first. -->

>[!NOTE]
>
>Vista previa: 29 de octubre de 2026
>Versión rápida de producción: 12 de noviembre de 2026
>Producción para todos: 21 de enero de 2027

Para mejorar el rendimiento en un gran número de registros, hemos realizado las siguientes mejoras en las vistas de tabla y cronología:

* La vista ahora carga los 500 primeros registros inicialmente, con registros adicionales cargados automáticamente a medida que se desplaza por lotes de 500.
* La búsqueda rápida y la agrupación solo afectan a los registros cargados actualmente en la vista.

Para obtener más información, vea [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md) y [Administrar la vista de escala de tiempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).

<!--

## Additional permissions for users other than requestors to submitted requests

>[!NOTE]
>
>Preview: October 28, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

Workspace managers can now define what access to submitted requests users other than requestors have.

By editing the Permissions area of a request form, you can define additional access for other users to requests submitted using the form.

You can grant permissions to workspace users or any other users, groups, teams, job roles or companies in the system. Once defined in the request queue, the permissions are granted automatically when the request is submitted, and any permission changes apply only to new requests.

Prior to this enhancement, you could only grant permissions to requestors.

For information, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

-->

## Reordenación manual de la agrupación en la vista de cronología

>[!NOTE]
>
>Vista previa: 29 de octubre de 2026
>Versión rápida de producción: 12 de noviembre de 2026
>Producción para todos: 21 de enero de 2027

Ahora puede arrastrar y soltar agrupaciones, subagrupaciones y registros para crear un orden personalizado en la vista de cronología. La organización manual se conserva en todas las sesiones y puede cambiar sin problemas entre la ordenación manual y la ordenación basada en el campo a medida que cambian las necesidades de planificación.

La funcionalidad de arrastrar y soltar está disponible tanto para las calles como para las versiones apiladas de la vista de cronología.

Para obtener más información, consulte [administrar la vista de cronología](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Reglas empresariales para tipos de registros globales

>[!NOTE]
>
>Vista previa: 28 de octubre de 2026
>Versión rápida de producción: 12 de noviembre de 2026
>Producción para todos: 21 de enero de 2027

Los administradores de Workspace ahora pueden configurar reglas empresariales en tipos de registro global tanto en los espacios de trabajo principales como en los secundarios. Las reglas se aplican a todos los registros del mismo tipo en todos los espacios de trabajo en los que se agregan.

Las reglas de negocio agregadas en espacios de trabajo globales se muestran como de solo lectura en espacios de trabajo secundarios donde se importaron los tipos de registro. Las reglas de negocio agregadas en espacios de trabajo secundarios se muestran como de solo lectura en los espacios de trabajo principales donde se crearon originalmente los tipos de registro. Las reglas solo se pueden editar en los espacios de trabajo en los que se crean.

Para obtener más información, consulte [Configurar reglas empresariales de tipo de registro](/help/quicksilver/planning/architecture/configure-business-rules.md).

## Establecer la configuración de solicitud predeterminada para la funcionalidad Rellenar formulario en solicitudes de Planning

>[!NOTE]
>
>Vista previa: 21 de octubre de 2026
>Versión rápida de producción: 12 de noviembre de 2026
>Producción para todos: 21 de enero de 2027

Ahora puede personalizar el mensaje que ven los usuarios al utilizar la capacidad de formulario Rellenar con tecnología de IA al enviar una solicitud de Planning.

Puede crear una solicitud predeterminada al crear un formulario de solicitud para solicitudes de Planning.

Para obtener más información, consulte [Crear y administrar un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
