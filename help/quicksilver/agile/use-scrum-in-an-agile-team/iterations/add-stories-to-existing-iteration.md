---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Agregar historias a una iteración existente
description: Puede añadir historias a una iteración de muchas maneras.
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 85%

---

# Añadir usuarios a una iteración existente

Puede añadir historias a una iteración de cualquiera de las siguientes maneras:

* Del registro de asuntos pendientes una vez creada la iteración, tal como se describe en la sección [Mover historias del registro de pendientes a una iteración o tablero [!UICONTROL Kanban]](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#move-stories-from-the-backlog-to-an-iteration-or--board) en [Administrar el registro de asuntos pendientes Agile](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* Desde la página [!UICONTROL Detalles] de la tarea o problema individual
* Desde una lista de tareas o problemas
* Desde un informe
* Desde un panel de control

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
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

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
* Si la tarea o el problema se asignan a un equipo ágil y se mueven a la iteración de otro equipo, la asignación del equipo no cambia.
* Si la tarea o el problema no se han asignado a un equipo, se asignará al equipo propietario de la iteración.
* No se pueden añadir tareas principales a la iteración. Si añade tareas secundarias, la tarea principal aparece en el tablero de Scrum como un carril.

>[!IMPORTANT]
>
>Una vez que la tarea pasa a la iteración, no se puede actualizar el [!UICONTROL Tipo de duración] ni la [!UICONTROL Restricción de tarea]. El [!UICONTROL Tipo de duración] está establecido en [!UICONTROL Simple] y la [!UICONTROL Restricción de tarea] está establecida en [!UICONTROL Fechas fijas] para mantener la escala de tiempo de la tarea coherente con la escala de tiempo de la iteración.

1. Abra la tarea o el problema que desee agregar a una iteración.
O
Vaya al proyecto, informe o panel que contiene la tarea o el problema que desea agregar a una iteración. A continuación, seleccione una o varias tareas o problemas.

1. Haga clic en **[!UICONTROL Más]** ![Icono de más](assets/more-icon.png) > **[!UICONTROL Agregar a la iteración]**.
No puede asignar tareas o problemas asignados a equipos no ágiles.

1. En el cuadro **[!UICONTROL Agregar a]**, empiece a escribir el nombre de la iteración y selecciónela cuando aparezca en la lista.

   >[!NOTE]
   >
   >Puede trasladar una historia de una iteración existente a otra nueva.

1. Haga clic en **[!UICONTROL Add]**.
