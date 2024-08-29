---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Editar información de la historia
description: Al ver un mosaico de historia en el panel Kanban, cierta información está disponible para editar en línea, directamente desde el mosaico de historia.
author: Lisa
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Editar información de la historia

## Comprender qué información se puede ver y editar {#understand-what-information-can-be-viewed-and-edited}

Al ver un mosaico de historia en el tablero [!UICONTROL Kanban], está disponible la información de la siguiente tabla. Puede editar la mayor parte de la información en línea, directamente desde el mosaico de artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Información</strong> </th> 
   <th><strong>Visible</strong> </th> 
   <th><strong>En línea editable</strong> </th> 
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
   <td> <p>La cantidad de puntos u horas completadas en la historia y la cantidad de puntos u horas asignadas a la historia<br>Estos números se utilizan para calcular y mostrar el porcentaje completado de cada historia.</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Percent Complete] para cada artículo y problema.<br>[!UICONTROL El porcentaje completado] de la iteración se calcula según el [!UICONTROL Porcentaje completado] de cada artículo.<br></p> <p>Al actualizar [!UICONTROL Porcentaje completado] para una historia o un problema, puede elegir cualquier número entre 0 y 100.</p> </td> 
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
   <td> <p>Cualquier campo adicional (incluidos los campos personalizados) que se pueda haber agregado a la vista Agile modificando la vista Agile, tal como se describe en "Creación y personalización de una vista Agile" en <a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Información general de vistas en [!DNL Adobe Workfront]</a></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

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
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ver y editar información en un mosaico de artículo

{{step1-to-team}}

1. (Opcional) Haga clic en el icono **[!UICONTROL Cambiar equipo]** ![Cambiar icono de equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo Kanban en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Vaya al tablero [!UICONTROL Kanban].
1. Expanda el mosaico de artículo para ver todos los campos asociados con el artículo.

   ![](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. (Opcional) Para editar un campo, haga clic en el campo y realice los cambios necesarios.
Debe tener [!UICONTROL Editar] derechos sobre la tarea o el problema para editar el mosaico de la historia.
Para obtener más información sobre cada campo y si se puede editar, consulte [Comprender qué información se puede ver y editar](#understand-what-information-can-be-viewed-and-edited).

>[!NOTE]
>
>Para cambiar el [!UICONTROL Porcentaje completado], debe escribir un número entre 0 y 100. El campo no es un control deslizante que se pueda mover.
