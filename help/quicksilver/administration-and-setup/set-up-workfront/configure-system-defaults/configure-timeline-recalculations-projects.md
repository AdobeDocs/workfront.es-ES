---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: Configurar el recálculo de cronología para proyectos
description: Recalcular las cronologías permite a los administradores ver cómo las fuerzas de fuera del proyecto están impactando en la cronología del proyecto. La cronología de un proyecto hace referencia a las fechas planificadas y proyectadas del proyecto.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 91%

---

# Configurar el recálculo de cronología para proyectos

Recalcular las cronologías permite a los administradores ver cómo las fuerzas de fuera del proyecto están impactando en la cronología del proyecto. La cronología de un proyecto hace referencia a las fechas planificadas y proyectadas del proyecto.

Como administrador de [!DNL Adobe Workfront], puede recalcular manualmente las cronologías de todos los proyectos del sistema. Los propietarios de proyectos también pueden recalcular manualmente las cronologías de proyectos individuales. Para obtener más información, consulte [Recalcular la cronología de los proyectos](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

Este artículo describe cómo usted, como administrador de [!DNL Workfront], puede determinar cómo y cuándo [!DNL Workfront] calcula automáticamente las cronologías del proyecto mediante la configuración de las preferencias del proyecto en el área [!UICONTROL Configuración].

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar recálculos automáticos

Como administrador de [!DNL Adobe Workfront], puede configurar cuándo [!DNL Workfront] recalcula automáticamente las cronologías del proyecto. [!DNL Workfront] puede recalcular las cronologías del proyecto cada noche o cuando cambie el ámbito del proyecto, o ambas.

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Preferencias del proyecto]** > **[!UICONTROL Proyectos].**

1. En la sección **[!UICONTROL Cronologías]**, habilite o deshabilite una o ambas de las opciones de configuración siguientes. De forma predeterminada, ambas configuraciones están habilitadas.

   * **Todas las noches:** [!DNL Workfront&#x200B;&#x200B;&#x200B;] recalcula las cronologías una vez cada 24 horas, por la noche, solo para los proyectos que tienen el estado [!UICONTROL Actual] y que se han actualizado en los últimos tres meses. Según la carga del sistema y otros factores, la hora de recálculo podría retrasarse más de 24 horas.

     En este caso, [!DNL Workfront] recalcula la cronología de todos los proyectos que tienen el [!UICONTROL Tipo de actualización] definido como [!UICONTROL Automático] o [!UICONTROL Automático y al cambiar].

   * **Cuando cambia el ámbito de un proyecto**: para obtener información sobre lo que constituye un cambio de ámbito del proyecto, consulte [Recalcular la cronología de los proyectos](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

     En este caso, [!DNL Workfront] recalcula la cronología de todos los proyectos que tienen el Tipo de actualización definido como [!UICONTROL Automático y al cambiar] o [!UICONTROL Solo al cambiar].
Para obtener información sobre los tipos de actualización del proyecto, consulte [Información general sobre el tipo de actualización del proyecto](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. Haga clic en **[!UICONTROL Guardar]**.

   La cronología de todos los proyectos del sistema se recalcula automáticamente según el tipo de actualización de cada proyecto.

>[!IMPORTANT]
>
>Para los entornos de vista previa y espacio aislado de actualización personalizado, el recálculo por la noche está deshabilitado y las escalas de tiempo del proyecto no se recalculan automáticamente. Debe recalcular manualmente la cronología del proyecto para los entornos de Vista previa y de la Zona protegida de actualización personalizada. Para obtener más información, consulte [Recalcular líneas de tiempo de proyecto](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md).


## Recalcular cronologías para toda la instancia de [!DNL Workfront]

Puede ejecutar el diagnóstico [!UICONTROL Recalcular cronología] para recalcular manualmente todas las cronologías en el sistema de [!DNL Workfront]. Esto permite a todos los administradores de proyecto ver la influencia de los cambios externos inmediatamente, tanto en las fechas planificadas como en las proyectadas. Para obtener más información, consulte [Usar Diagnósticos para activar procesos automatizados](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
