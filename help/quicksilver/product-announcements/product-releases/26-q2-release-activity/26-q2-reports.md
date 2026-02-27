---
title: Mejoras en los informes del segundo trimestre de 2026
description: Mejoras en los informes del segundo trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bc2fee9-fa86-41c7-80e7-44bf3e8077d8
source-git-commit: aceb9f7bd6c62036838b15d74ee2a9b7843e5c11
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 16%

---

# Mejoras en los informes del segundo trimestre de 2026

Esta página describe las mejoras de los informes realizadas con la versión del segundo trimestre de 2026 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del segundo trimestre de 2026, consulte [Información general de la versión del segundo trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Etiquetas de campo personalizado que se muestran al crear informes

>[!NOTE]
>
>Vista previa: 26 de febrero de 2026
>Versión rápida de producción: viernes, 12 de marzo de 2026
>Producción para todos: viernes, 16 de abril de 2026

La etiqueta de campo personalizado ahora se muestra antes del nombre del campo y el objeto en las herramientas de creación de informes, lo que le ayuda a localizar los campos con mayor facilidad. Las etiquetas de campo también se muestran al definir filtros, vistas y agrupaciones en listas.

La etiqueta de campo personalizado está diseñada para la interfaz del sistema, mientras que el nombre del campo se utiliza frecuentemente para fines de API y almacenamiento back-end, y puede no ser tan útil al localizar un campo.

Para obtener más información, consulte [Crear un informe personalizado](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Carpetas de informe compartibles

>[!NOTE]
>
>Vista previa: 26 de febrero de 2026
>Versión rápida de producción: viernes, 12 de marzo de 2026
>Producción para todos: viernes, 16 de abril de 2026

Ahora puede organizar y compartir informes utilizando carpetas de informes que se pueden compartir. Esta nueva función ayuda a los equipos que administran grandes volúmenes de informes a mantener un control de acceso escalable y coherente:

* **Crear estructuras de carpetas organizadas**: los administradores del sistema pueden crear carpetas de nivel superior y los usuarios con acceso de administración pueden crear subcarpetas de hasta 4 niveles de profundidad.
* **Controles granulares de permisos**: Comparta carpetas con dos niveles de permisos:
   * Ver: Los usuarios pueden abrir informes y compartir carpetas
   * Administrar: los usuarios pueden editar los detalles de la carpeta, agregar o quitar elementos y recibir automáticamente acceso de administración a todos los informes de la carpeta
* **Permisos heredados**: los permisos se aplican en cascada desde las carpetas principales a todas las subcarpetas e informes del árbol de carpetas
* **Experiencia de lista mejorada**: Cuando habilite carpetas compartibles, tendrá acceso a la experiencia de lista mejorada. Para obtener más información, consulte [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


Para obtener más información, consulte [Usar carpetas de informes que se pueden compartir](/help/quicksilver/reports-and-dashboards/reports/report-usage/use-sharable-report-folders.md).

## Etiquetas de fecha mejoradas para agrupaciones de gráficos en paneles de lienzo

>[!NOTE]
>
>Vista previa: 26 de febrero de 2026
>Versión rápida de producción: viernes, 12 de marzo de 2026
>Producción para todos: viernes, 16 de abril de 2026

>[!NOTE]
>
>Paneles de lienzo se encuentra en la versión beta.

Los gráficos que agrupan datos por fecha ahora muestran etiquetas de fecha más claras y legibles. Con esta actualización, las etiquetas de fecha se ajustan dinámicamente en función de la opción Agrupar por seleccionada, como día, semana, mes o año, lo que facilita la lectura e interpretación rápida de los gráficos:

<table> <tbody> <tr> <td>Day</td> <td>Muestra la fecha completa. Ejemplo: 12/3/2026</td> </tr> <tr> <td>Semana</td> <td>Muestra una fecha de inicio de semana con formato. Por ejemplo, 8 de marzo de 2026</td> </tr> <tr> <td>Mes</td> <td>Muestra el mes y el año. Ejemplo de marzo de 2026</td> </tr> <tr> <td>Año</td> <td>Muestra solo el año. Ejemplo: 2026</td> </tr> </tbody> </table>

Anteriormente, las agrupaciones de gráficos siempre mostraban la fecha de inicio del período seleccionado en formato numérico.
