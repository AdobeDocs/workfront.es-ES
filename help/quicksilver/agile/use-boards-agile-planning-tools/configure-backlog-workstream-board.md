---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: Configurar el registro de pendientes en un panel de flujo de trabajo
description: Puede elegir mostrar una columna de registro de asuntos pendientes en un tablero de una secuencia de trabajo y definir una consulta para las tarjetas que se incorporan al registro de asuntos pendientes del tablero desde la lista de tarjetas de la secuencia de trabajo.
author: Lisa
feature: Agile
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 97%

---

# Configurar el registro de asuntos pendientes en un tablero de flujo de trabajo

>[!IMPORTANT]
>
>Las secuencias de trabajo solo están disponibles para un grupo específico de clientes.

Puede elegir mostrar una columna de registro de asuntos pendientes en un tablero de una secuencia de trabajo y definir una consulta para las tarjetas que se incorporan al registro de asuntos pendientes del tablero desde la lista de tarjetas de la secuencia de trabajo.

>[!NOTE]
>
>Si añade una tarjeta nueva en la columna de registro de asuntos pendientes que no coincide con los criterios de consulta, la tarjeta desaparecerá del registro de asuntos pendientes cuando se actualice el tablero y solo estará disponible en la lista de tarjetas. Puede cambiar la consulta en cualquier momento para ajustar qué tarjetas aparecen en la columna del registro de asuntos pendientes.

La columna de registro de asuntos pendientes y la consulta no están disponibles en tableros independientes. Para obtener información acerca de cómo añadir una columna de entrada a un tablero independiente, consulte [Añadir una columna de entrada a un tablero](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o superior</p> 
   <p>Solicitud o superior</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar el registro de asuntos pendientes en un tablero de flujo de trabajo

{{step1-to-boards}}

1. Abra la secuencia de trabajo en la que desee trabajar. Para abrir una secuencia de trabajo, haga clic en [!UICONTROL **Ver secuencia de trabajo**].
1. Haga clic en cualquier tablero de la secuencia de trabajo para abrirlo.
1. Haga clic en [!UICONTROL **Configurar**] a la derecha del tablero para abrir el panel Configurar.
1. Active [!UICONTROL **Incluir una columna del registro de asuntos pendientes en este tablero**].

   La columna del registro de asuntos pendientes se añade a la izquierda del tablero. Permanece en blanco hasta que se le aplica una consulta.

1. Expanda [!UICONTROL **Consulta en el registro de asuntos pendientes**].

   >[!NOTE]
   >
   >Es posible que ya se haya aplicado una consulta predeterminada al registro de asuntos pendientes, que muestra todos los elementos de trabajo de la lista de tarjetas que tienen un estado y el estado no sea Completado.

1. Haga clic en [!UICONTROL **Añadir condición**] y haga clic en el campo “vacío”.
1. Seleccione el campo por el que desea realizar la consulta.

   Los campos que puede elegir son los campos predeterminados de una tarjeta.

1. Seleccione el modificador de la consulta.

   Las opciones del modificador dependen de los campos a los que se puedan aplicar. Por ejemplo, el campo “nombre” no tiene como modificadores “mayor que” o “menor que” porque estos modificadores solo se aplican a números.

1. Seleccione el valor.

   El valor no está disponible cuando se utiliza “existe” o “no existe” como modificador.

   Por ejemplo, si elige “Fecha de vencimiento” y “existe”, el registro de asuntos pendientes mostrará las tarjetas con fechas de vencimiento asignadas. Las tarjetas que no tengan fecha de vencimiento no se incluirán en el registro de asuntos pendientes.

1. (Opcional) Haga clic en [!UICONTROL **Añadir condición**] para añadir otra condición a la consulta.

   ![Consulta en el Registro de asuntos pendientes](assets/backlog-query-wrkstrm-board.png)

1. (Opcional) Haga clic en [!UICONTROL **Crear grupo**] para añadir un grupo de condiciones conectadas a la primera condición con un operador OR.
1. Haga clic en [!UICONTROL **Guardar consulta**].

   La consulta se aplica y las tarjetas que cumplen los criterios aparecen en la columna del registro de asuntos pendientes.
