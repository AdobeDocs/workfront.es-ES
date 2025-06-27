---
title: Mejoras del proyecto del tercer trimestre de 2025
description: Mejoras del proyecto del tercer trimestre de 2025
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 33fa5a61-5300-402c-9f80-f2701f7999a8
source-git-commit: f02a07c0bc4568d7e0fa25ca6e880024423527b7
workflow-type: tm+mt
source-wordcount: '741'
ht-degree: 7%

---

# Mejoras del proyecto del tercer trimestre de 2025

Esta página describe las mejoras del proyecto realizadas con la versión del tercer trimestre de 2025 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del tercer trimestre de 2025, consulte [Información general de la versión del tercer trimestre de 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Se ha reemplazado el campo Horas reales existentes por Horas reales heredadas y se ha creado el nuevo campo Horas reales

>[!NOTE]
>
> Previsualización y producción: 24 de junio de 2025 

Se ha agregado un nuevo campo Horas reales que almacena el tiempo registrado de los proyectos, las tareas y los problemas en horas, con precisión decimal. El campo se almacena en la base de datos de Workfront como `actualWorkRequiredDouble`.

El campo existente de Horas reales ha cambiado a Horas reales heredadas. El campo almacena el tiempo registrado para proyectos, tareas y problemas en minutos y se almacena en la base de datos de Workfront como `actualWorkRequired`.

Los campos Horas reales y Horas reales heredadas están visibles en las vistas e informes de proyectos, tareas y problemas.

El campo Horas reales visible en la sección de detalles del proyecto, tareas y problemas representa las nuevas horas reales.

>[!IMPORTANT]
>
>Dependiendo de cuándo se registraron las horas, podría haber una discrepancia entre las horas reales y las horas reales heredadas de un proyecto, tarea o problema.<br>
>>Se dan los siguientes escenarios:
>
>* Las horas reales representan las horas registradas en los proyectos, las tareas y los problemas desde mayo de 2021.
>* Las horas reales heredadas representan las horas registradas en los proyectos, tareas y problemas durante la duración del proyecto, la tarea o el problema. Esto incluye las horas registradas antes de mayo de 2021 hasta la hora actual.
>  ><br>Es posible que tenga que actualizar los informes para reflejar el nuevo campo y sus valores.
>  ><br>Workfront utiliza las horas reales heredadas para calcular los costes laborales reales.

Para obtener más información, vea [Ver horas reales](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md).


## Cambio en la forma en que se almacenan las horas reales en la base de datos para las llamadas API

>[!NOTE]
>
>* Vista previa: Con la próxima versión de la API, programada para más adelante en 2025
>* Lanzamiento rápido de la producción: con la próxima versión de la API, programada para más adelante en 2025
>* Producción para todos los clientes: con la próxima versión de la API, programada para más adelante en 2025

Esta actualización presenta un cambio en la forma en que se almacenan las horas reales de los proyectos, las tareas y los problemas en la base de datos. A partir de esta actualización, las horas reales utilizarán un campo de valor de `actualWorkRequiredDouble` (con un valor en horas).

Antes de esta actualización, las horas reales se almacenaban con un valor de `actualWorkRequired` (con un valor en minutos). Esta actualización garantizará un recuento más preciso de las horas reales al calcularlas mediante una llamada de API.

Debido a este cambio, es posible que tenga que actualizar cualquier llamada de API que haga referencia al campo de valor original. No debe realizar ningún cambio si utiliza un campo de valor de `actualWorkRequiredExpression` en las llamadas a la API.

Esta actualización no cambia los cálculos de Horas reales para proyectos, tareas y problemas, en columnas de campos personalizados calculados.

## Actualizar en mediante el control deslizante Porcentaje completado de un encabezado de tarea o problema

>[!NOTE]
>
>* Vista previa: miércoles, 27 de mayo de 2025
>* Versión rápida de producción: 27 de mayo de 2025
>* Producción para todos los clientes: 27 de mayo de 2025

Hemos actualizado el modo en que funciona el control deslizante porcentaje completado para tareas y problemas.

Ya está disponible la siguiente funcionalidad:

* Cuando se desliza la burbuja azul Porcentaje completado en el encabezado de una tarea o un problema, el porcentaje completado de la tarea o del problema ahora se actualizará en incrementos de cinco puntos. Antes de esta actualización, al deslizar la burbuja azul Porcentaje completado, se actualizaban las tareas o los problemas en incrementos de un punto.

* Puede hacer doble clic en la burbuja azul y actualizarla manualmente con cualquier número deseado sin utilizar el control deslizante. Esta funcionalidad no ha cambiado.

No se han introducido otros cambios en la actualización del porcentaje completado de tareas y problemas en otras áreas de Workfront.

Para obtener más información, consulte [Ver y actualizar el porcentaje completado de las tareas](/help/quicksilver/manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).

## Mayor transparencia al utilizar el Asistente de IA en proyectos, tareas y problemas

>[!NOTE]
>
>* Vista previa: martes, 19 de mayo de 2025
>* Versión rápida de producción: 19 de mayo de 2025
>* Producción para todos los clientes: 19 de mayo de 2025

Para aclarar cómo AI Assistant encuentra respuestas a preguntas sobre proyectos, tareas y problemas de Workfront, hemos agregado esta información a la respuesta a la pregunta. Ahora, el Asistente de IA incluye su información de búsqueda en la salida. Puede utilizar esta información como una forma de comprobar que AI Assistant identificó correctamente la pregunta que se estaba haciendo y comprender el contexto de la respuesta.

Anteriormente, esta información no estaba disponible en la respuesta del asistente de IA.

Para obtener información sobre cómo usar el Asistente de IA para obtener información sobre los elementos de Workfront, vea [Usar el Asistente de IA para trabajar con proyectos, tareas y problemas](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).
