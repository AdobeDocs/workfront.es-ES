---
filename: configure-card-falloff.md
content-type: reference
navigation-topic: boards
title: Configurar la caída de tarjetas
description: Puede configurar un tablero para que las tarjetas se archiven o se caigan del tablero según una programación.
author: Lisa
feature: Agile
exl-id: 0e4f6b3c-75aa-4314-9cb0-737e5a9d3bda
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Configurar la caída de tarjetas

Puede configurar un tablero para que se archiven las tarjetas o &quot;se caigan&quot; del tablero según una programación. Puede configurar las tarjetas de una columna en particular para que se caigan del tablero en un determinado número de días o semanas.

Cuando una tarjeta se cae del tablero, se archiva. Puede mostrar tarjetas archivadas con un filtro. Para obtener más información, vea [Filtrar y buscar en un tablero](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

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

## Configurar la caída de tarjetas

{{step1-to-boards}}

1. Acceda a un tablero. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Haga clic en **[!UICONTROL Configurar]** a la derecha del tablero para abrir el panel Configurar.
1. Expandir **[!UICONTROL Tarjetas]**.
1. Activar **[!UICONTROL Archivar automáticamente las tarjetas del tablero]**.

   ![Configuración de caída de tarjeta](assets/card-falloff-switch.png)

1. Seleccione cuándo desea archivar las tarjetas del tablero. Puede elegir hasta 8 semanas o hasta 60 días.

   La fecha se determina a partir de la última modificación de la tarjeta.

1. Seleccione la columna de la que desea quitar las tarjetas.
1. Haz clic en **[!UICONTROL Guardar]** en el mensaje de confirmación.
1. Haga clic en **[!UICONTROL Ocultar configuración]** para cerrar el panel [!UICONTROL Configurar]. Los ajustes de configuración se aplican automáticamente al actualizar el tablero.
