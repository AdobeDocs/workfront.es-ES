---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Agregar historias a una iteración existente
description: Puede añadir historias a una iteración de muchas maneras.
author: Courtney
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/dOaVAx6iEbdP-hzSgKpS8drVTtmmhG-rjvZIsN19RH8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 568
ht-degree: 81%

---

# Añadir usuarios a una iteración existente

Puede añadir historias a una iteración de cualquiera de las siguientes maneras:

* Del registro de pendientes una vez creada la iteración, como se describe en la sección [Mover historias del registro de pendientes a una iteración o [!UICONTROL Panel Kanban]](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#move-stories-from-the-backlog-to-an-iteration-or--board) de [Administrar el registro de pendientes Agile](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* Desde la página [!UICONTROL Detalles] de la tarea o problema individual
* Desde una lista de tareas o problemas
* Desde un informe
* Desde un panel de control

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p> 
   <p>Trabajo o superior</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Administrar el acceso al proyecto en el que se encuentra la historia </td> 
  </tr>
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Comprender cómo afecta la adición de historias a las fechas de las tareas

De manera predeterminada, cuando añade una tarea existente a una iteración, la [!UICONTROL Fecha de inicio planificada] y la [!UICONTROL Fecha de finalización planificada] de la tarea se establecen de la siguiente manera:

### [!UICONTROL Fecha de inicio planificada] de la tarea

* La tarea utiliza la fecha de inicio de la iteración cuando:

   * El proyecto no tiene una [!UICONTROL fecha de inicio planificada] establecida.
   * La [!UICONTROL fecha planificada de inicio] del proyecto es *antes de* o *en* la fecha de inicio de la iteración.

* La tarea utiliza la [!UICONTROL fecha de inicio planificada] del proyecto cuando:

   * La [!UICONTROL fecha planificada de inicio] del proyecto es *después* de la fecha de inicio de la iteración.

### [!UICONTROL Fecha planificada de finalización] de la tarea

* La tarea utiliza la fecha de finalización de la iteración cuando:

   * El proyecto no tiene [!UICONTROL fecha planificada de finalización] establecida.
   * La [!UICONTROL fecha planificada de inicio] del proyecto es *antes o en* la fecha de inicio de la iteración o la [!UICONTROL fecha planificada de finalización] del proyecto es *antes o en* la fecha de finalización de la iteración.

* La tarea utiliza la [!UICONTROL fecha planificada de finalización] del proyecto cuando:

   * La [!UICONTROL fecha planificada de inicio] del proyecto es *después de* la fecha de inicio de la iteración y la [!UICONTROL fecha planificada de finalización] del proyecto es *después* de la fecha de finalización de la iteración.

Puede configurar equipos de Scrum individuales para que utilicen las fechas del proyecto de forma predeterminada, en lugar de las fechas de iteración. Para obtener más información, consulte la sección [Configurar cómo se aplican las fechas al añadir elementos de trabajo a una iteración](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) en el artículo [Configurar Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Añadir un artículo a una iteración existente

Puede añadir cualquier tarea o problema a cualquier iteración si tiene acceso de Administración al proyecto. Tenga en cuenta lo siguiente al mover una tarea o un problema a una iteración:

* Si añade varios equipos, la tarea o el problema solo se pueden mostrar en la iteración de un equipo. Esta es la iteración que elige en el paso tres siguiente.
* Si la tarea o el problema se asignan a un equipo Agile y se mueven a la iteración de otro equipo, la asignación del equipo no cambia.
* Si la tarea o el problema no se han asignado a un equipo, se asignará al equipo propietario de la iteración.
* No se pueden añadir tareas principales a la iteración. Si añade tareas secundarias, la tarea principal aparece en el tablero de Scrum como un carril.

>[!IMPORTANT]
>
>Una vez que la tarea pasa a la iteración, no se puede actualizar el [!UICONTROL Tipo de duración] ni la [!UICONTROL Restricción de tarea]. El [!UICONTROL Tipo de duración] está establecido en [!UICONTROL Simple] y la [!UICONTROL Restricción de tarea] está establecida en [!UICONTROL Fechas fijas] para mantener la escala de tiempo de la tarea coherente con la escala de tiempo de la iteración.

1. Abra la tarea o el problema que desee agregar a una iteración.
O
Vaya al proyecto, informe o panel que contiene la tarea o el problema que desea agregar a una iteración. A continuación, seleccione una o varias tareas o problemas.

1. Haga clic en **[!UICONTROL Más]** ![Icono de más](assets/more-icon.png) > **[!UICONTROL Agregar a la iteración]**.
No puede asignar tareas o problemas asignados a equipos que no sean de Agile.

1. En el cuadro **[!UICONTROL Agregar a]**, empiece a escribir el nombre de la iteración y selecciónela cuando aparezca en la lista.

   >[!NOTE]
   >
   >Puede trasladar una historia de una iteración existente a otra nueva.

1. Haga clic en **[!UICONTROL Add]**.
