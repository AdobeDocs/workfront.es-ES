---
product-area: projects
navigation-topic: manage-projects
title: Asignación de campos de proyecto de Microsoft a proyectos de Adobe Workfront
description: La mayoría de los proyectos de Adobe Workfront y Microsoft Project son compatibles. Este artículo describe cómo los campos de proyecto más comunes de las dos aplicaciones se asignan entre sí.
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
source-git-commit: c566eb094e96abca6073554433434822c567bc34
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 3%

---

# Asignación de campos de proyecto de Microsoft a proyectos de Adobe Workfront

La mayoría de los proyectos de Adobe Workfront y Microsoft Project son compatibles. Con las dos aplicaciones, puede hacer lo siguiente:

* Exportar proyectos de Microsoft Project e importarlos en Workfront
* Exporte proyectos desde Workfront e impórtelos en Microsoft Project. 

Para obtener más información sobre la importación de proyectos de Microsoft Project a Workfront, consulte [Importar un proyecto desde un proyecto de Microsoft](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

Para obtener más información sobre cómo exportar un proyecto desde Workfront para importarlo a un proyecto de Microsoft, consulte [Exportar un proyecto a un proyecto de Microsoft](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md).

Al realizar estas importaciones de datos, es importante comprender cómo se traduce la información de una aplicación a otra. La mayoría de las veces, tendrá que realizar algunas modificaciones manuales en el proyecto una vez completada la importación. 

## Información general sobre la asignación de campos

>[!NOTE]
>
>Las fechas planificadas no siempre se corresponden entre ambos sistemas. Las discrepancias se pueden contabilizar a través de la programación y las diferencias en las preferencias del sistema entre Workfront y Microsoft Project. Estas discrepancias de fechas también pueden provocar diferencias en el esfuerzo, la duración y el porcentaje completado.

| **Campo de proyecto de Microsoft** | **Campo Workfront** |
|---|---|
| Título del proyecto | Nombre del proyecto |
| Fechas de inicio y finalización | Fechas de inicio y finalización previstas |
| Nombre de la tarea | Nombre de la tarea |
| Duración de la tarea | Duración planificada de la tarea |
| Trabajo de tareas | Horas planificadas para la tarea |
| Tarea % completada | Tarea % completado (según la duración de la tarea) |
| Trabajo de tarea % completado | Tarea % completado (según las horas previstas de la tarea) |
| Inicio y finalización programados | Fechas de inicio y finalización previstas |
| Inicio y fin reales | Fechas reales de inicio y finalización |
| Nombre del recurso | Asignación de tarea |
| Unidades de asignación | Porcentaje de asignación de asignaciones |
| Nota de tarea | Descripción de tarea |
| Predecesora | Predecesora |

## Información general sobre los datos que no se incluyen

Hay varios campos de proyecto que no se importan ni exportan desde Workfront.

Estos campos incluyen, entre otros, los siguientes:

* Documentos adjuntos
* Campos personalizados (en los niveles de proyecto o tarea)
* Notas de Workfront
* Problemas
* Retraso negativo en tareas con una relación predecesora Start/Finish (las tareas se importan sin retraso)
* Asignaciones
* Restricciones de tareas

   >[!NOTE]
   Dado que las restricciones no se asignan entre Microsoft Project y Workfront, asegúrese de que haya relaciones predecesoras entre las tareas. De lo contrario, es posible que las fechas de inicio y finalización planificadas de las tareas no sean exactas en el proyecto importado. 
