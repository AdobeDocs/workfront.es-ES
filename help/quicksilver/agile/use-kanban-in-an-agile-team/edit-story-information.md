---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Editar información de la historia
description: Al ver el mosaico de una historia en el tablero Kanban, determinada información está disponible para editar en línea, directamente desde el mosaico de la historia.
author: Courtney
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YNFdopcCAju4MaN2oqssN0Q6H7k0Stg3udO0AipWIMs
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 340
ht-degree: 77%

---

# Editar información de una historia

## Comprender qué información se puede ver y editar {#understand-what-information-can-be-viewed-and-edited}

Al ver el mosaico de una historia en el tablero [!UICONTROL Kanban], está disponible la información de la siguiente tabla. Puede editar la mayor parte de la información en línea, directamente desde el mosaico de la historia.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Información</strong> </th> 
   <th><strong>Visible</strong> </th> 
   <th><strong>Editable en línea</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>El nombre de la historia con un vínculo directamente a la tarea o al problema</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>El nombre del proyecto con un vínculo directamente al proyecto</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>La cantidad de puntos u horas completados en la historia y la cantidad de puntos u horas asignados a la historia<br>Estos números se utilizan para calcular y mostrar el porcentaje completado de cada historia.</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>El [!UICONTROL Porcentaje completado] de cada artículo y problema.<br>[!UICONTROL El porcentaje completado] de la iteración se calcula según el [!UICONTROL Porcentaje completado] de cada artículo.<br></p> <p>Al actualizar el [!UICONTROL Percent Complete] de una historia o un problema, puede elegir cualquier número entre 0 y 100.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>A quién se asigna la historia</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Color o categoría del mosaico</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Cualquier campo adicional (incluidos los campos personalizados) que se pueda haber agregado a la vista de Agile modificando la vista de Agile, tal como se describe en "Creación y personalización de una vista de Agile" en <a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Información general de vistas en [!DNL Adobe Workfront]</a></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p> 
   <p>Trabajo o superior</p> </td> 
  </tr>
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ver y editar información en un mosaico de historia

{{step1-to-team}}

1. (Opcional) Haga clic en el icono de **[!UICONTROL Cambiar equipo]** ![icono de Cambiar equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo Kanban en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Vaya al tablero [!UICONTROL Kanban].
1. Expanda el mosaico de la historia para ver todos los campos asociados al artículo.

   ![Tarjeta de historia](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. (Opcional) Para editar un campo, haga clic en el campo y realice los cambios necesarios.
Debe tener [!UICONTROL Editar] derechos sobre la tarea o el problema para editar el mosaico de la historia.
Para obtener más información sobre cada campo y si se puede editar, consulte [Comprender qué información se puede ver y editar](#understand-what-information-can-be-viewed-and-edited).

>[!NOTE]
>
>Para cambiar el [!UICONTROL Porcentaje completado], debe escribir un número entre 0 y 100. El campo no es un regulador que se pueda mover.
