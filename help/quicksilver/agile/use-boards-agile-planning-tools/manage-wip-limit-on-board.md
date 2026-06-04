---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Administrar el límite de trabajo en curso (WIP) en un tablero
description: Puede configurar un límite de trabajo en curso (WIP) para cada columna de un tablero.
author: Courtney
feature: Agile
exl-id: 7901c6e7-75a4-41e4-b288-d527c4a6d031
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jOCQTCkNgEZfE8O4-KyKVjEluncwWx0vh5NdrKHC9vg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 242
ht-degree: 20%

---

# Administrar el límite de [!UICONTROL Trabajo en curso] (WIP) en un tablero

Puede configurar un límite de [!UICONTROL trabajo en curso] (WIP) para cada columna de un tablero.

El límite de trabajo en curso es simplemente una advertencia visual y no le impide tener más elementos en cada columna que el límite establecido.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
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

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Definir el límite de WIP en una columna

{{step1-to-boards}}

1. Acceda a un tablero. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Busque la columna a la que desee agregar el límite de trabajo en curso.

   Para agregar una nueva columna, consulte [Administrar columnas del tablero](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

1. Haga clic en el menú **[!UICONTROL Más]** de la columna y seleccione **[!UICONTROL Editar]** para abrir el área de Configuración.
1. En [!UICONTROL Directivas de columna], habilite la directiva **[!UICONTROL Trabajo en curso] límite** para limitar el número de tarjetas que se pueden agregar a la columna.
1. Escriba el número de límite en el campo **[!UICONTROL Establecer límite]**.

   ![WIP limit for column](assets/boards-wip-limit-in-column.png)

   El número de tarjetas y el límite se muestran en la parte superior de la columna. Si la columna contiene más tarjetas que el límite, el contador se vuelve rojo.

   ![Contador de límite de WIP](assets/boards-wip-limit-counter.png)

1. Haga clic en **[!UICONTROL Cerrar]** para salir del área de [!UICONTROL Configuración] y ver la columna y sus tarjetas.
