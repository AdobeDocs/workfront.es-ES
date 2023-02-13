---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: Crear un equipo ágil
description: Adobe Workfront permite a los equipos ágiles completar su trabajo de forma progresiva y organizada.
author: Lisa
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 0%

---

# Crear un equipo ágil

[!DNL Adobe Workfront] permite a los equipos ágiles completar el trabajo de forma progresiva y organizada.

Cualquier usuario de la organización puede ver el equipo ágil y todos los componentes ágiles del equipo, incluidos el trabajo pendiente, las iteraciones, el tablero de artículos y los artículos individuales. Sin embargo, solo los miembros del equipo con [!UICONTROL Editar] el acceso al trabajo puede realizar cambios en el trabajo asignado al equipo.

[!DNL Workfront] admite las siguientes metodologías ágiles:

* **[!UICONTROL Anulación]**: Los equipos tienen un trabajo atrasado que debe hacerse. Cuando el equipo está listo para trabajar en un fragmento específico de trabajo, el trabajo pasa del trabajo acumulado a una iteración. Para obtener información más detallada sobre la administración de un equipo de depuración, consulte [Anular en un equipo ágil](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL Kanban]:** Los equipos mueven el trabajo en la vista Kanban a través de estados predeterminados. Los estados predeterminados son: retraso, en proceso y finalizado. Para obtener información más detallada sobre la administración de un equipo Kanban, consulte [Kanban en un equipo ágil](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

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
   <td> <p>[!UICONTROL Plan] para crear un nuevo equipo ágil; [!UICONTROL Work] o superior para convertir un equipo en un equipo ágil</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan o tipo de licencia tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Decidir sobre una metodología ágil

Puede utilizar una metodología ágil de Scrum o Kanban para su equipo ágil. Cada metodología ofrece diversos beneficios. La forma en que funciona su equipo ágil determina la metodología ágil que elija utilizar.

Metodologías ágiles tanto de Scrum como de Kanban en [!DNL Workfront] permite mover artículos a través de un tablero de artículos para indicar un cambio de estado y el progreso del artículo.

Metodologías ágiles de Scrum y Kanban en [!DNL Workfront] difieren en los siguientes modos:

### Ventajas de usar Kanban en [!DNL Workfront]

La variable [!DNL Kanban] metodología ágil en [!DNL Workfront] le permite mover artículos más fácilmente entre un tablero de artículos ágil y, a la vez, limitar la cantidad de trabajo en curso. No hay fechas de inicio y finalización al usar la variable [!DNL Kanban] metodología ágil.

La siguiente funcionalidad admite esta metodología:

* Mostrar el trabajo atrasado en el [!DNL Kanban] tablero de historia ágil.\
   Para obtener más información, consulte [Añada el trabajo atrasado al [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* Configure los elementos en el registro anterior para que se agreguen automáticamente al [!UICONTROL Kanban] tablero de artículos ágil cuando se mueven otros elementos a un estado que coincide con Complete.\
   Para obtener más información, consulte la sección [Configurar artículos para que se agreguen automáticamente desde el registro acumulado](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) en el artículo [Configurar Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configure un límite de trabajo en curso (WIP) para que se muestre en la [!UICONTROL Kanban] tablero de historia ágil.\
   Para obtener más información, consulte [Administrar el límite de trabajo en curso (WIP) en el panel Kanban](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Beneficios del uso de Scrum en [!DNL Workfront]

La metodología ágil de Scrum en [!DNL Workfront] permite agregar un conjunto de artículos a una iteración ágil y crear un tablero de artículos para esa iteración. La iteración se basa en las fechas de inicio y finalización definidas.

La siguiente funcionalidad admite esta metodología:

* Incluir problemas en la variable [!UICONTROL Anulación] tablero de historia
* Incluir problemas en el trabajo pendiente de un equipo ágil
* Las subtareas se pueden mostrar en la [!UICONTROL Anulación] tablero de historia
* Ver un gráfico desglosado para ver el progreso con respecto a los artículos durante la iteración\
   Para obtener más información, consulte [Descripción general de la tabla de correspondencias de Agile](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Crear un nuevo equipo ágil

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Equipos]**.
1. Haga clic en el **[!UICONTROL Cambiar equipos]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png)y haga clic en **[!UICONTROL Crear nuevo equipo]**.

   ![Seleccione Crear nuevo equipo.](assets/create-new-team-350x198.png)

1. Especifique la siguiente información sobre la variable [!UICONTROL Nuevo equipo] diálogo:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Name]</strong> </td> 
      <td>Escriba un nombre para el nuevo equipo ágil.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Éste es un equipo Agile]</strong> </td> 
      <td>Seleccione esta opción para configurar este nuevo equipo para que sea un equipo ágil.</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL Group]</strong> </td> 
      <td> <p>Empiece a escribir el nombre de un grupo que desee agregar al equipo y, a continuación, seleccione el nombre cuando aparezca en la lista desplegable.</p> <p>Nota: Cuando se asigna un equipo a un grupo o subgrupo, cualquier administrador de grupo de ese grupo o subgrupo puede administrar el equipo sin ser miembro de él. Los administradores de grupo pueden ir al área [!UICONTROL Teams] desde el [!UICONTROL Main Menu] y hacer clic en la flecha [!UICONTROL Switch Teams] <img src="assets/switch-team-icon.png" alt="Icono Cambiar equipo"> para enumerar todos los equipos asignados a los grupos que administran.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Integrantes del equipo]</strong> </td> 
      <td>Empiece a escribir el nombre de un usuario que formará parte del equipo y, a continuación, seleccione el nombre cuando aparezca en la lista desplegable.<br>Repita este proceso para agregar varios usuarios al equipo.<br>Como los usuarios pueden estar en más de un equipo, pueden estar en equipos ágiles y no ágiles.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Descripción]</strong> </td> 
      <td><p>Escriba una descripción para el equipo.</p> <p>La descripción se muestra en la parte superior derecha del área [!UICONTROL Teams] cuando se selecciona el equipo.</p>
      <p>Si la descripción es larga, puede hacer clic en ella para mostrar la descripción completa en una ventana emergente. Si tiene acceso para editar la [!UICONTROL configuración del equipo], también puede editar la descripción directamente en la ventana emergente.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Crear]**.

   Para obtener información sobre la configuración de un equipo Agile, consulte los siguientes artículos:

   * [Configurar [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configurar [!UICONTROL Anulación]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Conversión de un equipo existente en un equipo ágil

Puede convertir un equipo existente en un equipo ágil:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Equipos]**.
1. Haga clic en el **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png), seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Seleccione el equipo que desea convertir en un equipo ágil.
1. Haga clic en el **[!UICONTROL Más]** a continuación, seleccione **[!UICONTROL Editar]**.\
   Solo los integrantes del equipo con una [!UICONTROL Plan] o [!UICONTROL Trabajo] licencia consulte esta opción.\
   ![](assets/edit-team-settings-350x205.png)

1. En el **[!UICONTROL Águila]** , seleccione **[!UICONTROL Este es un equipo Agile]**.

1. En el **[!UICONTROL Metodología]** , seleccione si el equipo utilizará una **[!UICONTROL Anulación]** o **[!UICONTROL Kanban]** metodología ágil.

1. Haga clic en **Guarde los cambios.**

   Para obtener información sobre la configuración de un equipo Agile, consulte los siguientes artículos:

   * [Configurar [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configurar [!UICONTROL Anulación]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
