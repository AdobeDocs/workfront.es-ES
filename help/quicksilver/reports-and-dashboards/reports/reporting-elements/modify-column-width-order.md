---
product-area: reporting
navigation-topic: reporting-elements
title: Modificar el ancho y el orden de las columnas
description: Lea este artículo para obtener más información sobre las directrices sobre el ancho de columna y cómo cambiar el ancho y el orden de las columnas en Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: ece3f908-a0da-45d4-9f4f-0b34c69ce8fa
source-git-commit: 332c744ab9b760268620461ed2cb2551caf383cf
workflow-type: tm+mt
source-wordcount: '1066'
ht-degree: 0%

---

# Modificar el ancho y el orden de las columnas

A continuación se ofrecen directrices sobre cómo funcionan los anchos de columna en Adobe Workfront:

* Workfront define el ancho de las columnas de las listas y los informes de forma predeterminada.
* Workfront ajusta automáticamente el ancho de las columnas según la información `valueformat` de todas las listas e informes, a menos que se especifique lo contrario en el modo de texto de la columna.

  >[!NOTE]
  >
  >Workfront no ajusta el ancho de las columnas según la información de `valueformat` en las listas disponibles en las áreas Configuración e Informes.

  El valor `valueformat` define qué tipo de información se muestra en la columna. Por ejemplo, las columnas que muestran un número son más estrechas que las columnas que muestran el campo Descripción.

* Puede personalizar el ancho de las columnas de las listas e informes de Workfront para que coincida con sus necesidades, según el tipo de información que desee mostrar en las columnas.

  Puede modificar el ancho de las columnas temporalmente, mientras ve una lista o informe, o permanentemente, ajustando el ancho de la columna en el generador de vistas. Para obtener información acerca de cómo modificar temporalmente el ancho de las columnas, vea la sección [Consideraciones al modificar temporalmente el ancho y el orden de las columnas](#considerations-when-temporarily-modifying-the-width-and-order-of-columns) en este artículo.

* Las columnas que aparecen en las vistas integradas tienen anchos definidos previamente por Workfront y codificados. Para modificar estos anchos, debe actualizar manualmente el ancho de estas columnas con el modo de texto en el generador de vistas.

  Para obtener información acerca de cómo modificar la columna en modo de texto, vea [Ver: editar permanentemente el ancho de una columna](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Solicitud o superior </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p>Editar el acceso a Informes, Paneles y Calendarios para editar la vista de un informe</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Administración de permisos de un informe para editar una vista de un informe</p> <p>Administrar permisos a una vista para editarla</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Modificar el ancho y el orden de las columnas

Puede modificar el ancho y el orden de las columnas de los informes de las siguientes maneras:

* [Modificar el ancho y el orden de las columnas temporalmente](#modify-width-and-order-of-columns-temporarily)
* [Modificar el ancho y el orden de las columnas de forma permanente](#modify-width-and-order-of-columns-permanently)

### Modificar temporalmente el ancho y el orden de las columnas {#modify-width-and-order-of-columns-temporarily}

Puede arrastrar bordes de columna para cambiar el tamaño de las columnas y arrastrar y soltar columnas para reordenarlas temporalmente en la mayoría de las listas del sitio de Workfront. Esto incluye informes, vistas, informes sobre paneles y la vista Gantt.

Para obtener más información acerca de las listas de Workfront, consulte el artículo [Introducción a las listas en Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* [Consideraciones al modificar temporalmente el ancho y el orden de las columnas](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)
* [Cambiar tamaño de columnas temporalmente](#resize-columns-temporarily)
* [Reordenar las columnas temporalmente](#reorder-columns-temporarily)

#### Consideraciones al modificar temporalmente el ancho y el orden de las columnas {#considerations-when-temporarily-modifying-the-width-and-order-of-columns}

Puede modificar temporalmente el ancho y el orden de las columnas de una lista sin editar su vista.

Tenga en cuenta lo siguiente al cambiar temporalmente el tamaño y ordenar las columnas:

* Al cambiar el tamaño de las columnas, los nuevos tamaños de columna se almacenan en el almacenamiento local del explorador y se guardan de forma predeterminada. Si utiliza un explorador diferente o borra la caché o los datos de navegación, los tamaños de columna se revierten al tamaño predeterminado. Al actualizar la página, se mantienen los cambios realizados en el ancho de las columnas.

>[!NOTE]
> 
>El ancho de las columnas está limitado por el tamaño de la ventana del explorador; si se actualiza la página, el ancho de las columnas se reduce hasta que todas las columnas caben en la ventana sin necesidad de desplazarse horizontalmente. Para forzar que una columna sea más ancha de lo que cabrá en el explorador, debe establecer el ancho de la columna en el modo de texto tal como se describe en [Modificar el ancho y el orden de las columnas de forma permanente](#modify-width-and-order-of-columns-permanently) y evitar ajustar manualmente el ancho de las columnas arrastrando sus bordes.
>

* Al reordenar las columnas, el orden elegido se mantiene únicamente hasta que se aleja de la lista o se actualiza la página del explorador. Después de salir de la lista o actualizar la página del explorador, las columnas vuelven a su orden predeterminado.
* Para obtener un rendimiento óptimo, las columnas que está reordenando no deben tener más de 100 elementos en la lista.
* Al cambiar el tamaño de las columnas, los cambios sólo se aplican a la vista que está utilizando actualmente y sólo son visibles para usted. Al compartir una vista con otro usuario, no se comparten los tamaños de columna definidos.
* Después de cambiar el tamaño de una columna arrastrando su borde hacia la derecha, se conserva el ancho de la columna contigua, excepto en los casos siguientes:

   * El área Configuración
   * El área Informes
   * Listas de documentos e informes

  >[!NOTE]
  >
  >No puede mover el borde izquierdo de una columna más allá del borde izquierdo de la columna contigua en ninguna lista.

* Si exporta cualquier lista a un archivo, el orden temporal de las columnas no se transfiere al archivo exportado. El archivo exportado muestra el orden de las columnas en la lista original, antes de que se hayan reorganizado las columnas.

Para obtener más información acerca de cómo exportar datos de listas e informes, vea el artículo [Exportar datos](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

#### Cambiar el tamaño de columnas temporalmente {#resize-columns-temporarily}

1. Vaya a la lista que desee modificar.
1. Arrastre el borde de una columna hasta que la columna alcance el tamaño deseado.\
   ![](assets/column-resize-350x124.png)

#### Reordenar las columnas temporalmente {#reorder-columns-temporarily}

1. Vaya a la lista que desee modificar.
1. Haga clic en una columna que desee mover a otra ubicación para elegir la columna.
1. Arrastre la columna a la ubicación correcta.
1. Coloque la columna en la ubicación para moverla.

   ![](assets/column-reorder-350x118.png)

>[!TIP]
>
>Esto resulta especialmente útil cuando se visualiza simultáneamente el gráfico Gantt y la vista de lista. Al ver el gráfico Gantt, las columnas pueden quedar ocultas. Para ver una columna mientras se muestra el gráfico Gantt, simplemente arrastre la columna que desee ver para que se muestre en el lado izquierdo de la página.

### Modificar el ancho y el orden de las columnas de forma permanente {#modify-width-and-order-of-columns-permanently}

Para reordenar las columnas de forma permanente, consulte la sección [Crear o personalizar una vista estándar](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-a-standard-view) en el artículo [Información general de las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Solo se puede modificar de forma permanente el ancho de una columna mediante el modo de texto.

Para obtener más información acerca del uso del modo de texto y la modificación permanente del ancho de una columna, vea el artículo [Información general sobre usos comunes del modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
