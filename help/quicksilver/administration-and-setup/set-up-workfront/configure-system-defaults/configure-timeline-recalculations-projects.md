---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: Configurar cálculos de escala de tiempo para proyectos
description: Volver a calcular las escalas de tiempo permite a los administradores ver cómo las fuerzas fuera del proyecto están impactando en la cronología del proyecto. La cronología de un proyecto hace referencia a las fechas planificadas y proyectadas del proyecto.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 7c2d6d1960752a109c02039c1af8d1d1850bcb8c
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Configurar cálculos de escala de tiempo para proyectos

Volver a calcular las escalas de tiempo permite a los administradores ver cómo las fuerzas fuera del proyecto están impactando en la cronología del proyecto. La cronología de un proyecto hace referencia a las fechas planificadas y proyectadas del proyecto.

Como administrador de [!DNL Adobe Workfront], puede recalcular manualmente las escalas de tiempo de todos los proyectos del sistema. Los propietarios de proyectos también pueden recalcular manualmente las escalas de tiempo para proyectos individuales. Para obtener más información, vea [Volver a calcular escalas de tiempo de proyectos](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

Este artículo describe cómo usted, como administrador de [!DNL Workfront], puede determinar cómo y cuándo [!DNL Workfront] calcula automáticamente las escalas de tiempo del proyecto mediante la configuración de las preferencias del proyecto en el área [!UICONTROL Configuración].

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td><p>Nuevo: [!UICONTROL Standard]</p>
   O
   <p>Actual: [!UICONTROL plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL Administrador del sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar cálculos automáticos

Como administrador de [!DNL Adobe Workfront], puede configurar cuándo [!DNL Workfront] recalcula automáticamente las escalas de tiempo del proyecto. [!DNL Workfront] puede recalcular las escalas de tiempo del proyecto cada noche o cuando cambie el ámbito del proyecto, o ambas cosas.

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Preferencias de proyecto]** > **[!UICONTROL Proyectos].**

1. En la sección **[!UICONTROL Líneas de tiempo]**, habilite o deshabilite una o ambas de las opciones de configuración siguientes. De forma predeterminada, ambas configuraciones están habilitadas.

   * **Todas las noches:** [!DNL Workfront&#x200B;&#x200B;&#x200B;] recalcula las escalas de tiempo una vez cada 24 horas, por la noche, solo para los proyectos que tienen el estado [!UICONTROL Actual] y que se han actualizado en los últimos tres meses. Según la carga del sistema y otros factores, el tiempo de recalculación podría retrasarse más de 24 horas.

     En este caso, [!DNL Workfront] vuelve a calcular la escala de tiempo de todos los proyectos que tienen un [!UICONTROL Tipo de actualización] de [!UICONTROL Automático] o [!UICONTROL Automático y al cambiar].

   * **Cuando cambia el ámbito de un proyecto**: para obtener información acerca de lo que constituye un cambio de ámbito de proyecto, vea [Volver a calcular las escalas de tiempo de un proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

     En este caso, [!DNL Workfront] vuelve a calcular la escala de tiempo de todos los proyectos que tienen un tipo de actualización de [!UICONTROL Automático y al cambiar] o [!UICONTROL Solo al cambiar].
Para obtener información sobre los tipos de actualización del proyecto, vea [Información general sobre el tipo de actualización del proyecto](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. Haga clic en **[!UICONTROL Guardar]**.

   La cronología de todos los proyectos del sistema se vuelve a calcular automáticamente según el tipo de actualización de cada proyecto.

>[!IMPORTANT]
>
>Para los entornos de vista previa y espacio aislado de actualización personalizado, el recálculo por la noche está deshabilitado y las escalas de tiempo del proyecto no se recalculan automáticamente. Debe recalcular manualmente la cronología del proyecto para los entornos de Vista previa y de la Zona protegida de actualización personalizada. Para obtener más información, vea [Volver a calcular escalas de tiempo de proyectos](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md).


## Volver a calcular escalas de tiempo para toda la instancia de [!DNL Workfront]

Puede ejecutar el diagnóstico [!UICONTROL Recalcular escala de tiempo] para recalcular manualmente todas las escalas de tiempo en el sistema [!DNL Workfront]. Esto permite a todos los gestores de proyectos ver la influencia de los cambios externos inmediatamente, tanto en las fechas planificadas como en las proyectadas. Para obtener más información, consulte [Usar diagnósticos para almacenar en déclencheur procesos automatizados](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
