---
title: Configurar una visualización de barras en el lienzo de informes
description: Configurar una visualización de barras en el lienzo de informes
hidefromtoc: true
hide: true
exl-id: 7dc4f156-d262-482f-aa82-c905f0d1b20f
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 43%

---

# Configurar una visualización de barras en el lienzo de informes

Una visualización de barras puede ayudarle a contar rápidamente una historia sobre los datos resaltando información importante mediante barras horizontales.

## Requisitos previos

Antes de empezar, debe inscribirse en la versión beta del lienzo del sistema de informes. Para obtener más información, consulte la [Versión beta del lienzo del sistema de informes: descripción general](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Configuración de una visualización de barras

>[!NOTE]
>
>Todos los cambios se guardan automáticamente al crear y editar los bloques del informe.

1. Comience agregando un bloque de visualización con el tipo de visualización **Bar** a un informe, como se explica en [Agregar o editar un bloque de visualización en el lienzo de informes](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md).

1. Haga clic en el icono Editar visualización ![Editar icono](assets/edit-icon.png) en la esquina superior derecha de la visualización y, a continuación, realice una de las siguientes acciones.

   1. En la pestaña **Configuración**, haga lo siguiente:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Tipo de visualización</td>
         <td><p>Cambie a un tipo diferente de visualización. Si lo hace, es posible que cambien las opciones posteriores del menú.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Eje vertical</td>
         <td><p>Seleccione los datos que desea representar a lo largo del borde izquierdo vertical o del eje Y de la visualización de barras. La visualización compara los elementos de este eje según cada elemento del eje horizontal.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Eje horizontal</td>
         <td><p>En el menú desplegable de la izquierda, seleccione los datos que desee representar a lo largo del eje horizontal o X. Los elementos de este eje se muestran como barras comparativas, según sus valores.</p><p>En el menú desplegable de la derecha, seleccione cómo desea que la visualización calcule y muestre los valores a lo largo del eje horizontal:</p>
          <ul>
           <li><p><b>Count</b>: el número de valores</p></li>
           <li><p><b>Sum</b>: el total de todos los valores </p></li>
           <li><p><b>Average</b>: el promedio de todos los valores</p></li>
           <li><p><b>Minimum</b>: solo el valor más bajo</p></li>
           <li><p><b>Maximum</b>: solo el valor más alto</p></li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">+ Agregar valor</td>
         <td>Agregue otro campo que desee rastrear a lo largo del eje horizontal.</td>
        </tr>
       </tbody>
      </table>

   1. En la pestaña **Datos**:

      | Fuente de datos (menú desplegable) | Cambie la fuente de datos para visualizar otra tabla en el lienzo del informe. |
      |---|---|
      | Mostrar la fuente de datos | Active esta opción para mostrar la tabla de origen para la visualización en el lienzo del informe o desactive la opción para ocultarla. |

      {style="table-layout:auto"}

      <!--   
      NOLAN-FLAG: convert table to html. 
      -->

1. Haga clic en cualquier lugar fuera del menú de configuración de visualización para cerrarla.
