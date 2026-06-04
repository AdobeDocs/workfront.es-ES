---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Resumen del tipo de actualización del proyecto
description: El tipo de actualización de un proyecto indica cómo calcula Adobe Workfront la escala de tiempo de un proyecto. Los cambios en el plan del proyecto pueden activar cambios en la escala de tiempo del proyecto. La escala de tiempo del proyecto debe recalcularse automática o manualmente para garantizar que esté actualizado con estos cambios.
author: Alina
feature: Work Management
exl-id: a6394961-2ac8-4b95-aa1b-dba8108c612f
TQID: https://experienceleague.adobe.com/bLY-ljw7HxR2kXRpi9jzMkSKbGSKhDrvzogvK5-wZ90
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 520
ht-degree: 69%

---

# Información general sobre los tipos de actualización de un proyecto

El tipo de actualización de un proyecto indica cómo calcula Adobe Workfront la escala de tiempo de un proyecto. Los cambios en el plan del proyecto pueden activar cambios en la escala de tiempo del proyecto. La escala de tiempo del proyecto debe recalcularse automática o manualmente para garantizar que esté actualizado con estos cambios.

Para obtener información sobre cómo recalcular la escala de tiempo del proyecto, consulte [Recalcular las escalas de tiempo del proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

## Tipos de actualización de proyecto

Existen cuatro tipos de actualización para un proyecto, en función de cuándo desee que Workfront recalcule la escala de tiempo del proyecto. Elija un tipo de actualización de la lista siguiente.

Para obtener información sobre cómo actualizar el tipo de actualización del proyecto, consulte [Seleccionar el tipo de actualización del proyecto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

>[!IMPORTANT]
>
>Si la cronología de un proyecto supera los 15 años, Workfront no calcula la cronología automáticamente o al cambiar. El tipo de actualización de un proyecto de más de 15 años siempre es manual.

* **Automático y al cambiar:** Esta es la configuración predeterminada. La cronología del proyecto se actualiza cada vez que se produce un cambio en el proyecto o en otro proyecto del que depende la cronología. La cronología del proyecto también se actualiza cada noche.\
  Esta es la configuración recomendada, ya que garantiza que la cronología del proyecto siempre esté actualizada.

  Al actualizar una tarea o el proyecto y activar un recálculo de la cronología, se muestran inmediatamente todas las fechas disponibles, lo que le permite continuar trabajando. En proyectos con más de 100 tareas, las fechas que requieren cálculos más largos se atenúan.

  ![Fechas atenuadas al editar en línea](assets/dates-dimmed-when-insline-editing-350x146.png)

  Esto indica que el recálculo aún no ha finalizado y que las fechas están sujetas a cambios.

* **Solo cambio:** La escala de tiempo del proyecto se actualiza cada vez que se produce un cambio en el proyecto o en otro proyecto del que depende la escala de tiempo; no se producen actualizaciones programadas.\
  Es posible que desee seleccionar esta opción si le preocupa el rendimiento del sistema y si los cambios rara vez se producen en el proyecto o en otros proyectos de los que depende la escala de tiempo.

* **Solo automático:** La escala de tiempo del proyecto se actualiza cada noche; no se actualiza inmediatamente después de realizar los cambios.\
  Es posible que desee seleccionar esta opción si le preocupa el rendimiento del sistema y si se producen muchos cambios cada día en el proyecto o en otros proyectos de los que depende la cronología.

  >[!NOTE]
  >
  >Un proyecto no se recalcula automáticamente cada noche si se encuentra en estado de Planificación. Solo se recalcula al cambiar.

* **Solo manual:** La escala de tiempo del proyecto solo se actualiza cuando selecciona la opción **Volver a calcular escalas de tiempo**, tal como se describe en la sección &quot;Recalculación manual&quot; del artículo [Volver a calcular escalas de tiempo del proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
  Es posible que desee seleccionar esta opción si realiza muchos cambios en el proyecto al mismo tiempo y desea que el cálculo de la escala de tiempo se produzca después de realizar todos los cambios (en lugar de después de cada cambio individual).
