---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Usar fechas planificadas en un informe de calendario
description: Un informe de calendario es un informe dinámico que proporciona una representación visual del trabajo. Puede utilizar los campos Fecha planificada en un informe de calendario para tareas, problemas y proyectos.
author: Jenny
feature: Reports and Dashboards
exl-id: 27bf6f03-2f6b-4556-a715-75c4a21bfbbb
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 90%

---

# Utilizar [!UICONTROL Fechas planificadas] en un informe de calendario

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.</span> 
-->

Un informe de calendario es un informe dinámico que proporciona una representación visual del trabajo. Puede utilizar los campos de [!UICONTROL Fechas planificadas] en un informe de calendario para los siguientes objetos:

* Tareas
* Problemas
* Proyectos

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles y Calendarios</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Administrar el acceso al informe de calendario</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar el grupo de elementos

Puede elegir cómo desea que se muestre el grupo de elementos en el calendario.

{{step1-to-calendars}}

1. Seleccione el calendario al que desee agregar un nuevo grupo de elementos.
O
Haga clic en **[!UICONTROL + Nuevo calendario]** y escriba el nombre del calendario.

   >[!NOTE]
   >
   >Para crear un informe de calendario, debe tener acceso de edición a los informes, paneles de control y calendarios de su nivel de acceso.

1. A la izquierda, haga clic en **[!UICONTROL Añadir al calendario]** y luego haga clic en **[!UICONTROL Añadir elementos avanzados]**.

1. Especifique lo siguiente:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Name this group of items]</strong></td>
      <td>Escriba un nombre para el grupo de elementos.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Color]</strong></td>
      <td>Seleccione un color para el grupo de elementos. Todos los elementos se muestran en el color seleccionado en el informe de calendario.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Date Field]</strong></td>
      <td><p>Elija <strong>[!UICONTROL Planned dates]</strong>. Para obtener más información sobre las fechas planificadas, consulte </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-start-date.md" class="MCXref xref">Información general sobre la fecha de inicio planificada del proyecto</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Información general sobre la fecha de inicio planificada de la tarea</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Información general sobre la fecha planificada de finalización de la tarea</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Establecer la fecha planificada de finalización del proyecto</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>En el calendario, se debe mostrar</strong></td>
      <td><p>Elija cómo desea que se muestren las fechas:</p>
       <ul>
        <li><strong>[!UICONTROL Start Date Only]</strong>: el calendario muestra el objeto en una sola fecha.</li>
        <li><strong>[!UICONTROL End Date Only]</strong>: el calendario muestra el objeto en una sola fecha.</li>
        <li><strong>[!UICONTROL Duration] (de inicio a fin)</strong>: el calendario muestra el objeto durante un periodo de días.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Switch to actual dates when available]</strong></td>
      <td><p>El calendario cambia automáticamente a las fechas reales cuando están disponibles. <br>Elija <strong>[!UICONTROL Yes]</strong> o <strong>[!UICONTROL No]</strong> para cambiar a las fechas reales cuando estén disponibles. Para obtener más información sobre las fechas reales, consulte</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Información general sobre la fecha real de inicio del proyecto </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Información general sobre la fecha de finalización real del proyecto </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. Continúe en la sección siguiente.

## Agregar objetos al grupo de elementos en Vista previa

Después de configurar cómo desea que se muestren los elementos, debe añadir los objetos que desea ver en el calendario a la agrupación.

1. En la sección **[!UICONTROL ¿Qué desea añadir al calendario?]**, seleccione

   * **[!UICONTROL Tareas]**
   * **[!UICONTROL Proyectos]**
   * **[!UICONTROL Problemas]**


1. Haga clic en **[!UICONTROL Añadir tareas]**, **[!UICONTROL Añadir proyectos]** o **[!UICONTROL Añadir problemas]**, según el tipo de objeto que esté añadiendo al calendario.

1. En el menú desplegable, empiece a escribir el nombre del campo y, a continuación, seleccione el origen del campo del objeto que desea mostrar en el calendario (por ejemplo, **[!UICONTROL Tareas tardías]**).
1. Establezca una instrucción de condición para la agrupación de calendario.


   ![Seleccionar objeto para el calendario](assets/calendar-field-name.png)

   Para obtener más información sobre la configuración de condiciones, consulte [Modificadores de filtro y condición](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Opcional) Especifique objetos adicionales para la agrupación de calendario repitiendo los pasos del 1 al 4.

1. En el campo **[!UICONTROL Establecer las etiquetas Tareas/Proyectos/Problemas para que sean...]**, seleccione cómo se etiquetan los objetos de esta agrupación de calendario en el calendario.

   >[!NOTE]
   >
   >Si las opciones de etiqueta predeterminadas no están disponibles para un objeto determinado, se muestra el nombre del objeto en su lugar. Por ejemplo, cuando se selecciona la etiqueta [!UICONTROL Tarea principal] y no hay ninguna tarea principal asociada al objeto, [!DNL Adobe Workfront] muestra el nombre de objeto que está viendo en el calendario.

   ![establecer etiquetas de tarea](assets/set-task-labels.png)
1. Haga clic en **[!UICONTROL Guardar]**.

1. Haga clic en **[!UICONTROL Guardar]**.

