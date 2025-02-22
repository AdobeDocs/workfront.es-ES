---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Añadir un gráfico a un informe
description: Puede mejorar los informes agregando un gráfico. Puede agregar gráficos a los informes existentes o a los informes que esté creando.
author: Nolan
feature: Reports and Dashboards
exl-id: 9b58d68c-4b7b-4344-bde3-7c65e2e1aac8
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '2747'
ht-degree: 3%

---

# Añadir un gráfico a un informe

<!--Audited: 11/2024-->

Puede mejorar los informes agregando un gráfico. Puede agregar gráficos a los informes existentes o a los informes que esté creando.

Antes de agregar un gráfico a un informe, debe crear una Vista y una Agrupación para el informe.

No puede agregar gráficos a la mayoría de los informes a menos que agrupe primero la información en el informe. El único gráfico que se puede agregar sin agrupar es un gráfico de medición.

Para obtener información acerca de las vistas, consulte [Información general sobre vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Para obtener más información sobre las agrupaciones, consulte [Información general sobre agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

Si el informe muestra demasiados elementos, no se creará ningún gráfico. En este caso, también debe agregar un Filtro al informe para reducir el número de resultados en el informe.

Para obtener más información sobre los filtros, vea [Resumen de filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> 
      <p>Nuevo:</p>
         <ul>
         <li><p>Estándar</p></li>
         </ul>
      <p>Actual:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuración de nivel de acceso</td> 
   <td> <p>Acceso de Edición a informes, paneles y calendarios</p> <p>Acceso de edición a filtros, vistas y agrupaciones</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Añadir un gráfico a un informe

1. Vaya a un informe existente o cree un nuevo informe. Para obtener más información sobre cómo crear un nuevo informe, vea [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. (Condicional) Si fue a un informe existente, haga clic en **Acciones de informe** > **Editar**.

1. Asegúrese de que la ficha **Columnas (Ver)** se ha actualizado para mostrar la información que desea incluir en el gráfico en el informe.

   Para obtener información sobre cómo crear o modificar la vista del informe, consulte [Crear o editar vistas en Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

1. Haga clic en la ficha **Agrupaciones** y agregue una agrupación.

   >[!TIP]
   >
   >* Solo se puede agregar un gráfico a un informe cuando los resultados del informe están agrupados.
   >* Los gráficos no admiten agrupaciones en modo de texto. Para obtener más información acerca de las agrupaciones en modo de texto, vea [Editar una agrupación mediante el modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md).
   >* Si agrega una sola agrupación que representa una métrica, todos los gráficos, excepto un gráfico circular, muestran cada resultado en la agrupación con el mismo color.

   Para obtener más información sobre cómo crear agrupaciones, consulte [Crear agrupaciones en Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-groupings.md).

1. Seleccione la ficha **Gráfico**.

1. Haga clic en un tipo de gráfico para seleccionarlo.\
   ![Selección del tipo de gráfico](assets/unshimmed-report-builder-chart.png)

1. Seleccione entre los siguientes tipos de gráficos:

   * [Gráfico de columnas](#column-chart)
   * [Gráfico de barras](#bar-chart)
   * [Gráfico circular](#pie-chart)
   * [Gráfico de líneas](#line-chart)
   * [Gráfico de medición](#gauge-chart)
   * [Gráfico de burbujas](#bubble-chart)

1. Haga clic en **Guardar + Cerrar** para guardar el gráfico y el informe.

### Gráfico de columnas {#column-chart}

Para agregar un gráfico de **columnas** al informe:

1. Empiece a agregar un gráfico al informe, tal como se describe en [Agregar un gráfico a un informe](#add-a-chart-to-a-report).

1. En el campo **Eje izquierdo (Y)**, seleccione los valores que desee incluir en el eje Y del gráfico y, a continuación, seleccione cómo desea que se resuma la información en el campo **Resumido por**.

1. (Opcional) Haga clic en **Colores personalizados** para asignar los colores preferidos a cada una de las columnas.\
   Para obtener más información acerca de cómo personalizar los colores del gráfico, vea [Personalizar colores del gráfico](#customize-chart-colors).

1. En el campo **Eje inferior (X)**, seleccione la agrupación que desee incluir en el gráfico.

1. (Opcional) Haga clic en **Mostrar en 3D** para mostrar el gráfico en una vista tridimensional.

1. (Opcional) **Columnas de grupo**: seleccione esta opción para definir cómo desea que se agrupen las columnas.\
   Seleccione entre las siguientes opciones:

   * Haga clic en una de las siguientes opciones para seleccionar cómo se van a mostrar las columnas agrupadas:

      * **Uno al lado del otro**
      * **Apiladas**
      * **Apiladas al 100%**

   * Seleccione la agrupación que desee incluir en el gráfico en el menú desplegable **Agrupar datos por**.
   * (Opcional) Haga clic en **Colores personalizados** para personalizar los colores de las columnas.\
     Para obtener más información acerca de cómo personalizar los colores del gráfico, vea [Personalizar colores del gráfico](#customize-chart-colors).

1. (Opcional) Haga clic en **Gráfico combinado** para incluir un valor adicional en el gráfico, así como la forma en que desea que se resuma la información.\
   Tenga en cuenta las siguientes opciones:

   * **Trazar en el eje secundario**: seleccione esta opción para trazar los datos en el lado derecho del gráfico.
   * **Tipo de gráfico**: seleccione si desea que este valor adicional se muestre como una línea o como una tercera columna.

1. Haga clic en **Guardar + Cerrar** para guardar el gráfico y el informe.

### Gráfico de barras {#bar-chart}

Para agregar un gráfico de **barras** al informe:

1. Empiece a agregar un gráfico al informe, tal como se describe en [Agregar un gráfico a un informe](#add-a-chart-to-a-report).

1. En el campo **Eje inferior (X)**, seleccione los valores que desee incluir en el eje X del gráfico y, a continuación, seleccione cómo desea que se resuma la información en el campo **Resumido por**.

1. (Opcional) Haga clic en **Colores personalizados** para personalizar los colores de las barras.\
   Para obtener más información acerca de cómo personalizar los colores del gráfico, vea [Personalizar colores del gráfico](#customize-chart-colors).

1. En el campo **Eje izquierdo (Y)**, seleccione la agrupación que desee incluir en el gráfico.

1. (Opcional) Haga clic en **Mostrar en 3D** para mostrar el gráfico en una vista tridimensional.

1. (Opcional) Haga clic en **Barras de grupo** para definir cómo desea que se agrupen las barras.\
   Seleccione entre las siguientes opciones:

   * Haga clic en una de las siguientes opciones para seleccionar cómo se van a mostrar las barras agrupadas:

      * **Uno al lado del otro**
      * **Apiladas**
      * **Apiladas al 100%**

   * Seleccione cómo desea agrupar la información del gráfico en el menú desplegable **Agrupar datos por**.
   * (Opcional) Haga clic en **Colores personalizados** para personalizar los colores de las columnas.\
     Para obtener más información acerca de cómo personalizar los colores del gráfico, vea [Personalizar colores del gráfico](#customize-chart-colors).

1. (Opcional) Haga clic en **Gráfico combinado** para incluir un valor adicional en el gráfico, así como la forma en que desea que se resuma la información.

1. Haga clic en **Guardar + Cerrar** para guardar el gráfico y el informe.

>[!IMPORTANT]
>
>Limite los gráficos de barras a 23 barras o menos, ya que los gráficos de barras que incluyen más de 23 barras no mostrarán correctamente todas las etiquetas de barras.

### Gráfico circular {#pie-chart}

Para agregar un gráfico **circular** al informe:

1. Empiece a agregar un gráfico al informe, tal como se describe en [Agregar un gráfico a un informe](#add-a-chart-to-a-report).

1. En el campo **Valores**, seleccione los valores que desea que se muestren en el informe y, a continuación, seleccione cómo desea que se resuma la información en el campo **Resumido por**.\
   En el campo **Cuñas**, seleccione la Agrupación que desee incluir en el gráfico. La agrupación se representa mediante las cuñas del gráfico.

1. (Opcional) Haga clic en **Colores personalizados** para personalizar los colores de las cuñas del gráfico.\
   Para obtener más información acerca de cómo personalizar los colores del gráfico, vea [Personalizar colores del gráfico](#customize-chart-colors).

1. (Opcional) Haga clic en **Mostrar en 3D** para mostrar el gráfico en una vista tridimensional.

1. En el campo **Mostrar resultados como**, seleccione cómo desea que se muestren los resultados en el gráfico. Tenga en cuenta las siguientes opciones:

   * **Porcentaje**: los resultados del gráfico se muestran como un porcentaje.
   * **Números**: los resultados del gráfico se muestran como un número.

1. Haga clic en **Guardar + Cerrar** para guardar el gráfico y el informe.

### Gráfico de líneas {#line-chart}

Para agregar un gráfico de **Líneas** al informe:

1. Empiece a agregar un gráfico al informe, tal como se describe en [Agregar un gráfico a un informe](#add-a-chart-to-a-report).

1. En el campo **Eje izquierdo (Y)**, seleccione los valores que desee incluir en el eje Y del gráfico y, a continuación, seleccione cómo desea que se resuma la información en el campo **Resumido por**.

1. En el campo **Eje inferior (X)**, seleccione la agrupación que desee incluir en el gráfico.

1. (Opcional) Haga clic en **Líneas de grupo** para seleccionar una agrupación adicional para el gráfico.\
   (Opcional) Haga clic en **Colores personalizados** para personalizar los colores de la nueva agrupación.\
   Para obtener más información acerca de cómo personalizar los colores del gráfico, vea [Personalizar colores del gráfico](#customize-chart-colors).

1. (Opcional) Haga clic en **Gráfico combinado** para combinar las líneas por un valor adicional.\
   Considere las siguientes opciones:

   * Seleccione el valor que desea incluir en el gráfico, así como la forma en que desea resumir la información.
   * Haga clic en el campo **Trazar en el eje secundario** para trazar los datos en el lado derecho del gráfico.

1. Haga clic en **Guardar + Cerrar** para guardar el gráfico y el informe.

### Gráfico de medición {#gauge-chart}

Un gráfico de **Medición** muestra el número de registros que cumplen ciertos criterios en un formato de medición. El indicador de la medición señala al número de registros que cumplen los criterios seleccionados en la vista y la agrupación del informe. No se requiere una agrupación de informes para configurar un gráfico de medición.

Para agregar un gráfico de **Medición** a tu informe:

1. Empiece a agregar un gráfico al informe, tal como se describe en [Agregar un gráfico a un informe](#add-a-chart-to-a-report).

1. En el campo **Valores**, seleccione los valores que desea que se muestren en el informe y, a continuación, seleccione cómo desea que se resuma la información en el campo **Resumido por**. Si selecciona **Número de registros**, los valores mostrados son el objeto del informe.

1. En el campo **Indicadores**, seleccione la agrupación que desee incluir en el gráfico. La agrupación se representa mediante la línea indicadora del gráfico.\
   Si tiene una agrupación que contiene dos elementos, en el gráfico se muestran dos indicadores.\
   Por ejemplo, si tiene una Agrupación de estados de proyecto y hay dos estados de proyecto (Actual y En espera), el gráfico Medición contiene dos indicadores. Ellos indicarán el número de proyectos que se encuentran en ese estado.\
   (Opcional) Seleccione **Total** en el campo **Indicadores** para mostrar el total de objetos seleccionados en el campo **Valores**.

1. (Opcional) Haga clic en **Agregar otro intervalo de valores** para agregar un intervalo de valores al gráfico.

1. (Opcional) En el campo **Rango de valores**, especifique el rango de valores y el color para representar esos valores que se mostrarán en el gráfico Medición.

1. Haga clic en **Guardar + Cerrar** para guardar el gráfico y el informe.

### Gráfico de burbujas {#bubble-chart}

Puede mostrar hasta tres campos de un objeto en un gráfico de **burbujas**. Esto significa que se pueden mostrar hasta cuatro puntos de datos en un gráfico de burbujas. Cada entidad con tres campos asociados se muestra como un círculo que expresa dos de los campos dentro de su ubicación dentro de los ejes X e Y. El tercer campo se representa mediante el tamaño del círculo.

Para agregar un gráfico de **burbujas** al informe:

1. Empiece a agregar un gráfico al informe, tal como se describe en [Agregar un gráfico a un informe](#add-a-chart-to-a-report).

1. En el campo **Eje izquierdo (Y)**, seleccione los valores que desee incluir en el eje Y del gráfico. Los valores provienen de la vista del informe. Especifique cómo desea que se resuma la información en el campo **Resumido por**.

1. En el campo **Eje inferior (X)**, seleccione los valores que desee incluir en el eje X del gráfico. Los valores provienen de la vista del informe. Especifique cómo desea resumir la información.

   >[!NOTE]
   >
   >Asegúrese de tener al menos una columna resumida para que este campo esté activo.\
   >Para obtener más información sobre cómo resumir la información en una columna de informe, vea [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. En el campo **Tamaño de burbuja**, seleccione los valores que desee representar por el tamaño de las burbujas en el gráfico. Los valores provienen de la vista del informe. Especifique cómo desea resumir la información.

   >[!NOTE]
   >
   >Asegúrese de tener al menos una columna resumida para que este campo esté activo.\
   >Para obtener más información sobre cómo resumir la información en una columna de informe, vea [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. En el campo **Burbujas**, seleccione la agrupación que desee incluir en el gráfico. La agrupación se representa mediante la colocación de las burbujas en el gráfico.

1. En el campo **Color de burbuja**, seleccione el campo que desee que se represente con los colores de las burbujas.

   El **Color de burbuja** puede ser una Agrupación que usted defina en el informe, pero la opción solo está disponible si elige una Agrupación en el campo **Burbujas** que contenga el **Nombre** de un objeto principal relativo al objeto del informe, como **Nombre del proyecto** para un informe de tareas o **Nombre del programa** para un informe de proyecto.

   Por ejemplo, si seleccionó **Nombre del proyecto** en un informe de tareas, puede agregar **Estado de la tarea** como el campo **Color de burbuja**.

   ![Estado de la tarea como color de burbuja](assets/bubbles-field-correct-can-select-bubbles-color-example.png)

   Sin embargo, si seleccionó **Estado de la tarea** para el campo **Burbujas**, no podrá seleccionar un campo de **Color de burbuja**. Tampoco puede seleccionar **Nombre de proyecto** para el campo **Color de burbuja**, aunque seleccione **Nombre de proyecto** para el campo **Burbujas**.

   ![No se puede seleccionar el color de burbuja](assets/bubbles-field-wrong-cannot-select-bubbles-color-example.png)

1. Haga clic en **Guardar + Cerrar** para guardar los cambios en el generador de interfaces.

## Personalizar colores del gráfico {#customize-chart-colors}

Puede permitir que Workfront seleccione los colores de los elementos del gráfico o puede personalizarlos mientras agrega un gráfico a los informes. Si el gráfico contiene una sola Agrupación que representa una métrica, como un informe de tareas que muestra el número de tareas agrupadas por Fecha real de finalización, cada resultado de la Agrupación se muestra en el mismo color.

Solo puede elegir un color para los campos que se muestran en la vista del informe. Puede elegir varios colores, uno para cada opción, para los campos mostrados en la agrupación del informe.

>[!IMPORTANT]
>
>Para los campos de fecha, solo puede seleccionar un color para los elementos del gráfico.

Para personalizar los colores del gráfico:

1. Al crear un informe, ve a la pestaña **Gráfico** en Report Builder.

1. Seleccione un tipo de gráfico para agregarlo al informe.\
   Para obtener más información sobre cómo agregar un gráfico al informe, consulte [Agregar un gráfico a un informe](#add-a-chart-to-a-report).

1. Haga clic en **Colores personalizados** cuando este campo esté disponible.\
   Aparece el cuadro de diálogo Colores personalizados.\
   ![Colores personalizados en gráficos](assets/unshimmed-custom-colors-in-charts.png)

   >[!NOTE]
   >
   >Puede asociar colores personalizados a cualquier campo que pueda agrupar y con algunos campos que se pueden mostrar en una vista, incluidos los campos personalizados. Los campos personalizados o las opciones personalizadas de los campos que elija en el cuadro de diálogo Color personalizado distinguen entre mayúsculas y minúsculas.

1. Considere la posibilidad de seleccionar cualquiera de las siguientes opciones:

   * **Usar un color**: todos los elementos del gráfico se mostrarán en el color seleccionado.
   * **Agregar color**: agregue un color personalizado para un posible valor del campo seleccionado.
   * **Quitar todos**: seleccione esta opción para quitar todos los valores de campo y colores especificados anteriormente.
   * **Sin valor**: seleccione este campo y un color personalizado para mostrar la columna del gráfico que agrupa los elementos &quot;sin valor&quot;. Son elementos que no se pueden agrupar por ninguna de las opciones del campo seleccionado en la agrupación.
   * **Todos los demás valores**: seleccione este campo y un color personalizado para mostrar todos los demás elementos de gráfico cuyas opciones no estén definidas anteriormente.

     >[!NOTE]
     >
     >Los colores que ha editado más recientemente se muestran a la derecha del botón **Colores personalizados**. Cuando pasa el ratón sobre un color, se muestra el nombre del campo asociado a él. También puede hacer clic en un color para editarlo sin volver a abrir **Colores personalizados**.

1. Para elegir un color:
Haga clic dentro del selector de color para seleccionar un color.
O
Especifique un valor hexadecimal del color.

1. Haga clic en cualquier lugar fuera del cuadro de diálogo Colores personalizados para cerrarlo. Los colores que ha seleccionado se guardan automáticamente.

1. Haga clic en **Guardar + Cerrar** para guardar el gráfico y ejecutar el informe.

## Exportar un gráfico

Puede exportar un gráfico a un archivo .pdf.

Para exportar un gráfico:

1. En la ficha Gráfico de un informe, haga clic en **Exportar** para exportar el gráfico a .pdf.\
   Se descargará un archivo .pdf en el equipo.

1. Abra el archivo .pdf.\
   El archivo exportado incluye la siguiente información:

   * Una imagen del gráfico.
   * Un título que es el nombre del informe.
   * Un nombre de archivo único que se basa en el nombre del informe.
   * Pie de página con la fecha y hora de exportación del informe y el número de página.

## Eliminación de un gráfico de un informe

Para eliminar un gráfico de un informe:

1. Abra la ficha **Gráfico** de Report Builder.

1. Haga clic en el botón &quot;x&quot; a la derecha de los tipos de gráficos para eliminar el gráfico.

1. Haga clic en **Guardar + Cerrar**.

## Limitaciones al trabajar con gráficos

Tenga en cuenta las siguientes limitaciones al trabajar con gráficos:

* La sección **Vista previa de gráfico** a la derecha de Report Builder no contiene datos reales de su informe. Debe guardar el gráfico y verlo desde la ficha **Gráfico** para poder verlo con sus datos.

* Algunos elementos del gráfico no se pueden editar:

   * No se puede cambiar el tipo de fuente ni el tamaño de los valores de cada elemento.
   * No puede cambiar los nombres de los ejes en el gráfico.

* No se puede editar el pie de ilustración del gráfico.
* Al utilizar campos calculados para las agrupaciones, no se puede hacer clic en los elementos del gráfico.
* La mayor cantidad de puntos de datos que se pueden mostrar en un gráfico es de cuatro, en un gráfico de burbujas. Todos los demás tipos de gráficos muestran dos puntos de datos o un máximo de tres.
