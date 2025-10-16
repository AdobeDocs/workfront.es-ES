---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Agregar una subtarea a una historia existente en el Panel Kanban
description: Revise este artículo para aprender a crear subtareas para historias existentes en el tablero Kanban.
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 91%

---

# Añadir una subtarea a un artículo existente en el tablero Kanban

Al crear subtareas para historias existentes, tenga en cuenta lo siguiente:

**Cuando la configuración del [!UICONTROL Modo de finalización de resumen] del proyecto está establecida en [!UICONTROL Manual]:**

* Puede mover una historia principal con subtareas a [!UICONTROL Completado], que actualiza la historia principal al 100 % y el [!UICONTROL Estado] a [!UICONTROL Completado]. Las subtareas no se actualizan.
* Para actualizar el [!UICONTROL Porcentaje completado] de la historia, debe actualizarlo desde la pestaña [!UICONTROL Historias] o desde la página [!UICONTROL Detalles] del objeto.

**Cuando la configuración del [!UICONTROL Modo de finalización de resumen] del proyecto está establecida en [!UICONTROL Automático]:**

* No se puede mover la historia principal por el tablero. Para actualizar el [!UICONTROL Porcentaje completado] de la historia, debe actualizar el [!UICONTROL Porcentaje completado] para cualquier subtarea. El [!UICONTROL Porcentaje completado] de la historia se calcula en función del [!UICONTROL Porcentaje completado] de todas las subtareas.
* Al mover una historia principal con subtareas a [!UICONTROL Completado], se actualiza la historia principal al 100 % y el [!UICONTROL Estado] a [!UICONTROL Completado]. Las subtareas también se actualizan al 100 % y el [!UICONTROL Estado] se actualiza a [!UICONTROL Completado].

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td>Acceso de contribución o administración a la tarea en la que se encuentra la subtarea</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Añadir una subtarea a una historia existente en el tablero [!UICONTROL Kanban]

1. Vaya al tablero [!UICONTROL Kanban] que contiene la historia donde desea añadir una subtarea.
1. Haga clic en el nombre de la tarea en el mosaico de la historia del tablero [!UICONTROL Kanban].
1. Añada una subtarea a la tarea como lo haría en cualquier otra lista de tareas dentro de [!DNL Workfront], tal como se describe en [Crear subtareas](../../manage-work/tasks/create-tasks/create-subtasks.md).
