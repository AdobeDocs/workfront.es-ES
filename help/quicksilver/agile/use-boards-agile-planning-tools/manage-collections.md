---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Administrar flujos de trabajo
description: Un flujo de trabajo es un grupo configurable de tableros y tarjetas para colaborar en el trabajo.
author: Lisa
feature: Agile
source-git-commit: 8c02f5364154bdc343512416d0c7e38ef563a170
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 3%

---

# Administrar flujos de trabajo

Un flujo de trabajo es un grupo configurable de tableros y tarjetas para colaborar en el trabajo. Los flujos de trabajo pueden incluir distintos tipos de tableros creados a partir de plantillas y una lista de tarjetas de elementos de trabajo. En un flujo de trabajo, se puede realizar un seguimiento del trabajo en iteraciones o sprints.

Para obtener más información, consulte [Usar la lista de tarjetas](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) y [Creación de una iteración en un flujo de trabajo](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

Los flujos de trabajo aparecen en el tablero junto con los tableros individuales a los que tiene acceso que no forman parte de un flujo de trabajo. Para obtener información sobre el tablero de tableros, consulte [Usar el tablero de tableros](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md). Puede hacer clic en cualquier nombre de tablero del tablero para abrirlo.

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
   <td> <p>[!UICONTROL Request] o superior</p> </td> 
  </tr> 
 </tbody> 
</table>

## Creación de un flujo de trabajo

{{step1-to-boards}}

1. Haga clic en **[!UICONTROL Agregar flujo de trabajo]** en el [!UICONTROL Flujos de trabajo] del panel.
1. Escriba un nombre para reemplazarlo **[!UICONTROL Flujo de trabajo sin título]** y pulse Intro.

   Puede agregar tableros al flujo de trabajo o hacer clic en [!UICONTROL **Todos los tableros**] para volver al tablero.

## Crear un tablero nuevo en un flujo de trabajo

1. Si aún no está en un flujo de trabajo, haga clic en [!UICONTROL **Ver flujo de trabajo**] en el tablero para abrir un flujo de trabajo existente.
1. Haga clic en **[!UICONTROL Agregar tablero]** en el [!UICONTROL Tableros] del flujo de trabajo.
1. Seleccione una plantilla para el tablero.

| Plantilla | Descripción |
|---------|----------|
| Tablero básico | Se proporcionan tres columnas predeterminadas en el tablero. Puede agregar nuevas columnas y cambiar el nombre o eliminar las columnas predeterminadas. <p>No se aplica ninguna directiva de columna. |
| Tablero Kanban | En el tablero se proporcionan las columnas siguientes: Retraso, Nuevo, En curso, Completado y En espera. Puede agregar nuevas columnas y cambiar el nombre o eliminar las columnas predeterminadas.<p>Para utilizar el trabajo pendiente, debe configurar filtros para la columna de admisión. Para obtener más información, consulte [Agregar una columna de admisión a un tablero](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Para revisar las directivas predeterminadas de cada columna, haga clic en el botón [!UICONTROL **Más** menú] en una columna y seleccione [!UICONTROL **Editar**]. Puede cambiar cualquiera de estas directivas preconfiguradas. Para obtener más información, consulte [Administrar columnas de tablero](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| Tablero retrospectivo | En el tablero se proporcionan las columnas siguientes: ¿Qué fue bien? Qué se podría mejorar? A quién debemos homenajear? Qué podemos hacer para avanzar más rápido? Puede agregar nuevas columnas y cambiar el nombre o eliminar las columnas predeterminadas. <p>No se aplica ninguna directiva de columna. |
| Proceso de iteración | Este es el tablero utilizado para definir y ejecutar una iteración. <p>En el tablero se proporcionan las columnas siguientes: Retraso, Nuevo, En curso, Completado y En espera. No se puede agregar ninguna columna al tablero. <p>Para revisar las directivas predeterminadas de cada columna, haga clic en el botón [!UICONTROL **Más**] en una columna y seleccione [!UICONTROL **Editar**]. Puede cambiar cualquiera de estas directivas preconfiguradas. Para obtener más información, consulte [Administrar columnas de tablero](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

Para obtener más información sobre la configuración del tablero, consulte [Crear o editar un tablero](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## Filtrar la lista de tableros en un flujo de trabajo

Cuando se aplican filtros que no son los predeterminados en la lista de tableros, se muestra un indicador en el icono de filtro ![Filtro aplicado](assets/boards-filterapplied-30x30.png). Haga clic en [!UICONTROL **Borrar todo**] para eliminar todos los filtros y haga clic en [!UICONTROL **Ocultar filtros**] para cerrar el panel de filtro.

{{step1-to-boards}}

1. En el tablero, haga clic en [!UICONTROL **Ver flujo de trabajo**] para abrir un flujo de trabajo.
1. Haga clic en el [!UICONTROL **Tableros**] si no se muestra.
1. Haga clic en [!UICONTROL **Filtro**].
1. Seleccione los tableros que desee ver por estado (tableros archivados, tableros activos o todos los tableros).
1. Seleccione los tableros que desea ver por plantilla.

## Agregar miembros a un flujo de trabajo

Para poder ver el flujo de trabajo y su contenido, se deben agregar personas y equipos al flujo de trabajo como miembros. Un miembro del flujo de trabajo puede agregar y eliminar miembros del flujo de trabajo y ver qué tableros están en el flujo de trabajo.

>[!NOTE]
>
>Un miembro del flujo de trabajo no puede abrir un tablero en un flujo de trabajo hasta que se añada a ese tablero específico como miembro.

{{step1-to-boards}}

1. En el tablero, haga clic en [!UICONTROL **Ver flujo de trabajo**] para abrir un flujo de trabajo.
1. Haga clic en el **[!UICONTROL Agregar miembro]** icono ![Agregar miembros](assets/boards-addmember-spectrum-25x25.png) para agregar miembros y equipos al flujo de trabajo.

   Este es el mismo proceso que agregar miembros a un tablero. Para obtener más información, consulte [Agregar o quitar miembros de un tablero](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

## Configuración de un flujo de trabajo

{{step1-to-boards}}

1. En el tablero, haga clic en [!UICONTROL **Ver flujo de trabajo**] para abrir un flujo de trabajo.
1. Haga clic en [!UICONTROL **Configurar**] para abrir el [!UICONTROL Configurar flujo de trabajo] panel.
1. (Opcional) Escriba una descripción del flujo de trabajo. Esta descripción se muestra en el panel.

   El número total de tarjetas, el número de tarjetas señaladas y el número de iteraciones se muestran en la sección Lista de tarjetas . Haga clic en [!UICONTROL **Ver lista**] para abrir la lista y añadir tarjetas. Para obtener más información, consulte [Usar la lista de tarjetas](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   Si se ha definido una iteración, se muestra su fecha de inicio, el número de tarjetas y el número de puntos. Haga clic en [!UICONTROL **Ver tablero de iteración**] para abrir el tablero. Para obtener más información, consulte [Creación de una iteración en un flujo de trabajo](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. Haga clic en [!UICONTROL **Agregar fuente**] para definir un origen para importar tarjetas en el flujo de trabajo. En este momento, la única fuente disponible es [!DNL Adobe Workfront].
1. Añada filtros para importar tareas y problemas desde Workfront como tarjetas.

   Añadir filtros para fuentes de flujo de trabajo es lo mismo que agregar filtros para una columna de admisión en un tablero básico o un tablero kanban. Para obtener más información, consulte [Agregar una columna de admisión a un tablero](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

