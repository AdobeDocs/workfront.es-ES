---
title: Mejoras del administrador en el primer trimestre de 2026
description: Mejoras del administrador en el primer trimestre de 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: a524dd5519f450543e486d83bff6134a15f548d7
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 13%

---

# Mejoras del administrador en el primer trimestre de 2026

Esta página describe las mejoras realizadas por el administrador con la versión del primer trimestre de 2026 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del primer trimestre de 2026, consulte [Información general de la versión del primer trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Administrar prioridades en la plantilla de diseño

>[!NOTE]
>
>Esta función no está disponible temporalmente en el entorno de vista previa
>Vista previa: 2 de diciembre de 2025
>Versión rápida de producción: 14 de enero de 2026
>Producción para todos: 15 de enero de 2026


Ahora puede habilitar o deshabilitar las prioridades para usuarios específicos en la plantilla de diseño. Si anteriormente tenía las prioridades deshabilitadas para su organización, permanecerá deshabilitada en la plantilla de diseño con este cambio.

Las prioridades se incluirán automáticamente para los tipos de licencia que tienen acceso predeterminado a las solicitudes. Por ejemplo, una licencia de colaborador verá Solicitudes, Tableros y Prioridades de forma predeterminada en el Menú principal, mientras que una licencia externa solo verá Documentos y Tableros porque no tiene acceso para ver o enviar solicitudes.


Para obtener más información, consulte [Personalizar el menú principal con una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

## Comprobar conflictos de varios formularios para campos personalizados calculados

>[!NOTE]
>
>Vista previa: 18 de diciembre de 2025
>Versión rápida de producción: 14 de enero de 2026
>Producción para todos: 15 de enero de 2026

El mismo campo calculado puede tener diferentes fórmulas cuando se adjunta a diferentes formularios personalizados. Si dos o más formularios que contienen el mismo campo calculado están adjuntos a un objeto, las fórmulas deben ser idénticas en todos los formularios. No se permite editar la fórmula si el cambio podría provocar un conflicto.

Para proporcionar visibilidad sobre los objetos que pueden verse afectados al editar una expresión en campos personalizados, se ha añadido una opción para comprobar si hay conflictos. Este cuadro de diálogo muestra todos los objetos que pueden verse afectados por el cambio de la fórmula, agrupados por tipo de objeto. Puede desplazarse a los detalles de cada objeto y revisar los campos para decidir si el campo se debe quitar de cualquiera de los formularios o la expresión debe permanecer sin cambios.

Para obtener más información, consulte [Añadir campos calculados a un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).


## Fecha de entrada e ID de Introducido por almacenado en objetos personalizados

>[!NOTE]
>
>Vista previa: 13 de noviembre de 2025
>Versión rápida de producción: 13 de noviembre de 2025
>Producción para todos: 13 de noviembre de 2025

La fecha de entrada y el ID introducido ahora se almacenan en formularios, campos y secciones personalizados. Puede utilizar estas opciones de datos en los informes como filtros, vistas o agrupaciones. Para mostrarlos en la lista de formularios, campos o secciones personalizados en la configuración, agregue Fecha de entrada e Introducido por: Nombre como columnas en una vista nueva o existente.

>[!NOTE]
>
>La fecha de entrada y las entradas introducidas por ID solo están disponibles en formularios, campos y secciones personalizados creados el 13 de noviembre de 2025 o posteriormente.

## Actualizaciones de los nombres de los botones al editar una plantilla de diseño

>[!NOTE]
>
>Vista previa: 30 de octubre de 2025
>Versión rápida de producción: 13 de noviembre de 2025
>Producción para todos: 15 de enero de 2026

Para proporcionar más coherencia con otras áreas de la configuración, como el diseñador de formularios personalizados, los botones que ve al editar una plantilla de diseño han cambiado a **Aplicar**, **Guardar y cerrar** y **Cancelar**. La nueva opción, **Aplicar**, le permite guardar los cambios realizados en la plantilla de diseño y seguir editando. Anteriormente, las opciones disponibles eran **Guardar** y **Cancelar**.

Para obtener más información, consulte [Crear y administrar plantillas de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Administración de campos mejorada con el indicador Activo en los campos personalizados

>[!NOTE]
>
>Vista previa: 30 de octubre de 2025
>Versión rápida de producción: 13 de noviembre de 2025
>Producción para todos: 15 de enero de 2026

Cuando hay un gran número de campos personalizados en el sistema, la administración de esos campos en formularios e informes personalizados puede resultar difícil. Ahora puede marcar los campos personalizados como inactivos con la nueva marca **Active**. Este indicador está disponible cuando se trabaja con un campo en un formulario personalizado o cuando se agrega o edita un campo de la lista Campos.

Si marca un campo como inactivo:

* Se excluye de los informes, filtros, vistas u otros lugares de Workfront donde puede agregar un campo personalizado
* No está disponible en la biblioteca de campos para agregarlo a otros formularios personalizados

>[!NOTE]
>
>Si se marca un campo existente como inactivo, no estará disponible para su uso en elementos de informes y formularios personalizados a partir de ese momento. Si el campo inactivo se utiliza actualmente en un informe o un formulario, el campo y sus datos históricos permanecen en su lugar.

Para obtener más información, consulte [Adición o edición de campos personalizados, saltos de sección o widgets](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/edit-a-custom-field.md).




