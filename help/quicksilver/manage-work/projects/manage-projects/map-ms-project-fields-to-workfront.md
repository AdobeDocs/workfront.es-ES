---
product-area: projects
navigation-topic: manage-projects
title: Asignar campos de proyecto de Microsoft a proyectos de Adobe Workfront
description: La mayoría de los proyectos de Adobe Workfront y Microsoft Project son compatibles. Este artículo describe cómo se asignan entre sí los campos de proyecto más comunes de las dos aplicaciones.
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
source-git-commit: c566eb094e96abca6073554433434822c567bc34
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 3%

---

# Asignar campos de proyecto de Microsoft a proyectos de Adobe Workfront

La mayoría de los proyectos de Adobe Workfront y Microsoft Project son compatibles. Con las dos aplicaciones, puede hacer lo siguiente:

* Exportar proyectos de Microsoft Project e importarlos en Workfront
* Exporte proyectos desde Workfront e impórtelos a Microsoft Project. 

Para obtener más información sobre cómo importar proyectos desde un proyecto de Microsoft en Workfront, vea [Importar un proyecto desde un proyecto de Microsoft](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

Para obtener más información sobre cómo exportar un proyecto desde Workfront para importarlo en un proyecto de Microsoft, vea [Exportar un proyecto a un proyecto de Microsoft](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md).

Al realizar estas importaciones de datos, es importante comprender cómo se traduce la información de una aplicación a otra. La mayoría de las veces, tendrá que realizar algunas modificaciones manuales en el proyecto, una vez completada la importación. 

## Información general de asignación de campos

>[!NOTE]
>
>Las fechas planificadas no siempre se corresponden entre ambos sistemas. Las discrepancias se pueden contabilizar a través de la programación y las diferencias en las preferencias del sistema entre Workfront y Microsoft Project. Estas discrepancias de fechas también pueden provocar diferencias en el esfuerzo, la duración y el porcentaje completado.

| **Campo de proyecto de Microsoft** | **Campo de Workfront** |
|---|---|
| Título del proyecto | Nombre del proyecto |
| Fechas de inicio y finalización | Fechas planificadas de inicio y finalización |
| Nombre de la tarea | Nombre de la tarea |
| Duración de la tarea | Duración planificada de la tarea |
| Trabajo de tarea | Horas planificadas para la tarea |
| % de tarea finalizada | % de tarea completada (según la duración de la tarea) |
| Trabajo de tarea % completado | Porcentaje completado de la tarea (según las horas planificadas de la tarea) |
| Inicio y fin programados | Fechas planificadas de inicio y finalización |
| Comienzo y fin reales | Fechas reales de inicio y finalización |
| Nombre del medio | Asignación de tareas |
| Unidades de asignación | Porcentaje de asignación de asignación |
| Nota de tarea | Descripción de tarea |
| Predecesora | Predecesora |

## Información general sobre los datos no incluidos

Hay varios campos de proyecto que no se importan ni exportan desde Workfront.

Estos campos incluyen, entre otros, los siguientes:

* Archivos adjuntos del documento
* Campos personalizados (en los niveles de proyecto o tarea)
* Notas de Workfront
* Problemas
* Retraso negativo en tareas con una relación predecesora de Comienzo/Fin (las tareas se importan sin el retardo)
* Asignaciones
* Restricciones de tarea

  >[!NOTE]
  >
  >Dado que las restricciones no se asignan entre Microsoft Project y Workfront, asegúrese de que haya relaciones de predecesoras entre las tareas. De lo contrario, es posible que las fechas planificadas de inicio y finalización de las tareas no sean precisas en el proyecto importado. 
