---
navigation-topic: get-started-with-workfront
title: Usar listas mejoradas
description: Las listas mejoradas utilizan un formato de tabla para mostrar los elementos de la lista y tienen un aspecto diferente al de las listas estándar
author: Lisa
feature: Get Started with Workfront
exl-id: 4c25ed54-b147-4fd3-8d00-6f1ba61bbd38
source-git-commit: dc820b4012fec494ce5ebb1baefb4ee0df214916
workflow-type: tm+mt
source-wordcount: '1124'
ht-degree: 7%

---

# Uso de listas mejoradas

{{preview-fast-release-general}}

Las listas mejoradas están disponibles en algunas áreas de Adobe Workfront. Estas listas utilizan un formato de tabla para mostrar los elementos de la lista, y tienen un aspecto diferente al de las listas estándar. También se mejora la administración de vistas, incluidos el filtrado, la agrupación, la administración de columnas y la búsqueda.

Para obtener información sobre las listas estándar, consulte [Introducción a las listas en Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

>[!NOTE]
>
>Cada lista mejorada puede configurarse de forma diferente para ayudarle a mostrar los datos que necesita. No todas las listas utilizarán todas las características descritas en este artículo, y algunas listas pueden tener características especializadas que sólo se aplican a esa lista.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td>
   <p>Colaborador o superior</p>
   <p>Solicitud o superior</p></td>
  </tr>
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Objetos que utilizan listas mejoradas

A continuación se muestran algunos tipos de listas de objetos de Workfront que utilizan el formato de lista mejorado y algunas de las áreas en las que se muestran de forma predeterminada cuando tiene derechos para ver el objeto.

>[!NOTE]
>
>Esta lista no es completa. Cada una de estas listas de objetos también puede aparecer en un informe o en un panel de control. Por ejemplo, un informe de proyecto o un panel de control que contenga un informe de proyecto también mostrará una lista de proyectos.

| Lista de Workfront | Ubicación de la lista de objetos |
|--- |--- |
| Prioridades | <ul><li>Inicio > seleccione el icono Prioridades en el menú de la izquierda</li><li>Menú principal > Prioridades</li></ul> |
| Lista de solicitudes | <ul><li>Solicitudes (solo nueva experiencia)</li><li>Widget de Mis solicitudes en Inicio</li></ul> |
| Lista de tipos de cambio | <ul><li>Configuración > Preferencias del proyecto > Tasas de cambio</li></ul> |

## Adición y edición de elementos en una lista mejorada

Según la configuración de la lista mejorada, podría haber dos formas de agregar un elemento a la lista:

* Haga clic en un botón situado encima de la lista. Esta opción abre un cuadro de diálogo en el que se introduce información y se guarda.
* Haga clic en **Nueva fila** al final de la lista. Esta opción agrega una nueva fila a la tabla y se introduce información en cada celda.

  Las listas mejoradas admiten estos tipos de campos:

   * Texto
   * Número
   * Divisa
   * Fecha
   * Fecha y hora
   * Lista desplegable de selección única/múltiple
   * Escritura anticipada
   * Párrafo
   * Usuario asignado (uno o varios)
   * Selector de color

  Al editar una celda, cada tipo de campo tiene sus propias opciones de edición.

Para editar un elemento de la lista, haga doble clic en la celda que desee editar y escriba la información. Algunas celdas pueden ser de solo lectura.

![Ejemplo de lista mejorada](assets/glist-exchange-rates.png)

## Utilice la barra de acciones y el menú Más en una lista mejorada

Al seleccionar la casilla de verificación situada junto a un elemento de la lista mejorada, la barra de acciones aparece en la parte inferior de la pantalla y muestra las acciones que puede realizar con dicho elemento. Algunas acciones pueden ser específicas de esa lista y no aparecen en ninguna otra.

>[!NOTE]
>
>Varias listas mejoradas pueden permitir seleccionar un solo elemento, editar de forma masiva (seleccionando más de un elemento) o no seleccionar ningún elemento.

Haga clic en un botón de la barra de acciones para realizar esa acción, como ver el elemento de la lista, eliminarlo o editarlo.

Si no hay acciones disponibles para el elemento seleccionado, la barra de acciones indica &quot;No hay acciones disponibles&quot;.

![Ejemplo de barra de acciones](assets/glist-action-bar-exchange-rates.png)

El menú **Más** es el menú de tres puntos que aparece junto a un campo principal en un elemento de la lista cuando pasa el ratón por encima. (El campo principal es la columna situada más a la izquierda de la tabla).

Haga clic en el menú para ver acciones adicionales para el elemento. Algunas acciones pueden ser específicas de esa lista y no aparecen en ninguna otra.

![Ejemplo de menú más](assets/glist-more-menu-exchange-rates.png)

## Personalización de columnas en una lista mejorada

Algunas listas mejoradas permiten ocultar y mostrar columnas y reordenarlas.

1. Haga clic en **Columnas** sobre la lista.

   ![Ejemplo de columnas de visualización](assets/glist-display-move-columns.png)

1. Utilice las teclas de alternancia para mostrar u ocultar columnas de la lista.
1. Para reordenar las columnas, haga clic en el icono **Arrastrar** y mueva una columna a la ubicación que desee. Al mover columnas, la lista cambia automáticamente.

   >[!NOTE]
   >
   >El campo principal es la columna situada más a la izquierda de la tabla. Se fija en la primera posición y no se puede cambiar su columna. Si el número de columnas es grande, el campo principal se bloquea a la izquierda y, cuando se desplaza horizontalmente, siempre lo ve.
   >
   >El icono junto al nombre de un campo muestra el tipo de campo, como el campo de texto o de fecha.

   <span class="preview">Aparece un indicador en el botón **Columnas** cuando las columnas están ocultas. El indicador no aparece al reordenar las columnas.</span>

   ![Indicador de columnas ocultas](assets/glist-columns-hidden-indicator.png)

## Filtrar y agrupar elementos en una lista mejorada

Los filtros le ayudan a reducir la cantidad de información que se muestra en la lista. Las agrupaciones separan los objetos de la lista en áreas basadas en criterios específicos.

### Uso de filtros

1. Haga clic en **Filtro** sobre la lista.
1. En el cuadro Filtro, haga clic en **Agregar condición**.
1. Seleccione un campo por el que filtrar.
1. Seleccione un modificador de filtro, como &quot;Tiene cualquiera de&quot;, &quot;No tiene ninguno de&quot;, &quot;Es anterior a&quot; o &quot;Es posterior a&quot;. Las opciones del modificador son diferentes según el tipo de campo por el que esté filtrando.
1. Seleccione el valor o los valores del campo. Según el tipo de campo por el que filtre, se le puede pedir que seleccione el elemento de una lista, lo busque o utilice un calendario para seleccionar un intervalo de fechas.

   ![Filtrar en listas mejoradas](assets/glist-filter-with-options.png)

   El filtro se aplica automáticamente a la lista.

1. Haga clic en **Agregar condición** para agregar otra condición al filtro como una instrucción OR.
1. Cuando se aplique el filtro, puede volver a abrir las opciones de **Filter** para cambiar las opciones de filtro o borrar todos los filtros.

   <span class="preview">Aparece un indicador en el botón **Filtro** cuando se aplica un filtro a la lista.</span>

   ![Indicador de filtro aplicado](assets/glist-filter-applied-indicator.png)

### Usar agrupaciones

1. Haga clic en **Grupo** sobre la lista.
1. Seleccione una agrupación para organizar la lista.

   ![Seleccionar una agrupación](assets/glist-grouping-choose-a-group-by.png)

1. Cuando se aplique la agrupación, puede volver a abrir las opciones de Grupo para contraer o expandir todas las agrupaciones a la vez, cambiar la agrupación para agruparla por un campo diferente o borrar todas las agrupaciones.

   ![Agrupación en listas mejoradas](assets/glist-group-by-due-date-priorities.png)

   <span class="preview">Aparece un indicador en el botón **Grupo** cuando se aplica una agrupación a la lista.</span>

   ![Indicador aplicado de agrupación](assets/glist-grouping-applied-indicator.png)

## Ordenar y buscar en una lista mejorada

Para ordenar columnas individuales, vaya a la columna y haga clic en la flecha hacia abajo. Un icono junto al nombre de una columna indica que la lista está ordenada por los valores de esa columna y la dirección de la ordenación.

>[!NOTE]
>
>Es posible que algunas columnas no se puedan ordenar.

![Ordenar por una columna](assets/glist-sort-by-column.png)

Para ordenar el trabajo dentro de una agrupación, abra **Grupo** y seleccione si desea ordenar en orden ascendente o descendente.

![Ordenar en una agrupación](assets/sort-in-groups.png)

Para buscar, escriba el término de búsqueda en el campo de búsqueda situado encima de la lista. Los resultados se resaltan en la lista a medida que escribe.

![Término de búsqueda resaltado](assets/glist-search-highlighted.png)
