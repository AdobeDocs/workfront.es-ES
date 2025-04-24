---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Usar fechas proyectadas en un informe de calendario
description: Un informe de calendario es un informe dinámico que proporciona una representación visual del trabajo. Puede utilizar los campos Fecha proyectada en un informe de calendario para tareas, problemas y proyectos.
author: Lisa
feature: Reports and Dashboards
exl-id: 39e16f0b-c10d-429e-9eb5-d4847c7e4ed9
source-git-commit: 5c0278607faf65b58abeb9b813e403f97032a965
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 91%

---

# Usar [!UICONTROL Fechas proyectadas] en un informe de calendario

Un informe de calendario es un informe dinámico que proporciona una representación visual del trabajo. Se puede mostrar información de la fecha en un informe de calendario para los objetos siguientes:

* Tareas
* Problemas
* Proyectos

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
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td><p>Nuevo: estándar</p>
       <p>o</p>
       <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso [!UICONTROL Edit] a [!UICONTROL Reports], [!UICONTROL Dashboards] y [!UICONTROL Calendars]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Acceso [!UICONTROL Manage] al informe de calendario</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar el grupo de elementos

Puede elegir cómo desea que se muestre el grupo de elementos en el calendario.

{{step1-to-calendars}}

1. Seleccione el calendario al que desee agregar un nuevo grupo de elementos, haga clic en el menú Más y, a continuación, **Editar**.
O
Haga clic en **[!UICONTROL + Nuevo calendario]**, escriba el nombre del proyecto y haga clic en **[!UICONTROL Agregar elementos avanzados]**.

   >[!NOTE]
   >
   >Debe tener el acceso [!UICONTROL Editar] en [!UICONTROL Informes], [!UICONTROL Paneles] y [!UICONTROL Calendarios] en su nivel de acceso para crear un informe de calendario.

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
      <td><p>Elija <strong>[!UICONTROL Projected dates]</strong>. Para obtener más información sobre las fechas proyectadas, consulte </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-projected-start-date.md" class="MCXref xref">Información general sobre la fecha de inicio proyectada del proyecto</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Información general sobre la fecha proyectada de finalización de proyectos, tareas y problemas</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL On the calendar, show]</strong></td>
      <td><p>Elija cómo desea que se muestren las fechas:</p>
       <ul>
        <li><strong>[!UICONTROL Start Date Only]</strong>: el calendario muestra el objeto en una sola fecha.</li>
        <li><strong>[!UICONTROL End Date Only]</strong>: el calendario muestra el objeto en una sola fecha.</li>
        <li><strong>[!UICONTROL Duration] (Start to End)</strong>: el calendario muestra el objeto durante un período de días.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Switch to Actual Dates when available]</strong></td>
      <td><p>El calendario cambia automáticamente a las fechas reales cuando están disponibles. <br>Elija <strong>[!UICONTROL Yes]</strong> o <strong>[!UICONTROL No]</strong> para cambiar a las fechas reales cuando estén disponibles. Para obtener más información sobre las fechas reales, consulte</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Información general sobre la fecha real de inicio del proyecto </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Información general sobre la fecha de finalización real del proyecto </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. Continúe en la sección siguiente.

## Añadir objetos al grupo de elementos

Después de configurar cómo desea que se muestren los elementos, debe añadir los objetos que desea ver en el calendario a la agrupación.

1. En la sección **[!UICONTROL ¿Qué desea añadir al calendario?]**, seleccione

   * **[!UICONTROL Tareas]**
   * **[!UICONTROL Proyectos]**
   * **[!UICONTROL Problemas]**
   * **[!UICONTROL Días libres]**
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

