---
title: Configuración de una visualización de barras en el lienzo de informes
description: Configuración de una visualización de barras en el lienzo de informes
author: Nolan
feature: Reports and Dashboards
exl-id: 7dc4f156-d262-482f-aa82-c905f0d1b20f
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 3%

---


# Configuración de una visualización de barras en el lienzo de informes

Una visualización de barras puede ayudarle a contar rápidamente una historia sobre sus datos al resaltar información importante mediante barras horizontales.

## Requisitos previos

Antes de comenzar, debe inscribirse en la versión beta del lienzo de informes. Para obtener más información, consulte [Reporting Canvas beta: información general](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## Configuración de una visualización de barras

>[!NOTE]
>
>Todos los cambios se guardan automáticamente a medida que crea y edita los bloques en el informe.

1. Comience agregando un bloque de visualización con la variable **Barra** tipo de visualización de un informe, tal como se explica en [Añadir o editar un bloque de visualización en el Lienzo de informes](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md).

1. Haga clic en el icono Editar visualización . ![](assets/edit-icon.png) en la esquina superior derecha de la visualización, realice una de las acciones siguientes.

   1. En el **Configuración** pestaña:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Tipo de visualización</td>
         <td><p>Cambie a un tipo de visualización diferente. Si lo hace, las siguientes opciones del menú podrían cambiar.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Eje vertical</td>
         <td><p>Seleccione los datos que desea representar a lo largo del borde izquierdo vertical o el eje Y de la visualización de barras. La visualización compara los elementos de este eje según cada elemento del eje horizontal.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Eje horizontal</td>
         <td><p>En el menú desplegable de la izquierda, seleccione los datos que desee representar a lo largo del eje horizontal o X. Los elementos de este eje se muestran como barras comparativas, en función de sus valores.</p><p>En el menú desplegable derecho, seleccione cómo desea que la visualización calcule y muestre los valores a lo largo del eje horizontal:</p>
          <ul>
           <li><p><b>Recuento</b>: El número de valores</p></li>
           <li><p><b>Sum</b>: El total de todos los valores </p></li>
           <li><p><b>Promedio</b>: El promedio de todos los valores</p></li>
           <li><p><b>Mínimo</b>: solo el valor más bajo</p></li>
           <li><p><b>Máximo</b>: Solo el valor más alto</p></li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">+ Agregar valor</td>
         <td>Agregue otro campo que desee rastrear a lo largo del eje horizontal.</td>
        </tr>
       </tbody>
      </table>

   1. En el **Datos** pestaña:

      | Fuente de datos (menú desplegable) | Cambie la fuente de datos para la visualización a otra tabla del lienzo del informe. |
      |---|---|
      | Mostrar fuente de datos | Active esta opción para mostrar la tabla de origen de la visualización en el lienzo del informe o desactive la opción para ocultarla. |

      {style=&quot;table-layout:auto&quot;}

      <!--   
      NOLAN-FLAG: convert table to html. 
      -->

1. Haga clic en cualquier lugar fuera del menú de configuración de visualización para cerrarlo.
