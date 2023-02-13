---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Añadir artículos a una iteración existente
description: Puede agregar artículos a una iteración de muchas maneras.
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Añadir artículos a una iteración existente

Puede agregar artículos a una iteración de cualquiera de estas formas:

* A partir del trabajo acumulado después de crear la iteración, como se describe en la sección [Mover artículos del trabajo pendiente a una iteración o [!UICONTROL Kanban] tablero](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#moving-stories-from-the-backlog) en [Administrar el trabajo atrasado ágil](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* En el [!UICONTROL Detalles] página de la tarea o problema individual
* De una tarea o lista de problemas
* A partir de un informe
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
   <td> <p>[!UICONTROL Work] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>[!UICONTROL Worker] o superior</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Acceso de [!UICONTROL Administrar] al proyecto en el que se encuentra el artículo</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Comprender cómo la adición de artículos afecta a las fechas de las tareas

De forma predeterminada, cuando se agrega una tarea existente a una iteración, la variable [!UICONTROL Fecha de inicio planeada] y [!UICONTROL Fecha de finalización planeada] se establecen de la siguiente manera:

### Tarea [!UICONTROL Fecha de inicio planeada]

* La tarea utiliza la fecha de inicio de la iteración cuando:

   * El proyecto no tiene un [!UICONTROL Fecha de inicio planeada] configurado.
   * El [!UICONTROL Fecha de inicio planeada] es *before* o *en* la fecha de inicio de la iteración.

* La tarea utiliza el [!UICONTROL Fecha de inicio planeada] cuando:

   * El [!UICONTROL Fecha de inicio planeada] es *after* la fecha de inicio de la iteración.

### Tarea [!UICONTROL Fecha de finalización planeada]

* La tarea utiliza la fecha de finalización de la iteración cuando:

   * El proyecto no tiene un [!UICONTROL Fecha de finalización planeada] configurado.
   * El [!UICONTROL Fecha de inicio planeada] es *antes o después* la fecha de inicio de la iteración o el [!UICONTROL Fecha de finalización planeada] es *antes o después* la fecha de finalización de la iteración.

* La tarea utiliza el [!UICONTROL Fecha de finalización planeada] cuando:

   * El [!UICONTROL Fecha de inicio planeada] es *after* la fecha de inicio de la iteración y el [!UICONTROL Fecha de finalización planeada] es *after* la fecha de finalización de la iteración.

Puede configurar equipos de Anulación individuales para que utilicen las fechas del proyecto de forma predeterminada, en lugar de las fechas de iteración. Para obtener más información, consulte la sección [Configurar cómo se aplican las fechas al agregar elementos de trabajo a una iteración](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) en el artículo [Configurar la anulación](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Agregar un artículo a una iteración existente

Para añadir artículos a una iteración directamente desde la tarea o el problema:

>[!IMPORTANT]
>
>Una vez que la tarea pasa a la iteración, no se puede actualizar la variable [!UICONTROL Tipo de duración] o [!UICONTROL Restricción de tarea]. [!UICONTROL Tipo de duración] está configurado como [!UICONTROL Sencilla] y [!UICONTROL Restricción de tarea] está configurado como [!UICONTROL Fechas fijas] para mantener la línea de tiempo de la tarea coherente con la línea de tiempo de la iteración.

### Desde la pestaña tareas o problemas

Puede añadir cualquier tarea o problema a cualquier iteración si tiene acceso de gestión al proyecto. Tenga en cuenta lo siguiente al mover una tarea o problema a una iteración:

* Si agrega varios equipos, la tarea o el problema solo se pueden mostrar en la iteración de un equipo. Esta es la iteración que elige en el paso 3 siguiente.
* Si la tarea o el problema se asigna a un equipo ágil y se mueve a la iteración de otro equipo, la asignación de equipo no cambia.
* Si la tarea o el problema no está asignado a un equipo, la tarea o el problema se asigna al equipo propietario de la iteración.
* No se pueden agregar tareas principales a la iteración. Si agrega cualquier tarea secundaria, la tarea principal aparece en la tabla de depuración como una guía.

1. Vaya al proyecto, informe o panel que contenga la tarea o el problema que desee agregar a una iteración.
1. Seleccione una o varias tareas o problemas.
1. Haga clic en **[!UICONTROL Más]** ![](assets/more-icon.png) > **[!UICONTROL Agregar a iteración]**.\
   No puede asignar tareas ni problemas asignados a equipos que no sean ágiles.

1. En el **[!UICONTROL Agregar historias]** , escriba el nombre de la iteración.

   >[!NOTE]
   >
   >Puede mover un artículo de una iteración existente a una nueva.

1. Si va a añadir tareas, haga clic en **[!UICONTROL Agregar historias]**.\
   O\
   Si está agregando problemas, haga clic en **[!UICONTROL Agregar problemas]**.
