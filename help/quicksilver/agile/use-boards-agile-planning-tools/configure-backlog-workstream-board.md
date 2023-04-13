---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: Configuración del trabajo pendiente en un tablero de flujos de trabajo
description: Puede elegir mostrar una columna de trabajo pendiente en un tablero en un flujo de trabajo y definir una consulta para las tarjetas que se arrastran al trabajo acumulado del tablero desde la lista de tarjetas del flujo de trabajo.
author: Lisa
source-git-commit: b58831d50c2be421c666515808091aa4863bb471
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Configuración del trabajo pendiente en un tablero de flujos de trabajo

Puede elegir mostrar una columna de trabajo pendiente en un tablero en un flujo de trabajo y definir una consulta para las tarjetas que se arrastran al trabajo acumulado del tablero desde la lista de tarjetas del flujo de trabajo. Estas opciones no están disponibles en tableros independientes. Para obtener información sobre cómo agregar una columna de admisión a un tablero independiente, consulte [Agregar una columna de admisión a un tablero](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

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

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Configuración del trabajo pendiente en un tablero de flujos de trabajo

{{step1-to-boards}}

1. Abra el flujo de trabajo en el que desee trabajar. Para abrir un flujo de trabajo, haga clic en [!UICONTROL **Ver flujo de trabajo**].
1. Haga clic en cualquier tablero del flujo de trabajo para abrirlo.
1. Haga clic en [!UICONTROL **Configurar**] a la derecha del tablero para abrir el panel Configurar .
1. Activar [!UICONTROL **Incluir una columna de trabajo pendiente en este tablero**].

   La columna de trabajo atrasado se agrega a la izquierda del tablero. Permanecerá en blanco hasta que se le aplique una consulta.

1. Expandir [!UICONTROL **Consulta de atrasos**].
1. Haga clic en [!UICONTROL **Añadir condición**] y haga clic en el campo &quot;vacío&quot;.
1. Seleccione el campo por el que desea realizar la consulta.

   Los campos entre los que puede elegir son los campos predeterminados de una tarjeta.

1. Seleccione el modificador de consulta.

   Las opciones son: es igual a, no es igual a, existe y no existe.

   Ejemplo: Si elige Fecha de vencimiento y existe, el registro de atrasos mostrará las tarjetas con fechas de vencimiento asignadas. Las tarjetas sin fecha de vencimiento no se arrastrarán al registro acumulado.

1. Seleccione el valor .

   El valor solo está disponible cuando se usa igual o no igual que como modificador.

1. (Opcional) Haga clic en [!UICONTROL **Añadir condición**] para agregar otra condición a la consulta.

   ![Consulta de Registro de asuntos pendientes](assets/backlog-query-wrkstrm-board.png)

1. (Opcional) Haga clic en [!UICONTROL **Crear grupo**] para añadir un grupo de condiciones conectadas a la primera condición con un operador OR.
1. Haga clic en [!UICONTROL **Guardar consulta**].

   La consulta se aplica y las tarjetas que cumplen los criterios aparecen en la columna de &quot;backlog&quot;.
