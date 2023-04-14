---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: Configuración del trabajo pendiente en un tablero de flujos de trabajo
description: Puede elegir mostrar una columna de trabajo pendiente en un tablero en un flujo de trabajo y definir una consulta para las tarjetas que se arrastran al trabajo acumulado del tablero desde la lista de tarjetas del flujo de trabajo.
author: Lisa
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: 75bb5af9564947a39e1cb46f9d6be2c03eb07acc
workflow-type: tm+mt
source-wordcount: '416'
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

   >[!NOTE]
   >
   >Es posible que ya se haya aplicado una consulta predeterminada al registro acumulado, que muestra todos los elementos de trabajo de la lista de tarjetas que no pertenecen a una iteración y que no están en estado Complete .

1. Haga clic en [!UICONTROL **Añadir condición**] y haga clic en el campo &quot;vacío&quot;.
1. Seleccione el campo por el que desea realizar la consulta.

   Los campos entre los que puede elegir son los campos predeterminados de una tarjeta.

1. Seleccione el modificador de consulta.

   Las opciones del modificador dependen de los campos a los que se puedan aplicar. Por ejemplo, el campo &quot;nombre&quot; no tiene &quot;bueno que&quot; o &quot;menor que&quot; como opciones modificadoras porque esos modificadores solo se aplican a los números.

1. Seleccione el valor .

   El valor no está disponible cuando se usa &quot;existe&quot; o &quot;no existe&quot; como modificador.

   Por ejemplo, si elige &quot;Fecha de vencimiento&quot; y &quot;existe&quot;, el registro de atrasos mostrará tarjetas con fechas de vencimiento asignadas. Las tarjetas sin fecha de vencimiento no se arrastrarán al registro acumulado.

1. (Opcional) Haga clic en [!UICONTROL **Añadir condición**] para agregar otra condición a la consulta.

   ![Consulta de Registro de asuntos pendientes](assets/backlog-query-wrkstrm-board.png)

1. (Opcional) Haga clic en [!UICONTROL **Crear grupo**] para añadir un grupo de condiciones conectadas a la primera condición con un operador OR.
1. Haga clic en [!UICONTROL **Guardar consulta**].

   La consulta se aplica y las tarjetas que cumplen los criterios aparecen en la columna de &quot;backlog&quot;.
