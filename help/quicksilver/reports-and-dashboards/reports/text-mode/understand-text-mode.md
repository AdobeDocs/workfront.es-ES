---
product-area: reporting
navigation-topic: text-mode-reporting
title: Información general sobre el modo de texto
description: Puede crear un informe o una lista en Adobe Workfront utilizando la interfaz de modo estándar o de modo de texto al crear los elementos que conforman el informe o la lista.
author: Nolan
feature: Reports and Dashboards
exl-id: 8be8cbd0-da1b-4e90-a52e-dc352f646d18
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 88%

---

# Información general sobre el modo de texto

<!-- Audited: 1/2025 -->

<!--(NOTE: Linked to the UI (for the areas mentioned in the comments below and the new NWE filters as well))-->

<!--(NOTE: Alina: ***Linked to other articles. Do not move, rename or change url.Linked to the product, in the report builder, when using a field that is not recognized in standard mode.)-->

<!--(NOTE: This will be linked to the Ninja feature about adding a filter to the User typeahead field (which originally is open only for text mode filters). Update the Context Sensitive sheet at release time)-->

Puede crear un informe o una lista en Adobe Workfront utilizando la interfaz de modo estándar o de modo de texto al crear los elementos que conforman el informe o la lista.

La interfaz estándar permite hacer referencia a campos y sus atributos que están disponibles en la interfaz de Workfront.

Con el modo de texto puede hacer referencia a campos y atributos que puede que no estén disponibles en el modo estándar, pero que están disponibles en la base de datos de Workfront.

Para obtener más información sobre la creación de informes con el modo de texto, incluidas clases, vídeos y tutoriales, consulte la sección de aprendizaje en el sitio de Adobe Experience League.

## Consideraciones antes de utilizar el modo de texto

>[!TIP]
>
>También puede ampliar las posibilidades de los campos personalizados calculados utilizando una versión del modo texto para los campos personalizados. La sintaxis y las reglas para crear un campo personalizado calculado son diferentes de las que se usan en informes y listas. Para obtener información sobre cómo añadir un campo personalizado calculado, consulte [Añadir campos calculados a un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

* Antes de empezar a usar el modo de texto en los informes, le recomendamos encarecidamente que tome nuestras clases sobre informes avanzados para comprender mejor nuestro lenguaje del modo de texto.
* Le recomendamos que utilice el modo estándar para garantizar que los informes que crea permanezcan intactos cuando se actualice el software de Workfront. Aunque el modo de texto le permite crear vistas, filtros y agrupaciones más complejos, también es más complicado de mantener y no hay ninguna garantía cuando se actualiza el software de Workfront.
* Le recomendamos que siempre intente crear todos los elementos de creación de informes en la interfaz estándar y cambiar al generador de modo de texto solo para algunos ajustes.

  >[!TIP]
  >
  >El uso del generador estándar le proporciona bloques de creación y patrones de código importantes que puede utilizar al modificar el código en modo de texto.

* Hay un conjunto de reglas y una sintaxis única que debe utilizar para generar correctamente informes y listas en modo de texto. Antes de comenzar, asegúrese de estar familiarizado con la sintaxis de Workfront para el modo de texto.

  Para obtener información sobre la sintaxis y las reglas para usar el modo de texto, consulte [Resumen de sintaxis de en modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

* Después de personalizar un elemento de creación de informes en el modo de texto, es posible que no pueda volver al modo estándar (en una vista) o que se elimine el código del elemento que ha creado (en filtros y agrupaciones). Esto se debe a que no todos los campos compatibles con el modo de texto son compatibles con el modo estándar.

## Interfaz de modo estándar

La interfaz del modo estándar muestra campos para asignar los elementos de la aplicación que desea mostrar en un informe o una lista. La interfaz de modo estándar es un conjunto de menús desplegables desde los que puede seleccionar los campos que desea mostrar en sus informes o listas.

Para obtener más información sobre la interfaz de modo estándar y aprender a crear un informe o una lista, consulte lo siguiente:

* [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
* [Elementos para la creación de informes: filtros, vistas y agrupaciones](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)

## Interfaz de modo de texto

El modo de texto permite crear vistas, filtros, agrupaciones y solicitudes más complejas, y así utilizar campos que no están disponibles en la interfaz del modo estándar. En Workfront, el modo de texto es una colección de instrucciones codificadas que indican qué objetos desea mostrar en un informe o una lista.

Para obtener una lista completa de todos nuestros campos sobre los que se puede realizar informes, consulte el [Explorador de API](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>No todos los campos disponibles a través de la API están disponibles a través de la interfaz de modo de texto. Si utiliza el campo correcto en el código de modo de texto y no muestra los resultados esperados, es posible que el campo solo se pueda registrar a través de la API.

## Acceder a los elementos para la creación de informes y al modo de edición de texto {#access-reporting-elements-and-edit-text-mode}

El acceso a la interfaz de modo de texto es similar para vistas, agrupaciones y filtros al acceder a ellos desde un informe o una lista.

Para obtener información sobre el uso del modo de texto en vistas, filtros y agrupaciones, consulte:

* [Editar una vista usando el modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
* [Editar un filtro mediante el modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
* [Edición de una agrupación mediante el modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

Las indicaciones personalizadas solo se pueden editar en modo de texto. Solo puede acceder a las indicaciones desde un informe.

Para obtener información sobre el acceso a la interfaz de modo de texto para las indicaciones personalizadas, consulte [Añadir una indicación a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Razones habituales para utilizar el modo de texto {#common-reasons-to-use-text-mode}

Además de crear indicaciones personalizadas que solo se pueden configurar mediante el modo de texto, le recomendamos que utilice Report Builder para crear sus vistas, filtros y agrupaciones. Sin embargo, hay algunos casos en los que puede utilizar el modo de texto para mejorar los informes y las listas.

Para obtener más información sobre los usos comunes del modo de texto, vea [Información general sobre los usos comunes del modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
