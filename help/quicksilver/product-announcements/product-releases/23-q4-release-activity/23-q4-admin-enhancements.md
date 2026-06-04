---
title: Mejoras del administrador en el cuarto trimestre de 2023
description: Mejoras del administrador en el cuarto trimestre de 2023
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7ed37978-b821-488e-9ca1-b81825255be3
TQID: https://experienceleague.adobe.com/6-hscCn7M4UgFBhZVCsugo-ulyuFVc4nyBKKVNN3ZiM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 317
ht-degree: 97%

---

# Mejoras del administrador en el cuarto trimestre de 2023

En esta página se describen todas las mejoras en el administrador realizadas con la versión del cuarto trimestre de 2023 en el entorno de vista previa. Estas mejoras estaban disponibles en el entorno de producción con la versión 23.10.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de lanzamiento del cuarto trimestre de 2023, consulte [Información general de la versión del cuarto trimestre de 2023](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).

## Decisiones sobre pruebas y documentos disponibles para los clientes del modelo de licencia heredada

Los clientes heredados que aún no han realizado la transición al nuevo modelo de licencia de Adobe Workfront ahora pueden ver en un solo informe los datos con el número de decisiones de prueba/documento por usuario al mes. Estos datos están disponibles cuando se ejecuta un informe de Decisiones de usuarios.

Para obtener más información, vea [Explicación de los objetos en Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) y [Ver el número de decisiones de prueba y documento para todos los usuarios](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/view-number-of-decisions-for-users.md).

## Los campos calculados en formularios personalizados ahora pueden utilizar el comodín $$USER

El comodín `$$USER` ya está disponible en los campos personalizados calculados y en los campos de búsqueda externos del nuevo diseñador de formularios. La referencia a `$$USER` en un cálculo añade el identificador del usuario actual. También puede utilizar el comodín con otro campo. Por ejemplo, `$$USER.{name}` añadiría el nombre del usuario actual.

Para obtener más información sobre los campos calculados, consulte [Añadir campos calculados con el diseñador de formularios](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Añadir opciones de valor de una API externa a un formulario personalizado

Ahora hay disponible un nuevo tipo de campo, **Búsqueda externa**, en el diseñador de formularios personalizados. Cuando los datos están almacenados en un sistema externo, este tipo de campo le permite cargar opciones desde una API externa y filtrar según otros valores de campo del formulario personalizado.

Cuando se añade el formulario a un objeto, los valores devueltos por la API aparecen en un campo desplegable y el usuario puede seleccionar uno.

>[!NOTE]
>
>El nuevo tipo de campo **Búsqueda externa** no está disponible en el generador de formularios heredados.

Para obtener más información, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
