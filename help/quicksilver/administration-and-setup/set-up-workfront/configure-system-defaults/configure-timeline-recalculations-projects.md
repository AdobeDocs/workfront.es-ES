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
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Configurar cálculos de escala de tiempo para proyectos

Volver a calcular las escalas de tiempo permite a los administradores ver cómo las fuerzas fuera del proyecto están impactando en la cronología del proyecto. La cronología de un proyecto hace referencia a las fechas planificadas y proyectadas del proyecto.

Como administrador de [!DNL Adobe Workfront], puede recalcular manualmente las escalas de tiempo de todos los proyectos del sistema. Los propietarios de proyectos también pueden recalcular manualmente las escalas de tiempo para proyectos individuales. Para obtener más información, vea [Volver a calcular escalas de tiempo de proyectos](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

Este artículo describe cómo usted, como administrador de [!DNL Workfront], puede determinar cómo y cuándo [!DNL Workfront] calcula automáticamente las escalas de tiempo del proyecto mediante la configuración de las preferencias del proyecto en el área [!UICONTROL Configuración].

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente para realizar los pasos de este artículo:

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Nivel de acceso de administrador del sistema</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

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

## Volver a calcular escalas de tiempo para toda la instancia de [!DNL Workfront]

Puede ejecutar el diagnóstico [!UICONTROL Recalcular escala de tiempo] para recalcular manualmente todas las escalas de tiempo en el sistema [!DNL Workfront]. Esto permite a todos los gestores de proyectos ver la influencia de los cambios externos inmediatamente, tanto en las fechas planificadas como en las proyectadas. Para obtener más información, consulte [Usar diagnósticos para almacenar en déclencheur procesos automatizados](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
