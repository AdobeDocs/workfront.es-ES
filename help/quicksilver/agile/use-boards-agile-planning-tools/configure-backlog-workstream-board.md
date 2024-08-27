---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: Configurar el registro de pendientes en un panel de flujo de trabajo
description: Puede elegir mostrar una columna de registro de pendientes en un tablero de un flujo de trabajo y definir una consulta para las tarjetas que se incorporan al registro de asuntos pendientes del tablero desde la lista de tarjetas del flujo de trabajo.
author: Lisa
feature: Agile
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# Configurar el registro de pendientes en una placa de flujo de trabajo

>[!IMPORTANT]
>
>Los flujos de trabajo solo están disponibles para un grupo específico de clientes.

Puede elegir mostrar una columna de registro de pendientes en un tablero de un flujo de trabajo y definir una consulta para las tarjetas que se incorporan al registro de asuntos pendientes del tablero desde la lista de tarjetas del flujo de trabajo.

>[!NOTE]
>
>Si agrega una tarjeta nueva en la columna de registro de pendientes que no coincide con los criterios de consulta, la tarjeta desaparecerá del registro de asuntos pendientes cuando se actualice el tablero y solo estará disponible en la lista de tarjetas. Puede cambiar la consulta en cualquier momento para ajustar qué tarjetas aparecen en la columna de registro de pendientes.

La columna de registro de pendientes y la consulta no están disponibles en tableros independientes. Para obtener información acerca de cómo agregar una columna de entrada a un tablero independiente, vea [Agregar una columna de entrada a un tablero](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td> 
   <p>Nuevo: [!UICONTROL Contributor] o superior</p> 
   <p>o</p>
   <p>Actual: [!UICONTROL Request] o superior</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar el registro de pendientes en una placa de flujo de trabajo

{{step1-to-boards}}

1. Abra el flujo de trabajo en el que desee trabajar. Para abrir un flujo de trabajo, haga clic en [!UICONTROL **Ver flujo de trabajo**].
1. Haga clic en cualquier tablero del flujo de trabajo para abrirlo.
1. Haga clic en [!UICONTROL **Configurar**] a la derecha del tablero para abrir el panel Configurar.
1. Activar [!UICONTROL **Incluir una columna de registro de pendientes en este tablero**].

   La columna de registro de pendientes se agrega a la izquierda del tablero. Permanece en blanco hasta que se le aplica una consulta.

1. Expandir [!UICONTROL **consulta de registro de pendientes**].

   >[!NOTE]
   >
   >Es posible que ya se haya aplicado una consulta predeterminada al registro de pendientes, que muestre todos los elementos de trabajo de la lista de tarjetas que tienen un estado y el estado no es Completo.

1. Haga clic en [!UICONTROL **Agregar condición**] y haga clic en el campo &quot;vacío&quot;.
1. Seleccione el campo por el que desea realizar la consulta.

   Los campos que puede elegir son los campos predeterminados de una tarjeta.

1. Seleccione el modificador de consulta.

   Las opciones del modificador dependen de los campos a los que se puedan aplicar. Por ejemplo, el campo &quot;nombre&quot; no tiene como modificadores &quot;mayor que&quot; o &quot;menor que&quot; porque estos modificadores sólo se aplican a números.

1. Seleccione el valor.

   El valor no está disponible cuando se utiliza &quot;existe&quot; o &quot;no existe&quot; como modificador.

   Por ejemplo, si elige &quot;Fecha de vencimiento&quot; y &quot;existe&quot;, el registro de pendientes mostrará las tarjetas con fechas de vencimiento asignadas. Las tarjetas que no tengan fecha de vencimiento no se incluirán en el registro de pendientes.

1. (Opcional) Haga clic en [!UICONTROL **Agregar condición**] para agregar otra condición a la consulta.

   ![Consulta de registro de pendientes](assets/backlog-query-wrkstrm-board.png)

1. (Opcional) Haga clic en [!UICONTROL **Crear grupo**] para agregar un grupo de condiciones conectadas a la primera condición con un operador OR.
1. Haga clic en [!UICONTROL **Guardar consulta**].

   La consulta se aplica y las tarjetas que cumplen los criterios aparecen en la columna registro de pendientes.
