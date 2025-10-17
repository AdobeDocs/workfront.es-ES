---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Editar información de la historia
description: Al ver el mosaico de una historia en el tablero Kanban, determinada información está disponible para editar en línea, directamente desde el mosaico de la historia.
author: Jenny
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 90%

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
   <td> <p>El [!UICONTROL Percent Complete] de cada historia y problema.<br>El [!UICONTROL The Percent Complete] de la iteración se calcula según el [!UICONTROL Percent Complete] de cada artículo.<br></p> <p>Al actualizar el [!UICONTROL Percent Complete] de una historia o un problema, puede elegir cualquier número entre 0 y 100.</p> </td> 
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
   <td> <p>Cualquier campo adicional (incluidos los campos personalizados) que se pueda haber añadido a la vista de Agile modificando la vista de Agile, tal como se describe en "Creación y personalización de una vista de Agile" en <a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Información general sobre las vistas en [!DNL Adobe Workfront]</a></p> </td> 
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
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p> 
   <p>Trabajo o superior</p> </td> 
  </tr>
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
