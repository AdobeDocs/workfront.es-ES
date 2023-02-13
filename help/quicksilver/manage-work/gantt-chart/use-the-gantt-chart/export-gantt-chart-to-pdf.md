---
navigation-topic: use-the-gantt-chart
title: Exportar el diagrama de Gantt al PDF
description: Puede exportar el diagrama de Gantt a un PDF.
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 0%

---

# Exportar el [!UICONTROL Diagrama de Gantt] al PDF

Puede exportar la variable [!UICONTROL Diagrama de Gantt] a un PDF.

Después de exportar la variable [!UICONTROL Diagrama de Gantt] al PDF, puede imprimirlo o adjuntarlo a un correo electrónico para compartirlo con otros usuarios.

## Requisitos de acceso

Debe tener lo siguiente para seguir los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>[!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>[!UICONTROL View] o acceso superior a Proyectos y tareas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>[!UICONTROL View] o acceso superior al proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Exportar el [!UICONTROL Diagrama de Gantt]

1. Acceda a la [!UICONTROL Diagrama de Gantt] que desea exportar a PDF, tal como se describe en [Introducción a [!UICONTROL Diagrama de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. Asegúrese de haber configurado la variable [!UICONTROL Diagrama de Gantt] para mostrar la información adecuada antes de exportarla.

   >[!NOTE]
   >
   >Si exporta el [!UICONTROL Diagrama de Gantt] de una lista de proyectos, el archivo PDF contiene solo los proyectos de la lista, no las tareas de cada proyecto. Si desea exportar una lista de tareas, puede hacerlo desde el proyecto al que están asociadas, o creando un informe de tareas y mostrando los resultados del informe en la variable [!UICONTROL Vista Gantt].

   Puede configurar la siguiente información:

   * Filtros, Vistas y Agrupaciones como desee en la lista de tareas. Todos los filtros y agrupamientos seleccionados en la vista de lista se mantienen cuando se visualiza el [!UICONTROL Diagrama de Gantt]. Las vistas se reflejan en las [!UICONTROL Diagrama de Gantt] solo en la lista que se muestra junto a la [!UICONTROL Diagrama de Gantt] en la primera página. Las vistas no se muestran en la variable [!UICONTROL Diagrama de Gantt] en sí.

      >[!TIP]
      >
      >Para dejar más espacio para el [!UICONTROL Diagrama de Gantt] aplique una vista que contenga el menor número posible de columnas.

   * Las opciones de configuración de [!UICONTROL Diagrama de Gantt]. Por ejemplo, puede habilitar hitos, fechas y [!UICONTROL líneas de base]o [!UICONTROL porcentaje completado] para que aparezca en el [!UICONTROL Diagrama de Gantt].

      Para obtener más información, consulte   [Configure cómo se muestra la información en la variable [!UICONTROL Diagrama de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

      >[!NOTE]
      >
      > Las asignaciones no se muestran en la [!UICONTROL Diagrama de Gantt] cuando la variable [!UICONTROL Diagrama de Gantt] se exporta a PDF. Cuando la variable [!UICONTROL Diagrama de Gantt] se exporta a PDF, las asignaciones se muestran solo en la vista de lista.

   * El periodo de tiempo que se muestra en la variable [!UICONTROL Diagrama de Gantt].\

      Para obtener más información, consulte [Visualización de información en la [!UICONTROL Diagrama de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

      La forma en que se muestra el periodo de tiempo en el archivo de exportación depende de si selecciona **[!UICONTROL Lo que veo]** o **[!UICONTROL Varias páginas]** en un paso posterior.

1. (Opcional) Para incluir solo determinadas tareas en el PDF exportado, seleccione las tareas que desee incluir.

   Si no selecciona ninguna tarea, todas las tareas se incluyen en el PDF exportado.

   Por ejemplo, si está viendo la variable [!UICONTROL Diagrama de Gantt] para un proyecto que contiene 50 tareas, pero que desea mostrar solo 10 tareas en el [!UICONTROL Diagrama de Gantt], seleccione las 10 tareas que desee mostrar.

1. Haga clic en el icono de impresora.\
   La variable **[!UICONTROL Exportar a PDF]** se muestra.\
   ![export_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. Seleccione si desea exportar solo lo que ve o todo el [!UICONTROL Diagrama de Gantt]:

   * **[!UICONTROL Lo que veo]:** Exporta todas las tareas (incluidas las subtareas) que se muestran en la pantalla antes de exportar hasta 500 elementos. (Esto no es lo que se muestra en la variable **[!UICONTROL Vista previa]** sección; el [!UICONTROL Vista previa] contiene solo datos de ejemplo.)

      Las subtareas se incluyen en el PDF exportado aunque la tarea principal esté contraída y las subtareas no estén visibles. Para incluir solo tareas principales, seleccione las tareas principales que desee incluir y deje las subtareas sin seleccionar.

      Puede usar la variable **[!UICONTROL Ampliar a]** menú desplegable o la herramienta de control deslizante para mostrar solo una parte del [!UICONTROL Diagrama de Gantt], tal como se describe en [Visualización de información en la [!UICONTROL Diagrama de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md) .

   * **[!UICONTROL Varias páginas]:** Exporta todo [!UICONTROL Diagrama de Gantt], incluso lo que no es visible en la pantalla actual hasta 500 elementos.\

      Puede usar la variable **[!UICONTROL Ampliar a]** menú desplegable o la herramienta de control deslizante para determinar cuánta información se muestra en cada página, tal como se describe en [Configure cómo se muestra la información en la variable [!UICONTROL Diagrama de Gantt]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). Seleccione una opción más granular para mostrar más páginas para exportar, o seleccione una opción menos granular para mostrar menos páginas para exportar.

      >[!NOTE]
      >
      >Si necesita exportar un [!UICONTROL Diagrama de Gantt] que contenga más de 500 elementos, aplique un filtro a la lista antes de ver el [!UICONTROL Diagrama de Gantt] de modo que se muestren menos de 500 elementos o 250 páginas. Para obtener información sobre cómo aplicar un filtro, consulte  [Información general sobre filtros en [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
      >
      >
      >No se puede exportar todo el diagrama de Gantt en las siguientes circunstancias:
      >
      >   
      >   
      >   * Cuando ocupa más de 250 páginas
      >   * Cuando contiene más de 500 elementos





1. Si el PDF se imprimirá después de exportarse a PDF, en la **[!UICONTROL Tamaño de página]** menú desplegable, seleccione el tamaño del papel al que desee imprimir.\
   Puede seleccionar **[!UICONTROL Letra]**, **[!UICONTROL Información legal]**, **[!UICONTROL Contabilidad]**, **[!UICONTROL A1]**, **[!UICONTROL A2]**, **[!UICONTROL A3]** (solo disponible para algunos idiomas), o **[!UICONTROL A4]**.
1. En el **[!UICONTROL Orientación de la página]** , seleccione si desea que el PDF se exporte en orientación horizontal o vertical.
1. Select **[!UICONTROL Mostrar leyenda]** si desea incluir la leyenda en el PDF exportado.
1. Haga clic en **[!UICONTROL Exportar]**.

   El pdf de la [!UICONTROL Diagrama de Gantt] se crea y descarga en el equipo.

   Observe la leyenda situada en la parte inferior del archivo exportado. Solo explica las opciones que ha activado en su [!UICONTROL Diagrama de Gantt] y que están disponibles en la lista de tareas.

   Por ejemplo, los hitos se muestran en la leyenda solo si tiene al menos una tarea asociada a un hito.

   ![gantt_chart_with_update__limited__leyenda.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
