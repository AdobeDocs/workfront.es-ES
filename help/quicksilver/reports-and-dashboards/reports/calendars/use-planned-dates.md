---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Usar fechas planificadas en un informe de calendario
description: Un informe de calendario es un informe dinámico que proporciona una representación visual del trabajo. Puede usar los campos Fecha planificada en un informe de calendario para tareas, problemas y proyectos.
author: Lisa
feature: Reports and Dashboards
exl-id: 27bf6f03-2f6b-4556-a715-75c4a21bfbbb
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 1%

---

# Usar [!UICONTROL Fechas planificadas] en un informe de calendario

Un informe de calendario es un informe dinámico que proporciona una representación visual del trabajo. Puede usar [!UICONTROL campos Fecha planificada] en un informe de calendario para los objetos siguientes:

* Tareas
* Problemas
* Proyectos

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Acceso de [!UICONTROL Edit] a [!UICONTROL Reports], [!UICONTROL Dashboards] y [!UICONTROL Calendars]</p> <p>Nota: si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Acceso de [!UICONTROL Manage] al informe de calendario</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Configurar el grupo de elementos

Puede elegir cómo desea que se muestre el grupo de elementos en el calendario.

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront] y luego haga clic en **[!UICONTROL Calendarios]**.

1. Seleccione el calendario al que desee agregar un nuevo grupo de elementos.\
   O\
   Haga clic en **[!UICONTROL + Nuevo calendario]** y escriba el nombre del calendario.

   >[!NOTE]
   >
   >Para crear un informe de calendario, debe tener acceso de edición a los informes, paneles y calendarios de su nivel de acceso.

1. A la izquierda, haga clic en **[!UICONTROL Agregar al calendario]** y luego haga clic en **[!UICONTROL Agregar elementos avanzados]**.

1. Especifique lo siguiente:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Designar nombre para este grupo de elementos]</strong></td>
      <td>Escriba un nombre para el grupo de elementos.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Color]</strong></td>
      <td>Seleccione un color para el grupo de elementos. Todos los elementos se muestran en el color seleccionado en el informe de calendario.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Campo de fecha]</strong></td>
      <td><p>Elija <strong>[!UICONTROL Fechas planificadas]</strong>. Para obtener más información sobre las fechas planificadas, consulte </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-start-date.md" class="MCXref xref">Descripción general de la fecha planificada de inicio del proyecto</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Información general sobre la fecha planificada de inicio de la tarea</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Información general sobre la fecha planificada de finalización de la tarea</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Establecer la fecha planificada de finalización del proyecto</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>En el calendario, se debe mostrar</strong></td>
      <td><p>Elija cómo desea que se muestren las fechas:</p>
       <ul>
        <li><strong>[!UICONTROL Solo fecha de inicio]</strong>: el calendario muestra el objeto en una sola fecha.</li>
        <li><strong>[!UICONTROL End Date Only]</strong>: el calendario muestra el objeto en una sola fecha.</li>
        <li><strong>[!UICONTROL Duration] (Start to End)</strong>: El calendario muestra el objeto durante un período de días.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Cambiar a fechas reales cuando estén disponibles]</strong></td>
      <td><p>El calendario cambia automáticamente a las fechas reales cuando están disponibles. <br>Elija <strong>[!UICONTROL Yes]</strong> o <strong>[!UICONTROL No]</strong> para cambiar a las fechas reales cuando estén disponibles. Para obtener más información sobre las fechas reales, consulte</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Descripción general de la fecha real de inicio del proyecto </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Descripción general del proyecto Fecha real de finalización </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. Continúe en la siguiente sección.

## Agregar objetos al grupo de elementos

Después de configurar cómo desea que se muestren los elementos, debe agregar los objetos que desea ver en el calendario a la agrupación.

1. En el **[!UICONTROL ¿Qué desea agregar al calendario?]** sección, seleccione

   * **[!UICONTROL Tareas]**
   * **[!UICONTROL Proyectos]**
   * **[!UICONTROL Problemas]**

1. Haga clic en **[!UICONTROL Agregar tareas]**, **[!UICONTROL Agregar proyectos]** o **[!UICONTROL Agregar problemas]**, según el tipo de objeto que esté agregando al calendario.\
   ![Seleccionar objeto para el calendario](assets/field-name.png)

1. En el menú desplegable, empiece a escribir el nombre del campo y, a continuación, seleccione el origen del campo del objeto que desea mostrar en el calendario (por ejemplo, **[!UICONTROL Tareas tardías]**).
1. Establezca una instrucción de condición para la agrupación de calendario.

   ![Instrucción de condición](assets/condition-statement-calendar.png)

   Para obtener más información sobre la configuración de condiciones, consulte [Modificadores de filtro y condición](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Opcional) Especifique objetos adicionales para la agrupación de calendario repitiendo los pasos del 1 al 4.
1. En el campo **[!UICONTROL Establecer las etiquetas Tareas/Proyectos/Problemas para que sean...]**, seleccione cómo se etiquetan los objetos de esta agrupación de calendario en el calendario.

   >[!NOTE]
   >
   >Si las opciones de etiqueta predeterminadas no están disponibles para un objeto determinado, se muestra el nombre del objeto en su lugar. Por ejemplo, cuando se selecciona la etiqueta [!UICONTROL Tarea principal] y no hay ninguna tarea principal asociada al objeto, [!DNL Adobe Workfront] muestra el nombre de objeto que está viendo en el calendario.

1. Haga clic en **[!UICONTROL Guardar]**.
