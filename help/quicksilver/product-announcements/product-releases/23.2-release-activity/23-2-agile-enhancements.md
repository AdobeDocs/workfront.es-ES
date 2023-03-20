---
title: 23.2 Mejoras ágiles
description: 23.2 Mejoras ágiles
author: Courtney
draft: Probably
feature: Product Announcements
source-git-commit: 96819e5d81a063ad623350a0a75428629d6f7b6d
workflow-type: tm+mt
source-wordcount: '1124'
ht-degree: 0%

---

# 23.2 Mejoras ágiles

En esta página se describen todas las mejoras ágiles realizadas con la versión 23.2 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno Producción con la versión 23.2.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de versión 23.2, consulte [Resumen de la versión 23.2](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## Funcionalidad de iteración disponible en Adobe Workfront Boards

Hay varias funciones nuevas disponibles en los Workfront Boards que permiten utilizar la funcionalidad Agile Scrum. Estas funciones incluyen:

* Flujos de trabajo para agrupar tableros relacionados con el mismo equipo y colaborar en el trabajo
* Una lista de tarjetas, o trabajo atrasado, con la opción de utilizar fuentes para conectar tarjetas a tareas y problemas de Workfront
* Tableros de procesos de planificación e iteración

Tenga en cuenta que se ha cambiado el nombre de las colecciones a flujos de trabajo. Los flujos de trabajo le ayudan a visualizar los datos de diferentes maneras. Puede mostrar elementos en tarjetas en una lista, en un tablero o en una iteración. Las tarjetas de un flujo de trabajo también se pueden compartir entre varios tableros. Puede facilitar fácilmente los flujos de trabajo mediante tarjetas y tableros en un flujo de trabajo.

Para obtener más información, consulte [Administrar flujos de trabajo](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md), [Creación de una iteración en un flujo de trabajo](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md)y [Usar la lista de tarjetas](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md). Los dos segundos artículos no estarán disponibles en Principal hasta que publique mi rama.

## Agregar tareas y problemas de listas e informes a una lista de tarjetas de flujo de trabajo

Ahora puede agregar tareas o problemas existentes a un flujo de trabajo en los tableros de Workfront directamente desde una lista o vista de informe. Los elementos que agregue al flujo de trabajo se agregarán a la lista de tarjetas como tarjetas no planificadas.

Para obtener más información, consulte [Agregar tareas o problemas existentes a un tablero](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).

## Añadir campos personalizados a tarjetas en un tablero

Ahora puede incluir campos personalizados en los tableros de Adobe Workfront. El campo ya debe crearse en Workfront. No se pueden diseñar ni crear nuevos campos personalizados dentro de un tablero.

Al igual que los campos predeterminados, puede elegir mostrar el campo personalizado en la vista completa de una tarjeta y la vista condensada en el tablero.

Cualquier dato del campo personalizado de la tarjeta es de solo lectura.

Para obtener más información, consulte [Personalización de los campos que se muestran en una tarjeta](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

## Agregar tareas y problemas de listas e informes a un tablero de Workfront

Ahora puede agregar tareas o problemas existentes a un tablero de Workfront directamente desde una lista o vista de informe. Cualquier elemento que agregue al tablero se convertirá en tarjetas conectadas.

Además, el campo Tableros ahora está disponible para agregarlo a listas e informes para tareas o problemas. Este campo muestra todos los tableros a los que se ha añadido una tarea o un problema.

Para obtener más información, consulte [Agregar tareas o problemas existentes a un tablero](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).


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
