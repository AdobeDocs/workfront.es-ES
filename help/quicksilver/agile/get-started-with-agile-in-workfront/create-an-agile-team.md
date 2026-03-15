---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: Crear un equipo ágil
description: Adobe Workfront permite a los equipos ágiles completar el trabajo de forma gradual y organizada.
author: Courtney
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 13%

---

# Crear un equipo de Agile

<!--Audited: 01/2024-->

[!DNL Adobe Workfront] permite a los equipos ágiles completar el trabajo de forma incremental y organizada.

Cualquier usuario de la organización puede ver el equipo de Agile y todos los componentes de Agile del equipo, incluidos los trabajos atrasados, las iteraciones, el guion gráfico y las historias individuales. Sin embargo, sólo los miembros del equipo con [!UICONTROL Editar] acceso al trabajo pueden realizar cambios en el trabajo asignado al equipo.

[!DNL Workfront] admite las siguientes metodologías ágiles:

* **[!UICONTROL Scrum]**: Los equipos tienen un trabajo atrasado que necesita hacerse. Cuando el equipo está listo para trabajar en un trozo de trabajo específico, el trabajo se mueve del trabajo atrasado a una iteración. Para obtener información más detallada sobre la administración de un equipo de Scrum, vea [Scrum en un equipo de Agile](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL Kanban]:** Los equipos mueven el trabajo en la vista Kanban a través de estados predeterminados. Los estados predeterminados son: trabajo pendiente, en proceso y terminado. Para obtener información más detallada sobre la administración de un equipo de Kanban, vea [Kanban en un equipo de Agile](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

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
   <p>Planificar la creación de un nuevo equipo ágil</p>
  <p>Trabajo o superior para convertir un equipo en un equipo ágil</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Decidir una metodología ágil

Puede utilizar una metodología Scrum o Kanban Agile para su equipo Agile. Cada metodología ofrece diversos beneficios. La forma de trabajar de su equipo Agile determina la metodología Agile que elija usar.

Las metodologías Scrum y Kanban Agile en [!DNL Workfront] le permiten mover historias a través de un tablero de historias para indicar un cambio de estado y el progreso de la historia.

Las metodologías Scrum y Kanban Agile en [!DNL Workfront] difieren en las siguientes maneras:

### Ventajas de usar Kanban en [!DNL Workfront]

La metodología ágil de [!DNL Kanban] en [!DNL Workfront] te permite mover historias con más facilidad a través de un panel de artículos ágil al tiempo que limita la cantidad de trabajo en curso. No hay fechas de inicio y finalización al utilizar la metodología [!DNL Kanban] Agile.

La siguiente funcionalidad admite esta metodología:

* Mostrar el registro atrasado en el tablero de artículos Ágile [!DNL Kanban].
Para obtener más información, vea [Agregar el retraso al panel [!UICONTROL Kanban]](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* Configure los elementos del registro atrasado para que se agreguen automáticamente al tablero de artículos [!UICONTROL Kanban] Agile cuando se muevan otros elementos a un estado que equipare con Complete.
Para obtener más información, vea la sección [Configurar los artículos que se van a agregar automáticamente desde el registro atrasado](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) en el artículo [Configurar Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configure un límite de trabajo en curso (trabajo en curso) para que se muestre en el tablero de artículos [!UICONTROL Kanban] Agile.
Para obtener más información, vea [Administrar el límite de trabajo en curso (trabajo en curso) en el panel kanban](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Ventajas de usar Scrum en [!DNL Workfront]

La metodología Scrum Agile de [!DNL Workfront] le permite agregar un conjunto de historias a una iteración Ágil y crear un panel de historias para esa iteración. La iteración se basa en las fechas de inicio y fin que defina.

La siguiente funcionalidad admite esta metodología:

* Incluir problemas en el panel de artículos [!UICONTROL Scrum]
* Incluir problemas en el trabajo atrasado de un equipo ágil
* Las subtareas se pueden mostrar en el panel de artículos de [!UICONTROL Scrum]
* Visualización de un gráfico de desglose para ver el progreso en relación con los artículos durante la iteración
Para obtener más información, consulte [Descripción general del gráfico de descomposición ágil](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Crear un equipo de Agile

{{step1-to-team}}

1. Haga clic en el icono **[!UICONTROL Cambiar equipos]** ![Cambiar equipo](assets/switch-team-icon.png) y, a continuación, haga clic en **[!UICONTROL Crear nuevo equipo]**.

   ![Seleccione Crear nuevo equipo](assets/create-new-team.png)

   Aparecerá el cuadro Nuevo equipo.

1. Especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Nombre de equipo]</strong> </td> 
      <td>Escriba un nombre para el nuevo equipo ágil.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Este es un equipo ágil]</strong> </td> 
      <td>Seleccione esta opción para configurar este nuevo equipo para que sea un equipo ágil.</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>[!UICONTROL Is Active]</strong> </td> 
      <td>Seleccione esta opción para activar este equipo. Los equipos inactivos no son visibles para otros usuarios para asignarlos a trabajo. </td> 
     </tr>


   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL Group]</strong> </td> 
      <td> <p>Comience a escribir el nombre de un grupo para agregarlo al equipo y, a continuación, seleccione el nombre cuando aparezca en la lista desplegable.</p> <p><b>NOTA</b></p> <p> Cuando se asigna un equipo a un grupo o subgrupo, cualquier administrador de grupo de ese grupo o subgrupo puede administrar el equipo sin ser miembro del equipo. Los administradores de grupo pueden ir al área [!UICONTROL Teams] desde el [!UICONTROL Main Menu] y hacer clic en la flecha [!UICONTROL Switch Teams] <img src="assets/switch-team-icon.png" alt="Icono Cambiar de equipo"> para mostrar todos los equipos asignados a los grupos que administran.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Miembros del equipo]</strong> </td> 
      <td>Empiece a escribir el nombre del usuario que va a formar parte del equipo y, a continuación, seleccione el nombre cuando aparezca en la lista desplegable.<br>Repita este proceso para agregar varios usuarios al equipo.<br>Dado que los usuarios pueden estar en más de un equipo, pueden estar en equipos tanto Agile como no Agile.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Descripción de]</strong> </td> 
      <td><p>Escriba una descripción para el equipo.</p> <p>La descripción se muestra en la parte superior derecha del área [!UICONTROL Teams] cuando se selecciona el equipo.</p>
      <p>Si la descripción es larga, puede hacer clic en ella para mostrar la descripción completa en una ventana emergente. Si tiene acceso para editar la [!UICONTROL team settings], también puede editar la descripción directamente en el elemento emergente.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Crear]**.

   Para obtener información sobre la configuración de un equipo ágil, vea los siguientes artículos:

   * [Configurar [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configurar [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Convertir un equipo existente en un equipo ágil

Puede convertir un equipo existente en un equipo ágil:

{{step1-to-team}}

1. Haga clic en el icono **[!UICONTROL Cambiar equipo]** ![icono Cambiar equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Seleccione el equipo que desea convertir en un equipo ágil.
1. Haga clic en el menú **[!UICONTROL Más]** y, a continuación, seleccione **[!UICONTROL Editar]**.

   Sólo los miembros del equipo con una licencia [!UICONTROL Standard], [!UICONTROL Plan] o [!UICONTROL Work] pueden ver esta opción.
   ![Seleccionar edición](assets/edit-team-settings.png)

1. En la sección **[!UICONTROL Águila]**, seleccione **[!UICONTROL Este es un equipo ágil]**.

1. En la sección **[!UICONTROL Metodología]**, selecciona si el equipo utilizará una metodología **[!UICONTROL Scrum]** o **[!UICONTROL Kanban]** Agile.

1. Haga clic en **Guardar cambios**.

   El equipo se guarda como un equipo ágil. Puede configurar el nuevo equipo como un equipo Scrum o Kanban al editar el equipo.

   Para obtener más información, consulte los siguientes artículos:

   * [Configurar [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configurar [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
