---
content-type: release-notes
title: Actividad de la versión del primer trimestre de 2026 para Adobe Workfront Planning
description: Esta es la actividad de lanzamiento del producto Adobe Workfront Planning para el primer trimestre de 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: d60123df6e18025a886809fa390137bdf9287e6e
workflow-type: tm+mt
source-wordcount: '2014'
ht-degree: 1%

---

# Actividad de la versión del primer trimestre de 2026 para Adobe Workfront Planning

Este artículo describe las funciones que se lanzarán para Workfront Planning durante la versión del primer trimestre de 2026.

<!--keep the sentence below for all future quarterly release pages-->

Para obtener una lista de todas las características publicadas para Adobe Workfront Planning, consulte [Actividad de la versión de Adobe Workfront Planning: índice de artículo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).


## Los tipos de registros globales se pueden compartir desde el espacio de trabajo secundario

>[!NOTE]
>
>Vista previa: 15 de enero de 2026
>Versión rápida de producción: 15 de enero de 2026
>Producción para todos: 15 de enero de 2026
>[!BADGE Fuera del horario]{type=Neutral}

Ahora puede compartir tipos de registros globales que agregó a un espacio de trabajo secundario desde ese espacio de trabajo. Los usuarios también recibirán los mismos permisos para todos los registros del espacio de trabajo secundario que esté compartiendo.

>[!NOTE]
>
>Los usuarios pueden tener permisos diferentes para el mismo tipo de registro global en el espacio de trabajo principal o en cualquier otro espacio de trabajo secundario en el que se haya agregado el tipo de registro. Los permisos de tipo de registro y Workspace se transfieren a los registros.

Antes de este cambio, sólo se podía compartir el tipo de registro global desde su espacio de trabajo principal original.

Para obtener más información, vea [Información general sobre el tipo de registro entre espacios de trabajo](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).


## Los registros agregados a un tipo de registro global en un espacio de trabajo secundario no son visibles desde otros espacios de trabajo secundarios

>[!NOTE]
>
>Vista previa: 15 de enero de 2026
>Versión rápida de producción: 15 de enero de 2026
>Producción para todos: 15 de enero de 2026
>[!BADGE Fuera del horario]{type=Neutral}

Los registros agregados a un tipo de registro global en un espacio de trabajo secundario sólo son visibles desde ese espacio de trabajo o desde el espacio de trabajo principal original del tipo de registro. Antes de esta actualización, los registros añadidos a un espacio de trabajo secundario también eran visibles desde otros espacios de trabajo secundarios en los que podría haber tenido permisos de visualización.

Para obtener más información, vea [Información general sobre el tipo de registro entre espacios de trabajo](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

## Creación de jerarquías de tipo de registro en espacios de trabajo

>[!NOTE]
>
>Vista previa: 23 de diciembre de 2025
>Versión rápida de producción: 14 de enero de 2026
>Producción para todos: 15 de enero de 2026

Ahora puede definir jerarquías flexibles pero estructuradas entre tipos de registros u objetos.

Las jerarquías son conexiones entre tipos de registros. Puede tener hasta 4 tipos de registros y objetos conectados en una jerarquía, y hasta 5 jerarquías en un espacio de trabajo. El primer tipo de registro de la jerarquía es el primer padre.

Puede utilizar jerarquías para organizar el trabajo y visualizar cómo la estrategia fluye hacia la ejecución.

Tenga en cuenta lo siguiente al crear jerarquías:

* Sólo puede conectar tipos de registros de Planning desde un espacio de trabajo y proyectos de Workfront en una jerarquía.
* Un tipo de registro o proyecto solo puede tener un objeto principal en el mismo espacio de trabajo.
* Un tipo de registro puede ser el principal en varias jerarquías.
* Los tipos de registro conectables no se pueden utilizar en jerarquías de espacios de trabajo que no sean los suyos propios.
* Los tipos de registros globales sólo se pueden utilizar en jerarquías en los espacios de trabajo en los que se crearon o a los que se agregaron.

Para obtener más información, consulte [Información general sobre jerarquía y ruta de exploración](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Nuevas rutas de exploración unificadas agregadas a las páginas de los registros

>[!NOTE]
>
>Vista previa: 23 de diciembre de 2025
>Versión rápida de producción: 14 de enero de 2026
>Producción para todos: 15 de enero de 2026

Cuando se crean jerarquías entre tipos de registros, se generan rutas de exploración para los registros que pertenecen a esos tipos de registros.

Registrar rutas de exploración refleja su lugar en una jerarquía. Después de crear jerarquías, puede ver la ruta de exploración de un registro en la parte superior de su página, indicando qué otros objetos principales o secundarios están conectados a él. Las jerarquías son coherentes en Workfront y Planning.

Por ejemplo, puede ver la jerarquía de Planning de un proyecto cuando está conectado a tipos de registros de Planning en su ruta de exploración de Planning y su jerarquía de Workfront cuando está conectado a tipos de objetos de Workfront, como Portafolios o Programas, en Workfront.

Para obtener más información, consulte [Información general sobre jerarquía y ruta de exploración](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).


## Mejoras en las páginas de registros conectadas

>[!NOTE]
>
>Vista previa: 19 de diciembre de 2025
>Producción rápida: 14 de enero de 2026
>Producción para todos: 15 de enero de 2026

Para ofrecerle una mayor flexibilidad a la hora de trabajar con páginas de registros conectados, hemos mejorado la funcionalidad de las vistas en esta área de Workfront Planning. A continuación se indican mejoras en las páginas de registros conectados de un registro:

* Ahora puede agregar una escala de tiempo y una vista de calendario a la página de registros conectada de un registro.
* Ahora puede compartir todas las vistas desde una página de registros conectada. Las vistas compartidas desde estas páginas son visibles en todo el sistema para todos los usuarios con los que las comparte en cualquier otra área de Workfront Planning. Todas las vistas compartidas en cualquier otra área de Planning también son visibles en la página de registros conectados para los mismos usuarios con los que se comparten.
* Se ha agregado una restricción para permitir solamente una página de registros conectados por cada tipo de objeto o registro. Antes de esta mejora, se podían añadir varias páginas para el mismo tipo de objeto o registro. Ahora puede utilizar varias vistas para el mismo tipo de registro en una página de registros conectada.
* Hemos agregado un vínculo **Nueva fila** en la parte inferior de una vista de tabla y un botón **Conectar registros** en el área superior derecha de la página de registros conectada. Antes de esta mejora, el vínculo **Nueva fila** y el botón **Conectar registros** existían solamente en una página conectada a un proyecto.

Para obtener más información, vea [Agregar la página Registros conectados a un registro](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

## Compartir vistas en la página Registros conectados de proyectos

>[!NOTE]
>
>Vista previa: 18 de diciembre de 2025
>Versión rápida de producción: 14 de enero de 2026\
>Producción para todos: 15 de enero de 2026

Para que sea más fácil asegurarse de ver la información que necesita, hemos agregado la capacidad de compartir vistas a la página Registros conectados de proyectos. Ahora puede compartir vistas con otros usuarios, equipos o grupos.

Para obtener más información, vea [Agregar la página Registros conectados a un registro](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

## El comodín de usuario actual ya está disponible en los filtros de vista de conexión del proyecto

>[!NOTE]
>
>Vista previa: 18 de diciembre de 2025
>Versión rápida de producción: 14 de enero de 2026\
>Producción para todos: 15 de enero de 2026

Para facilitar el filtrado de las conexiones de proyecto que se le aplican, hemos creado un comodín de usuario actual. Ahora, al filtrar, puede seleccionar &quot;Yo (usuario conectado)&quot;. El filtro se aplica al usuario que está viendo la lista de solicitudes.

Esto puede resultar práctico al agregar un filtro a una vista que utilizarán varios usuarios. Cada usuario verá los resultados de los filtros que se les apliquen.

El comodín está disponible en campos donde el valor es un usuario.

Para obtener más información sobre la configuración de vistas de conexión del proyecto, incluidos los filtros, vea [Agregar una página Registros conectados a un registro](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).


## Mejoras en la página principal de Workspace

>[!IMPORTANT]
>
>Esto se ha eliminado temporalmente de los entornos de Previsualización y Producción.

>[!NOTE]
>
>Vista previa: 18 de diciembre de 2025
>Producción rápida: 14 de enero de 2026
>Producción para todos: 15 de enero de 2026

Se han realizado las siguientes mejoras en la página principal de Workspaces en Workfront Planning:

* Una experiencia de desplazamiento más rápida y dinámica. Esto es especialmente visible si su organización tiene un gran número de espacios de trabajo y para administradores del sistema.

* Hemos añadido un cuadro de búsqueda que ahora le permite buscar un espacio de trabajo específico por nombre.

* Se cambió el nombre de la ficha **Otros espacios de trabajo** a **Todos los espacios de trabajo** e incluye todos los espacios de trabajo para los que tiene al menos permisos de Vista, incluidos los que ha creado.

Para obtener más información, consulte [Edición de espacios de trabajo](/help/quicksilver/planning/architecture/edit-workspaces.md).


## Adición del campo de conexión Marca a Productos y Personas de forma predeterminada en GenStudio Workspace

>[!NOTE]
>
>Vista previa: 11 de diciembre de 2025
>Versión rápida de producción: 11 de diciembre de 2025
>Producción para todos: 11 de diciembre de 2025
>[!BADGE Fuera del horario]{type=Neutral}

El campo de conexión con la marca GenStudio for Performance Marketing ahora se agrega de forma predeterminada a los tipos de registro Productos y Personas en el espacio de trabajo de GenStudio de Workfront Planning.

Su organización debe tener Workfront Planning y Adobe GenStudio for Performance Marketing.

Antes de esta mejora, solo podía agregar el campo de conexión de marca manualmente a cualquier tipo de registro, incluidos Productos y Personas. Aún puede conectar manualmente el tipo de registro de Brand GenStudio a otros tipos de registro en Workfront Planning.

Para obtener más información, consulte [Introducción a la integración de Adobe Workfront Planning y Adobe GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).

## Restringir la eliminación de permisos de usuarios de GenStudio for Performance Marketing de Planning

>[!NOTE]
>
>Vista previa: 11 de diciembre de 2025
>Versión rápida de producción: 11 de diciembre de 2025
>Producción para todos: 11 de diciembre de 2025
>[!BADGE Fuera del horario]{type=Neutral}

Se ha agregado una protección que impide eliminar los permisos de los usuarios de GenStudio for Performance Marketing de los objetos de Workfront Planning. Con esta mejora, ya no puede quitar usuarios de GenStudio del espacio de trabajo de GenStudio en Planning, ni puede deshabilitar los permisos heredados para tipos de registro en el espacio de trabajo de GenStudio, si esos permisos incluyen usuarios de GenStudio. Antes de esta mejora, cuando eliminaba estos usuarios del espacio de trabajo de GenStudio en Planning, también perdían permisos para tipos de registros en GenStudio.

Su organización debe tener Workfront Planning y Adobe GenStudio for Performance Marketing.

Para obtener más información, consulte [Introducción a la integración de Adobe Workfront Planning y Adobe GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).


## Se ha eliminado el uso compartido público de vistas en un tipo de registro global en un espacio de trabajo secundario


>[!NOTE]
>
>Vista previa: 3 de diciembre de 2025
>Versión rápida de producción: 4 de diciembre de 2025
>Producción para todos: 15 de enero de 2026


Se ha eliminado la pestaña Uso compartido público al compartir una vista para un registro global en un espacio de trabajo secundario. No se puede compartir una vista públicamente desde un tipo de registro global agregado a otro espacio de trabajo desde un tipo de registro global existente. Puede compartir una vista de tipo de registro global públicamente desde su espacio de trabajo original.

Para obtener más información, consulte [Compartir vistas](/help/quicksilver/planning/access/share-views.md).


## Conectar marcas GenStudio for Performance Marketing con tipos de registros de Workfront Planning

>[!NOTE]
>
>Vista previa: 13 de noviembre de 2025
>Versión rápida de producción: 13 de noviembre de 2025
>Producción para todos: 13 de noviembre de 2025

Ahora puede conectar tipos de registros de Workfront Planning con marcas de Adobe GenStudio for Performance Marketing. Su organización debe tener Workfront Planning y Adobe GenStudio for Performance Marketing.

Para obtener más información, consulte [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md).


## Nuevo cuadro de búsqueda de campos en los iconos Filtros, Campos y Colores de fila en las vistas de Planning

>[!NOTE]
>
>Vista previa: 6 de noviembre de 2025
>Versión rápida de producción: 11 de diciembre de 2025
>Producción para todos: 15 de enero de 2026

Ahora puede buscar un campo específico al crear un elemento de vista en una vista de tipo de registro. Se han agregado cuadros de búsqueda al crear un filtro, ordenar, agrupar o al configurar los campos o colores de fila. Antes de esta mejora, simplemente podía desplazarse por la lista de campos disponibles.

Esta mejora está disponible en todas las vistas de tipo de registro.

Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).


## Tipos de registros globales y la posibilidad de agregarlos como tipos de registros existentes a otros espacios de trabajo

>[!NOTE]
>
>Vista previa: 16 de octubre de 2025
>Versión rápida de producción: 13 de noviembre de 2025
>Producción para todos: 15 de enero de 2026

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
>Versión rápida de producción: 13 de noviembre de 2025
>Producción para todos: 15 de enero de 2026

Hemos introducido un límite de 30 campos de conexión para cada tipo de registro.

NOTA: Si su organización tiene actualmente más de 30 campos de conexión para un tipo de registro, puede mantener los campos adicionales que exceden el límite de 30. Sin embargo, no se pueden agregar más campos de conexión a los tipos de registro que superen el límite. En adelante, se aplicará el nuevo límite de 30 campos de conexión.

Para obtener más información, vea [Información general sobre los tipos de registros conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Establecer valores descriptivos para las opciones de campos de tipo selección

>[!NOTE]
>
>Vista previa: 16 de octubre de 2025
>Versión rápida de producción: 13 de noviembre de 2025
>Producción para todos: 15 de enero de 2026

Al agregar opciones de campo a un campo de selección única o múltiple, Workfront ahora asigna valores descriptivos únicos a cada opción. Antes de esta mejora, Workfront generaba un ID alfanumérico difícil de comprender y utilizar en las llamadas a la API y otras integraciones.

Tenga en cuenta lo siguiente con esta mejora:

* Los nuevos valores se agregarán a las nuevas opciones de campo. Las opciones de campo existentes conservarán sus ID alfanuméricos.

* Los valores de opción son únicos para un campo, pero se pueden repetir entre diferentes campos.

* Cambiar el nombre de una opción no actualiza su valor original.

* Los valores de opción se muestran en minúsculas y están separados por guiones bajos en el caso de opciones de varias palabras. Si utiliza una etiqueta ya utilizada como otro nombre de opción para el mismo campo, Workfront añade un número secuencial al valor.

Para obtener más información, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).






