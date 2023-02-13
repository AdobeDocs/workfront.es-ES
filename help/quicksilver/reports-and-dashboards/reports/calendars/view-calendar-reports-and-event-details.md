---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Ver informes de calendario y detalles de eventos
description: Puede ver los informes de calendario y los detalles de eventos que ha creado o compartido con usted en Adobe Workfront.
author: Lisa
feature: Reports and Dashboards
exl-id: db016e91-43e4-400c-ac9d-1639c7f94479
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '715'
ht-degree: 0%

---

# Ver informes de calendario y detalles de eventos

Puede ver los informes de calendario y los detalles de eventos que ha creado o compartido con usted en Adobe Workfront.

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
   <td> <p>[!UICONTROL Request] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>[!UICONTROL View] o acceso superior a [!UICONTROL Reports], [!UICONTROL Dashboards] y [!UICONTROL Calendars]</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Permisos de [!UICONTROL View] o superiores para el informe de calendario</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Ver un informe de calendario

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Calendarios]**.

   Según el nivel de acceso, es posible que vea los siguientes calendarios en la lista:

   * Su valor predeterminado [!DNL Adobe Workfront] calendario\

      Workfront crea un calendario en función de los proyectos, tareas y problemas que se le hayan asignado o que se le hayan asignado a equipos, grupos o funciones a los que se le haya asignado.
   * Calendarios que ha creado\

      Para obtener más información sobre la creación de calendarios, consulte [Información general sobre los informes del calendario](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

   * Calendarios que otros usuarios han compartido con usted\

      Para obtener más información sobre cómo compartir calendarios, consulte [[!UICONTROL Compartir un calendario] informe](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

1. (Condicional) Haga clic en el **[!UICONTROL Ver]** y, a continuación, seleccione la duración del calendario que desee ver.\
   ![Duración del calendario](assets/view-menu-calendar-report-350x189.png)\
   Puede elegir entre las siguientes vistas de informes de calendario:

   * **[!UICONTROL Mes]**: Muestra cuatro semanas del calendario
   * **[!UICONTROL Semana]**: Muestra una semana del calendario
   * **[!UICONTROL Gantt]**: Muestra una vista continua del calendario\

      ![[!UICONTROL Gantt] informe de calendario](assets/gantt-calendar-report.png)
Puede ver más eventos en un [!UICONTROL Gantt] para visualizarla, desplácese hacia abajo o hacia los lados. Un símbolo de carga aparece cuando los datos se rellenan para la vista.
   >[!NOTE]
   >
   >En el [!UICONTROL Mes] y [!UICONTROL Semana] las vistas, los eventos actuales o futuros (incluidos los eventos que abarcan varios días, siempre que contengan hoy o un día futuro) tienen sombreado que corresponde al color del proyecto o la agrupación del calendario. Los eventos anteriores tienen sombreado más claro para indicar que ya no están actualizados, pero aún puede seleccionar y ver esos eventos.

1. (Opcional) Si está viendo el calendario en la variable [!UICONTROL Mes] o [!UICONTROL Semana] vistas, puede cambiar la vista de calendario con las siguientes opciones:

   * Para incluir o excluir fines de semana:

      1. En el **[!UICONTROL Calendario]** barra de herramientas, haga clic en **[!UICONTROL Acciones de calendario]** y, en la lista desplegable, seleccione **[!UICONTROL Mostrar fin de semana]** o **[!UICONTROL Ocultar fin de semana]**.
   * Para cambiar rápidamente las fechas mostradas:

      1. En el **[!UICONTROL Calendario]** en la barra de herramientas, haga clic en la flecha izquierda del indicador de fecha para moverse hacia atrás en el calendario o en la flecha derecha para avanzar.\

         ![Haga clic en la flecha para cambiar la fecha](assets/click-arrows-to-change-dates-calendar-report.png)\
         Las fechas mostradas se ajustan mediante un intervalo basado en la vista de calendario actual. Por ejemplo, si está viendo el calendario en la variable [!UICONTROL Semana] , el calendario se muestra una semana hacia adelante o una semana hacia atrás, en función de la flecha seleccionada.

      1. (Opcional) Para volver al día actual, haga clic en **Today**.


1. (Opcional) Para ver un calendario en pantalla completa, haga clic en las flechas de pantalla completa en el lado derecho del **[!UICONTROL Calendario]** barra de herramientas.
   ![Haga clic en la flecha para cambiar la fecha](assets/click-arrows-to-change-dates-calendar-report.png)\
   Pulse Esc para volver a la vista normal del calendario.

1. (Opcional) Para ocultar los eventos de un proyecto o de una agrupación de calendario vinculada al calendario, borre la agrupación del proyecto o del calendario en la lista del proyecto.
   ![Ocultar eventos](assets/hide-events-for-project-or-cal-grouping.png)\
   Puede volver a hacer visibles los eventos seleccionando la opción [!UICONTROL proyecto] o la agrupación de calendario en la lista de proyectos.

## Ver detalles de eventos de informes de calendario

Puede ver los detalles de un evento en un calendario, tanto para los eventos actuales como los anteriores.

1. Vaya al evento para el que desee conocer los detalles y, a continuación, haga clic en el evento .\
   Se abre una página de detalles del evento.\
   ![calendar_report_EventDetails.png](assets/calendar-report-eventdetails-350x145.png)

1. (Opcional) Para ver más detalles sobre el objeto:

   1. Pase el ratón sobre el nombre del proyecto, la tarea o el problema.

      Se abre una página de detalles para el objeto.\
      ![additional_object_details_-_calendar_report.png](assets/additional-object-details---calendar-report-350x131.png)

   1. (Opcional) Para abrir el proyecto, la tarea o el problema asociados, haga clic en el título del objeto.
   1. (Opcional) Para cerrar todas las páginas de detalles abiertas, haga clic en cualquier lugar fuera de las páginas de detalles del evento.
