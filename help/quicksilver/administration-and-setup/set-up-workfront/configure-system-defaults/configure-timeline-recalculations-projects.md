---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: Configurar cálculos de escala de tiempo para proyectos
description: Volver a calcular las escalas de tiempo permite a los administradores ver cómo las fuerzas fuera del proyecto están impactando en la cronología del proyecto. La cronología de un proyecto hace referencia a las fechas planificadas y proyectadas del proyecto.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 4705c3fc76c1544f8c71e70a773432f164282abb
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# Configurar cálculos de escala de tiempo para proyectos

Volver a calcular las escalas de tiempo permite a los administradores ver cómo las fuerzas fuera del proyecto están impactando en la cronología del proyecto. La cronología de un proyecto hace referencia a las fechas planificadas y proyectadas del proyecto.

Como un [!DNL Adobe Workfront] administrador, puede recalcular manualmente las escalas de tiempo para todos los proyectos del sistema. Los propietarios de proyectos también pueden recalcular manualmente las escalas de tiempo para proyectos individuales. Para obtener más información, consulte [Recalcular escalas de tiempo del proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

Este artículo describe cómo, como [!DNL Workfront] administrador, puede determinar cómo y cuándo [!DNL Workfront] calcula automáticamente las escalas de tiempo del proyecto configurando las preferencias del proyecto en [!UICONTROL Configurar] área.

## Requisitos de acceso

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
   <td> <p>Nivel de acceso de administrador del sistema</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo [!DNL Workfront] El administrador puede modificar su nivel de acceso. Consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar cálculos automáticos

Como un [!DNL Adobe Workfront] administrador, puede configurar cuando [!DNL Workfront] recalcula automáticamente las escalas de tiempo del proyecto. [!DNL Workfront] Puede recalcular las escalas de tiempo del proyecto cada noche, cuando cambie el ámbito del proyecto o ambas cosas.

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha, o la [!UICONTROL **Menú principal**] icono ![](assets/lines-main-menu.png) en la esquina superior izquierda de [!DNL Workfront], si está disponible, haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Clic **[!UICONTROL Preferencias de proyecto]** > **[!UICONTROL Proyectos].**

1. En el **[!UICONTROL Cronología]** , habilite o deshabilite una o ambas de las opciones de configuración siguientes. De forma predeterminada, ambas configuraciones están habilitadas.

   * **Cada noche:** [!DNL Workfront&#x200B;&#x200B;&#x200B;] recalcula las escalas de tiempo una vez cada 24 horas, por la noche, solo para los proyectos con un estado de [!UICONTROL Actual] y que se han actualizado en los últimos tres meses. Según la carga del sistema y otros factores, el tiempo de recalculación podría retrasarse más de 24 horas.

     En este caso, [!DNL Workfront] vuelve a calcular la escala de tiempo de todos los proyectos que tienen un [!UICONTROL Tipo de actualización] de [!UICONTROL Automático] o [!UICONTROL Automático y al cambiar].

   * **Cuando cambie el ámbito de un proyecto**: para obtener información sobre lo que constituye un cambio en el ámbito del proyecto, consulte [Recalcular escalas de tiempo del proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

     En este caso, [!DNL Workfront] vuelve a calcular la escala de tiempo de todos los proyectos que tienen un tipo de actualización de [!UICONTROL Automático y al cambiar] o [!UICONTROL Solo al cambiar].
Para obtener información sobre los tipos de actualización del proyecto, consulte [Resumen del tipo de actualización del proyecto](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. Haga clic en **[!UICONTROL Guardar]**.

   La cronología de todos los proyectos del sistema se vuelve a calcular automáticamente según el tipo de actualización de cada proyecto.

## Volver a calcular las escalas de tiempo para todo [!DNL Workfront] instancia

Puede ejecutar el [!UICONTROL Recalcular escala de tiempo] diagnóstico para recalcular manualmente todas las escalas de tiempo en [!DNL Workfront] sistema. Esto permite a todos los gestores de proyectos ver la influencia de los cambios externos inmediatamente, tanto en las fechas planificadas como en las proyectadas. Para obtener más información, consulte [Utilice Diagnóstico para almacenar en déclencheur los procesos automatizados](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
