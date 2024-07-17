---
navigation-topic: use-the-gantt-chart
title: Exportar el gráfico Gantt a PDF
description: Puede exportar el diagrama de Gantt a un PDF.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 0%

---

# Exportar el [!UICONTROL gráfico Gantt] al PDF

Puede exportar el [!UICONTROL diagrama de Gantt] a un PDF.

Después de exportar el [!UICONTROL diagrama de Gantt] a PDF, puede imprimirlo o adjuntarlo a un mensaje de correo electrónico para compartirlo con otros usuarios.

## Requisitos de acceso

Debe tener lo siguiente para seguir los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>[!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>[!UICONTROL View] o acceso superior a Proyectos y tareas</p> <p>Nota: si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>[!UICONTROL View] o acceso superior al proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Exportar [!UICONTROL gráfico Gantt]

1. Obtenga acceso al [!UICONTROL gráfico Gantt] que desea exportar al PDF, tal como se describe en [Introducción al [!UICONTROL gráfico Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. Asegúrese de haber configurado el [!UICONTROL gráfico Gantt] para que muestre la información adecuada antes de exportarlo.

   >[!NOTE]
   >
   >Si exporta el [!UICONTROL diagrama de Gantt] desde una lista de proyectos, el archivo de PDF contendrá sólo los proyectos de la lista, no las tareas de cada proyecto. Si desea exportar una lista de tareas, puede hacerlo desde el proyecto con el que están asociadas o creando un informe de tareas y mostrando los resultados del informe en la [!UICONTROL vista Gantt].

   Puede configurar la siguiente información:

   * Filtros, Vistas y Agrupaciones según desee en la lista de tareas. Los filtros y agrupaciones seleccionados en la vista de lista se mantienen al ver el [!UICONTROL gráfico Gantt]. Las vistas se reflejan en el [!UICONTROL gráfico Gantt] exportado solamente en la lista que se muestra al lado del [!UICONTROL gráfico Gantt] en la primera página. Las vistas no se muestran en el propio [!UICONTROL gráfico Gantt].

     >[!TIP]
     >
     >Para dejar más espacio para el propio [!UICONTROL gráfico Gantt], aplique una vista que contenga el menor número posible de columnas.

   * Opciones de configuración en el [!UICONTROL gráfico Gantt]. Por ejemplo, puede habilitar hitos, fechas, [!UICONTROL líneas de base] o [!UICONTROL porcentaje completado] para que aparezcan en el [!UICONTROL gráfico Gantt].

     Para obtener más información, consulte   [Configure cómo se muestra la información en el [!UICONTROL gráfico Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

     >[!NOTE]
     >
     > Las asignaciones no se muestran en el [!UICONTROL gráfico Gantt] cuando el [!UICONTROL gráfico Gantt] se exporta al PDF. Cuando se exporta el [!UICONTROL diagrama de Gantt] al PDF, las asignaciones solo se muestran en la vista de lista.

   * Período de tiempo que se muestra en el [!UICONTROL gráfico Gantt].\

     Para obtener más información, vea [Ver información en el [!UICONTROL gráfico Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

     La forma en que se muestra el período de tiempo en el archivo de exportación depende de si selecciona **[!UICONTROL Lo que veo]** o **[!UICONTROL Varias páginas]** en un paso posterior.

1. (Opcional) Para incluir solo determinadas tareas en el PDF exportado, seleccione las tareas que desee incluir.

   Si no selecciona ninguna tarea, todas las tareas se incluyen en el PDF exportado.

   Por ejemplo, si está viendo el [!UICONTROL gráfico Gantt] de un proyecto que contiene 50 tareas, pero desea mostrar solamente 10 tareas en el [!UICONTROL gráfico Gantt] exportado, seleccione las 10 tareas que desee mostrar.

1. Haga clic en el icono de impresora.\
   Se muestra el cuadro de diálogo **[!UICONTROL Exportar a PDF]**.\
   ![export_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. Seleccione si desea exportar solamente lo que ve o todo el [!UICONTROL gráfico Gantt]:

   * **[!UICONTROL Lo que veo]:** Exporta todas las tareas (incluidas las subtareas) que se muestran en la pantalla antes de exportar un máximo de 500 elementos. (Esto no es lo que se muestra en la sección **[!UICONTROL Preview]**; la sección [!UICONTROL Preview] contiene solo datos de ejemplo).

     Las subtareas se incluyen en el PDF exportado incluso si la tarea principal está contraída y las subtareas no son visibles. Para incluir sólo las tareas principales, seleccione las tareas principales que desee incluir y deje las subtareas sin seleccionar.

     Puede usar el menú desplegable **[!UICONTROL Zoom hasta]** o la herramienta deslizante para mostrar solo una parte del [!UICONTROL gráfico Gantt], tal como se describe en [Visualización de información en el [!UICONTROL gráfico Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md) .

   * **[!UICONTROL Varias páginas]:** Exporta todo el [!UICONTROL gráfico Gantt], incluso el que no esté visible en la pantalla actual hasta 500 elementos.\

     Puede usar el menú desplegable **[!UICONTROL Zoom hasta]** o la herramienta deslizante para determinar cuánta información se muestra en cada página, como se describe en [Configurar cómo se muestra la información en el [!UICONTROL gráfico Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). Seleccione una opción más granular para mostrar más páginas para exportar o seleccione una opción menos granular para mostrar menos páginas para exportar.

     >[!NOTE]
     >
     >Si necesita exportar un [!UICONTROL gráfico Gantt] que contiene más de 500 elementos, aplique un filtro a la lista antes de ver el [!UICONTROL gráfico Gantt] para que se muestren menos de 500 elementos o 250 páginas. Para obtener información acerca de cómo aplicar un filtro, vea [Resumen de filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >No se puede exportar todo el diagrama de Gantt en las siguientes circunstancias:
     >
     >   
     >   
     >   * Cuando abarca más de 250 páginas
     >   * Cuando contiene más de 500 elementos




1. Si el PDF se imprimirá después de exportarlo al PDF, en el menú desplegable **[!UICONTROL Tamaño de página]**, seleccione el tamaño de papel en el que desea imprimir.\
   Puede seleccionar **[!UICONTROL Carta]**, **[!UICONTROL Legal]**, **[!UICONTROL Libro mayor]**, **[!UICONTROL A1]**, **[!UICONTROL A2]**, **[!UICONTROL A3]** (disponible solo para algunos idiomas) o **[!UICONTROL A4]**.
1. En la sección **[!UICONTROL Orientación de página]**, seleccione si desea que el PDF se exporte en orientación horizontal o vertical.
1. Seleccione **[!UICONTROL Mostrar leyenda]** si desea incluir la leyenda en el PDF exportado.
1. Haga clic en **[!UICONTROL Exportar]**.

   El PDF del [!UICONTROL gráfico Gantt] se crea y se descarga en el equipo.

   Observe la leyenda que aparece en la parte inferior del archivo exportado. En él se explican únicamente las opciones que ha habilitado en el [!UICONTROL gráfico Gantt] y que están disponibles en la lista de tareas.

   Por ejemplo, los hitos se muestran en la leyenda solo si tiene al menos una tarea asociada a un hito.

   ![gantt_chart_with_updated__limited__pie_de_ilustración.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
