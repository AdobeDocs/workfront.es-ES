---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Agregar o quitar miembros de un tablero
description: Las personas deben añadirse al tablero como miembros para poder ver el tablero y ser asignadas a las tarjetas.
author: Lisa
feature: Agile
exl-id: 8a46846c-f9b8-45cb-9923-e7596854557b
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Agregar o quitar miembros de un tablero

Las personas y los equipos deben agregarse al tablero como miembros para poder ver el tablero.

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

## Añadir miembros a un tablero

{{step1-to-boards}}

1. Cree un tablero nuevo o edite uno existente. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Haga clic en el icono **[!UICONTROL Agregar miembro]** ![Agregar miembros](assets/boards-addmember-spectrum-25x25.png).
1. En el cuadro **[!UICONTROL Agregar miembros]**, empiece a escribir un nombre y, a continuación, selecciónelo cuando aparezca en la lista.

   Puede seleccionar un miembro individual o un equipo. Si elige un equipo, el propio equipo se añade al tablero.

   >[!NOTE]
   >
   >Un usuario individual debe tener la opción **[!UICONTROL Ver]** o **[!UICONTROL Editar]** establecida en su nivel de acceso para equipos o no podrá ver el tablero.


   ![Agregar miembros al tablero](assets/boards-add-members.png)

## Quitar miembros de un tablero

{{step1-to-boards}}

1. Cree un tablero nuevo o edite uno existente. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Haga clic en el icono **[!UICONTROL Agregar miembro]** ![Agregar miembros](assets/boards-addmember-spectrum-25x25.png).
1. En el cuadro **[!UICONTROL Agregar miembros]**, haga clic en la X junto al nombre de una persona o equipo para quitarlos del tablero.

   ![Quitar miembro del tablero](assets/boards-remove-member-from-board-350x367.png)

   Cuando se elimina un miembro de un tablero, no se elimina de ninguna tarjeta a la que esté asignado. Para las tarjetas conectadas, las asignaciones también se actualizan en la tarea o el problema [!DNL Workfront].

   Los miembros solo se eliminan de este tablero. No se eliminan de otros tableros a los que pertenecen.

   >[!NOTE]
   >
   >No puede eliminar al propietario del tablero.
