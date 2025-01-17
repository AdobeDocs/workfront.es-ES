---
title: Mejoras del administrador en el primer trimestre de 2025
description: Mejoras del administrador en el primer trimestre de 2025
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: fa24040d-0403-4799-b690-c3d172797115
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 21%

---

# Mejoras del administrador en el primer trimestre de 2025

Esta página describe todas las mejoras de administrador realizadas con la versión del primer trimestre de 2025 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del primer trimestre de 2025, consulte [Información general de la versión del primer trimestre de 2025](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md).

## Ahora se admiten reglas de negocio para más objetos

>[!NOTE]
>
>Versión preliminar: 16 de enero de 2025; versión de producción para todos los clientes: con la versión 25.1 (enero de 2025)
>
>_Solo disponible para organizaciones en el plan Ultimate._

Ahora puede crear reglas de negocio y aplicar la validación a estos objetos adicionales: compañía, iteración, categoría de recurso no laboral, rol, usuario, asignación, conjunto de recursos, tiempo libre, documento y hora.

Los objetos siguientes ya eran compatibles con las reglas de negocio: Proyecto, Tarea, Solicitud, Portfolio, Programa, Gasto, Registro de facturación, Grupo, Riesgo y Tarjeta de tarifa.

Para obtener más información, consulte [Crear y editar reglas empresariales](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).

## Comparar objetos entre entornos para la promoción de entornos

>[!NOTE]
>
>Versión preliminar: 6 de enero de 2025; versión de producción para todos los clientes: con la versión 25.1 (enero de 2025)

Para facilitar la determinación de qué objeto debe incluirse en un paquete de promoción de entorno, se ha añadido la capacidad de comparar objetos entre entornos. Ahora puede seleccionar tipos de objetos y entornos. Workfront genera una lista de objetos de ese tipo, independientemente de si están presentes en el entorno de destino y de si ese objeto tiene diferencias entre el entorno de origen y el entorno de destino. A continuación, puede añadir objetos a un paquete directamente desde esta lista.

Anteriormente, si un usuario quería comparar objetos entre entornos, debía comprobar manualmente esos objetos.

Para obtener más información, vea [Comparar objetos entre entornos](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-compare.md).

## Más objetos disponibles para la promoción del entorno

>[!NOTE]
>
>Versión preliminar: 6 de enero de 2025; versión de producción para todos los clientes: con la versión 25.1 (enero de 2025)

Para ampliar las capacidades de la funcionalidad de promoción del entorno, hemos agregado más objetos. Ahora, puede agregar los siguientes objetos a un paquete de promoción de entorno:

* Ubicaciones
* Tarjetas de tarifas
* Asignaciones

Anteriormente, estos objetos no estaban disponibles para la promoción del entorno.

Para obtener más información sobre los objetos disponibles para la promoción del entorno, consulte [Objetos admitidos para la promoción del entorno](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion) en el artículo Información general sobre la promoción del entorno.

## Impedir mover tareas cuando hay horas registradas

>[!NOTE]
>
>Versión de vista previa: 19 de diciembre de 2024; versión de producción para todos los clientes: con la versión 25.1 (16 de enero de 2025)

Debido a que mover tareas o problemas que han registrado horas a veces puede causar problemas de cumplimiento o auditoría, hemos agregado una preferencia en el área de Preferencias de tarea y problemas de la Configuración que le permite evitar que los usuarios muevan tareas y problemas si hay horas registradas en ellos. Antes de esta mejora, los usuarios podían mover tareas y problemas a otros proyectos, incluso si se habían registrado horas en ellos.

Para obtener más información, consulte [Configurar las preferencias de tareas y problemas de todo el sistema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Preferencia para utilizar la programación de proyecto o de usuario para tareas de asignación única

>[!NOTE]
>
>Versión preliminar: viernes, 21 de noviembre de 2024; producción para la versión rápida: con la versión 24.12 (viernes, 12 de diciembre de 2024); producción para versión trimestral: con la versión 25.1 (viernes, 16 de enero de 2025)

Como administrador de sistemas o de grupos, ahora tiene una nueva preferencia que indica si Workfront debe utilizar la programación del proyecto o la del usuario para calcular la escala de tiempo del proyecto cuando asigna un usuario a una tarea y tanto el proyecto como el usuario están asociados a una programación. Antes de esta mejora, esta configuración existía para asignaciones de varios usuarios. La configuración ahora está disponible para asignaciones de un solo usuario a tareas.

Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Las reglas empresariales ahora admiten hipervínculos

>[!NOTE]
>
>Versión preliminar: viernes, 21 de noviembre de 2024; producción para la versión rápida: con la versión 24.12 (viernes, 12 de diciembre de 2024); producción para versión trimestral: con la versión 25.1 (viernes, 16 de enero de 2025)

Ahora puede incluir hipervínculos en el mensaje de error personalizado de una regla de negocio para guiar al usuario sobre cómo modificar su acción dentro de la restricción de la regla. La URL estática podría vincularse a la documentación u otras páginas que resultarían útiles para el usuario.

Para obtener más información, consulte [Crear y editar reglas de negocio](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).

## Ya está disponible el filtrado en los campos de escritura anticipada nativos

>[!NOTE]
>
>Versión preliminar: viernes, 21 de noviembre de 2024; producción para la versión rápida: con la versión 24.12 (viernes, 12 de diciembre de 2024); producción para versión trimestral: con la versión 25.1 (viernes, 16 de enero de 2025)

Cuando se agrega una referencia de campo nativo a un formulario personalizado y hace referencia a un campo de escritura anticipada (como Portfolio, Empresa o Propietario), ahora está disponible una opción de filtro. El filtro permite limitar los objetos que los usuarios pueden elegir cuando utilizan el campo. Este filtro personalizado funciona igual que un filtro en un campo de escritura anticipada personalizado, utilizando el modo de texto para definir el filtro.

Para obtener más información, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Icono &quot;Mover a&quot; añadido a los campos personalizados

>[!NOTE]
>
>Versión de vista previa: miércoles, 29 de octubre de 2024; producción para versión rápida: con la versión 24.11 (viernes, 14 de noviembre de 2024); producción para versión trimestral: con la versión 25.1 (viernes, 16 de enero de 2025)

Cuando un formulario personalizado contiene varias secciones con muchos campos, puede resultar difícil mover un campo de una sección a otra arrastrando y soltando. Se ha agregado un icono &quot;mover a&quot; a cada campo, que le permite seleccionar la sección en la que se coloca el campo.

Para obtener más información, vea [Organizar y obtener una vista previa de un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).
