---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Ver y editar la información de la historia en el panel de exploración
description: Al ver el mosaico de una historia en el tablero Kanban, determinada información está disponible para editar en línea, directamente desde el mosaico de la historia.
author: Jenny
feature: Agile
exl-id: 88d156ea-0913-425e-b3eb-6ae81d2d2336
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 56%

---

# Ver y editar la información de historia en el tablero de [!UICONTROL Scrum]

## Comprender qué información se puede ver y editar

Al ver un mosaico de artículo en el guion gráfico, está disponible la información de la siguiente tabla. Puede editar la mayor parte de la información en línea, directamente desde el mosaico de la historia.

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
   <td> <p>El nombre del proyecto con un vínculo directamente al proyecto<br>Este vínculo se muestra solamente en las historias (tareas principales, no subtareas) cuando se utiliza la vista Agile en una iteración; no se muestra cuando se utiliza una vista Agile en un proyecto.</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>La cantidad de puntos u horas completadas en la historia y la cantidad de puntos u horas asignadas a la historia<br>Estos números se utilizan para calcular y mostrar el [!UICONTROL Porcentaje completado] de cada historia.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>El [!UICONTROL Percent Complete] de cada historia y problema.<br>El [!UICONTROL Percent Complete] de la iteración se calcula según el [!UICONTROL Percent Complete] de cada artículo.</p> <p>Al actualizar el [!UICONTROL Percent Complete] de una historia o un problema, puede elegir cualquier número entre 0 y 100.</p> </td> 
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
   <td> <p>Cualquier campo adicional (incluidos los campos personalizados) que se pueda haber agregado a la vista Agile modificando la vista Agile, tal como se describe en "Creación y personalización de una vista de [!UICONTROL Agile]" en <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Información general de vistas en [!UICONTROL Adobe Workfront]</a>.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
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
   <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Acceso de [!UICONTROL Contribute] o [!UICONTROL Manage] a la tarea o al problema</td> 
  </tr>
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ver y editar información en un mosaico de historia

{{step1-to-team}}

1. (Opcional) Haga clic en el icono de **[!UICONTROL Cambiar equipo]** ![icono de Cambiar equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo de Scrum en el menú desplegable o busque un equipo en la barra de búsqueda.

1. En el panel izquierdo, seleccione **[!UICONTROL Iteraciones]** para elegir una iteración específica o seleccione **[!UICONTROL Iteración actual]**.

1. Vaya al panel de historia ágil [!UICONTROL Scrum].
1. Expanda el mosaico [!UICONTROL story] para ver todos los campos asociados con la historia.

   ![tarjeta de historia](assets/agile-storycard-scrum-2021-350x333.png)

1. (Opcional) Para editar un campo, haga clic en el campo y realice los cambios necesarios.

   Debe tener [!UICONTROL Editar] derechos sobre la tarea o el problema para editar el mosaico de la historia.

>[!NOTE]
>
>Para cambiar el [!UICONTROL Porcentaje completado], debe escribir un número entre 0 y 100. El campo no es un regulador que se pueda mover.
