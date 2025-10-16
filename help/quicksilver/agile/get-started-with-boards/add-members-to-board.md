---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Agregar o quitar miembros de un tablero
description: Los usuarios deben añadirse al tablero como miembros para poder ver el tablero y ser asignados a las tarjetas.
author: Lisa
feature: Agile
exl-id: 8a46846c-f9b8-45cb-9923-e7596854557b
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 60%

---

# Añadir o quitar miembros de un tablero

Los usuarios y los equipos deben añadirse al tablero como miembros para poder verlo.

El creador de un tablero es el propietario de forma predeterminada. El propietario del tablero es la única persona que puede eliminar ese tablero o actualizar sus filtros en el panel Configurar. Solamente un administrador del sistema o el propietario actual del tablero puede cambiar el propietario del tablero.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o superior</p> 
   <p>Solicitud o superior</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Añadir tarjetas a un tablero

{{step1-to-boards}}

1. Cree un tablero nuevo o edite uno existente. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Haga clic en el icono **[!UICONTROL Añadir miembro]** ![Añadir miembros](assets/boards-addmember-spectrum-25x25.png).
1. En el cuadro **[!UICONTROL Añadir miembros]**, empiece a escribir un nombre y, a continuación, selecciónelo cuando aparezca en la lista.

   Puede seleccionar un miembro individual o un equipo. Si elige un equipo, el propio equipo se añade al tablero.

   >[!NOTE]
   >
   >Un usuario individual debe tener la opción **[!UICONTROL Ver]** o **[!UICONTROL Editar]** configurada en su nivel de acceso para equipos, o no podrá ver el tablero.


   ![Añadir miembros al tablero](assets/boards-add-members.png)

## Quitar miembros de un tablero

{{step1-to-boards}}

1. Cree un tablero nuevo o edite uno existente. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Haga clic en el icono **[!UICONTROL Añadir miembro]** ![Añadir miembros](assets/boards-addmember-spectrum-25x25.png).
1. En el cuadro **[!UICONTROL Añadir miembros]**, haga clic en la X junto al nombre de una persona o equipo para quitarlos del tablero.

   ![Quitar usuario del tablero](assets/boards-remove-member-from-board-350x367.png)

   Cuando se elimina un miembro de un tablero, no se elimina de ninguna tarjeta a la que esté asignado. Para las tarjetas conectadas, las asignaciones también se actualizan en la tarea o el problema de [!DNL Workfront].

   Los miembros solo se eliminan de este tablero. No se eliminan de otros tableros a los que pertenecen.

   >[!NOTE]
   >
   >No puede eliminar al propietario del tablero.

## Cambiar el propietario del tablero

>[!NOTE]
>
>Solamente un administrador del sistema o el propietario actual del tablero puede cambiar el propietario del tablero. Un tablero solo puede tener un propietario.
>
>La capacidad de cambiar el propietario del tablero está disponible en tableros básicos, retrospectivos y Kanban, pero no en tableros dinámicos.

1. Acceda al tablero.
1. Haga clic en el menú **[!UICONTROL Más]** ![Menú más](assets/more-icon-spectrum.png) que está junto al nombre del tablero y, a continuación, elija **[!UICONTROL Cambiar propietario del tablero]**.
1. En el cuadro de diálogo Cambiar propietario del tablero, busque y seleccione el usuario que desea convertir en propietario.

   No puede buscar usuarios que ya sean miembros del tablero. Para convertir a un miembro existente en el propietario, primero debe eliminarlo del tablero. Convertir a un usuario en el propietario del tablero los añade al tablero.

   Solo un usuario puede ser el propietario del tablero. Un equipo no puede ser propietario.

1. Haga clic en [!UICONTROL **Actualizar**].
