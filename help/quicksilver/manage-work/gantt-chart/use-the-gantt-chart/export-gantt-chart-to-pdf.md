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

# Exporte el [!UICONTROL Gráfico Gantt] al PDF

Puede exportar la variable [!UICONTROL Gráfico Gantt] a un PDF.

Después de exportar el [!UICONTROL Gráfico Gantt] en PDF, puede imprimirlo o adjuntarlo a un correo electrónico para compartirlo con otros usuarios.

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
   <td> <p>[!UICONTROL View] o acceso superior a Proyectos y tareas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo [!DNL Workfront] El administrador puede modificar su nivel de acceso. Consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>[!UICONTROL View] o acceso superior al proyecto</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Exporte el [!UICONTROL Gráfico Gantt]

1. Acceda a la [!UICONTROL Gráfico Gantt] que desea exportar a PDF, tal como se describe en [Introducción a la [!UICONTROL Gráfico Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. Asegúrese de haber configurado la variable [!UICONTROL Gráfico Gantt] para mostrar la información adecuada antes de exportarla.

   >[!NOTE]
   >
   >Si exporta el [!UICONTROL Gráfico Gantt] a partir de una lista de proyectos, el archivo PDF contiene sólo los proyectos de la lista, no las tareas de cada proyecto. Si desea exportar una lista de tareas, puede hacerlo desde el proyecto con el que están asociadas o creando un informe de tareas y mostrando los resultados del informe en la [!UICONTROL Vista Gantt].

   Puede configurar la siguiente información:

   * Filtros, Vistas y Agrupaciones según desee en la lista de tareas. Los filtros y agrupaciones seleccionados en la vista de lista se mantienen al ver el [!UICONTROL Gráfico Gantt]. Las vistas se reflejan en el archivo exportado [!UICONTROL Gráfico Gantt] solo dentro de la lista que se muestra junto a la variable [!UICONTROL Gráfico Gantt] en la primera página. Las vistas no se muestran en [!UICONTROL Gráfico Gantt] sí mismo.

     >[!TIP]
     >
     >Para dejar más espacio para [!UICONTROL Gráfico Gantt] En sí, aplique una vista que contenga el menor número posible de columnas.

   * Opciones de configuración en [!UICONTROL Gráfico Gantt]. Por ejemplo, puede habilitar hitos, fechas, [!UICONTROL líneas de base], o [!UICONTROL por ciento completado] para que aparezca en [!UICONTROL Gráfico Gantt].

     Para obtener más información, consulte   [Configure cómo se muestra la información en la [!UICONTROL Gráfico Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

     >[!NOTE]
     >
     > Las asignaciones no se muestran en [!UICONTROL Gráfico Gantt] cuando la variable [!UICONTROL Gráfico Gantt] se exporta al PDF. Si la variable [!UICONTROL Gráfico Gantt] se exporta al PDF, las asignaciones sólo se muestran en la vista de lista.

   * El período de tiempo que se muestra en la [!UICONTROL Gráfico Gantt].\

     Para obtener más información, consulte [Visualización de información en [!UICONTROL Gráfico Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

     La forma en que se muestra el periodo de tiempo en el archivo de exportación depende de si selecciona **[!UICONTROL Lo que veo]** o **[!UICONTROL Varias páginas]** en un paso posterior.

1. (Opcional) Para incluir solo determinadas tareas en el PDF exportado, seleccione las tareas que desee incluir.

   Si no selecciona ninguna tarea, todas las tareas se incluyen en el PDF exportado.

   Por ejemplo, si está viendo el [!UICONTROL Gráfico Gantt] para un proyecto que contiene 50 tareas, pero en el que sólo desea mostrar 10 tareas en el archivo exportado [!UICONTROL Gráfico Gantt], seleccione las 10 tareas que desee mostrar.

1. Haga clic en el icono de impresora.\
   El **[!UICONTROL Exportar a PDF]** Cuadro de diálogo.\
   ![export_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. Seleccione si desea exportar solo lo que ve o todo el [!UICONTROL Gráfico Gantt]:

   * **[!UICONTROL Lo que veo]:** Exporta todas las tareas (incluidas las subtareas) que se muestran en la pantalla antes de exportar hasta 500 elementos. (Esto no es lo que se muestra en la **[!UICONTROL Previsualizar]** sección; la [!UICONTROL Previsualizar] contiene sólo datos de ejemplo.)

     Las subtareas se incluyen en el PDF exportado incluso si la tarea principal está contraída y las subtareas no son visibles. Para incluir sólo las tareas principales, seleccione las tareas principales que desee incluir y deje las subtareas sin seleccionar.

     Puede usar el complemento **[!UICONTROL Zoom hasta]** menú desplegable o la herramienta deslizante para mostrar solo una parte de la [!UICONTROL Gráfico Gantt], tal como se describe en [Visualización de información en [!UICONTROL Gráfico Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md) .

   * **[!UICONTROL Varias páginas]:** Exporta todo el [!UICONTROL Gráfico Gantt], incluso el que no esté visible en la pantalla actual hasta 500 elementos.\

     Puede usar el complemento **[!UICONTROL Zoom hasta]** menú desplegable o la herramienta deslizante para determinar cuánta información se muestra en cada página, tal como se describe en [Configure cómo se muestra la información en la [!UICONTROL Gráfico Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). Seleccione una opción más granular para mostrar más páginas para exportar o seleccione una opción menos granular para mostrar menos páginas para exportar.

     >[!NOTE]
     >
     >Si necesita exportar un [!UICONTROL Gráfico Gantt] que contiene más de 500 elementos, aplique un filtro a la lista antes de ver los [!UICONTROL Gráfico Gantt] para que se muestren menos de 500 elementos o 250 páginas. Para obtener información sobre cómo aplicar un filtro, consulte  [Resumen de filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >No se puede exportar todo el diagrama de Gantt en las siguientes circunstancias:
     >
     >   
     >   
     >   * Cuando abarca más de 250 páginas
     >   * Cuando contiene más de 500 elementos




1. Si el PDF se imprimirá después de exportarlo al PDF, en el **[!UICONTROL Tamaño de página]** , seleccione el tamaño del papel en el que desea imprimir.\
   Puede seleccionar **[!UICONTROL Carta]**, **[!UICONTROL Legal]**, **[!UICONTROL Libro Mayor]**, **[!UICONTROL A1]**, **[!UICONTROL A2]**, **[!UICONTROL A3]** (disponible solo para algunos idiomas), o **[!UICONTROL A4]**.
1. En el **[!UICONTROL Orientación de página]** , seleccione si desea que el PDF se exporte en orientación horizontal o vertical.
1. Seleccionar **[!UICONTROL Mostrar leyenda]** si desea incluir la leyenda en el PDF exportado.
1. Clic **[!UICONTROL Exportar]**.

   El pdf del [!UICONTROL Gráfico Gantt] se crea y se descarga en el equipo.

   Observe la leyenda que aparece en la parte inferior del archivo exportado. En él se explican únicamente las opciones que ha habilitado en su [!UICONTROL Gráfico Gantt] y que están disponibles en la lista de tareas.

   Por ejemplo, los hitos se muestran en la leyenda solo si tiene al menos una tarea asociada a un hito.

   ![Gantt_chart_with_updated__limited__leyenda.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
