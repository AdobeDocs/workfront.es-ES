---
product-area: projects
navigation-topic: manage-projects
title: Asignar campos de proyecto de Microsoft a proyectos de Adobe Workfront
description: La mayoría de los proyectos de Adobe Workfront y Microsoft Project son compatibles. Este artículo describe cómo se asignan entre sí los campos de proyecto más comunes de las dos aplicaciones.
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
TQID: https://experienceleague.adobe.com/WdFf5O8kKyY43PsHLEINDaLzsEa0idHZPNz83O12bTI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 396
ht-degree: 84%

---

# Asignar campos de proyecto de Microsoft a proyectos de Adobe Workfront

La mayoría de los proyectos de Adobe Workfront y Microsoft Project son compatibles. Con las dos aplicaciones, puede hacer lo siguiente:

* Exportar proyectos de Microsoft Project e importarlos a Workfront
* Exportar proyectos de Workfront e importarlos a Microsoft Project

Para obtener más información sobre cómo importar proyectos de Microsoft Project a Workfront, consulte [Importar un proyecto de Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

Para obtener más información sobre cómo exportar un proyecto de Workfront para importarlo a Microsoft Project, consulte [Exportar un proyecto a Microsoft Project](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md).

Al realizar estas importaciones de datos, es importante comprender cómo se traduce la información de una aplicación a otra. La mayoría de las veces, tendrá que realizar algunas modificaciones manuales en el proyecto una vez completada la importación.

## Información general de asignación de campos

>[!NOTE]
>
>Las fechas planificadas no siempre se corresponden entre ambos sistemas. Las discrepancias se pueden contabilizar a través de la programación y las diferencias en las preferencias del sistema entre Workfront y Microsoft Project. Estas discrepancias de fechas también pueden provocar diferencias en el esfuerzo, la duración y el porcentaje completado.

| **Campo de Microsoft Project** | **Campo de Workfront** |
|---|---|
| Título del proyecto | Nombre del proyecto |
| Fecha de inicio y finalización | Fechas planificadas de inicio y finalización |
| Nombre de la tarea | Nombre de la tarea |
| Duración de la tarea | Duración planificada de la tarea |
| Trabajo de tarea | Horas planificadas de la tarea |
| % de tarea finalizada | Porcentaje completado de la tarea (según la duración de la tarea) |
| Trabajo de tarea % completado | Porcentaje completado de la tarea (según las horas planificadas de la tarea) |
| Inicio y finalización planificados | Fechas planificadas de inicio y finalización |
| Comienzo y fin reales | Fechas reales de inicio y finalización |
| Nombre del recurso | Asignación de una tarea |
| Unidades de asignación | Porcentaje de asignación |
| Nota de la tarea | Descripción de la tarea |
| Predecesora | Predecesora |

## Información general sobre los datos no incluidos

Hay varios campos de proyecto que no se importan ni exportan desde Workfront.

Estos campos incluyen, entre otros, los siguientes:

* Archivos adjuntos del documento
* Campos personalizados (en los niveles de proyecto o tarea)
* Notas de Workfront
* Problemas
* Retraso negativo en tareas con una relación predecesora de Inicio/Fin (las tareas se importan sin el retardo)
* Asignaciones
* Restricciones de tareas

  >[!NOTE]
  >
  >Dado que las restricciones no se asignan entre Microsoft Project y Workfront, asegúrese de que haya relaciones de predecesoras entre las tareas. De lo contrario, es posible que las fechas planificadas de inicio y finalización de las tareas no sean precisas en el proyecto importado.
