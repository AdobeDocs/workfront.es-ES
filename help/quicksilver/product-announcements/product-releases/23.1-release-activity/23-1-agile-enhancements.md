---
title: 23.1 Mejoras ágiles
description: 23.1 Mejoras ágiles
author: Courtney
draft: Probably
feature: Product Announcements
exl-id: 4bd041a5-a6e3-4fe3-ae23-45980701e904
source-git-commit: f0e21f9b2846c5665474903a2910ce9f41cdf810
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 0%

---

# 23.1 Mejoras ágiles

En esta página se describen todas las mejoras de Agile realizadas en la versión 23.1 del entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción en la semana del 16 de enero de 2023.

Para obtener una lista de todos los cambios disponibles con la versión 23.1, consulte [Resumen de la versión 23.1](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

## Planificación de recortes para placas Workfront

Las nuevas funciones de planificación de Scrum de las placas Adobe Workfront ofrecen opciones flexibles para administrar sus procesos ágiles. Con estas herramientas puede:

* Seguimiento del trabajo en iteraciones o sprints
* Utilice la velocidad para orientar los compromisos de equipo
* Seguimiento de la interrupción y la tasa de finalización

Las funciones de planificación de Scrum serán un &quot;paso rápido&quot; después de la versión 23.1.

## Fechas de vencimiento en tarjetas asignadas a la fecha de finalización planeada en el objeto Workfront

>[!NOTE]
>
>Esta función solo está disponible a través de la opción de inclusión de las funciones iniciales para Workfront Board.

Las fechas de vencimiento de las tarjetas conectadas en los Workfront Boards ahora se asignan a la fecha de finalización planificada en el objeto Workfront asociado. Si actualiza la fecha de vencimiento en una tarjeta, la fecha de finalización prevista se actualiza en la tarea o el problema. Al cambiar la fecha de finalización planificada también se cambia la fecha de vencimiento en la tarjeta. Anteriormente, la fecha de vencimiento de la tarjeta era una entrada manual y no se asignaba a ninguna fecha de una tarea o problema.

La asignación de fechas también se aplica a los elementos de la lista de comprobación conectados que se sincronizan con las subtareas.

La fecha de vencimiento de las tarjetas conectadas y las tarjetas ad hoc ahora también incluye un campo de hora.

Para obtener más información, consulte [Usar tarjetas conectadas en tableros](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[Ver una demostración en vídeo de esta función](https://video.tv.adobe.com/v/3411952/){target=_blank}

## Los elementos de la lista de comprobación del tablero y las subtareas de Workfront ahora están vinculados

>[!NOTE]
>
>Esta función solo está disponible a través de la opción de inclusión de las funciones iniciales para Workfront Board.

Cuando se agrega una tarjeta conectada a un tablero para una tarea de Workfront, todas las subtareas se importan como elementos de la lista de comprobación de la tarjeta. Además, cuando se crea un elemento de lista de comprobación en una tarjeta conectada, se agrega una subtarea a la tarea de Workfront. Los elementos de la lista de comprobación relacionados con problemas no están conectados a ningún objeto de Workfront.

Anteriormente, los elementos de la lista de comprobación y las subtareas no estaban vinculados. Si desea incluir una subtarea en el tablero, puede importarla como una tarjeta conectada independiente o agregar manualmente un elemento de la lista de comprobación a una tarjeta.

Para obtener más información, consulte [Usar tarjetas conectadas en tableros](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) y [Administrar los elementos de la lista de comprobación en las tarjetas](/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md).

[Ver una demostración en vídeo de esta función](https://video.tv.adobe.com/v/3411951/){target=_blank}

## Contador de tarjetas en las columnas del tablero

>[!NOTE]
>
>Esta función solo está disponible a través de la opción de inclusión de las funciones iniciales para Workfront Board.

Hay disponible una nueva configuración para activar un contador de tarjetas para todas las columnas de un tablero. Si utiliza el límite de WIP en una columna, no se agregará un contador de tarjeta independiente.

Para obtener más información, consulte [Administrar columnas de tablero](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

## Buscar y ordenar en el tablero

>[!NOTE]
>
>Esta función solo está disponible a través de la opción de inclusión de las funciones iniciales para Workfront Board.

Ahora puede ordenar el tablero por nombre o fecha del tablero y buscar un tablero específico en la lista.

Para obtener más información, consulte [Usar el tablero de tableros](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md).

## El estado aparece en la tarjeta

>[!NOTE]
>
>Esta función solo está disponible a través de la opción de inclusión de las funciones iniciales para Workfront Board.

Si a una tarjeta de un tablero se le asigna un estado, el estado ahora se muestra en la tarjeta, de modo que no tenga que abrir la tarjeta para ver el estado. Esta mejora se aplica tanto a tarjetas específicas como a tarjetas conectadas.

Para obtener más información, consulte [Usar tarjetas conectadas en tableros](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) y [Agregar una tarjeta ad hoc a un tablero](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

![estado en tarjeta](/help/quicksilver/product-announcements/product-releases/assets/boards-connected-card-details-110922.png)

## Tarjetas enlazables ahora disponibles en tableros

>[!NOTE]
>
>Esta función solo está disponible a través de la opción de inclusión de las funciones iniciales para Workfront Board.

Ahora puede enviar un vínculo a una tarjeta específica a otro usuario del tablero. La persona debe tener acceso para ver el tablero antes de poder abrir el vínculo.

Cuando se abre una tarjeta en un tablero, la dirección URL del explorador tiene este aspecto:

```
https://<Workfront-URL>/boards/<board-id>/card/<card-id>. 
```

Puede copiar la dirección URL completa y enviarla a otra persona. Accederán directamente a la tarjeta de apertura cuando accedan al vínculo.

Anteriormente, los vínculos estaban disponibles para tableros, pero no para tarjetas específicas.

Para obtener información sobre tarjetas, consulte [Agregar una tarjeta ad hoc a un tablero](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) y [Usar tarjetas conectadas en tableros](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Filtrar por conexión en tableros

>[!NOTE]
>
>Esta función solo está disponible a través de la opción de inclusión de las funciones iniciales para Workfront Board.

La lista de filtros de un tablero ahora incluye la opción de filtrar por conexión, que muestra todas las tarjetas conectadas para un proyecto específico. También puede filtrar por tarjetas que no estén conectadas.

Para obtener más información, consulte [Filtrar y buscar en un tablero](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

[Ver una demostración en vídeo de esta función](https://video.tv.adobe.com/v/3412381/){target=_blank}

## Archivar tarjetas de un tablero según una programación

>[!NOTE]
>
>Esta función solo está disponible a través de la opción de inclusión de las funciones iniciales para Workfront Board.

Puede configurar un tablero para que las tarjetas se archiven o se &quot;quiten&quot; del tablero según una programación. Hay opciones disponibles para configurar tarjetas en una columna en particular para archivarlas en un determinado número de días o semanas. Por ejemplo, puede definir la caída para que las tarjetas de una columna Completa se archiven después de que estén en la columna durante dos semanas.

Si desea volver a mostrar las tarjetas después de que queden fuera del tablero, puede configurar el filtro de tablero para que muestre las tarjetas archivadas.

Para obtener más información, consulte [Configuración de la caída de tarjetas](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).

[Ver una demostración en vídeo de esta función](https://video.tv.adobe.com/v/3412323/){target=_blank}
