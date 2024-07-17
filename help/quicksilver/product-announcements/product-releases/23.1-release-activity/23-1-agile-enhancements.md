---
title: 23.1 Mejoras de Agile
description: 23.1 Mejoras de Agile
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bd041a5-a6e3-4fe3-ae23-45980701e904
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 0%

---

# 23.1 Mejoras de Agile

Esta página describe todas las mejoras de Agile realizadas con la versión 23.1 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción el 16 de enero de 2023.

Para obtener una lista de todos los cambios disponibles con la versión 23.1, consulte [Información general sobre la versión 23.1](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

## Planificación de Scrum para tableros de Workfront

Las nuevas funciones de planificación de Scrum en los tableros de Adobe Workfront ofrecen opciones flexibles para administrar sus procesos ágiles. Con estas herramientas, puede:

* Seguimiento del trabajo en iteraciones o sprints
* Usar la velocidad para guiar los compromisos del equipo
* Rastrear evolución y tasa de finalización

Las funciones de planificación de Scrum serán de &quot;seguimiento rápido&quot; después de la versión 23.1.

## Las fechas de vencimiento en las tarjetas se asignan a la fecha planificada de finalización en el objeto Workfront

>[!NOTE]
>
>Esta función solo está disponible a través de la inclusión de funciones anticipada para tableros de Workfront.

Las fechas de vencimiento de las tarjetas conectadas en los paneles de Workfront ahora se asignan a la fecha planificada de finalización del objeto de Workfront asociado. Si actualiza la fecha de vencimiento en una tarjeta, la fecha planificada de finalización se actualiza en la tarea o el problema. Al cambiar la fecha planificada de finalización, también se cambia la fecha límite de la tarjeta. Anteriormente, la fecha de vencimiento de la tarjeta era una entrada manual y no se asignaba a ninguna fecha de una tarea o un problema.

La asignación de fechas también se aplica a los elementos de la lista de comprobación conectados que están sincronizados con las subtareas.

La fecha de vencimiento en las tarjetas conectadas y en las tarjetas ad hoc ahora también incluye un campo de hora.

Para obtener más información, consulte [Usar tarjetas conectadas en tableros](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[Ver una demostración en vídeo de esta característica](https://video.tv.adobe.com/v/3411952/){target=_blank}

## Los elementos de la lista de comprobación de tableros y las subtareas de Workfront ahora están vinculados

>[!NOTE]
>
>Esta función solo está disponible a través de la inclusión de funciones anticipada para tableros de Workfront.

Cuando se agrega una tarjeta conectada a un tablero para una tarea de Workfront, las subtareas se importan como elementos de lista de comprobación en la tarjeta. Además, cuando se crea un elemento de lista de comprobación en una tarjeta conectada, se agrega una subtarea a la tarea de Workfront. Los elementos de la lista de comprobación de problemas no están conectados a ningún objeto de Workfront.

Anteriormente, los elementos de la lista de comprobación y las subtareas no estaban vinculados. Si desea incluir una subtarea en el tablero, puede importarla como una tarjeta conectada por separado o agregar manualmente un elemento de lista de comprobación a una tarjeta.

Para obtener más información, consulte [Usar tarjetas conectadas en tableros](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) y [Administrar elementos de listas de comprobación en tarjetas](/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md).

[Ver una demostración en vídeo de esta característica](https://video.tv.adobe.com/v/3411951/){target=_blank}

## Contador de tarjetas en columnas del tablero

>[!NOTE]
>
>Esta función solo está disponible a través de la inclusión de funciones anticipada para tableros de Workfront.

Hay disponible un nuevo ajuste de configuración para activar un contador de tarjetas para todas las columnas de un tablero. Si utiliza el límite de trabajo en curso en una columna, no se agrega un contador de tarjetas independiente.

Para obtener más información, consulte [Administrar columnas del tablero](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

## Buscar y ordenar en el tablero

>[!NOTE]
>
>Esta función solo está disponible a través de la inclusión de funciones anticipada para tableros de Workfront.

Ahora puede ordenar el tablero por nombre o fecha del tablero y buscar un tablero específico en la lista.

Para obtener más información, consulte [Usar el tablero de tableros](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md).

## El estado se muestra en la tarjeta

>[!NOTE]
>
>Esta función solo está disponible a través de la inclusión de funciones anticipada para tableros de Workfront.

Si se asigna un estado a una tarjeta de un tablero, el estado ahora se muestra en la tarjeta para que no tenga que abrirla para ver su estado. Esta mejora se aplica tanto a tarjetas ad hoc como a tarjetas conectadas.

Para obtener más información, consulte [Usar tarjetas conectadas en tableros](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) y [Agregar una tarjeta ad hoc a un tablero](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

![estado en la tarjeta](/help/quicksilver/product-announcements/product-releases/assets/boards-connected-card-details-110922.png)

## Tarjetas enlazables ahora disponibles en tableros

>[!NOTE]
>
>Esta función solo está disponible a través de la inclusión de funciones anticipada para tableros de Workfront.

Ahora puede enviar un vínculo a una tarjeta específica a otro usuario de tableros. La persona debe tener acceso para ver el tablero antes de poder abrir el vínculo.

Cuando abre una tarjeta en un tablero, la dirección URL del explorador tiene este aspecto:

```
https://<Workfront-URL>/boards/<board-id>/card/<card-id>. 
```

Puede copiar la dirección URL completa y enviarla a otra persona. Irán directamente a la tarjeta abierta cuando accedan al vínculo.

Anteriormente, los vínculos estaban disponibles para tableros, pero no para tarjetas específicas.

Para obtener información sobre las tarjetas, consulte [Agregar una tarjeta ad hoc a un tablero](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) y [Usar tarjetas conectadas en los tableros](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Filtrar por conexión en tableros

>[!NOTE]
>
>Esta función solo está disponible a través de la inclusión de funciones anticipada para tableros de Workfront.

La lista de filtros de un tablero ahora incluye la opción de filtrar por conexión, que muestra todas las tarjetas conectadas para un proyecto específico. También puede filtrar por tarjetas que no estén conectadas.

Para obtener más información, vea [Filtrar y buscar en un tablero](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

[Ver una demostración en vídeo de esta característica](https://video.tv.adobe.com/v/3412381/){target=_blank}

## Archivar tarjetas de un tablero en una programación

>[!NOTE]
>
>Esta función solo está disponible a través de la inclusión de funciones anticipada para tableros de Workfront.

Puede configurar un tablero para que se archiven las tarjetas o &quot;se caigan&quot; del tablero según una programación. Hay opciones disponibles para configurar tarjetas en una columna en particular para archivarlas en un determinado número de días o semanas. Por ejemplo, puede definir la visita en orden previsto para que las tarjetas de una columna Completar se archiven después de que estén en la columna durante dos semanas.

Si desea volver a mostrar las tarjetas después de que se caigan del tablero, puede definir el filtro del tablero para que muestre las tarjetas archivadas.

Para obtener más información, consulte [Configurar la caída de la tarjeta](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).

[Ver una demostración en vídeo de esta característica](https://video.tv.adobe.com/v/3412323/){target=_blank}
