---
title: 23.2 Mejoras ágiles
description: 23.2 Mejoras ágiles
author: Courtney
draft: Probably
feature: Product Announcements
source-git-commit: 8a209bbe64b7b69b41cd9e4d2f603ff58491ba30
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# 23.2 Mejoras ágiles

En esta página se describen todas las mejoras ágiles realizadas con la versión 23.2 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno Producción con la versión 23.2.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de versión 23.2, consulte [Resumen de la versión 23.2](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

<!--

## Iteration functionality available in Adobe Workfront Boards

Several new features available in Workfront Boards make it possible to use agile Scrum functionality. These features include:

* Workstreams for grouping boards related to the same team, and collaborating on work
* A list of cards, or backlog of work, with the option to use sources to connect cards to Workfront tasks and issues
* Iteration planning and iteration process boards

Note that collections have been renamed to workstreams. Workstreams help you visualize data in different ways. You can display items on cards in a list, on a board, or on an iteration. Cards in a workstream can also be shared among multiple boards. You can easily facilitate workflows using cards and boards in a workstream.

For more information, see [Manage workstreams](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md), [Create an iteration](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration.md), and [Use the card list](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md). Second two articles will not be available in Main until I publish my branch.

## Add tasks and issues to Boards workstreams from lists and reports

You can now add existing tasks or issues to a workstream in Workfront Boards directly from a list or report view. Any items you add to the workstream are added to the card list as unplanned cards.

For more information, see [Add existing tasks or issues to a board](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).

-->

## Registro de horas en tarjetas conectadas en un tablero

>[!NOTE]
>
>Esta función solo está disponible a través de la opción de inclusión de las funciones iniciales para Workfront Board.

Ahora puede registrar horas en tarjetas conectadas, del mismo modo que lo haría en una tarea o problema. Debe tener los permisos correctos para la tarea o el problema para registrar la hora.

Los campos de registro de tiempo no se muestran en las tarjetas conectadas de forma predeterminada. Debe habilitar **Horas** en el área Configurar debajo de Tarjetas.

Para obtener más información, consulte [Usar tarjetas conectadas en tableros](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Personalización de la visualización de campos en una tarjeta

>[!NOTE]
>
>Esta función solo está disponible a través de la opción de inclusión de las funciones iniciales para Workfront Board.


La personalización ya está disponible para configurar qué campos se muestran en una tarjeta, tanto en la vista completa cuando la tarjeta está abierta como en la vista de tarjeta condensada en el tablero. Cuando desactiva un campo, no se muestra en ninguna de las vistas. También puede activar un campo en la vista completa y ocultarlo de la vista condensada.

Para obtener más información, consulte [Personalización de los campos que se muestran en una tarjeta](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

[Ver una demostración en vídeo de esta función](https://video.tv.adobe.com/v/3415710/){target=_blank}

## Definir un estado predeterminado para las tarjetas movidas a una columna de tablero

>[!NOTE]
>
>Esta función solo está disponible a través de la opción de inclusión de las funciones iniciales para Workfront Board.

Ahora puede establecer un estado predeterminado para aplicarlo a las tarjetas movidas a una columna específica; para ello, seleccione un estado personalizado y un estado del sistema en las políticas de columna. Al mover una tarjeta a la columna , Workfront intenta primero aplicar el estado personalizado (por ejemplo, Esperando comentarios). Si el estado personalizado no está disponible para esa tarjeta, Workfront aplicará el estado del sistema en su lugar (por ejemplo, En espera). Además, si el estado de la tarea o problema conectado se cambia al estado personalizado o del sistema establecido en la directiva de columna, la tarjeta se mueve automáticamente a la columna .

Anteriormente, se le pedía que seleccionara un estado para cada tarjeta que se moviera a la columna si había varios estados disponibles.

Para obtener más información, consulte [Administrar columnas](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

[Ver una demostración en vídeo de esta función](https://video.tv.adobe.com/v/3415711/){target=_blank}

## Colecciones ahora disponibles en Adobe Workfront Boards

>[!NOTE]
>
>Esta función solo está disponible a través de la opción de inclusión de las funciones iniciales para Workfront Board.

Ahora puede crear colecciones en el panel de tableros. Una colección es un grupo de tableros para colaborar en el trabajo. Una vez que haya asignado un nombre a la colección, puede agregar tableros a la colección mediante un conjunto de plantillas que ofrezcan una configuración predefinida, como los nombres de columna. También puede mover tableros independientes a una colección. Una vez que un tablero está en una colección, se puede mover a otra colección, pero no puede convertirse en un tablero independiente.

Añadir miembros a una colección funciona del mismo modo que agregar miembros a un tablero. Una persona o equipo debe ser miembro de la colección antes de poder agregarlos como miembros en un tablero de la colección.

Para obtener más información, consulte [Administrar colecciones](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

[Ver una demostración en vídeo de esta función](https://video.tv.adobe.com/v/3415609/){target=_blank}

## El campo Estimation de las tarjetas conectadas se asigna al campo Story Points de los objetos Workfront

>[!NOTE]
>
>Esta función solo está disponible a través de la opción de inclusión de las funciones iniciales para Workfront Board.

El campo Estimation de las tarjetas conectadas en Workfront Boards ahora se asigna al campo Story Points para el objeto Workfront asociado.

El nuevo campo Puntos de artículo es un campo de forma libre editable que se puede agregar a una vista de una lista o informe para tareas o problemas. No está vinculado a las horas planificadas ni a las asignaciones de equipo.

Anteriormente, la estimación de la tarjeta era una entrada manual y no se asignaba a ningún campo de una tarea o problema.

Además, el campo Estimation de las tarjetas ad hoc y conectadas ya no tiene un límite de caracteres. Anteriormente, el número máximo de caracteres era de 99.

Para obtener más información, consulte [Usar tarjetas conectadas en tableros](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Tarjeta de vista previa en la columna de admisión

>[!NOTE]
>
>Esta función solo está disponible a través de la opción de inclusión de las funciones iniciales para Workfront Board.

Ahora puede hacer clic en una tarjeta conectada en la columna de admisión para ver una versión de solo visualización de su contenido. No se puede editar el contenido de la tarjeta hasta que la tarjeta se mueva de la columna de admisión a otra columna del tablero.
