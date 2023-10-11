---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Administrar flujos de trabajo
description: Un flujo de trabajo es un grupo configurable de tableros y tarjetas para colaborar en el trabajo.
author: Lisa
feature: Agile
exl-id: c46c42e8-e14d-414d-b883-c4d885338e42
source-git-commit: 4e5bff5ad62dce8766072e04e3a2b89371a90f03
workflow-type: tm+mt
source-wordcount: '915'
ht-degree: 2%

---

# Administrar flujos de trabajo

>[!IMPORTANT]
>
>Los flujos de trabajo solo están disponibles para un grupo específico de clientes.

Un flujo de trabajo es un grupo configurable de tableros y tarjetas para colaborar en el trabajo. Los flujos de trabajo pueden incluir diferentes tipos de tableros creados a partir de plantillas y una lista de tarjetas de elementos de trabajo. En un flujo de trabajo, se puede realizar un seguimiento del trabajo en iteraciones o sprints.

Para obtener más información, consulte [Usar la lista de tarjetas](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) y [Creación de una iteración en un flujo de trabajo](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

Los flujos de trabajo aparecen en el tablero junto con los tableros a los que tiene acceso que no forman parte de un flujo de trabajo. Para obtener información sobre el tablero de tableros, consulte [Uso del tablero de mandos](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md). Puede hacer clic en cualquier nombre de tablero del tablero para abrirlo.

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

## Crear un flujo de trabajo

{{step1-to-boards}}

1. Clic **[!UICONTROL Agregar flujo de trabajo]** en el [!UICONTROL Flujos de trabajo] del tablero de mandos.
1. Escriba un nombre para reemplazar **[!UICONTROL Flujo de trabajo sin título]** y pulse Intro.

   Puede añadir tableros al flujo de trabajo o hacer clic en [!UICONTROL **Todos los tableros**] para volver al tablero.

## Creación de un nuevo tablero en un flujo de trabajo

1. Si aún no se encuentra en un flujo de trabajo, haga clic en [!UICONTROL **Ver flujo de trabajo**] en el panel para abrir un flujo de trabajo existente.
1. Clic **[!UICONTROL Añadir tablero]** en el [!UICONTROL Tableros] del flujo de trabajo.
1. Seleccione una plantilla para el tablero.

| Plantilla | Descripción |
|---------|----------|
| Tablero básico | Se proporcionan tres columnas predeterminadas en el tablero. Puede agregar nuevas columnas y cambiar el nombre de las columnas predeterminadas o eliminarlas. <p>No se aplican políticas de columna. |
| Tablero Kanban | Se proporcionan las siguientes columnas en el tablero: Registro de pendientes, Nuevo, En curso, Completado y En espera. Puede agregar nuevas columnas y cambiar el nombre de las columnas predeterminadas o eliminarlas.<p>Para utilizar el registro de pendientes, debe configurar filtros para la columna de entrada. Para obtener más información, consulte [Agregar una columna de entrada a un tablero](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Para revisar las directivas predeterminadas de cada columna, haga clic en [!UICONTROL **Más** menú] en una columna y seleccione [!UICONTROL **Editar**]. Puede cambiar cualquiera de estas directivas preconfiguradas. Para obtener más información, consulte [Administrar columnas del tablero](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| Tablero retrospectivo | En el tablero se proporcionan las siguientes columnas: ¿Qué ha ido bien? Qué se podría mejorar? A quién debemos homenajear? Qué podemos hacer para avanzar más rápido? Puede agregar nuevas columnas y cambiar el nombre de las columnas predeterminadas o eliminarlas. <p>No se aplican políticas de columna. |
| Proceso de iteración | Este es el tablero utilizado para definir y ejecutar una iteración. <p>Se proporcionan las siguientes columnas en el tablero: Registro de pendientes, Nuevo, En curso, Completado y En espera. No se puede añadir ninguna columna al tablero. <p>Para revisar las directivas predeterminadas de cada columna, haga clic en [!UICONTROL **Más**] en una columna y seleccione [!UICONTROL **Editar**]. Puede cambiar cualquiera de estas directivas preconfiguradas. Para obtener más información, consulte [Administrar columnas del tablero](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

Para obtener más información sobre la configuración del tablero, consulte [Crear o editar un tablero](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## Filtrado de la lista de tableros de un flujo de trabajo

Cuando se aplican filtros distintos de los predeterminados en la lista del tablero, se muestra un indicador en el icono de filtro ![Filtro aplicado](assets/boards-filterapplied-30x30.png). Clic [!UICONTROL **Borrar todo**] para eliminar todos los filtros, y haga clic en [!UICONTROL **Ocultar filtros**] para cerrar el panel de filtro.

{{step1-to-boards}}

1. En el tablero, haga clic en [!UICONTROL **Ver flujo de trabajo**] para abrir un flujo de trabajo.
1. Haga clic en [!UICONTROL **Tableros**] pestaña si aún no se muestra.
1. Clic [!UICONTROL **Filtrar**].
1. Seleccione los tableros que desee ver por estado (tableros archivados, tableros activos o todos los tableros).
1. Seleccione los tableros que desee ver por plantilla.

## Añadir miembros a un flujo de trabajo

Las personas y los equipos deben agregarse al flujo de trabajo como miembros para poder ver el flujo de trabajo y su contenido. Un miembro del flujo de trabajo puede agregar y quitar miembros del flujo de trabajo y ver qué tableros hay en el flujo de trabajo.

>[!NOTE]
>
>Un miembro del flujo de trabajo no puede abrir un tablero en un flujo de trabajo hasta que se añada a ese tablero específico como miembro.

{{step1-to-boards}}

1. En el tablero, haga clic en [!UICONTROL **Ver flujo de trabajo**] para abrir un flujo de trabajo.
1. Haga clic en **[!UICONTROL Añadir miembro]** icono ![Añadir miembros](assets/boards-addmember-spectrum-25x25.png) para agregar miembros y equipos al flujo de trabajo.

   Este es el mismo proceso que agregar miembros a un tablero. Para obtener más información, consulte [Agregar o quitar miembros de un tablero](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

## Añadir fuentes a un flujo de trabajo

Una fuente determina de dónde provienen las tarjetas del flujo de trabajo.

{{step1-to-boards}}

1. Haga clic en [!UICONTROL **Fuentes**] icono ![Icono Fuentes](assets/sources-icon.png) para definir un origen para importar tarjetas en el flujo de trabajo. En este momento, la única fuente disponible es [!DNL Adobe Workfront].
1. Agregue filtros para importar tareas y problemas de Workfront como tarjetas.

   Añadir filtros para fuentes de flujo de trabajo es lo mismo que añadir filtros avanzados para una columna de entrada en un panel básico o en un panel Kanban. Para obtener más información, consulte [Agregar una columna de entrada a un tablero](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Configuración de un flujo de trabajo

{{step1-to-boards}}

1. En el tablero, haga clic en [!UICONTROL **Ver flujo de trabajo**] para abrir un flujo de trabajo.
1. Clic [!UICONTROL **Configurar**] para abrir [!UICONTROL Configurar flujo de trabajo] panel.
1. (Opcional) Expandir [!UICONTROL **Workstream**] y escriba una descripción del flujo de trabajo. Esta descripción se muestra en el panel.
1. (Opcional) Expandir [!UICONTROL **Iteraciones**] para definir un proceso de iteración para este flujo de trabajo.

   El número total de tarjetas, el número de tarjetas señaladas y el número de iteraciones se muestran en la sección Lista de tarjetas. Clic [!UICONTROL **Ver lista**] para abrir la lista y agregar tarjetas. Para obtener más información, consulte [Usar la lista de tarjetas](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   Si ya se ha definido una iteración, se muestran su fecha de inicio, el número de tarjetas y el número de puntos. Clic [!UICONTROL **Ver tablero**] para abrir el tablero de iteraciones. Para obtener más información, consulte [Creación de una iteración en un flujo de trabajo](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. (Opcional) Expandir [!UICONTROL **Etiquetas**] para añadir etiquetas al flujo de trabajo. Busque una etiqueta o escriba un nuevo nombre de etiqueta en el cuadro de búsqueda y pulse Intro para crearla.
