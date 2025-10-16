---
navigation-topic: use-the-gantt-chart
title: Exportar el gráfico Gantt a PDF
description: Puede exportar el diagrama de Gantt a una PDF. Después, puede imprimirlo o adjuntarlo a un correo electrónico para compartirlo con otros usuarios.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '979'
ht-degree: 40%

---

# Exportar el [!UICONTROL gráfico Gantt] a PDF

<!--Audited: 08/2025-->

Puede exportar el [!UICONTROL gráfico Gantt] a una PDF. Después, puede imprimirlo o adjuntarlo a un correo electrónico para compartirlo con otros usuarios.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de [!UICONTROL Adobe Workfront]</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront]</td> 
   <td> <p>[!UICONTROL Light] o superior</p>
   <p>[!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>[!UICONTROL View] o acceso superior a Proyectos y tareas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>[!UICONTROL View] o acceso superior al proyecto y las tareas</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] license</td> 
   <td> <p>New:[!UICONTROL Light] or higher</p>
   <p>Current:[!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL View] or higher access to Projects and Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL View] or higher access to the project</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

## Exportar el [!UICONTROL gráfico Gantt]

1. Obtenga acceso al [!UICONTROL gráfico Gantt] que desea exportar a PDF, tal como se describe en [Introducción al [!UICONTROL gráfico Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. Configure el [!UICONTROL gráfico Gantt] para que muestre la información adecuada que desea exportar.

   >[!NOTE]
   >
   >Si exporta el [!UICONTROL gráfico Gantt] desde una lista de proyectos, el archivo de PDF contendrá sólo los proyectos de la lista, no las tareas de cada proyecto. Si desea exportar una lista de tareas, puede hacerlo desde el proyecto con el que están asociadas o creando un informe de tareas y mostrando los resultados del informe en la [!UICONTROL vista Gantt].

   Configure cualquiera de la siguiente información:

   * Haga clic en los iconos **Filtros**, **Ver** y **Agrupación** situados encima del [!UICONTROL gráfico Gantt] y agregue o edite el filtro, la vista o la agrupación existente aplicados a la lista de elementos del [!UICONTROL gráfico Gantt].

     Los filtros y agrupaciones seleccionados en la vista de lista se mantienen al ver el [!UICONTROL gráfico Gantt]. Las vistas se reflejan en el [!UICONTROL gráfico Gantt] exportado solamente en la lista que se muestra al lado del [!UICONTROL gráfico Gantt] en la primera página. Las vistas no se muestran en el propio [!UICONTROL gráfico Gantt].

     >[!TIP]
     >
     >Para dejar más espacio para el [!UICONTROL gráfico Gantt], aplique una vista que contenga el menor número posible de columnas.

   * Seleccione la opción **Cambiar a fechas proyectadas** para ver las fechas proyectadas en lugar de las planificadas. De forma predeterminada, se muestran las Fechas planificadas.

   * Haga clic en el icono **Configuración** ![Icono de configuración](assets/settings-icon.png) en la esquina superior derecha del gráfico Gantt y seleccione la información que desee ver. Una vez seleccionada, esta información se incluye en el archivo Gantt PDF exportado.

     Seleccione entre las siguientes opciones:

      * Fechas reales
      * Asignaciones
      * Línea base
      * Fecha de confirmación
      * % Finalizado
      * Ruta crítica
      * Diamantes de hito
      * Líneas de hito
      * Predecesoras
      * Estado de progreso
      * Fechas planificadas (condicionales)
      * Fechas proyectadas (condicionales)

     Para obtener más información, consulte [Configure cómo se muestra la información en el [!UICONTROL gráfico Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

     >[!NOTE]
     >
     > Las asignaciones no se muestran en el [!UICONTROL gráfico Gantt] cuando el [!UICONTROL gráfico Gantt] se exporta a PDF. Una vez exportadas, las asignaciones solo se muestran en la vista de lista.

   * Período de tiempo que se muestra en el [!UICONTROL gráfico Gantt]. La forma en que se muestra en el archivo de exportación depende de si selecciona **[!UICONTROL Lo que veo]** o **[!UICONTROL Varias páginas]** en un paso posterior.

     Para obtener más información, vea [Ver información en el [!UICONTROL gráfico Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).



1. (Opcional) Para incluir solo determinadas tareas en el PDF exportado, seleccione las tareas que desee incluir. Si no selecciona ninguna tarea, todas las tareas se incluyen en el PDF exportado.

   Por ejemplo, si está viendo el [!UICONTROL gráfico Gantt] de un proyecto que contiene 50 tareas, pero desea mostrar solamente 10 tareas en el [!UICONTROL gráfico Gantt] exportado, seleccione las 10 tareas que desee mostrar.

1. Haga clic en el icono de impresora ![Icono de impresora](assets/printer-icon.png) en la esquina superior derecha del gráfico Gantt.
Se muestra el cuadro de diálogo **[!UICONTROL Exportar a PDF]**.

   ![Cuadro de diálogo Exportar a PDF](assets/exported-gantt-ui-350x225.png)

1. En la sección **Exportar**, seleccione entre las siguientes opciones para indicar si desea exportar sólo lo que ve o todo el [!UICONTROL gráfico Gantt]:

   * **[!UICONTROL Lo que veo]:** Exporta todas las tareas (incluidas las subtareas) que se muestran en la pantalla antes de exportar un máximo de 500 elementos. (Esto no es lo que se muestra en la sección **[!UICONTROL Preview]**; la sección **Preview** solo contiene datos de ejemplo).

     Las subtareas se incluyen en el PDF exportado incluso si la tarea principal está contraída y las subtareas no son visibles. Para incluir sólo las tareas principales, seleccione las tareas principales que desee incluir y deje las subtareas sin seleccionar.

     >[!TIP]
     >
     >Puede usar la herramienta de zoom o del control deslizante para mostrar sólo una parte del [!UICONTROL gráfico Gantt], tal como se describe en [Visualización de información en el [!UICONTROL gráfico Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md). Seleccione una opción más granular para mostrar más páginas para exportar o seleccione una opción menos granular para mostrar menos páginas para exportar.


   * **[!UICONTROL Varias páginas]:** Exporta todo el [!UICONTROL gráfico Gantt] (hasta 500 elementos), incluidos los elementos que no están visibles en la pantalla actual.

     >[!NOTE]
     >
     >* Si necesita exportar un [!UICONTROL gráfico Gantt] que contiene más de 500 elementos, aplique un filtro a la lista antes de ver el [!UICONTROL gráfico Gantt] para que se muestren menos de 500 elementos o 250 páginas. Para obtener información sobre cómo aplicar un filtro, consulte [Descripción general de filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >* No se puede exportar todo el gráfico Gantt en las siguientes circunstancias:
     >   
     >   * Cuando abarca más de 250 páginas.
     >   * Cuando contiene más de 500 elementos.


1. Si el PDF se imprimirá después de exportarlo a PDF, seleccione el tamaño de papel en el que desea imprimir en el menú desplegable **[!UICONTROL Tamaño de página]**.
Puede seleccionar entre las siguientes opciones:

   * **[!UICONTROL Carta]**
   * **[!UICONTROL Legal]**
   * **[!UICONTROL Libro Mayor]**
   * **[!UICONTROL A1]**
   * **[!UICONTROL A2]**
   * **[!UICONTROL A3]** (disponible solo para algunos idiomas)
   * **[!UICONTROL A4]**
1. En la sección **[!UICONTROL Orientación de página]** seleccione si desea que el PDF se exporte en orientación horizontal o vertical.
1. Seleccione **[!UICONTROL Mostrar leyenda]** si desea incluir la leyenda en el PDF exportado.
1. Haga clic en **[!UICONTROL Exportar]**. El PDF se crea y se descarga en el equipo.

   La leyenda de la parte inferior del archivo exportado explica únicamente las opciones que ha habilitado en el [!UICONTROL gráfico Gantt] y que están disponibles en la lista de tareas. Por ejemplo, los hitos se muestran en la leyenda solo si tiene al menos una tarea asociada a un hito.

   ![gantt_chart_with_updated__limited__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
