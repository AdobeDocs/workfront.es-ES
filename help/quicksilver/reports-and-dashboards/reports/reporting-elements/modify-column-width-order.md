---
product-area: reporting
navigation-topic: reporting-elements
title: Modificar el ancho y el orden de las columnas
description: Lea este artículo para obtener más información sobre las directrices de anchura de columna y cómo cambiar el ancho y el orden de las columnas en Workfront.
author: Lisa
feature: Reports and Dashboards
exl-id: ece3f908-a0da-45d4-9f4f-0b34c69ce8fa
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 0%

---

# Modificar el ancho y el orden de las columnas

A continuación se proporcionan directrices sobre cómo funcionan los anchos de columna en Adobe Workfront:

* Workfront define de forma predeterminada la anchura de las columnas de las listas y los informes.
* Workfront ajusta automáticamente la anchura de las columnas según la variable `valueformat`en todas las listas e informes, a menos que se especifique lo contrario en el modo de texto de la columna.

   >[!NOTE]
   >
   >Workfront no ajusta la anchura de las columnas según la variable `valueformat` información de las listas disponibles en las áreas Configuración e Informes .

   La variable `valueformat` define qué tipo de información se muestra en la columna. Por ejemplo, las columnas que muestran un número son más estrechas que las columnas que muestran el campo Descripción .

* Puede personalizar la anchura de las columnas de las listas e informes de Workfront para adaptarla a sus necesidades, en función del tipo de información que desee mostrar en las columnas.

   Puede modificar el ancho de las columnas temporalmente mientras visualiza una lista o informe, o de forma permanente, ajustando el ancho de la columna en el generador de vistas. Para obtener información sobre la modificación temporal del ancho de las columnas, consulte la [Consideraciones al modificar temporalmente la anchura y el orden de las columnas](#considerations-when-temporarily-modifying-the-width-and-order-of-columns) en este artículo.

* Las columnas que aparecen en las vistas integradas tienen anchos definidos previamente por Workfront que están codificados de forma rígida. Para modificar estos anchos, debe actualizar manualmente la anchura de estas columnas mediante el modo de texto en el generador de vistas.

   Para obtener información sobre cómo modificar la columna en modo de texto, consulte [Ver: editar permanentemente el ancho de una columna](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan de Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Editar acceso a filtros, vistas y grupos</p> <p>Editar acceso a informes, tableros y calendarios para editar la vista en un informe</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Administrar permisos en un informe para editar una vista en un informe</p> <p>Administrar permisos en una vista para editarla</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Modificar el ancho y el orden de las columnas

Puede modificar el ancho y el orden de las columnas en los informes de las siguientes maneras:

* [Modificación temporal del ancho y el orden de las columnas](#modify-width-and-order-of-columns-temporarily)
* [Modificar el ancho y el orden de las columnas de forma permanente](#modify-width-and-order-of-columns-permanently)

### Modificación temporal del ancho y el orden de las columnas {#modify-width-and-order-of-columns-temporarily}

Puede arrastrar los bordes de las columnas para cambiar el tamaño de las columnas y arrastrar y soltar columnas para reordenarlas temporalmente en la mayoría de las listas del sitio de Workfront. Esto incluye informes, vistas, informes sobre tableros y la vista Gantt.

Para obtener más información sobre las listas de Workfront, consulte el artículo [Introducción a las listas en Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* [Consideraciones al modificar temporalmente la anchura y el orden de las columnas](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)
* [Cambiar el tamaño de las columnas temporalmente](#resize-columns-temporarily)
* [Reordenar columnas temporalmente](#reorder-columns-temporarily)

#### Consideraciones al modificar temporalmente la anchura y el orden de las columnas {#considerations-when-temporarily-modifying-the-width-and-order-of-columns}

Puede modificar temporalmente el ancho y el orden de las columnas de una lista sin editar su vista.

Tenga en cuenta lo siguiente cuando cambie temporalmente el tamaño de las columnas y las ordene:

* Al cambiar el tamaño de las columnas, los nuevos tamaños de columna se almacenan en el almacenamiento local del explorador y se guardan de forma predeterminada. Usar un explorador diferente o borrar la caché o examinar los datos hace que los tamaños de columna se reviertan al valor predeterminado. Al actualizar la página, se mantienen los cambios realizados en el ancho de las columnas.
* Al reordenar las columnas, el orden que elija se mantiene únicamente hasta que salga de la lista o actualice la página del explorador. Después de salir de la lista o de actualizar la página del explorador, las columnas vuelven a su orden predeterminado.
* Para obtener un rendimiento óptimo, las columnas que está reordenando no deben tener más de 100 elementos en la lista.
* Al cambiar el tamaño de las columnas, los cambios solo se aplican a la vista que está utilizando y solo usted puede ver. Compartir una vista con otro usuario no comparte los tamaños de columna que haya definido.
* Después de cambiar el tamaño de una columna arrastrando su borde a la derecha, se conserva el ancho de la columna vecina, excepto en lo siguiente:

   * Área de configuración
   * El área de informes
   * Listas de documentos e informes

   >[!NOTE]
   >
   >No se puede mover el borde izquierdo de una columna más allá del borde izquierdo de la columna vecina de ninguna lista.

* Si exporta cualquier lista a un archivo, el orden temporal de las columnas no se transfiere al archivo exportado. El archivo exportado muestra el orden de las columnas de la lista original antes de reordenar las columnas.

Para obtener más información sobre la exportación de datos de listas e informes, consulte el artículo [Exportar datos](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

#### Cambiar el tamaño de las columnas temporalmente {#resize-columns-temporarily}

1. Vaya a la lista que desee modificar.
1. Arrastre el borde de una columna hasta que alcance el tamaño deseado.\
   ![](assets/column-resize-350x124.png)

#### Reordenar columnas temporalmente {#reorder-columns-temporarily}

1. Vaya a la lista que desee modificar.
1. Haga clic en una columna que desee mover a otra ubicación para elegir la columna.
1. Arrastre la columna a la ubicación correcta.
1. Coloque la columna en la ubicación para moverla.

   ![](assets/column-reorder-350x118.png)

>[!TIP]
>
>Esto resulta especialmente útil cuando se visualizan simultáneamente el diagrama de Gantt y la vista de lista. Al ver el diagrama de Gantt, las columnas pueden ocultarse. Para ver una columna mientras se muestra el gráfico de Gantt, simplemente arrastre la columna que desee ver para que se muestre en el lado izquierdo de la página.

### Modificar el ancho y el orden de las columnas de forma permanente {#modify-width-and-order-of-columns-permanently}

Para reordenar las columnas de forma permanente, consulte la sección [Crear o personalizar una vista estándar](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-a-standard-view) en el artículo [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Solo se puede modificar de forma permanente la anchura de una columna mediante el modo de texto.

Para obtener más información sobre el uso del modo de texto y la modificación permanente del ancho de una columna, consulte el artículo [Descripción general de los usos comunes del modo Texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
