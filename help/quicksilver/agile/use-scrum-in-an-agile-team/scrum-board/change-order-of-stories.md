---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Cambiar el orden de las historias en el panel de exploración
description: El orden en que aparecen las historias en el tablero de historias no indica la prioridad de las mismas. Sin embargo, esto puede afectar a la prioridad percibida al hacer que las historias sean más visibles. De manera predeterminada, las historias se muestran en orden alfabético dentro de cada columna de [!UICONTROL estado] en el tablero de historias.
author: Courtney
feature: Agile
exl-id: 326d78e0-06de-4b98-8fa6-102e0fd89d76
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Vy3r2L1yuMPvMesRxEohYAgA6geAlKYIRsstLp1kpt8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 401
ht-degree: 73%

---

# Cambiar el orden de las historias en el tablero de [!UICONTROL Scrum]

El orden en que aparecen las historias en el tablero de historias no indica la prioridad de las mismas. Sin embargo, esto puede afectar a la prioridad percibida al hacer que las historias sean más visibles. La prioridad se define en el registro de pendientes y, cuando las historias se llevan al guion gráfico, no tienen una prioridad establecida, porque se trabajará en ellas durante el lapso de tiempo de la iteración. Si las historias vuelven al registro de pendientes, puede reordenarlas allí para mostrar la prioridad.

De manera predeterminada, las historias se muestran en orden alfabético dentro de cada columna de estado en el tablero de historias. Las historias con calles de baño se muestran en la parte superior del guion gráfico, y las historias sin calles de baño se muestran por separado debajo de cualquier calle de baño.

Cuando reordena columnas en el tablero de historias, los cambios que realice se guardarán en la iteración o en el proyecto, por lo que se conservarán la próxima vez que usted u otro usuario consulten el tablero de historias. (Los cambios que realice no se revertirán al borrar la caché del explorador).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td> <p>Nuevo: [!UICONTROL Standard]</p> 
   o
   <p>Actual: [!UICONTROL Work] o superior</p> </td> 
  </tr>
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Cambiar el orden de las historias en una iteración

{{step1-to-team}}

1. (Opcional) Haga clic en el icono **[!UICONTROL Cambiar de equipo]** ![icono Cambiar de equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo de Scrum en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Vaya a la iteración o al proyecto que contiene las historias que desea reordenar.
1. Arrastre una tarjeta de historia o un diagrama de flujo a la ubicación vertical deseada dentro de una columna de estado del panel de la historia.

## Cambiar el orden de las historias en un proyecto

A diferencia de las iteraciones de Agile, no se puede cambiar el orden de los artículos al ver un proyecto en una vista de Agile. Para modificar el orden de las historias de un proyecto, debe ver el proyecto en una vista estándar.

Para obtener información sobre cómo cambiar la vista del proyecto, consulte [[!UICONTROL Administrar un proyecto] en la vista de [!UICONTROL Agile]](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md). En lugar de seleccionar una vista de Agile, seleccione una vista estándar.
