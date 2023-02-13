---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: Configurar nuevos cálculos de cronología para proyectos
description: El cálculo de las líneas de tiempo permite a los administradores ver cómo las fuerzas fuera del proyecto están afectando la cronología del proyecto. La cronología de un proyecto se refiere a las fechas previstas y proyectadas para el proyecto.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# Configurar nuevos cálculos de cronología para proyectos

El cálculo de las líneas de tiempo permite a los administradores ver cómo las fuerzas fuera del proyecto están afectando la cronología del proyecto. La cronología de un proyecto se refiere a las fechas previstas y proyectadas para el proyecto.

Como [!DNL Adobe Workfront] administrador, puede volver a calcular manualmente las líneas de tiempo de todos los proyectos del sistema. Los propietarios del proyecto también pueden volver a calcular manualmente las cronologías de los proyectos individuales. Para obtener más información, consulte [Volver a calcular las líneas de tiempo del proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

Este artículo describe cómo, como [!DNL Workfront] administrador, puede determinar cómo y cuándo [!DNL Workfront] calcula automáticamente las líneas de tiempo del proyecto configurando las preferencias del proyecto en la variable [!UICONTROL Configuración] .

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
   <td> <p>Nivel de acceso del administrador del sistema</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar nuevos cálculos automáticos

Como [!DNL Adobe Workfront] administrador, puede configurar cuando [!DNL Workfront] vuelve a calcular automáticamente las líneas de tiempo del proyecto. [!DNL Workfront] puede volver a calcular las líneas de tiempo del proyecto cada noche o cuando cambie el ámbito del proyecto, o ambas cosas.

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Preferencias de proyecto]** > **[!UICONTROL Proyectos].**

1. En el **[!UICONTROL Líneas de tiempo]** , habilite o deshabilite una o las dos opciones de configuración siguientes. De forma predeterminada, ambas configuraciones están habilitadas.

   * **Cada noche:** [!DNL Workfront&#x200B;&#x200B;&#x200B;] vuelve a calcular las líneas de tiempo por la noche solo para los proyectos que tienen un estado de [!UICONTROL Actual] y se han actualizado en los últimos tres meses.

      En este caso, [!DNL Workfront] vuelve a calcular la cronología de todos los proyectos que tienen un [!UICONTROL Tipo de actualización] de [!UICONTROL Automático] o [!UICONTROL Automático y en cambio].

   * **Cuando cambia el ámbito de un proyecto**: Para obtener información sobre lo que constituye un cambio en el ámbito de un proyecto, consulte [Volver a calcular las líneas de tiempo del proyecto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

      En este caso, [!DNL Workfront] vuelve a calcular la cronología de todos los proyectos que tienen un tipo de actualización de [!UICONTROL Automático y en cambio] o [!UICONTROL Solo cambio].
Para obtener información sobre los tipos de actualización del proyecto, consulte [Información general sobre el tipo de actualización del proyecto](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. Haga clic en **[!UICONTROL Guardar]**.

   La cronología de todos los proyectos del sistema se vuelve a calcular automáticamente en función del tipo de actualización de cada proyecto.

## Volver a calcular las líneas de tiempo para todo [!DNL Workfront] instancia

Puede ejecutar el [!UICONTROL Volver a calcular línea de tiempo] diagnóstico para volver a calcular manualmente todas las líneas de tiempo en el [!DNL Workfront] sistema. Esto permite a todos los administradores de proyectos ver la influencia de los cambios externos inmediatamente en las fechas planificadas y proyectadas. Para obtener más información, consulte [Usar diagnósticos para déclencheur de procesos automatizados](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
