---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Información general sobre el tipo de actualización del proyecto
description: El tipo de actualización de un proyecto indica cómo calcula Adobe Workfront la cronología de un proyecto. Los cambios en el plan del proyecto podrían déclencheur los cambios en la cronología del proyecto. La línea de tiempo del proyecto debe recalcularse automática o manualmente para asegurarse de que está actualizada con estos cambios.
author: Alina
feature: Work Management
exl-id: a6394961-2ac8-4b95-aa1b-dba8108c612f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Información general sobre el tipo de actualización del proyecto

El tipo de actualización de un proyecto indica cómo calcula Adobe Workfront la cronología de un proyecto. Los cambios en el plan del proyecto podrían déclencheur los cambios en la cronología del proyecto. La línea de tiempo del proyecto debe recalcularse automática o manualmente para asegurarse de que está actualizada con estos cambios.

Para obtener información sobre cómo volver a calcular la cronología del proyecto, consulte [Volver a calcular las líneas de tiempo del proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

## Tipos de actualización de proyecto

Hay cuatro tipos de actualización para un proyecto, según cuándo desee que Workfront vuelva a calcular la cronología del proyecto. Elija un tipo de actualización en la lista siguiente.

Para obtener información sobre cómo actualizar el tipo de actualización del proyecto, consulte [Seleccione el tipo de actualización del proyecto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

>[!IMPORTANT]
>
>Si la escala de tiempo de un proyecto supera los 15 años, Workfront no calcula la escala de tiempo automáticamente ni si cambia. El tipo de actualización de un proyecto que dure más de 15 años siempre es manual.

* **Automático y en cambio:** Esta es la configuración predeterminada. La cronología del proyecto se actualiza cada vez que se produce un cambio en el proyecto o en otro proyecto del que depende la cronología. La cronología del proyecto también se actualiza cada noche. \
   Esta es la configuración recomendada, ya que garantiza que la cronología del proyecto esté siempre actualizada.

   Cuando se actualiza una tarea o el proyecto y se genera un déclencheur para un nuevo cálculo de la cronología, todas las fechas disponibles se muestran inmediatamente, lo que le permite continuar trabajando. En los proyectos con más de 100 tareas, las fechas que requieren cálculos más largos aparecen atenuadas.

   ![](assets/dates-dimmed-when-insline-editing-350x146.png)

   Esto indica que el nuevo cálculo aún no ha finalizado y que las fechas están sujetas a cambios.

* **Cambiar solo:** La cronología del proyecto se actualiza cada vez que se produce un cambio en el proyecto o en otro proyecto del que depende la cronología; no se producen actualizaciones programadas.\
   Es posible que desee seleccionar esta opción si le preocupa el rendimiento del sistema y si los cambios raramente se producen en el proyecto o en otros proyectos de los que depende la cronología.

* **Solo automático:** La cronología del proyecto se actualiza cada noche; no se actualiza inmediatamente después de realizar los cambios.\
   Es posible que desee seleccionar esta opción si le preocupa el rendimiento del sistema y si se producen muchos cambios cada día en el proyecto o en otros proyectos de los que depende la cronología.

   >[!NOTE]
   >
   >Un proyecto no se vuelve a calcular automáticamente cada noche si está en estado de Planning. Solo se vuelve a calcular al cambiar.

* **Sólo manual:** La cronología del proyecto solo se actualiza cuando selecciona la opción para **Volver a calcular las líneas de tiempo**, tal como se describe en la sección &quot;Cálculo manual&quot; del artículo [Volver a calcular las líneas de tiempo del proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
   Es posible que desee seleccionar esta opción si está realizando muchos cambios en el proyecto al mismo tiempo y desea que el cálculo de la cronología se produzca después de que se hayan realizado todos los cambios (en lugar de después de cada cambio individual).
