---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Agregar historias a una iteración existente
description: Puede agregar historias a una iteración de muchas maneras.
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# Agregar historias a una iteración existente

Puede agregar historias a una iteración de cualquiera de las siguientes maneras:

* Del registro de pendientes una vez creada la iteración, como se describe en la sección [Mover historias del registro de pendientes a una iteración o [!UICONTROL Panel Kanban]](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#move-stories-from-the-backlog-to-an-iteration-or--board) de [Administrar el registro de pendientes Agile](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* Desde la página [!UICONTROL Detalles] de la tarea o problema individual
* Desde una tarea o lista de problemas
* Desde un informe
* Desde un tablero

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
   <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Acceso de [!UICONTROL Manage] al proyecto en el que se encuentra la historia </td> 
  </tr>
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Comprender cómo afecta la adición de historias a las fechas de tareas

De manera predeterminada, cuando agrega una tarea existente a una iteración, la [!UICONTROL Fecha planificada de inicio] y la [!UICONTROL Fecha planificada de finalización] de la tarea se establecen de la siguiente manera:

### Tarea [!UICONTROL Fecha planificada de inicio]

* La tarea utiliza la fecha de inicio de la iteración cuando:

   * El proyecto no tiene [!UICONTROL fecha planificada de inicio] establecida.
   * La [!UICONTROL fecha planificada de inicio] del proyecto es *anterior a* o *el* la fecha de inicio de la iteración.

* La tarea usa la [!UICONTROL fecha planificada de inicio] del proyecto cuando:

   * La [!UICONTROL fecha planificada de inicio] del proyecto es *posterior* a la fecha de inicio de la iteración.

### Tarea [!UICONTROL Fecha planificada de finalización]

* La tarea utiliza la fecha de finalización de la iteración cuando:

   * El proyecto no tiene [!UICONTROL fecha planificada de finalización] establecida.
   * La [!UICONTROL fecha planificada de inicio] del proyecto es *antes o el* la fecha de inicio de la iteración o la [!UICONTROL fecha planificada de finalización] del proyecto es *antes o el* de la fecha de finalización de la iteración.

* La tarea usa la [!UICONTROL fecha planificada de finalización] del proyecto cuando:

   * La [!UICONTROL fecha planificada de inicio] del proyecto es *después de* la fecha de inicio de la iteración y la [!UICONTROL fecha planificada de finalización] del proyecto es *después* de la fecha de finalización de la iteración.

Puede configurar equipos de Scrum individuales para que utilicen las fechas del proyecto de forma predeterminada, en lugar de las fechas de iteración. Para obtener más información, consulte la sección [Configurar cómo se aplican las fechas al agregar elementos de trabajo a una iteración](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) en el artículo [Configurar Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Añadir un artículo a una iteración existente

Puede agregar cualquier tarea o problema a cualquier iteración si tiene acceso de Administración al proyecto. Tenga en cuenta lo siguiente al mover una tarea o un problema a una iteración:

* Si agrega varios equipos, la tarea o el problema solo se pueden mostrar en la iteración de un equipo. Esta es la iteración que elige en el paso 3 a continuación.
* Si la tarea o el problema se asignan a un equipo Agile y se mueven a la iteración de otro equipo, la asignación del equipo no cambia.
* Si la tarea o el problema no se han asignado a un equipo, se asignará al equipo propietario de la iteración.
* No se pueden agregar tareas principales a la iteración. Si agrega tareas secundarias, la tarea principal aparece en el panel de exploración como una pista de baño.

>[!IMPORTANT]
>
>Una vez que la tarea pasa a la iteración, no se puede actualizar [!UICONTROL Tipo de duración] ni [!UICONTROL Restricción de tarea]. [!UICONTROL El tipo de duración] está establecido en [!UICONTROL Simple] y [!UICONTROL Restricción de tarea] está establecido en [!UICONTROL Fechas fijas] para mantener la escala de tiempo de la tarea coherente con la escala de tiempo de la iteración.

1. Abra la tarea o el problema que desee agregar a una iteración.
O
Vaya al proyecto, informe o panel que contiene la tarea o el problema que desea agregar a una iteración. A continuación, seleccione una o varias tareas o problemas.

1. Haga clic en **[!UICONTROL Más]** ![](assets/more-icon.png) > **[!UICONTROL Agregar a la iteración]**.
No puede asignar tareas o problemas asignados a equipos que no son Agile.

1. En el cuadro **[!UICONTROL Agregar a]**, empiece a escribir el nombre de la iteración y selecciónela cuando aparezca en la lista.

   >[!NOTE]
   >
   >Puede mover un artículo de una iteración existente a otra nueva.

1. Haga clic en **[!UICONTROL Agregar]**.
