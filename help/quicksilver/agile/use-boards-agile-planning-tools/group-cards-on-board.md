---
filename: group-cards-on-board
content-type: reference
navigation-topic: boards
title: Uso de grupos en un tablero
description: Puede agrupar las tarjetas en un tablero por usuario asignado o por etiqueta. Al seleccionar una opción para agrupar por, las tarjetas aparecen en formato de calle.
author: Lisa
feature: Agile
exl-id: 6f57a20e-0e47-4457-8605-9bce55c013ec
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Uso de grupos en un tablero

Puede agrupar las tarjetas en un tablero por usuario asignado o por etiqueta. Al seleccionar una opción para agrupar por, las tarjetas aparecen en formato de calle. Las tarjetas sin asignar o las tarjetas sin etiquetas aparecen en su propia calle.

>[!NOTE]
>
>Las tarjetas de la columna de entrada no se incluyen en un grupo y la columna de entrada se oculta cuando se aplica un grupo. Para obtener información sobre la columna de entrada, consulte [Agregar una columna de entrada a un tablero](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td> 
   <p>Nuevo: [!UICONTROL Contributor] o superior</p> 
   <p>o</p>
   <p>Actual: [!UICONTROL Request] o superior</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Agrupar tarjetas en un tablero

{{step1-to-boards}}

1. Acceda a un tablero. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Haga clic en **[!UICONTROL Grupo]** para abrir el panel del grupo a la izquierda del tablero.

   >[!NOTE]
   >
   >La configuración predeterminada para agrupar por es **[!UICONTROL None]**. Puede seleccionar esta opción en cualquier momento para quitar un grupo y mostrar solo las columnas del tablero.

1. Para agrupar las tarjetas, seleccione **[!UICONTROL Usuarios asignados]** o **[!UICONTROL Etiquetas]**.

   Las tarjetas se agrupan automáticamente. Haga clic en la flecha situada junto al nombre del grupo para contraerlo y expandirlo.

   ![Tarjetas agrupadas en un tablero](assets/group-by-assignee.png)

1. Seleccione lo que sucede cuando una tarjeta se mueve a otro grupo.

   * **[!UICONTROL Agregar a usuarios asignados] / [!UICONTROL Agregar a etiquetas]:** Los usuarios asignados o las etiquetas del nuevo grupo se agregan a la lista existente de usuarios asignados o etiquetas de la tarjeta.
   * **[!UICONTROL Anular a los usuarios asignados] / [!UICONTROL Anular las etiquetas]:** Los usuarios asignados o las etiquetas del nuevo grupo anulan a todos los demás usuarios asignados o etiquetas y se convierten en los únicos usuarios asignados o etiquetas de la tarjeta.

   ![[!UICONTROL Agrupar por opciones]](assets/group-by-rail.png)

1. Haga clic en **[!UICONTROL Ocultar grupos]** para ocultar el panel del grupo y mostrar el tablero completo.
