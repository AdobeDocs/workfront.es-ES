---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Agregar historias a una iteración existente
description: Puede agregar historias a una iteración de muchas maneras.
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# Agregar historias a una iteración existente

Puede agregar historias a una iteración de cualquiera de las siguientes maneras:

* Del registro de pendientes una vez creada la iteración, como se describe en la sección [Mover historias del registro de pendientes a una iteración o [!UICONTROL Panel Kanban]](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#moving-stories-from-the-backlog) de [Administrar el registro de pendientes Agile](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* Desde la página [!UICONTROL Detalles] de la tarea o problema individual
* Desde una tarea o lista de problemas
* Desde un informe
* Desde un tablero

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>[!UICONTROL Trabajo] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>[!UICONTROL Worker] o superior</p> <p>Nota: si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Acceso de [!UICONTROL Manage] al proyecto en el que se encuentra la historia</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

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

Puede configurar equipos de Scrum individuales para que utilicen las fechas del proyecto de forma predeterminada, en lugar de las fechas de iteración. Para obtener más información, consulte la sección [Configurar cómo se aplican las fechas al agregar elementos de trabajo a una iteración](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) en el artículo [Configurar Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Añadir un artículo a una iteración existente

Para agregar historias a una iteración directamente desde la tarea o el problema:

>[!IMPORTANT]
>
>Una vez que la tarea pasa a la iteración, no se puede actualizar [!UICONTROL Tipo de duración] ni [!UICONTROL Restricción de tarea]. [!UICONTROL El tipo de duración] está establecido en [!UICONTROL Simple] y [!UICONTROL Restricción de tarea] está establecido en [!UICONTROL Fechas fijas] para mantener la escala de tiempo de la tarea coherente con la escala de tiempo de la iteración.

### Desde la pestaña tareas o problemas

Puede agregar cualquier tarea o problema a cualquier iteración si tiene acceso de Administración al proyecto. Tenga en cuenta lo siguiente al mover una tarea o un problema a una iteración:

* Si agrega varios equipos, la tarea o el problema solo se pueden mostrar en la iteración de un equipo. Esta es la iteración que elige en el paso 3 a continuación.
* Si la tarea o el problema se asignan a un equipo Agile y se mueven a la iteración de otro equipo, la asignación del equipo no cambia.
* Si la tarea o el problema no se han asignado a un equipo, se asignará al equipo propietario de la iteración.
* No se pueden agregar tareas principales a la iteración. Si agrega tareas secundarias, la tarea principal aparece en el panel de exploración como una pista de baño.

1. Vaya al proyecto, informe o panel que contiene la tarea o el problema que desea agregar a una iteración.
1. Seleccione una o varias tareas o problemas.
1. Haga clic en **[!UICONTROL Más]** ![](assets/more-icon.png) > **[!UICONTROL Agregar a la iteración]**.\
   No puede asignar tareas o problemas asignados a equipos que no son Agile.

1. En el cuadro **[!UICONTROL Agregar historias]**, escriba el nombre de la iteración.

   >[!NOTE]
   >
   >Puede mover un artículo de una iteración existente a otra nueva.

1. Si está agregando tareas, haga clic en **[!UICONTROL Agregar historias]**.\
   O\
   Si está agregando problemas, haga clic en **[!UICONTROL Agregar problemas]**.
