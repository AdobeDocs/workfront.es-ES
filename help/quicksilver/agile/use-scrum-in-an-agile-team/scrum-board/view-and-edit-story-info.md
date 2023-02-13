---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Ver y editar la información del artículo en el tablero Anulación
description: Al ver un mosaico de artículo en el tablero Kanban, hay cierta información disponible para editarla en línea, directamente desde el mosaico de artículo.
author: Lisa
feature: Agile
exl-id: 88d156ea-0913-425e-b3eb-6ae81d2d2336
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# Ver y editar la información del artículo en el [!UICONTROL Anulación] tablero

## Comprender qué información se puede ver y editar

Cuando se visualiza un mosaico de artículo en el tablero de artículos, está disponible la información de la siguiente tabla. Puede editar la mayoría de la información en línea, directamente desde el mosaico del artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Información</strong> </th> 
   <th><strong>Visible</strong> </th> 
   <th><strong>Edición en línea</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>El nombre del artículo con un vínculo directamente a la tarea o al problema</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>El nombre del proyecto con un vínculo directo al proyecto<br>Este vínculo solo se muestra en los artículos (tareas principales, no subtareas) al utilizar la vista ágil en una iteración; no se muestra al utilizar una vista ágil en un proyecto.</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>El número de puntos u horas completadas en el artículo y el número de puntos u horas asignados al artículo<br>Estos números se utilizan para calcular y mostrar el [!UICONTROL Porcentaje completado] de cada artículo.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>El [!UICONTROL Porcentaje completado] para cada artículo y problema.<br>El [!UICONTROL Percent Complete] de la iteración se calcula en función del [!UICONTROL Percent Complete] de cada artículo.</p> <p>Al actualizar el [!UICONTROL Porcentaje completado] para un artículo o problema, puede elegir cualquier número entre 0 y 100.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>A quién se asigna el artículo</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Color o categoría del mosaico</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Cualquier campo adicional (incluidos los campos personalizados) que se pueda haber agregado a la vista ágil modificando la vista ágil, tal como se describe en "Creación y personalización de una vista [!UICONTROL Agile]" en <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Información general sobre las vistas en [!UICONTROL Adobe Workfront]</a>.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td> <p>[!UICONTROL Worker] o superior</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Editar acceso a la tarea o problema</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Ver y editar información en un mosaico de artículo

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Equipos]**.

1. (Opcional) Haga clic en el **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png), seleccione un nuevo equipo de Anulación en el menú desplegable o busque un equipo en la barra de búsqueda.

1. En el panel izquierdo, seleccione **[!UICONTROL Iteraciones]** para elegir una iteración específica, o seleccione **[!UICONTROL Iteración actual]**.

1. Vaya a la [!UICONTROL Anulación] tablero de historia ágil.
1. Expanda el [!UICONTROL historia] mosaico para ver todos los campos asociados al artículo.

   ![](assets/agile-storycard-scrum-2021-350x333.png)

1. (Opcional) Para editar un campo, haga clic en el campo y realice los cambios necesarios.

   Debe tener [!UICONTROL Editar] derechos de la tarea o el número para editar el mosaico del artículo.

>[!NOTE]
>
>Para cambiar el [!UICONTROL Porcentaje completado], debe escribir un número entre 0 y 100. El campo no es un control deslizante que se pueda mover.
