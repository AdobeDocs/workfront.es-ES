---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: Crear un equipo ágil
description: Adobe Workfront permite a los equipos de Agile completar el trabajo de forma incremental y organizada.
author: Lisa
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '1012'
ht-degree: 1%

---

# Crear un equipo ágil

<!--Audited: 01/2024-->

[!DNL Adobe Workfront] permite a los equipos de agile completar el trabajo de forma incremental y organizada.

Cualquier usuario de la organización puede ver el equipo Agile y todos los componentes Agile del equipo, incluidos el registro de pendientes, las iteraciones, el guion gráfico y las historias individuales. Sin embargo, solo los miembros del equipo con [!UICONTROL Editar] el acceso al trabajo puede realizar cambios en el trabajo asignado al equipo.

[!DNL Workfront] admite las siguientes metodologías agile:

* **[!UICONTROL Scrum]**: los equipos tienen un registro de pendientes del trabajo que debe realizarse. Cuando el equipo está listo para trabajar en una parte específica del trabajo, el trabajo se mueve del registro de pendientes a una iteración. Para obtener información más detallada sobre la administración de un equipo de Scrum, consulte [Scrum en un equipo ágil](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL Kanban]:** Los equipos mueven el trabajo en la vista Kanban a través de estados predeterminados. Los estados predeterminados son: registro de pendientes, en proceso y listo. Para obtener información más detallada sobre la gestión de un equipo Kanban, consulte [Kanban en un equipo ágil](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>Nuevo: estándar</p>
   Actual: 
   <ul><li><p>[!UICONTROL Plan] para crear un nuevo equipo Agile</p></li> 
   <li><p>[!UICONTROL Work] o superior para convertir un equipo en un equipo Agile</p></li></ul> </td> 
  </tr> 
 </tbody> 
</table>

Para averiguar qué plan o tipo de licencia tiene, póngase en contacto con su [!DNL Workfront] administrador.

+++

## Decidir una metodología ágil

Puede utilizar una metodología Agile de Scrum o Kanban para su equipo Agile. Cada metodología ofrece varios beneficios. La forma en que trabaja su equipo Agile determina la metodología Agile que elija utilizar.

Metodologías ágiles de Scrum y Kanban en [!DNL Workfront] permite mover historias a través de un guion gráfico para indicar un cambio de estado y el progreso de la historia.

Metodologías ágiles de Scrum y Kanban en [!DNL Workfront] difieren en los siguientes aspectos:

### Ventajas de utilizar Kanban en [!DNL Workfront]

El [!DNL Kanban] metodología Agile en [!DNL Workfront] le permite mover con mayor facilidad las historias a través de un panel de historias Agile al mismo tiempo que limita la cantidad de trabajo en curso. No hay fechas de inicio y finalización al utilizar [!DNL Kanban] metodología Agile.

La siguiente funcionalidad es compatible con esta metodología:

* Mostrar el registro de pendientes en [!DNL Kanban] agile story board.\
   Para obtener más información, consulte [Añada el registro de pendientes a [!UICONTROL Kanban] tablero](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* Configure los elementos del registro de pendientes para que se agreguen automáticamente al [!UICONTROL Kanban] guion gráfico de Agile cuando otros elementos se mueven a un estado que equivale a Completado.\
   Para obtener más información, consulte la sección [Configurar historias para que se agreguen automáticamente desde el registro de pendientes](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) en el artículo [Configurar Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configure un límite de trabajo en curso (WIP) para que se muestre en la [!UICONTROL Kanban] agile story board.\
   Para obtener más información, consulte [Administrar el límite de trabajo en curso (WIP) en el Panel Kanban](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Ventajas de usar Scrum en [!DNL Workfront]

La metodología Scrum agile en [!DNL Workfront] permite agregar un conjunto de historias a una iteración Agile y crear un guion gráfico para esa iteración. La iteración se basa en las fechas de inicio y finalización definidas.

La siguiente funcionalidad es compatible con esta metodología:

* Incluir problemas en [!UICONTROL Scrum] guion gráfico
* Incluir problemas en el registro de pendientes de un equipo Agile
* Las subtareas se pueden mostrar en la [!UICONTROL Scrum] guion gráfico
* Ver un gráfico de evolución para ver el progreso de las historias durante la iteración\
   Para obtener más información, consulte [Resumen del gráfico de evolución Agile](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Crear un equipo ágil

{{step1-to-team}}

1. Haga clic en **[!UICONTROL Cambiar equipos]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png), luego haga clic en **[!UICONTROL Crear nuevo equipo]**.

   ![Seleccione Crear nuevo equipo.](assets/create-new-team-350x198.png)

   Aparece el cuadro Nuevo equipo.

1. Especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Nombre de equipo]</strong> </td> 
      <td>Escriba un nombre para el nuevo equipo Agile.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Este es un equipo Agile]</strong> </td> 
      <td>Seleccione esta opción para configurar este nuevo equipo para que sea un equipo Agile.</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>[!UICONTROL Está Activo]</strong> </td> 
      <td>Seleccione esta opción para activar este equipo. Los equipos inactivos no son visibles para que otros usuarios los asignen al trabajo. </td> 
     </tr>


   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL Grupo]</strong> </td> 
      <td> <p>Empiece a escribir el nombre de un grupo para agregarlo al equipo y, a continuación, seleccione el nombre cuando aparezca en la lista desplegable.</p> <p><b>NOTA</b></p> <p> Cuando se asigna un equipo a un grupo o subgrupo, cualquier administrador de grupo de ese grupo o subgrupo puede administrar el equipo sin ser miembro del equipo. Los administradores de grupos pueden ir al área de [!UICONTROL Teams] desde el menú principal de [!UICONTROL] y hacer clic en la flecha de [!UICONTROL Switch Teams] <img src="assets/switch-team-icon.png" alt="Icono Cambiar equipo"> para enumerar todos los equipos asignados a los grupos que administran.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Miembros del equipo]</strong> </td> 
      <td>Empiece a escribir el nombre de un usuario para que esté en el equipo y, a continuación, seleccione el nombre cuando aparezca en la lista desplegable.<br>Repita este proceso para agregar varios usuarios al equipo.<br>Dado que los usuarios pueden estar en más de un equipo, pueden estar en equipos Agile y no Agile.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Descripción]</strong> </td> 
      <td><p>Escriba una descripción para el equipo.</p> <p>La descripción se muestra en la parte superior derecha del área de [!UICONTROL Teams] cuando se selecciona el equipo.</p>
      <p>Si la descripción es larga, puede hacer clic en ella para mostrar la descripción completa en una ventana emergente. Si tiene acceso para editar la configuración del equipo de [!UICONTROL], también puede editar la descripción directamente en la ventana emergente.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Crear]**.

   Para obtener información sobre la configuración de un equipo Agile, consulte los siguientes artículos:

   * [Configurar [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configurar [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Convertir un equipo existente en un equipo Agile

Puede convertir un equipo existente en un equipo Agile:

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront], luego haga clic en **[!UICONTROL Equipos]**.
1. Haga clic en **[!UICONTROL Cambiar equipo]** icono ![Icono Cambiar equipo](assets/switch-team-icon.png), seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Seleccione el equipo que desea convertir en un equipo Agile.
1. Haga clic en **[!UICONTROL Más]** menú, luego seleccione **[!UICONTROL Editar]**.\
   Solo los miembros del equipo con un [!UICONTROL Plan] o [!UICONTROL Trabajo] licencia consulte esta opción.\
   ![](assets/edit-team-settings-350x205.png)

1. En el **[!UICONTROL Agile]** , seleccione **[!UICONTROL Este es un equipo ágil]**.

1. En el **[!UICONTROL Metodología]** , seleccione si el equipo va a utilizar un **[!UICONTROL Scrum]** o **[!UICONTROL Kanban]** metodología Agile.

1. Clic **Guardar cambios.**

   El equipo se guarda como un equipo Agile. Puede configurar el nuevo equipo como un equipo de Scrum o Kanban cuando edite el equipo.

   Para obtener más información, consulte los siguientes artículos:

   * [Configurar [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configurar [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
