---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Agregar una subtarea a un artículo existente en el panel Kanban
description: Lea este artículo para aprender a crear subtareas para artículos existentes en el tablero Kanban.
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# Agregar una subtarea a un artículo existente en el panel Kanban

Al crear subtareas para artículos existentes, tenga en cuenta lo siguiente:

**Cuando la variable [!UICONTROL Modo de finalización de resumen] la configuración del proyecto se establece en [!UICONTROL Manual]:**

* Puede mover un artículo principal con subtareas a [!UICONTROL Completar], que actualiza el artículo principal al 100 % y la variable [!UICONTROL Estado] a [!UICONTROL Completar]. Las subtareas no se actualizan.
* Para actualizar el [!UICONTROL Porcentaje completado] para el artículo, debe actualizarlo desde el [!UICONTROL Historias] o desde la pestaña [!UICONTROL Detalles] del objeto.

**Cuando la variable [!UICONTROL Modo de finalización de resumen] la configuración del proyecto se establece en [!UICONTROL Automático]:**

* No se puede mover el artículo principal a otro lugar. Para actualizar el [!UICONTROL Porcentaje completado] para el artículo, debe actualizar el [!UICONTROL Porcentaje completado] para cualquier subtarea. La variable [!UICONTROL Porcentaje completado] para el artículo se calcula en función de la variable [!UICONTROL Porcentaje completado] de todas las subtareas.
* Mover un artículo principal con subtareas a [!UICONTROL Completar] actualiza el artículo principal al 100 % y la variable [!UICONTROL Estado] a [!UICONTROL Completar]. Las subtareas también se actualizan al 100% y la variable [!UICONTROL Estado] se actualiza a [!UICONTROL Completar].

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
   <td> <p>[!UICONTROL Worker] o superior</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede cambiar el nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Acceso de [!UICONTROL Contribute] o [!UICONTROL Manage] a la tarea en la que se encuentra la subtarea</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Agregue una subtarea a un artículo existente en el [!UICONTROL Kanban] tablero

1. Vaya a la [!UICONTROL Kanban] tablero que contiene el artículo en el que desea agregar una subtarea.
1. Haga clic en el nombre de la tarea en el mosaico de artículo del [!UICONTROL Kanban] tablero.
1. Agregue una subtarea a la tarea como lo haría en cualquier otra lista de tareas dentro de [!DNL Workfront], tal como se describe en [Crear subtareas](../../manage-work/tasks/create-tasks/create-subtasks.md).
