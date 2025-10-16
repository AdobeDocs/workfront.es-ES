---
content-type: release-notes
title: Actividad de la versión del primer trimestre de 2026 para Adobe Workfront Planning
description: Esta es la actividad de lanzamiento del producto Adobe Workfront Planning para el primer trimestre de 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: fdfb1ecb61fd85fa927fc7c3443c2a7f23409873
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 2%

---

# Actividad de la versión del primer trimestre de 2026 para Adobe Workfront Planning

Este artículo describe las funciones que se lanzarán para Workfront Planning durante la versión del primer trimestre de 2026.

<!--keep the sentence below for all future quarterly release pages-->

Para obtener una lista de todas las características publicadas para Adobe Workfront Planning, consulte [Actividad de la versión de Adobe Workfront Planning: índice de artículo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).


## Tipos de registros globales y la posibilidad de agregarlos como tipos de registros existentes a otros espacios de trabajo

>[!NOTE]
>
>Vista previa: 16 de octubre de 2025
>>Versión rápida de producción: 13 de noviembre de 2025
>>Producción para todos: 15 de enero de 2026

Al implementar Workfront Planning para una organización de varios equipos con flujos de trabajo comunes, es posible que necesite definir una estructura y metadatos coherentes para los tipos de registro clave (como Campañas o Entregables) que se pueden agregar a los espacios de trabajo de cada equipo para capturar y administrar su trabajo.

Además, es posible que necesite el trabajo de cada equipo para llegar a un nivel central.

En un flujo de trabajo de este tipo, puede asegurarse de que los equipos capturan su trabajo de forma coherente y, al mismo tiempo, desbloquean la visibilidad entre equipos, sin necesidad de añadir a todos los miembros de la organización a cada espacio de trabajo. Puede utilizar tipos de registros globales para conseguirlo.

Ahora puede designar un tipo de registro para que sea global y utilizarlo en varios espacios de trabajo. Los usuarios pueden utilizar la misma estructura de campos y conexiones que ya están configuradas en un espacio de trabajo central.

Para obtener más información, consulte los siguientes artículos:

* [Información general sobre el tipo de registro entre espacios de trabajo](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)

* [Configurar las capacidades del tipo de registro entre espacios de trabajo](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)

* [Agregar tipos de registros existentes desde otro espacio de trabajo](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)

## Nuevo límite para campos de conexión para un tipo de registro

>[!NOTE]
>
>Vista previa: 16 de octubre de 2025
>>Versión rápida de producción: 13 de noviembre de 2025
>>Producción para todos: 15 de enero de 2026

Hemos introducido un límite de 30 campos de conexión para cada tipo de registro.

NOTA: Si su organización tiene actualmente más de 30 campos de conexión para un tipo de registro, puede mantener los campos adicionales que exceden el límite de 30. Sin embargo, no se pueden agregar más campos de conexión a los tipos de registro que superen el límite. En adelante, se aplicará el nuevo límite de 30 campos de conexión.

Para obtener más información, vea [Información general sobre los tipos de registros conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Establecer valores descriptivos para las opciones de campos de tipo selección

>[!NOTE]
>
>Vista previa: 16 de octubre de 2025
>>Versión rápida de producción: 13 de noviembre de 2025
>>Producción para todos: 15 de enero de 2026

Al agregar opciones de campo a un campo de selección única o múltiple, Workfront ahora asigna valores descriptivos únicos a cada opción. Antes de esta mejora, Workfront generaba un ID alfanumérico difícil de comprender y utilizar en las llamadas a la API y otras integraciones.

Tenga en cuenta lo siguiente con esta mejora:

* Los nuevos valores se agregarán a las nuevas opciones de campo. Las opciones de campo existentes conservarán sus ID alfanuméricos.

* Los valores de opción son únicos para un campo, pero se pueden repetir entre diferentes campos.

* Cambiar el nombre de una opción no actualiza su valor original.

* Los valores de opción se muestran en minúsculas y están separados por guiones bajos en el caso de opciones de varias palabras. Si utiliza una etiqueta ya utilizada como otro nombre de opción para el mismo campo, Workfront añade un número secuencial al valor.

Para obtener más información, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).