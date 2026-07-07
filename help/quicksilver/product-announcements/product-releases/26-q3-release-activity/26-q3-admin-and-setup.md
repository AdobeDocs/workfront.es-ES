---
title: Mejoras del administrador en el tercer trimestre de 2026
description: Mejoras del administrador en el tercer trimestre de 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: d83d823426b42202e83cb4db64f85d27d4dca0bb
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 9%

---

# Mejoras del administrador en el tercer trimestre de 2026

Esta página describe las mejoras realizadas por el administrador con la versión del tercer trimestre de 2026 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del tercer trimestre de 2026, consulte [Información general de la versión del tercer trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Seguimiento de cambios para revisión y aprobación unificadas

>[!NOTE]
>
>Vista previa: 7 de julio de 2026Versión rápida de producción: 15 de julio de 2026Producción para todos: 16 de julio de 2026

La página Historial de cambios de Workfront ahora captura la actividad en los flujos de trabajo unificados de revisión y aprobación, lo que proporciona a los administradores un registro de control completo para los eventos de ciclo vital de revisión y documento.

Ahora se realiza un seguimiento de las acciones de aprobación, fase y participante. Estas acciones pueden incluir:

* Toma de una decisión de aprobación en el visor Frame.io
* Creación o eliminación de una aprobación
* Actualizar un documento, como cambiarle el nombre, moverlo o eliminarlo

Cada entrada incluye los campos rastreados estándar: fecha y hora, operación, nombre de usuario (o &quot;generado por el sistema&quot;) y nombre de objeto. No se incluyen los comentarios del visor de Frame.io.

Esta fase del seguimiento de cambios no incluye eventos MCP. Formarán parte de una versión futura.

Para obtener más información, vea [Ver y administrar el historial de cambios](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

<!--

## Internal lookup field replacing Typeahead field type

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

The new **Internal lookup** field type in custom forms provides dynamic filtering. It is similar to the Typeahead field type and allows users to search and select existing Workfront objects by typing part of the name. The filter on the internal lookup can reference the value in another field on the form, which is not possible with Typeaheads.

Multi-select is supported on internal lookups, and this field type also provides improved performance for large datasets. The following native Workfront objects are supported in internal lookups: Project, Company, Group, Job Role, Portfolio, Program, Team, Template, User, Task, Issue, Document, and Location.

The Internal lookup field type is replacing the Typeahead field type. You can quickly convert existing Typeahead fields to Internal lookups by clicking the button in the field options on the right. When you convert, historical data remains on the field and it is used the same way in reports.

>[!IMPORTANT]
>
>External integrations such as Workfront Fusion scenarios or API-based automations may reference legacy field structures and require updates after the conversion. You should verify any integrations before converting Typeahead fields to Internal lookup fields.

For more information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

-->

<!--

## Default value logic supported on native reference fields

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026
>
>This feature is only available for organizations on the Workflow Prime or Ultimate packages.

In custom forms, native reference fields now allow you to add default value logic.

This logic type on native reference fields is available only in the user interface and not in the Workfront API.

For information, see [Add default value logic to a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md#add-default-value-logic-to-a-custom-form) in the article [Add logic rules to custom forms and fields](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

-->

<!--

## Updates to native field filtering in custom forms

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

System filters that exist on native fields are now applied to the fields in custom forms and are visible to administrators.

When you add a native reference field that has a system filter applied, you can apply the same filter to the field in the custom form and modify the filter if needed in the Text Mode box.

Adding your own custom filter to the field overrides the system filter for the field. If you do not enter a custom filter, the system filter is applied by default.

Also, dynamic filtering is now available on native reference fields. A dynamic filter allows you to narrow the list of items based on the value of another field.

For example, when you use `?portfolioID={portfolio}.{ID}` in a Project field filter and a Portfolio native field is on the custom form, the Project field shows only projects that are in the selected portfolio. If the Portfolio field is left blank, then all projects are available in the Project field.

For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

-->

<!--

## Protect field names from accidental renaming

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

To protect integrations and data integrity, we've updated how field names can be edited in the field settings panel of a custom form.

Field names in the field settings panel are now read-only by default. You can still edit the field name, but renaming requires an explicit confirmation step. The field previously called **Name** has also been updated to **API Name** to better reflect its technical significance. The **Label** field remains editable.

For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#notes-on-field-names-and-labels).

-->

## Ver el historial de cambios de los objetos de Workfront

>[!NOTE]
>
>Vista previa: 11 de junio de 2026Versión rápida de producción: 11 de junio de 2026Producción para todos: 16 de julio de 2026

Para facilitarle la visualización de los cambios que se han producido en una lista central, hemos creado la lista Historial de cambios. Esta lista muestra información como el objeto, la operación y el origen del cambio (como un usuario o el sistema de Workfront).

Anteriormente, los registros de auditoría estaban disponibles, pero no cubrían los objetos.

Para obtener más información, vea [Ver y administrar el historial de cambios](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

## Nueva preferencia del sistema para convertir portafolios de almacenamiento heredado al almacenamiento en la nube de Adobe

>[!NOTE]
>
>Vista previa: 11 de junio de 2026Producción para todos: 11 de junio de 2026

Los administradores de Workfront ahora pueden convertir portafolios de almacenamiento heredado al almacenamiento en la nube de Adobe directamente desde Preferencias del sistema. Para convertir portafolios, selecciónelos en el nuevo campo Select portfolios to convert to enterprise storage y guarde la página.

Cuando un portafolio se convierte en almacenamiento en la nube de Adobe:

* Ya no puede mover proyectos que utilicen el almacenamiento de Workfront heredado a este portafolio
* Todos los nuevos proyectos creados en este portafolio utilizan el almacenamiento en la nube de Adobe
* Frame.io es el visor de documentos que utilizan el almacenamiento en la nube de Adobe
* Los objetos secundarios que utilizan el almacenamiento heredado de Workfront permanecen en el almacenamiento heredado

Anteriormente, al agregar un proyecto de almacenamiento en la nube de Adobe a una cartera de almacenamiento heredado, esta se convertía automáticamente en almacenamiento en la nube de Adobe.

Para obtener más información, consulte [Configurar las preferencias del sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Texto se sustitución enriquecido con tipo de campo de formato

>[!NOTE]
>
>Vista previa: 28 de mayo de 2026Versión rápida de producción: 11 de junio de 2026Producción para todos: 16 de julio de 2026

El nuevo tipo de campo **Texto enriquecido** de los formularios personalizados es un editor de texto robusto con opciones de formato como superíndice y subíndice, encabezados y tablas, además de las opciones tradicionales de negrita, cursiva, subrayado, viñetas, numeración, hipervínculos y comillas de bloque. El límite de caracteres sigue siendo de 15 000.

El tipo de campo Texto enriquecido reemplaza el tipo de campo Texto con formato. Puede convertir rápidamente el texto existente con campos de formato a texto enriquecido haciendo clic en el botón de las opciones de campo a la derecha. Al realizar la conversión, los datos históricos permanecen en el campo y se utilizan del mismo modo en los informes.

>[!IMPORTANT]
>
>Las integraciones externas, como los escenarios de Workfront Fusion o las automatizaciones basadas en API, pueden hacer referencia a estructuras de campo heredadas y requerir actualizaciones después de la conversión. Debe verificar cualquier integración antes de convertir los campos a texto enriquecido.

Para obtener más información, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Campos financieros nativos admitidos en los formularios personalizados

>[!NOTE]
>
>Vista previa: 28 de mayo de 2026Versión rápida de producción: 11 de junio de 2026Producción para todos: 16 de julio de 2026

Ahora puede incluir campos financieros nativos de Workfront en formularios personalizados. Anteriormente, los campos financieros no eran compatibles.

Los campos financieros disponibles a los que se puede hacer referencia dependen del tipo de formulario.

Para obtener más información, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-workfront-native-fields).

## Los formularios personalizados se pueden compartir en todo el sistema con acceso para adjuntarlos

>[!NOTE]
>
>Vista previa: 28 de mayo de 2026Versión rápida de producción: 11 de junio de 2026Producción para todos: 16 de julio de 2026

Se ha agregado una nueva opción de uso compartido, &quot;Todas las personas del sistema pueden ver y adjuntar&quot;, a los formularios personalizados. Al seleccionar esta opción, todos los usuarios de todo el sistema pueden adjuntar el formulario a otros objetos.

Al compartir en todo el sistema, se elimina la necesidad de compartir manualmente formularios y actualizar los permisos entre grupos u agencias cuando se agregan nuevos grupos.

Para obtener más información, consulte [Compartir un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## Nueva preferencia del sistema para aplicar campos obligatorios en la edición por lotes

>[!NOTE]
>
>Vista previa: 28 de mayo de 2026Versión rápida de producción: 11 de junio de 2026Producción para todos: 16 de julio de 2026

Actualmente, cuando se editan objetos por lotes, los campos obligatorios solo se aplican cuando un usuario modifica el campo. Si un campo no se modifica, se trata como opcional y no se valida.

Una nueva preferencia del sistema ahora le permite aplicar los campos obligatorios en la edición masiva. Para no permitir que se guarden objetos editados en lotes a menos que todos los campos obligatorios tengan valores, seleccione la opción **Aplicar siempre los campos obligatorios en la edición en lotes** en la página Configuración > Sistema > Preferencias.

Para obtener más información, consulte [Configurar las preferencias del sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).
