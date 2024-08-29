---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Agregar una subtarea a una historia existente en el Panel Kanban
description: Revise este artículo para aprender a crear subtareas para historias existentes en el Panel Kanban.
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---

# Agregar una subtarea a un artículo existente en el Panel Kanban

Al crear subtareas para artículos existentes, tenga en cuenta lo siguiente:

**Cuando la configuración de [!UICONTROL Modo de finalización de resumen] del proyecto está establecida en [!UICONTROL Manual]:**

* Puede mover una historia principal con subtareas a [!UICONTROL Completar], que actualiza la historia principal al 100% y el [!UICONTROL Estado] a [!UICONTROL Completar]. Las subtareas no se actualizan.
* Para actualizar el [!UICONTROL Porcentaje completado] de la historia, debe actualizarlo desde la ficha [!UICONTROL Historias] o desde la página [!UICONTROL Detalles] del objeto.

**Cuando la configuración de [!UICONTROL Modo de finalización de resumen] del proyecto está establecida en [!UICONTROL Automático]:**

* No se puede mover la historia principal de forma generalizada. Para actualizar el [!UICONTROL Porcentaje completado] de la historia, debe actualizar el [!UICONTROL Porcentaje completado] para cualquier subtarea. El [!UICONTROL porcentaje completado] para la historia se calcula en función del [!UICONTROL porcentaje completado] de todas las subtareas.
* Al mover una historia principal con subtareas a [!UICONTROL Completar], se actualiza la historia principal al 100% y el [!UICONTROL Estado] a [!UICONTROL Completar]. Las subtareas también se actualizan al 100% y [!UICONTROL Estado] se actualiza a [!UICONTROL Completado].

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td>Acceso de [!UICONTROL Contribute] o [!UICONTROL Manage] a la tarea en la que se encuentra la subtarea</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Agregar una subtarea a una historia existente en el tablero [!UICONTROL Kanban]

1. Vaya al tablero [!UICONTROL Kanban] que contiene la historia donde desea agregar una subtarea.
1. Haga clic en el nombre de la tarea en el mosaico de la historia del tablero [!UICONTROL Kanban].
1. Agregue una subtarea a la tarea como lo haría en cualquier otra lista de tareas dentro de [!DNL Workfront], como se describe en [Crear subtareas](../../manage-work/tasks/create-tasks/create-subtasks.md).
