---
title: Configuración de una visualización de columnas en el lienzo de informes
description: Configuración de una visualización de columnas en el lienzo de informes
hidefromtoc: true
hide: true
exl-id: 5a0cdcd4-b44b-4a63-964e-1c570cd9ff77
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 2%

---

# Configuración de una visualización de columnas en el lienzo de informes

Una visualización de columnas puede ayudarle a contar rápidamente una historia sobre sus datos resaltando información importante mediante columnas verticales.

## Requisitos previos

Antes de empezar, debe inscribirse en la versión beta del lienzo de informes. Para obtener más información, consulte [Lienzo de informes beta: descripción general](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Configuración de una visualización de columnas

>[!TIP]
>
>Todos los cambios se guardan automáticamente al crear y editar los bloques del informe.

1. Comience agregando un bloque de visualización con el tipo de visualización **Column** a un informe, como se explica en [Agregar o editar un bloque de visualización en el lienzo de informes](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md).

1. Haga clic en el icono Editar visualización ![](assets/edit-icon.png) en la esquina superior derecha de la visualización y, a continuación, realice una de las siguientes acciones.

   1. En la ficha **Configuración**:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Tipo de visualización</td>
         <td><p>Cambie a un tipo diferente de visualización. Si lo hace, es posible que cambien las opciones posteriores del menú.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Eje horizontal</td>
         <td><p>Seleccione los datos que desea representar a lo largo del eje horizontal o X de la visualización de columnas. La visualización compara los elementos de este eje según cada elemento del eje vertical.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Eje vertical</td>
         <td><p>En el menú desplegable de la izquierda, seleccione los datos que desee representar a lo largo del eje horizontal o Y. La visualización muestra los elementos de este eje como columnas comparativas, en función de sus valores.</p><p>En el menú desplegable de la derecha, seleccione cómo desea que se calculen esos valores en la visualización:</p>
          <ul>
           <li><p><b>Count</b>: El número de valores</p></li>
           <li><p><b>Sum</b>: El total de todos los valores </p></li>
           <li><p><b>Promedio</b>: El promedio de todos los valores</p></li>
           <li><p><b>Mínimo</b>: solo el valor más bajo</p></li>
           <li><p><b>Máximo</b>: Solo el valor más alto</p></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

   1. En la ficha **Datos**:

      | Fuente de datos (menú desplegable) | Cambie la fuente de datos para la visualización a otra tabla en el lienzo del informe. |
      |---|---|
      | Mostrar datos en Source | Active esta opción para mostrar la tabla de origen para la visualización en el lienzo del informe o desactive la opción para ocultarla. |

      {style="table-layout:auto"}

      <!--   
      NOLAN-FLAG: convert table to html. 
      -->

1. Haga clic en cualquier lugar fuera del menú de configuración de visualización para cerrarlo.
