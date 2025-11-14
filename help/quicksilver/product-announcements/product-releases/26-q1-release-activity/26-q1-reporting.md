---
title: Mejoras en los informes del primer trimestre de 2026
description: Mejoras en los informes del primer trimestre de 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 00483638948941c933e5f8bc8cb3edaf8e43fea1
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 11%

---

# Mejoras en los informes del primer trimestre de 2026

Esta página describe las mejoras de los informes realizadas con la versión del primer trimestre de 2026 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del primer trimestre de 2026, consulte [Información general de la versión del primer trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Duplicación de un informe en un panel de lienzo

>[!NOTE]
>
>Versión preliminar: viernes, 23 de octubre de 2025
>Producción para todos los clientes: viernes, 23 de octubre de 2025
>[!BADGE Fuera del horario]{type=Neutral}

Ahora puede duplicar un informe de KPI, tabla o gráfico en un panel de lienzo una vez creado. Una vez duplicado, puede editar el informe según sea necesario antes de guardar.

## Eliminación de opciones de campo de los filtros de informe

>[!NOTE]
>
>Vista previa: 6 de noviembre de 2025
>Versión rápida de producción: 13 de noviembre de 2025
>Producción para todos: 15 de enero de 2026

Se han eliminado las siguientes opciones de campo que anteriormente estaban disponibles al aplicar un filtro a un informe:

* ID de otros grupos
* Identificadores de otros roles
* ID de otros equipos

Se eliminaron debido a problemas asociados con los operadores No es igual a y Está en blanco. Si tiene un filtro existente que utiliza uno de estos campos, seguirá funcionando según lo esperado. Como alternativa, puede seguir utilizando estos campos en <code>textmode</code>, pero se recomienda evitar utilizar los operadores No es igual o Está en blanco al hacerlo.

Las siguientes opciones de campo están disponibles como alternativas:

* Otros grupos: ID
* Otros roles: ID
* Otros equipos: ID

## Se ha mejorado la visualización del recuento de agrupaciones en los paneles de lienzo

>[!NOTE]
>
>Vista previa: 6 de noviembre de 2025
>Versión rápida de producción: 13 de noviembre de 2025
>Producción para todos: 15 de enero de 2026

Cuando un informe de tabla tiene varias páginas de resultados y la tabla está configurada con agrupaciones, la tabla ahora muestra tanto la cantidad de registro de la página actual como el recuento general de registros de todas las páginas. Por ejemplo, si el informe de tabla tiene 7 agrupaciones y la primera página muestra 3, la tabla mostrará 3 de 7.


## Nuevas protecciones para mejorar los tiempos de carga en los paneles de lienzo

>[!NOTE]
>
>Vista previa: 6 de noviembre de 2025
>Versión rápida de producción: 13 de noviembre de 2025
>Producción para todos: 15 de enero de 2026

Para evitar demoras en el tiempo de carga y mejorar el rendimiento general en los paneles de lienzo, hemos aplicado límites en la cantidad de componentes de panel que se pueden agregar a un panel:

* Informes por tablero: límite de 25
* Agrupaciones en vistas de tabla: límite de 5
* Distancia desde el objeto base del informe: límite de 10
* Columnas en una vista de tabla: límite de 25
* Mensajes de filtro de nivel de panel: límite de 10