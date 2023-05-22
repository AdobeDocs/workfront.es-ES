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
source-wordcount: '673'
ht-degree: 0%

---

# Agregar historias a una iteración existente

Puede agregar historias a una iteración de cualquiera de las siguientes maneras:

* A partir del registro de pendientes una vez creada la iteración, tal como se describe en la [Mover historias del registro de pendientes a una iteración o [!UICONTROL Kanban] tablero](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#moving-stories-from-the-backlog) sección en [Administrar el registro de pendientes Agile](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* Desde el [!UICONTROL Detalles] página de la tarea o problema individual
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
   <td> <p>[!UICONTROL Worker] o superior</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo [!DNL Workfront] El administrador puede modificar su nivel de acceso. Consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Acceso de [!UICONTROL Manage] al proyecto en el que se encuentra la historia</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Comprender cómo afecta la adición de historias a las fechas de tareas

De forma predeterminada, cuando se agrega una tarea existente a una iteración, el [!UICONTROL Fecha planificada de inicio] y [!UICONTROL Fecha planificada de finalización] se establecen de la siguiente manera:

### Tarea [!UICONTROL Fecha planificada de inicio]

* La tarea utiliza la fecha de inicio de la iteración cuando:

   * El proyecto no tiene un [!UICONTROL Fecha planificada de inicio] set.
   * El proyecto de [!UICONTROL Fecha planificada de inicio] es *antes* o *el* la fecha de inicio de la iteración.

* La tarea utiliza el del proyecto [!UICONTROL Fecha planificada de inicio] cuando:

   * El proyecto de [!UICONTROL Fecha planificada de inicio] es *después* la fecha de inicio de la iteración.

### Tarea [!UICONTROL Fecha planificada de finalización]

* La tarea utiliza la fecha de finalización de la iteración cuando:

   * El proyecto no tiene un [!UICONTROL Fecha planificada de finalización] set.
   * El proyecto de [!UICONTROL Fecha planificada de inicio] es *antes o el* la fecha de inicio de la iteración o el proyecto [!UICONTROL Fecha planificada de finalización] es *antes o el* la fecha final de la iteración.

* La tarea utiliza el del proyecto [!UICONTROL Fecha planificada de finalización] cuando:

   * El proyecto de [!UICONTROL Fecha planificada de inicio] es *después* la fecha de inicio de la iteración y la fecha del proyecto [!UICONTROL Fecha planificada de finalización] es *después* la fecha final de la iteración.

Puede configurar equipos de Scrum individuales para que utilicen las fechas del proyecto de forma predeterminada, en lugar de las fechas de iteración. Para obtener más información, consulte la sección [Configurar cómo se aplican las fechas al agregar elementos de trabajo a una iteración](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) en el artículo [Configurar Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Añadir un artículo a una iteración existente

Para agregar historias a una iteración directamente desde la tarea o el problema:

>[!IMPORTANT]
>
>Una vez que la tarea pasa a la iteración, no se puede actualizar el [!UICONTROL Tipo de duración] o [!UICONTROL Restricción de tarea]. [!UICONTROL Tipo de duración] se establece en [!UICONTROL Sencilla] y [!UICONTROL Restricción de tarea] se establece en [!UICONTROL Fechas fijas] para mantener la escala de tiempo de las tareas coherente con la de la iteración.

### Desde la pestaña tareas o problemas

Puede agregar cualquier tarea o problema a cualquier iteración si tiene acceso de Administración al proyecto. Tenga en cuenta lo siguiente al mover una tarea o un problema a una iteración:

* Si agrega varios equipos, la tarea o el problema solo se pueden mostrar en la iteración de un equipo. Esta es la iteración que elige en el paso 3 a continuación.
* Si la tarea o el problema se asignan a un equipo Agile y se mueven a la iteración de otro equipo, la asignación del equipo no cambia.
* Si la tarea o el problema no se han asignado a un equipo, se asignará al equipo propietario de la iteración.
* No se pueden agregar tareas principales a la iteración. Si agrega tareas secundarias, la tarea principal aparece en el panel de exploración como una pista de baño.

1. Vaya al proyecto, informe o panel que contiene la tarea o el problema que desea agregar a una iteración.
1. Seleccione una o varias tareas o problemas.
1. Clic **[!UICONTROL Más]** ![](assets/more-icon.png) > **[!UICONTROL Agregar a iteración]**.\
   No puede asignar tareas o problemas asignados a equipos que no son Agile.

1. En el **[!UICONTROL Agregar historias]** , escriba el nombre de la iteración.

   >[!NOTE]
   >
   >Puede mover un artículo de una iteración existente a otra nueva.

1. Si está agregando tareas, haga clic en **[!UICONTROL Agregar historias]**.\
   O\
   Si está agregando problemas, haga clic en **[!UICONTROL Agregar problemas]**.
