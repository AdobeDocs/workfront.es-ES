---
title: Mejoras del administrador del cuarto trimestre de 2023
description: Mejoras del administrador del cuarto trimestre de 2023
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7ed37978-b821-488e-9ca1-b81825255be3
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# Mejoras del administrador del cuarto trimestre de 2023

Esta página describe todas las mejoras de administrador realizadas con la versión del cuarto trimestre de 2023 en el entorno de vista previa. Estas mejoras estaban disponibles en el entorno de producción con la versión 23.10 de.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del cuarto trimestre de 2023, consulte [Información general de la versión del cuarto trimestre de 2023](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).

## Decisiones de pruebas y documentos disponibles para los clientes del modelo de licencia heredado

Los clientes heredados que aún no han realizado la transición al nuevo modelo de licencia de Adobe Workfront ahora pueden ver en un solo informe los datos con el número de decisiones de prueba/documento por usuario al mes. Estos datos están disponibles cuando se ejecuta un informe de decisiones de usuarios.

Para obtener más información, vea [Comprender los objetos de Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) y y [Ver el número de decisiones sobre pruebas y documentos de todos los usuarios](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/view-number-of-decisions-for-users.md).

## Los campos calculados en formularios personalizados ahora pueden utilizar el comodín $$USER

El comodín `$$USER` ya está disponible en los campos personalizados calculados y en los campos de búsqueda externos del nuevo diseñador de formularios. La referencia a `$$USER` en un cálculo agrega el identificador del usuario actual. También puede utilizar el comodín con otro campo. Por ejemplo, `$$USER.{name}` agregaría el nombre del usuario actual.

Para obtener más información sobre los campos calculados, consulte [Agregar campos calculados con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Añadir opciones de valor de una API externa a un formulario personalizado

Ahora hay disponible un nuevo tipo de campo, **búsqueda externa**, en el diseñador de formularios personalizados. Cuando los datos están almacenados en un sistema externo, este tipo de campo le permite cargar opciones desde una API externa y filtrar según otros valores de campo del formulario personalizado.

Cuando se agrega el formulario a un objeto, los valores devueltos por la API aparecen en un campo desplegable y el usuario puede seleccionar uno.

>[!NOTE]
>
>El nuevo tipo de campo **Búsqueda externa** no está disponible en el generador de formularios heredado.

Para obtener más información, vea [Diseñar un formulario con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
