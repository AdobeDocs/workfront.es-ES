---
content-type: release-notes
title: Actividad de la versión del cuarto trimestre de 2025 para Adobe Workfront Planning
description: Esta es la actividad de lanzamiento del producto Adobe Workfront Planning para el cuarto trimestre de 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 4e1761f9-bf73-4355-925a-9136f2787a3f
source-git-commit: f7dcae5e6bcc8674ef37ef94282c50dc9ffe951d
workflow-type: tm+mt
source-wordcount: '900'
ht-degree: 9%

---

# Actividad de la versión del cuarto trimestre de 2025 para Adobe Workfront Planning

Este artículo describe las funciones que se lanzarán para Workfront Planning durante el cuarto trimestre de 2025.

<!--keep the sentence below for all future quarterly release pages-->

Para obtener una lista de todas las características publicadas para Adobe Workfront Planning, consulte [Actividad de la versión de Adobe Workfront Planning: índice de artículo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Nuevos límites para los campos de fórmula

>[!NOTE]
>
>* Vista previa: 28 de agosto de 2025
>* Versión rápida de producción: 11 de septiembre de 2025
>* Producción para todos los clientes: viernes, 16 de octubre de 2025

Hemos colocado los siguientes límites en los campos de fórmula:

* Hay un límite de 20 campos de fórmula por tipo de registro
* Hay un límite de 50 000 caracteres para una expresión de fórmula

Para obtener más información, vea [Descripción general del campo de fórmula](/help/quicksilver/planning/fields/formula-fields.md).

## Mostrar error cuando no se pueden resolver los valores de la fórmula

>[!NOTE]
>
>* Vista previa: 28 de agosto de 2025
>* Versión rápida de producción: 11 de septiembre de 2025
>* Producción para todos los clientes: viernes, 16 de octubre de 2025

Para indicar que hay un problema para resolver un campo de fórmula, el campo ahora se mostrará como &quot;#ERROR!&quot; en uno de los casos siguientes:

* Cuando se elimina un campo utilizado en una fórmula.

* Cuando un campo utilizado en un campo de búsqueda agregado se muestra como #ERROR!.

* Cuando un valor de fórmula no se puede mostrar en el formato seleccionado.

Para obtener más información, vea [Información general sobre los campos de fórmula](/help/quicksilver/planning/fields/formula-fields.md).

## Nuevas expresiones agregadas a los campos de fórmula en Planning

>[!NOTE]
>
>Vista previa: 7 de agosto de 2025
>>Producción para todos los clientes :August, 2025
>>[!BADGE Fuera del horario]{type=Neutral}

Se han agregado nuevas expresiones con el siguiente uso a los campos de fórmula en Workfront Planning y a los campos personalizados calculados en Workfront:

* **REMOVEACCENTS(string)**: quita las marcas diacríticas de todos los caracteres acentuados de la cadena de entrada.
* **REPLACEPATTERN (cadena, patrón, cadena de reemplazo)**: reemplaza las coincidencias del patrón dado por la cadena de reemplazo.
* **PASCAL(string)**: Convierte la cadena de entrada a PascalCase al poner en mayúscula la primera letra de cada palabra y eliminar todos los espacios.

Para obtener más información, consulte [Información general de expresiones de datos calculados](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

## Adición de los botones Maximizar y Minimizar a la ventana de creación del campo de fórmula

>[!NOTE]
>
>Vista previa: 31 de julio de 2025
>>Producción para todos los clientes: viernes, 31 de julio de 2025
>>[!BADGE Fuera del horario]{type=Neutral}

Se ha agregado un botón Maximizar para ampliar el campo Fórmula al crear o editar el campo en una vista de tabla de registros. Además, hemos agregado un botón Minimizar en la nueva ventana ampliada para volver al cuadro de creación de campos.

Para obtener más información, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

## La página Registros conectados ahora está disponible en el área de vista previa de un registro

>[!NOTE]
>
>* Vista previa: 31 de julio de 2025
>* Versión rápida de producción: 14 de agosto de 2025
>* Producción para todos los clientes: viernes, 16 de octubre de 2025

Ahora hemos hecho que la experiencia de la página de registros conectados en el cuadro de vista previa coincida con la de la página en la página completa del área de Detalles de un registro.

Antes de esta mejora, la visualización de registros conectados en una página de registros conectados solo era posible en la página completa del área de Detalles de un registro.

Para obtener más información, vea [Administrar el diseño de la página de registros](/help/quicksilver/planning/records/manage-the-record-page.md).

<!--## Updates to Requesting experience 

>[!NOTE]
>
>* Preview: July 31, 2025
>* Production fast release: August 14, 2025
>* Production for all customers: October 16, 2025

To create a better user experience when making requests in Workfront and Workfront Planning, we've updated the requesting experience. Now you can:

* View Workfront and Workfront Planning requests in a single list.
* Filter submitted requests based on criteria you specify.
* Search for and select Workfront request queues and Workfront Planning forms in a consolidated experience.
* Hide and reorder columns in the submitted requests list.

This update also features changes to the look and feel of the page.

Previously, Workfront and Workfront Planning requests were on separate tabs, and filters were not customizable.

For more information on creating requests see:

* For Workfront: [Create and submit requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)
* For Workfront Planning: [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md) -->

## Creación de registros en la vista de cronología

>[!NOTE]
>
>Vista previa: 24 de julio de 2025
>>Versión rápida de producción: 14 de agosto de 2025
>>Producción para todos los clientes: viernes, 16 de octubre de 2025

Ahora puede crear registros en la vista de escala de tiempo de un tipo de registro haciendo doble clic en cualquier lugar de la escala de tiempo.

Puede seleccionar el intervalo de fechas del registro o abrir la página del registro para editar todos sus detalles.

Antes de esta mejora, solo se podían agregar registros nuevos mediante el botón Nuevo registro o en línea en la vista de tabla.

Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).

## Opción Agregar uso compartido en el menú Más de una tarjeta de tipo de registro

>[!NOTE]
>
>Vista previa: 24 de julio de 2025
>>Versión rápida de producción: 14 de agosto de 2025
>>Producción para todos los clientes: viernes, 16 de octubre de 2025

Ahora puede compartir un tipo de registro desde el menú Más de la tarjeta de tipo de registro de la página del espacio de trabajo. Antes de esta mejora, la opción Compartir solo estaba disponible dentro de la página de tipo de registro.

Para obtener más información, vea [Compartir tipos de registros](/help/quicksilver/planning/access/share-record-types.md).

## Mostrar todas las vistas de Workfront Planning en modo de pantalla completa

>[!NOTE]
>
>Vista previa: 24 de julio de 2025
>>Versión rápida de producción: 14 de agosto de 2025
>>Producción para todos los clientes: viernes, 16 de octubre de 2025

Ahora puede mostrar todas las vistas de Workfront Planning (tabla, cronología y calendario) en modo de pantalla completa. La funcionalidad de vista se conserva y también puede cambiar la vista mientras está en pantalla completa.

Antes de esta mejora, esta funcionalidad no existía.

Para obtener más información, consulte [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).

## Agregar equipos como aprobadores en formularios de solicitud de Planning

>[!NOTE]
>
>Vista previa: 22 de julio de 2025
>>Producción para la versión rápida: 14 de agosto de 2025
>>Producción para todos los clientes: viernes, 16 de octubre de 2025

Para que el proceso de aprobación sea más flexible, se ha agregado la capacidad de agregar equipos como aprobadores en los formularios de solicitud de Planning. Ahora puede introducir y seleccionar nombres de equipo al configurar aprobadores. Cualquiera de los integrantes del equipo puede tomar una decisión, que cuenta como decisión de aprobación para todo el equipo.

Anteriormente, solo se podían asignar como aprobadores usuarios individuales.

Para obtener más información, consulte [Agregar una aprobación a un formulario de solicitud en Adobe Workfront Planning](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

## Nuevos campos para mostrar la información de aprobación del registro

>[!NOTE]
>
>Vista previa: 17 de julio de 2025
>>Producción para la versión rápida: 14 de agosto de 2025
>>Producción para todos los clientes: viernes, 16 de octubre de 2025

Presentamos los siguientes campos para capturar la información de aprobación de los registros creados al enviar una solicitud con una aprobación:

* Aprobado por
* Fecha de aprobación

Para obtener más información, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

## Rellenar automáticamente campos basados en agrupaciones aplicadas

>[!NOTE]
>
>Vista previa: 10 de julio de 2025
>>Versión rápida de producción: 14 de agosto de 2025
>>Producción para todos los clientes: viernes, 16 de octubre de 2025


Ahora, cuando tenga agrupaciones aplicadas a una vista de tabla, al agregar un registro a la tabla se rellenarán automáticamente los campos asociados con las agrupaciones a las que agregue el registro.

Si se han aplicado varias agrupaciones, el sistema rellena automáticamente los campos asociados a todas las agrupaciones solo cuando se agrega el registro al final de la lista dentro de los últimos criterios de agrupación.

Antes de esta mejora, tenía que actualizar manualmente los campos asociados a las agrupaciones.

Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md).
