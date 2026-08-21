---
title: Mejoras en los informes del cuarto trimestre de 2026
description: Mejoras en los informes del cuarto trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: a86f0169f804520be2828983a737c8c8d151792d
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 5%

---

# Mejoras en los informes del cuarto trimestre de 2026

Esta página describe las mejoras de los informes realizadas con la versión del cuarto trimestre de 2026 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del cuarto trimestre de 2026, consulte [Información general de la versión del cuarto trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

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
