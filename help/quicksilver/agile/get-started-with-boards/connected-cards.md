---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Usar tarjetas conectadas en tableros
description: Puede agregar una tarjeta en el tablero que esté conectada a tareas y problemas existentes en Workfront.
author: Lisa
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: f6bee61bbfbac98595d737fa002bbe01c0c573dc
workflow-type: tm+mt
source-wordcount: '1242'
ht-degree: 0%

---

# Usar tarjetas conectadas en tableros

Puede agregar una tarjeta del tablero que esté conectada a tareas y problemas existentes en [!DNL Workfront].

Cuando se actualiza cualquiera de los siguientes detalles para la tarjeta en una ubicación, se actualiza automáticamente en la otra ubicación:

* [!UICONTROL Nombre]
* [!UICONTROL Descripción]
* [!UICONTROL Personas asignadas]
* [!UICONTROL Estado]
* [!UICONTROL Fecha de finalización planificada]
* [!UICONTROL Estimación] / [!UICONTROL Puntos de artículo]

>[!NOTE]
>Una única tarea o problema conectado solo se puede añadir una vez por tablero. La misma tarea o problema se puede conectar a varios tableros.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>[!UICONTROL Request] o superior</p> </td> 
  </tr> 
  <tr>
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td>
   <td><p>[!UICONTROL View] o acceso superior a tareas y problemas</p></td>
  </tr>
  <tr>
   <td role="rowheader"><strong>Permisos de objeto</strong></td>
   <td><p>Permisos de [!UICONTROL View] o permisos superiores para la tarea o el problema de Workfront</p></td>
  </tr>
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Agregar una tarjeta conectada

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **[!UICONTROL Tableros]**.
1. Acceda a un tablero. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Haga clic en **[!UICONTROL Agregar tarjeta] > [!UICONTROL Tarjeta conectada]**.
1. Elija un proyecto y, a continuación, elija una tarea o un problema para agregar como tarjeta en el tablero.

   Puede seleccionar varios objetos y todos se añadirán como tarjetas independientes.

   >[!NOTE]
   >
   >* En los resultados de búsqueda solo están disponibles los objetos para los que tiene permisos. Si un elemento está tenue, ya se ha agregado al tablero.
   >* Al filtrar por **[!UICONTROL Proyectos de los que soy propietario]** o **[!UICONTROL Proyectos en los que estoy]**, no se incluyen los proyectos que equivalen a un estado de Finalización, Muerta o Rechazado. Puede seguir buscando esos proyectos con la variable **[!UICONTROL Todo]** filtro.


1. Haga clic en **[!UICONTROL Agregar]**.

   ![Buscar tarea o problema para conectar](assets/boards-tasksissues-350x94.png)

   La tarjeta se agrega en la parte inferior de la columna situada más a la izquierda. El [!DNL Workfront] y sus destinatarios se muestran en la tarjeta .

   >[!NOTE]
   >
   >Si un usuario asignado en la variable [!DNL Workfront] tarea o problema no es un miembro del tablero, no se asignan a la tarjeta.

   ![Tarjeta conectada](assets/boards-connected-card-first-added.png)

1. Haga clic en ![Abrir tarea o problema](assets/boards-launch-icon.png) para abrir el [!DNL Workfront] tarea o problema en una nueva pestaña del navegador.
1. Para editar los detalles de la tarjeta, haga clic en la tarjeta (no en el nombre de la tarjeta).

   O

   Haga clic en el **[!UICONTROL Más]** menú ![Más menú](assets/more-icon-spectrum.png) en la tarjeta y seleccione **[!UICONTROL Editar]**.

1. En el **[!UICONTROL Detalles de la tarjeta]** , añada o actualice la siguiente información:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Name]</strong></td> 
      <td>Al cambiar el nombre también se cambia el nombre en el [!DNL Workfront] objeto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Descripción]</strong></td> 
      <td>Al cambiar la descripción también se cambia la descripción en el [!DNL Workfront] objeto. Puede añadir direcciones URL en la descripción, que se convertirán en vínculos en los que se puede hacer clic cuando se guarde la tarjeta.</td> 
     </tr> 
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Asignados]</strong></td>
      <td><p>Para asignar más personas o un equipo a la tarjeta, empiece a escribir un nombre en el campo de búsqueda y selecciónelo cuando aparezca en la lista. Puede agregar personas y equipos. Sólo se permite una asignación de equipo en una tarjeta conectada.</p>
      <p>Los miembros asignados deben ser miembros del consejo o no aparecerán en la lista de selección. Cuando un equipo es miembro del tablero, los integrantes individuales del equipo se pueden asignar a la tarjeta.</p>
      <p>Los usuarios asignados que seleccione también se asignarán a la tarea o problema de [!DNL Workfront].</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Columna]</strong></td>
      <td>Seleccione la columna de la tarjeta.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Status]</strong></td>
      <td><p>Seleccione un estado para la tarjeta. Los valores predeterminados son [!UICONTROL New], [!UICONTROL In Progress] y [!UICONTROL Complete], pero cualquier estado personalizado definido para el elemento en [!DNL Workfront] también están disponibles.</p>
      <p>Si tiene directivas de columna habilitadas para actualizar valores de campo, al cambiar el estado en la tarjeta se mueve automáticamente la tarjeta a la columna correspondiente. Para obtener más información, consulte "Definición de configuración de columna y políticas" en el artículo <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">Administrar columnas de tablero</a>.</p>
      <p>Si hace clic en <strong>[!UICONTROL Marca completada]</strong> en la parte superior de la tarjeta, el estado cambia automáticamente a Completado.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Finalización planificada]</strong></td>
      <td>Al cambiar esta fecha también se cambia la fecha de finalización planificada en la [!DNL Workfront] objeto.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimación]</strong></td>
      <td><p>Número de horas durante las cuales se completará la tarjeta.</p><p>Al cambiar la estimación también se cambia el valor de los puntos de artículo en la [!DNL Workfront] objeto.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Etiquetas]</strong></td>
      <td><p>Busque y seleccione etiquetas para la tarjeta.</p>
      <p>Para obtener información sobre la creación de nuevas etiquetas, consulte <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">Agregar etiquetas</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Elementos de lista de comprobación]</strong> </td> 
      <td> <p>Haga clic en <strong>[!UICONTROL Agregar elemento de lista de comprobación]</strong>. A continuación, escriba el título del artículo y pulse Intro. Se agrega automáticamente otro elemento. Continúe introduciendo títulos para agregar más elementos.</p> <p>El contador de la parte superior de la lista de comprobación muestra el número de elementos completados y el número total de elementos.</p> <p>Para obtener más información sobre los elementos de la lista de comprobación, consulte <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">Administrar los elementos de la lista de comprobación en las tarjetas</a>.</p></td>
     </tr>
    </tbody> 
   </table>

   Utilice el panel de navegación de la izquierda para desplazarse entre grupos de campos en los detalles de la tarjeta.

   >[!NOTE]
   >
   >El panel de navegación izquierdo y la capacidad de agregar vínculos en los que se puede hacer clic en el campo Descripción solo están disponibles a través de la opción de inclusión de funciones anteriores para los tableros de Workfront.

1. Haga clic en **[!UICONTROL Cerrar]** para volver al tablero.
El objeto conectado, los usuarios asignados, las etiquetas, la fecha de vencimiento, el contador de la lista de comprobación, las horas estimadas y el estado se muestran en la tarjeta.

   ![Tarjeta agregada al tablero](assets/boards-connected-card-details-110922.png)

## Desconectar una tarjeta conectada

Puede desconectar una tarjeta conectada de su objeto Workfront y la tarjeta permanece en el tablero como una tarjeta ad hoc que puede editar.

Para desconectarse a nivel de tablero:

1. Acceda al tablero.
1. Haga clic en el **[!UICONTROL Más]** menú ![Más menú](assets/more-icon-spectrum.png) en la tarjeta conectada y seleccione **[!UICONTROL Desconectar]**.
1. Haga clic en **[!UICONTROL Desconectar]** en el mensaje de confirmación.

Para desconectarse a nivel de tarjeta:

1. Acceda al tablero y abra la tarjeta conectada.
1. Haga clic en el **[!UICONTROL Más]** menú ![Más menú](assets/more-icon-spectrum.png) en el área Conexión de los detalles de la tarjeta y seleccione **[!UICONTROL Desconectar]**.
1. Haga clic en **[!UICONTROL Desconectar]** en el mensaje de confirmación.

## Convertir una tarjeta ad hoc en una tarjeta conectada

Después de crear una tarjeta ad hoc, puede convertirla en una tarjeta conectada. Para obtener más información sobre las tarjetas ad hoc, consulte [Agregar una tarjeta ad hoc a un tablero](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

1. Acceda al tablero y abra la tarjeta ad hoc.
1. Compruebe el nombre y la descripción de la tarjeta. Se añaden a la tarea o al problema que cree en [!DNL Workfront].
1. En el [!UICONTROL Conexión] del área de los detalles de la tarjeta, haga clic en **[!UICONTROL Conectar con Workfront]**.
1. En el [!UICONTROL Tarjeta de conexión] , seleccione si está creando una tarea o un problema.
1. Busque y seleccione un proyecto al que añadir la tarea o el problema.

   >[!NOTE]
   >
   >* En los resultados de búsqueda solo están disponibles los objetos para los que tiene permisos.
   >* Al filtrar por **[!UICONTROL Proyectos de los que soy propietario]** o **[!UICONTROL Proyectos en los que estoy]**, proyectos que equivalen a [!UICONTROL Completar], [!UICONTROL Muerto]o [!UICONTROL Rechazado] no se incluyen. Puede seguir buscando esos proyectos con la variable **[!UICONTROL Todo]** filtro.


1. Haga clic en **[!UICONTROL Connect]**.

   ![Conectar tarjeta ad hoc a Workfront](assets/boards-connect-ad-hoc-card.png)

   El nombre del proyecto se muestra en el área Conexión de los detalles de la tarjeta.

1. Haga clic en **[!UICONTROL Cerrar]** para volver al tablero.

## Horas de registro en una tarjeta conectada

Debe tener los permisos correctos para registrar las horas en la tarea o problema conectado.

Los campos de registro de tiempo no se muestran en las tarjetas conectadas de forma predeterminada. Debe habilitar [!UICONTROL **Horas**] en el [!UICONTROL Configurar] área bajo [!UICONTROL Tarjetas]. Para obtener más información, consulte [Personalización de los campos que se muestran en una tarjeta](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Introduzca el número de horas para la tarea o el problema.
1. Seleccione un [!UICONTROL Tipo de hora] en el menú desplegable, si es diferente al predeterminado.
1. Haga clic en [!UICONTROL **Tiempo de registro**].

   ![Registrar horas en la tarjeta](assets/log-hours-on-card.png)

   El tiempo registrado en la tarjeta también se guarda en la tarea o problema conectado.

La hora de inicio de sesión en la tarjeta es la misma que la hora de inicio de sesión en una tarea o problema. Para obtener más información, consulte &quot;Tiempo de inicio de sesión en un proyecto, tarea o problema&quot; en el artículo [Tiempo de registro](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

