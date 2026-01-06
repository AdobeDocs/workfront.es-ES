---
title: Priorizar proyectos en optimizador de portafolios
product-area: portfolios;projects
navigation-topic: portfolio-optimizer
description: Puede priorizar los proyectos en el optimizador de portafolios para establecer el orden en que se deben completar.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 54e33746-5995-49de-8e21-bf973f0694a6
source-git-commit: 714e6e09f1429f0382c36d17d3f2aca95edcfbc6
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 93%

---

# Priorizar proyectos en [!UICONTROL Optimizador de portafolios]

Puede priorizar sus proyectos en [!UICONTROL Optimizador de portafolios] para establecer el orden en que se deben completar.

Tenga en cuenta lo siguiente al usar [!UICONTROL Optimizador de portafolios]:

* Los proyectos de la parte superior de [!UICONTROL Optimizador de portafolios] se consideran más importantes que los que aparecen en la parte inferior. Tendrá que completar los proyectos en orden de prioridad en [!UICONTROL Optimizador de portafolios] para que el portafolio se optimice.
* La prioridad de los proyectos de [!UICONTROL Optimizador de portafolios] no está relacionada con el campo [!UICONTROL Prioridad] ubicado en la ficha [!UICONTROL Detalles del proyecto] de un proyecto.

  El campo [!UICONTROL Prioridad] de la ficha [!UICONTROL Detalles del proyecto] es un indicador visual que se especifica manualmente para comprender la importancia que debe tener un proyecto.

* La prioridad de los proyectos en optimizador de portafolios es visible en [!DNL Resource Planner], si está habilitada allí. En [!DNL Resource Planner], los proyectos reciben recursos en el orden de prioridad de [!UICONTROL Planificador de recursos], y no en la de [!UICONTROL Prioridad de Portafolio].

  Para obtener información sobre cómo priorizar proyectos en [!UICONTROL Resource Planner], consulte el artículo [Priorizar proyectos en [!UICONTROL Planificador de recursos]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

* El área de **[!UICONTROL Priorización de proyectos]** de [!UICONTROL Optimizador de portafolios] muestra los proyectos en el orden de [!UICONTROL Fechas de inicio planificadas] y [!UICONTROL Valor neto] de forma predeterminada.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] paquete</td> 
   <td> <p>Workfront Prime o superior</p>
      <p>Flujo de trabajo Prime o superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de [!UICONTROL Edit] a [!UICONTROL Portfolios] y [!UICONTROL Proyectos]</p>  </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de [!UICONTROL Manage] al portafolio</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso para la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses*</td> 
   <td> <p>New: Standard</p>
   <p>Current: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[!UICONTROL Edit] access to Projects and Portfolios</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>Contribute or higher permissions to the projects</p> 
   <p>You must have Manage permissions to all the projects in the list to be able to use <b>Set project priority</b>.</p>
    </td> 
  </tr> 
 </tbody> 
</table>-->

## Cambiar la prioridad de los proyectos en [!UICONTROL Optimizador de portafolios]

{{step1-to-portfolios}}

1. (Opcional) Seleccione el filtro correcto en el menú desplegable **[!UICONTROL Filtro]** para ver la lista correcta de portafolios.
1. Haga clic en el nombre de un portafolio para abrirla.
1. Haga clic en **[!UICONTROL Optimización de carteras]** en el panel de navegación izquierdo.
1. En el área [!UICONTROL Optimización del proyecto], modifique la prioridad de sus proyectos arrastrando los proyectos en orden de prioridad y soltándolos en la posición de visualización deseada.

   ![Optimizador de Portfolio con proyectos](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

   Haga clic en **[!UICONTROL Establecer prioridad]** en el área de optimización del proyecto cuando termine de reorganizar los proyectos. Los proyectos recibirán un nuevo número en función del nuevo pedido.

1. Haga clic en **[!UICONTROL Guardar]** para guardar la nueva prioridad de proyecto en [!UICONTROL Optimizador de portafolios]. La prioridad aparece como un número en la columna número **#**.

   >[!TIP]
   >
   >Esto no cambia necesariamente el orden de los proyectos en [!UICONTROL Optimizador de portafolios], ya que la lista de proyectos puede ordenarse por una columna distinta a la columna **#**. Haga clic en el encabezado de columna **#** para ordenar la lista por prioridad de proyecto.

   Puede ver la prioridad del proyecto tal como aparece en [!UICONTROL Optimizador de portafolios] en el Planificador de recursos, habilitando la configuración **[!UICONTROL Mostrar prioridades de Portafolio]** en el Planificador de recursos.

   Para obtener información sobre cómo priorizar proyectos en [!UICONTROL Planificador de recursos], consulte el artículo [Priorizar proyectos en [!UICONTROL Planificador de recursos]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).
