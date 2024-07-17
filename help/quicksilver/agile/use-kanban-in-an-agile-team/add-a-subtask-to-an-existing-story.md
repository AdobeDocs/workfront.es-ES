---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Agregar una subtarea a un artículo existente en el Panel Kanban
description: Revise este artículo para aprender a crear subtareas para historias existentes en el Panel Kanban.
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '366'
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
   <td> <p>[!UICONTROL Worker] o superior</p> <p>Nota: si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede cambiar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Acceso de [!UICONTROL Contribute] o [!UICONTROL Manage] a la tarea en la que se encuentra la subtarea</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Agregar una subtarea a una historia existente en el tablero [!UICONTROL Kanban]

1. Vaya al tablero [!UICONTROL Kanban] que contiene la historia donde desea agregar una subtarea.
1. Haga clic en el nombre de la tarea en el mosaico de la historia del tablero [!UICONTROL Kanban].
1. Agregue una subtarea a la tarea como lo haría en cualquier otra lista de tareas dentro de [!DNL Workfront], como se describe en [Crear subtareas](../../manage-work/tasks/create-tasks/create-subtasks.md).
