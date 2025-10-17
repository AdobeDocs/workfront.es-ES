---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Uso de tarjetas conectadas en tableros
description: Puede añadir una tarjeta en el tablero que esté conectada a tareas y problemas existentes en Workfront.
author: Jenny
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1430'
ht-degree: 96%

---

# Usar tarjetas conectadas en los tableros

<!-- Audited: 2/2024 -->

Puede añadir una tarjeta en el tablero que esté conectada a tareas y problemas existentes en [!DNL Workfront].

Cuando se actualiza cualquiera de los siguientes detalles de la tarjeta en una ubicación, se actualiza automáticamente en la otra ubicación:

* [!UICONTROL Nombre]
* [!UICONTROL Descripción]
* [!UICONTROL Personas asignadas]
* [!UICONTROL Estado]
* [!UICONTROL Fecha planificada de finalización]
* [!UICONTROL Estimación] / [!UICONTROL Puntos de caso]
* [!UICONTROL Subtareas]
* [!UICONTROL Documentos]

Para sincronizar tarjetas conectadas con Workfront, haz clic en el menú **[!UICONTROL Más]** ![[!UICONTROL Menú Más]](assets/more-icon-spectrum.png) que está junto al nombre del tablero y selecciona **[!UICONTROL Sincronizar elementos conectados]**. Las tarjetas archivadas no se sincronizan con las tareas y problemas de Workfront. Si restaura una tarjeta, se volverá a sincronizar.

>[!NOTE]
>
>Una sola tarea o problema conectado solo se puede añadir una vez por tablero. La misma tarea o problema se puede conectar a varios tableros.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
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
  <tr>
   <td role="rowheader">Configuraciones de nivel de acceso</td>
   <td><p>Acceso de visualización o superior a tareas y problemas</p></td>
  </tr>
  <tr>
   <td role="rowheader">Permisos de objeto</td>
   <td><p>Permisos de visualización o superiores para la tarea o problema de Workfront</p>
</td>
  </tr>
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Añadir una tarjeta conectada

{{step1-to-boards}}

1. Acceda a un tablero. Para obtener más información, consulte [Crear o editar un tablero](../../agile/get-started-with-boards/create-edit-board.md).
1. Haga clic en **[!UICONTROL Añadir tarjeta] > [!UICONTROL Tarjeta conectada]**.
1. Elija un proyecto y, a continuación, elija una tarea o un problema para añadirlos como tarjeta en el tablero.

   Puede seleccionar varios objetos y todos se añadirán como tarjetas independientes.

   >[!NOTE]
   >
   >* En los resultados de la búsqueda solo están disponibles los objetos para los que tiene permisos. Si un elemento aparece atenuado, es que ya se ha añadido al tablero.
   >* Cuando se filtra por **[!UICONTROL Proyectos de mi propiedad]** o **[!UICONTROL Proyectos en los que participo]**, no se incluyen los proyectos que equivalen a un estado Completado, Inactivo o Rechazado. Puede seguir buscando esos proyectos con el filtro **[!UICONTROL Todos]**.

1. Haga clic en **[!UICONTROL Añadir]**.

   ![Buscar una tarea o problema para conectarlo](assets/boards-tasksissues-350x94.png)

   La tarjeta se añade en la parte inferior de la columna situada más a la izquierda. El objeto de [!DNL Workfront] conectado y sus usuarios asignados se muestran en la tarjeta.

   ![Tarjeta conectada](assets/boards-connected-card-first-added.png)

1. Haga clic en ![Abrir tarea o problema](assets/boards-launch-icon.png) para abrir la tarea o el problema de [!DNL Workfront] en una nueva ficha del explorador.
1. Para editar los detalles de la tarjeta, haga clic en la tarjeta (no en el nombre de la tarjeta).

   O

   Haga clic en el menú **[!UICONTROL Más]** ![menú Más ](assets/more-icon-spectrum.png) de la tarjeta y seleccione **[!UICONTROL Editar]**.

1. En el cuadro **[!UICONTROL Detalles de la tarjeta]**, añada o actualice la siguiente información:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Name]</strong></td> 
      <td>Al cambiar el nombre también se cambia el nombre del objeto [!DNL Workfront] conectado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td> 
      <td>Al cambiar la descripción también se cambia la descripción del objeto de [!DNL Workfront] conectado. Puede añadir direcciones URL en la descripción, que se convertirán en vínculos en los que se puede hacer clic cuando se guarde la tarjeta.</td> 
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Column]</strong></td>
      <td>Seleccione la columna de la tarjeta.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Status]</strong></td>
      <td><p>Seleccione un estado para la tarjeta. Los valores predeterminados son [!UICONTROL New], [!UICONTROL In Progress] y [!UICONTROL Complete], pero también están disponibles todos los estados personalizados definidos para el elemento de [!DNL Workfront].</p>
      <p>Si tiene habilitadas las directivas de columna para actualizar valores de campo, al cambiar el estado de la tarjeta, esta se desplaza automáticamente a la columna correspondiente. Para obtener más información, consulte “Definición de la configuración y las directivas de columna” en el artículo <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">Administrar columnas de tablero</a>.</p>
      <p>Si hace clic en <strong>[!UICONTROL Mark Complete]</strong> en la parte superior de la tarjeta, el estado cambiará automáticamente a Completado.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Planned Completion]</strong></td>
      <td>Al cambiar esta fecha, también se cambia la fecha planificada de finalización del objeto de [!DNL Workfront] conectado.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimation]</strong></td>
      <td><p>Número de horas que se completará la tarjeta.</p><p>Al cambiar la estimación también se cambia el valor de los puntos de la historia en el objeto de [!DNL Workfront] conectado.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Assignments]</strong></td>
      <td><p>Para asignar más personas o un equipo a la tarjeta, haga clic en <strong>[!UICONTROL Add Assignment]</strong> y empiece a escribir un nombre en el campo de búsqueda. A continuación, selecciónelo cuando se muestre en la lista de resultados. Puede añadir individuos y equipos. Solo se permite una asignación de equipo en una tarjeta conectada.</p>
      <p>Las personas asignadas que seleccione también se asignarán a la tarea o al problema de [!DNL Workfront].</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tags]</strong></td>
      <td><p>Busque y seleccione etiquetas para la tarjeta.</p>
      <p>Para obtener información sobre cómo crear nuevas etiquetas, consulte <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">Añadir etiquetas</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom fields]</strong></td>
      <td><p>Cualquier campo personalizado que añada se mostrará en esta área.</p>
      <p>Para obtener más información, consulte <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">Personalizar qué campos se muestran en una tarjeta</a>.</p></td>
     </tr>
     <tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Subtask]</strong></td>
      <td><p>Cualquier subtarea existente para la tarea aparecerá en esta sección. Haga clic en <strong>[!UICONTROL Add Subtask]</strong> para añadir una nueva subtarea.</p>
      <p>El contador de la parte superior de la sección muestra el número de subtareas completadas y el número total de subtareas.</p>
      <p>Para obtener más información acerca de las subtareas, consulte <a href="/help/quicksilver/agile/get-started-with-boards/manage-subtasks-on-boards.md">Administración de subtareas en tableros</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Checklist]</strong></td>
      <td><p>Haga clic en <strong>[!UICONTROL Add checklist item]</strong>. A continuación, escriba el título del elemento y pulse Intro. Se añade otro elemento automáticamente. Siga introduciendo títulos para añadir más elementos.</p>
      <p>El contador de la parte superior de la lista de comprobación muestra el número de elementos completados y el número total de elementos.</p> <p>Para obtener más información acerca de los elementos de la lista de comprobación, consulte <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">Administrar elementos de listas de comprobación en tarjetas</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Documents]</strong></td>
      <td>Para un documento existente, pase el puntero por encima de la miniatura del documento y haga clic en <strong>Vista previa</strong> para ver el archivo en el explorador o en <strong>Descargar</strong> para descargar el archivo en el equipo. Para ver un documento nuevo, consulte <a href="/help/quicksilver/agile/get-started-with-boards/add-documents-on-cards.md">Añadir documentos en tarjetas</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Hours]</strong></td>
      <td>Consulte “Registrar horas en una tarjeta conectada”, a continuación.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Comments]</strong></td>
      <td><p>Haga clic en el campo <strong>[!UICONTROL New comment]</strong> y escriba el comentario. Utilice las herramientas de formato para dar formato al texto. Para etiquetar a una persona o equipo, utilice el cuadro de búsqueda situado en la parte inferior del área de comentarios. El usuario no tiene que ser miembro del tablero. Los usuarios etiquetados en tarjetas conectadas recibirán notificaciones por correo electrónico.</p><p>Haga clic en <strong>[!UICONTROL Submit]</strong> para añadir el comentario a la tarjeta.</p>
      <p>Para obtener más información sobre los comentarios, consulte <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md">Actualizar trabajo</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL System activity]</strong></td> 
      <td><p>Si tiene <strong>Actividad del sistema</strong> habilitada como sección de tarjeta, la actividad se muestra en esta área.</p> <p>Para obtener más información, consulte <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">Personalizar los campos que se muestran en una tarjeta</a> y <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md">Actualizaciones con seguimiento del sistema</a>.</p></td>
     </tr>     
    </tbody> 
   </table>

   Utilice el panel de navegación izquierdo para desplazarse entre las secciones de los campos de los datos de la tarjeta.

1. Haga clic en **[!UICONTROL Cerrar]** para regresar al tablero.
El objeto conectado, los usuarios asignados, las etiquetas, la fecha de vencimiento, el contador de la lista de comprobación, las horas estimadas y el estado se muestran en la tarjeta.

   ![Tarjeta añadida al tablero](assets/boards-connected-card-details-110922.png)

## Desconectar una tarjeta conectada

Puede desconectar una tarjeta conectada de su objeto de Workfront y la tarjeta permanecerá en el tablero como una tarjeta ad hoc que puede editar.

Para desconectar a nivel del tablero, haga lo siguiente:

1. Acceda al tablero.
1. Haga clic en el menú **[!UICONTROL Más]** ![menú Más](assets/more-icon-spectrum.png) de la tarjeta conectada y seleccione **[!UICONTROL Desconectar]**.
1. Haga clic en **[!UICONTROL Desconectar]** en el mensaje de confirmación.

Para desconectar a nivel de la tarjeta:

1. Acceda al tablero y abra la tarjeta conectada.
1. Haga clic en el menú **[!UICONTROL Más]** ![menú Más](assets/more-icon-spectrum.png) del área Conexión de los detalles de la tarjeta y seleccione **[!UICONTROL Desconectar]**.
1. Haga clic en **[!UICONTROL Desconectar]** en el mensaje de confirmación.

## Convertir una tarjeta ad hoc en una tarjeta conectada

Después de crear una tarjeta ad hoc, puede convertirla en una tarjeta conectada. Para obtener más información acerca de las tarjetas ad hoc, consulte [Añadir una tarjeta ad hoc a un tablero](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

1. Acceda al tablero y abra la tarjeta ad hoc.
1. Compruebe el nombre y la descripción en la tarjeta. Se añadirán a la tarea o al problema que cree en [!DNL Workfront].
1. En el área [!UICONTROL Conexión] de los detalles de la tarjeta, haga clic en **[!UICONTROL Conectar con Workfront]**.
1. En la ventana [!UICONTROL Conectar tarjeta], seleccione si está creando una tarea o un problema.
1. Busque y seleccione un proyecto al que añadir la tarea o el problema.

   >[!NOTE]
   >
   >* En los resultados de la búsqueda solo están disponibles los objetos para los que tiene permisos.
   >* Cuando se filtra por **[!UICONTROL Proyectos de mi propiedad]** o **[!UICONTROL Proyectos en los que participo]**, no se incluyen los proyectos que equivalen a un estado [!UICONTROL Completado], [!UICONTROL Inactivo] o [!UICONTROL Rechazado]. Puede seguir buscando esos proyectos con el filtro **[!UICONTROL Todos]**.

1. Haga clic en **[!UICONTROL Conectar]**.

   ![Conectar la tarjeta ad hoc a Workfront](assets/boards-connect-ad-hoc-card.png)

   El nombre del proyecto se muestra en el área Conexión en los detalles de la tarjeta.

1. Haga clic en **[!UICONTROL Cerrar]** para regresar al tablero.

## Registrar horas en una tarjeta conectada

Debe tener los permisos correctos para registrar horas en la tarea o el problema conectado.

Los campos de registro de hora no se muestran en las tarjetas conectadas de forma predeterminada. Debe habilitar [!UICONTROL **Horas**] en el área de [!UICONTROL Configurar] en [!UICONTROL Tarjetas]. Para obtener más información, consulte [Personalizar los campos que se muestran en una tarjeta](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Introduzca el número de horas para la tarea o problema.
1. Seleccione un [!UICONTROL Tipo de hora] en el menú desplegable, si es diferente al predeterminado.
1. Haga clic en [!UICONTROL **Registrar hora**].

   ![Registrar las horas en la tarjeta](assets/log-hours-on-card.png)

   La hora registrada en la tarjeta también se guarda en la tarea o problema conectado.

Registrar la hora en la tarjeta es lo mismo que registrar la hora en una tarea o problema. Para obtener más información, consulte &quot;Registrar la hora en un proyecto, tarea o problema&quot; en el artículo [Registrar hora](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

