---
product-area: reporting
navigation-topic: reporting-elements
title: Modificar la anchura y el orden de las columnas
description: Lea este artículo para obtener más información sobre las directrices sobre la anchura de las columnas, para cambiar su anchura y orden en Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: ece3f908-a0da-45d4-9f4f-0b34c69ce8fa
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1012'
ht-degree: 96%

---

# Modificar la anchura y el orden de las columnas

<!-- Audited: 11/2024 -->

A continuación se ofrecen directrices sobre cómo funcionan las anchuras de las columnas en Adobe Workfront:

* Workfront define la anchura de las columnas de las listas y los informes de forma predeterminada.
* Workfront ajusta automáticamente la anchura de las columnas según la información de `valueformat` de todas las listas e informes, a menos que se especifique lo contrario en el modo de texto de la columna.

  >[!NOTE]
  >
  >Workfront no ajusta la anchura de las columnas según la información de `valueformat` en las listas disponibles en las áreas Configuración e Informes.

  El valor `valueformat` define qué tipo de información se muestra en la columna. Por ejemplo, las columnas que muestran un número son más estrechas que las columnas que muestran el campo Descripción.

* Puede personalizar la anchura de las columnas de las listas e informes de Workfront para que coincida con sus necesidades, según el tipo de información que desee mostrar en las columnas.

  Puede modificar la anchura de las columnas temporalmente, mientras ve una lista o informe, o permanentemente, ajustando la anchura de la columna en el generador de vistas. Para obtener información acerca de cómo modificar temporalmente la anchura de las columnas, consulte la sección [Consideraciones al modificar temporalmente la anchura y el orden de las columnas](#considerations-when-temporarily-modifying-the-width-and-order-of-columns) en este artículo.

* Las columnas que aparecen en las vistas integradas tienen anchuras definidas previamente por Workfront y codificadas de forma rígida. Para modificar estas anchuras, debe actualizar manualmente la anchura de estas columnas con el modo de texto en el generador de vistas.

  Para obtener información acerca de cómo modificar la columna en modo de texto, consulte [Vista: editar permanentemente la anchura de una columna](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Plan de Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> 
      <p>Nuevo:</p>
         <ul>
         <li><p>Colaborador o superior</p></li>
         </ul>
      <p>Actual:</p>
         <ul>
         <li><p>Solicitud o superior</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Acceso de edición a filtros, vistas y agrupaciones</p> <p>Acceso de edición a informes, paneles de control y calendarios para editar la vista de un informe</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Permisos de administración de un informe para editar una vista en un informe</p> <p>Permisos de administración de una vista para editarla</p></td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modificar la anchura y el orden de las columnas

Puede modificar la anchura y el orden de las columnas de los informes de las siguientes maneras:

* [Modificar la anchura y el orden de las columnas temporalmente](#modify-width-and-order-of-columns-temporarily)
* [Modificar la anchura y el orden de las columnas permanentemente](#modify-width-and-order-of-columns-permanently)

### Modificar la anchura y el orden de las columnas permanentemente {#modify-width-and-order-of-columns-temporarily}

Puede arrastrar bordes de columnas para cambiar el tamaño de las mismas y arrastrarlas y soltarlas para reordenarlas temporalmente en la mayoría de las listas del sitio de Workfront. Esto incluye informes, vistas, informes sobre paneles de control y la vista Gantt.

Para obtener más información acerca de las listas de Workfront, consulte el artículo [Introducción a las listas en Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* [Consideraciones al modificar temporalmente la anchura y el orden de las columnas](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)
* [Cambiar el tamaño de columnas temporalmente](#resize-columns-temporarily)
* [Reordene las columnas temporalmente](#reorder-columns-temporarily)

#### Consideraciones al modificar temporalmente la anchura y el orden de las columnas {#considerations-when-temporarily-modifying-the-width-and-order-of-columns}

Puede modificar temporalmente la anchura y el orden de las columnas de una lista sin editar su vista.

Tenga en cuenta lo siguiente al cambiar temporalmente el tamaño y ordenar las columnas:

* Al cambiar el tamaño de las columnas, los nuevos tamaños de columna se almacenan en el almacenamiento local del explorador y se guardan de forma predeterminada. Si utiliza un explorador diferente o borra la caché o los datos de navegación, los tamaños de columna se revierten al tamaño predeterminado. Al actualizar la página, se mantienen los cambios realizados en la anchura de las columnas.

>[!NOTE]
> 
>La anchura de las columnas está limitada por el tamaño de la ventana del explorador; si se actualiza la página, su anchura se reduce hasta que todas las columnas caben en la ventana sin necesidad de desplazarse horizontalmente. Para forzar que una columna sea más ancha de lo que cabe en el explorador, debe establecer la anchura de la columna en el modo de texto tal como se describe en [Modificar la anchura y el orden de las columnas permanentemente](#modify-width-and-order-of-columns-permanently) y evitar ajustar manualmente la anchura de las columnas arrastrando sus bordes.
>

* Al reordenar las columnas, el orden elegido se mantiene únicamente hasta que se aleja de la lista o se actualiza la página del explorador. Después de salir de la lista o actualizar la página del explorador, las columnas vuelven a su orden predeterminado.
* Para obtener un rendimiento óptimo, las columnas que está reordenando no deben tener más de 100 elementos en la lista.
* Al cambiar el tamaño de las columnas, los cambios solo se aplican a la vista que está utilizando actualmente y solo son visibles para usted. Al compartir una vista con otro usuario, no se comparten los tamaños de columna definidos.
* Después de cambiar el tamaño de una columna arrastrando su borde hacia la derecha, se conserva el ancho de la columna contigua, excepto en los casos siguientes:

   * El área de Configuración
   * El área de Informes
   * Listas de documentos e informes

  >[!NOTE]
  >
  >No puede mover el borde izquierdo de una columna más allá del borde izquierdo de la columna contigua en ninguna lista.

* Si exporta cualquier lista a un archivo, el orden temporal de las columnas no se transfiere al archivo exportado. El archivo exportado muestra el orden de las columnas en la lista original, antes de que se hayan reorganizado las columnas.

Para obtener más información acerca de cómo exportar datos de listas e informes, consulte el artículo [Exportar datos](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

#### Cambiar el tamaño de columnas temporalmente {#resize-columns-temporarily}

1. Vaya a la lista que desee modificar.
1. Arrastre el borde de un encabezado de columna hasta que la columna alcance el tamaño deseado.\
   ![Cambiar tamaño de columna](assets/column-resize-350x124.png)

#### Reordene las columnas temporalmente {#reorder-columns-temporarily}

1. Vaya a la lista que desee modificar.
1. Haga clic en el encabezado de columna que desee mover a la ubicación deseada y arrástrelo.

>[!TIP]
>
>Esto resulta especialmente útil cuando se visualiza simultáneamente el gráfico Gantt y la vista de lista. Al ver el gráfico Gantt, las columnas pueden quedar ocultas. Para ver una columna mientras se muestra el gráfico Gantt, simplemente arrastre la columna que desee ver para que se muestre en el lado izquierdo de la página.

### Modificar la anchura y el orden de las columnas permanentemente {#modify-width-and-order-of-columns-permanently}

Para reordenar las columnas de forma permanente, consulte la sección [Crear o personalizar una vista estándar](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-a-standard-view) en el artículo [Información general de las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Solo se puede modificar de forma permanente el ancho de una columna mediante el modo de texto.

Para obtener más información acerca del uso del modo de texto y la modificación permanente del ancho de una columna, vea el artículo [Información general sobre usos comunes del modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
