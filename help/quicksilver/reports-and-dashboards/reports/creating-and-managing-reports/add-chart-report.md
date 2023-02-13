---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Agregar un gráfico a un informe
description: Puede mejorar los informes agregando un gráfico. Puede agregar gráficos a informes existentes o a informes que esté creando.
author: Nolan
feature: Reports and Dashboards
exl-id: 9b58d68c-4b7b-4344-bde3-7c65e2e1aac8
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '2710'
ht-degree: 0%

---

# Agregar un gráfico a un informe

Puede mejorar los informes agregando un gráfico. Puede agregar gráficos a informes existentes o a informes que esté creando.

Antes de agregar un gráfico a un informe, debe crear una vista y un grupo para el informe. La mayoría de los gráficos no se pueden agregar a menos que la información se agrupe en el informe. El único gráfico que se puede agregar sin agrupar es un gráfico de medición.\
Para obtener información sobre cómo crear una vista, consulte [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).\
Para obtener más información sobre las agrupaciones, consulte [Información general sobre las agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

Si el informe muestra demasiados elementos, no se crea un gráfico. En este caso, también debe agregar un Filtro al informe para reducir la cantidad de resultados en el informe.\
Para obtener más información sobre los filtros, consulte [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y grupos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Agregar un gráfico a un informe

1. Vaya a un informe existente o cree un nuevo informe. Para obtener más información sobre la creación de un nuevo informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. (Condicional) Si ha ido a un informe existente, haga clic en **Acciones de informe** > **Editar**.

1. Asegúrese de que la variable **Columnas (Vista)** se ha actualizado para satisfacer las necesidades del informe.\
   Para obtener información sobre cómo crear o modificar la vista del informe, consulte [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Haga clic en el **Agrupaciones** y añada una agrupación.

   >[!TIP]
   >
   >* Solo se puede añadir un gráfico a un informe cuando se agrupan los resultados del informe.
   >* Las agrupaciones en modo texto no son compatibles con los gráficos. Para obtener más información sobre las agrupaciones en modo texto, consulte [Editar el modo de texto en una agrupación](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md).
   >* Si agrega una sola agrupación que represente una métrica, todos los gráficos excepto un gráfico circular mostrarán cada resultado en la agrupación con el mismo color.


   Para obtener más información sobre las agrupaciones, consulte [Información general sobre las agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Seleccione el **Gráfico** pestaña .
1. Haga clic en un tipo de gráfico para seleccionarlo.\
   ![](assets/qs-report-builder-chart-350x265.png)

1. Puede agregar los siguientes tipos de gráficos a un informe de Adobe Workfront:

   * [Gráfico de columnas](#column-chart)
   * [Gráfico de barras](#bar-chart)
   * [Gráfico circular](#pie-chart)
   * [Gráfico de líneas](#line-chart)
   * [Gráfico de medición](#gauge-chart)
   * [Gráfico de burbujas](#bubble-chart)

1. Haga clic en **Guardar + Cerrar** para guardar el gráfico y el informe.

### Gráfico de columnas {#column-chart}

Para agregar un **Columna** para el informe:

1. Comience a agregar un gráfico al informe, tal como se describe en [Agregar un gráfico a un informe](#add-a-chart-to-a-report).
1. En el **Eje izquierdo (Y)** , seleccione los valores que desea incluir en el eje Y del gráfico, así como la forma en que desea que se resume la información.
1. En el **Eje inferior (X)** , seleccione el grupo que desee incluir en el gráfico.
1. (Opcional) Seleccione **Colores personalizados** para asignar los colores preferidos a cada una de las columnas.\
   Para obtener más información sobre la personalización de colores de gráficos, consulte [Personalizar colores de gráficos](#customize-chart-colors).

1. (Opcional) Seleccione **Mostrar en 3D** para mostrar el gráfico en una vista tridimensional.
1. (Opcional) **Agrupar columnas**: Seleccione esta opción para definir cómo desea que se agrupen las columnas.\
   Seleccione entre las siguientes opciones:

   * Haga clic en una de las siguientes opciones para seleccionar cómo se van a mostrar las columnas agrupadas:\
      **- Lado a lado**

      **- Apiladas**
      **- Apiladas al 100%**

   * Seleccione el grupo que desee incluir en el gráfico.
   * (Opcional) Seleccione **Colores personalizados** para personalizar los colores de las columnas.\
      Para obtener más información sobre la personalización de colores de gráficos, consulte [Personalizar colores de gráficos](#customize-chart-colors).

1. (Opcional) Seleccione **Gráfico de combinación** para incluir un valor adicional en el gráfico, así como cómo desea que se resuma la información.\
   Tenga en cuenta las siguientes opciones:

   * **Diagrama de eje secundario**: Seleccione esta opción para trazar los datos en el lado derecho del gráfico.
   * **Tipo de gráfico**: Seleccione si desea que este valor adicional se muestre como una línea o como una tercera columna.\
      ![](assets/qs-column-chart-350x163.png)

1. Haga clic en **Guardar + Cerrar** para guardar el gráfico y el informe.

### Gráfico de barras {#bar-chart}

Para agregar un **Barra** para el informe:

1. Comience a agregar un gráfico al informe, tal como se describe en [Agregar un gráfico a un informe](#add-a-chart-to-a-report).
1. En el **Eje inferior (X)** , seleccione los valores que desea incluir en el eje X del gráfico, así como la forma en que desea que se resume la información.
1. En el **Eje izquierdo (Y)** , seleccione el grupo que desee incluir en el gráfico.
1. (Opcional) Seleccione **Colores personalizados** para personalizar los colores de las barras.\
   Para obtener más información sobre la personalización de colores de gráficos, consulte [Personalizar colores de gráficos](#customize-chart-colors).

1. (Opcional) Seleccione **Mostrar en 3D** para mostrar el gráfico en una vista tridimensional.
1. (Opcional)**Barras de grupo**: Seleccione esta opción para definir cómo desea que se agrupen las barras.\
   Seleccione entre las siguientes opciones:

   * Haga clic en una de las siguientes opciones para seleccionar cómo se mostrarán las barras agrupadas:\
      **- Lado a lado**

      **- Apiladas**
      **- Apiladas al 100%**

   * Seleccione el grupo que desee incluir en el gráfico.
   * (Opcional) Seleccione **Colores personalizados** para personalizar los colores de las columnas.\
      Para obtener más información sobre la personalización de colores de gráficos, consulte [Personalizar colores de gráficos](#customize-chart-colors).

1. (Opcional) Seleccione **Gráfico de combinación** para incluir un valor adicional en el gráfico, así como cómo desea que se resuma la información.\
   ![](assets/qs-bar-chart-350x167.png)

1. Haga clic en **Guardar + Cerrar** para guardar el gráfico y el informe.

### Gráfico circular {#pie-chart}

Para agregar un **Circular** para el informe:

1. Comience a agregar un gráfico al informe, tal como se describe en [Agregar un gráfico a un informe](#add-a-chart-to-a-report).
1. En el **Valores** , seleccione los valores que desea que se muestren en el informe y cómo desea que se resuman.\
   En el **Bodas** , seleccione el grupo que desee incluir en el gráfico. El Grouping está representado por las cuñas del gráfico.

1. (Opcional) Seleccione **Colores personalizados** para personalizar los colores de las cuñas del gráfico.\
   Para obtener más información sobre la personalización de colores de gráficos, consulte [Personalizar colores de gráficos](#customize-chart-colors).

1. (Opcional) Seleccione **Mostrar en 3D** para mostrar el gráfico en una vista tridimensional.
1. En el **Mostrar resultados como** , seleccione cómo desea que se muestren los resultados en el gráfico. Tenga en cuenta las siguientes opciones:

   * **Porcentaje**: Los resultados del gráfico se muestran como un porcentaje.
   * **Números**: Los resultados del gráfico se muestran como un número.\
      ![](assets/qs-pie-chart-350x171.png)

1. Haga clic en **Guardar + Cerrar** para guardar el gráfico y el informe.

### Gráfico de líneas {#line-chart}

Para agregar un **Línea** para el informe:

1. Comience a agregar un gráfico al informe, tal como se describe en [Agregar un gráfico a un informe](#add-a-chart-to-a-report).
1. En el **Eje izquierdo (Y)** , seleccione los valores que desea incluir en el eje Y del gráfico, así como la forma en que desea que se resume la información.
1. En el **Eje inferior (X)** , seleccione el grupo que desee incluir en el gráfico.
1. (Opcional) Seleccione un color para personalizar el color de la línea.
1. (Opcional) Seleccione **Líneas de grupo**, para seleccionar una agrupación adicional para el gráfico.\
   (Opcional) Seleccione **Colores personalizados** para personalizar los colores de la nueva agrupación.\
   Para obtener más información sobre la personalización de colores de gráficos, consulte [Personalizar colores de gráficos](#customize-chart-colors).

1. (Opcional) Seleccione **Gráfico de combinación** para combinar las líneas con un valor adicional.\
   Tenga en cuenta las siguientes opciones:

   * Seleccione el valor que desea incluir en el gráfico, así como cómo desea que se resuma la información.
   * Seleccione el **Diagrama de eje secundario** para representar los datos en el lado derecho del gráfico.\
      ![](assets/qs-line-chart-350x172.png)

1. Haga clic en **Guardar + Cerrar** para guardar el gráfico y el informe.

### Gráfico de medición {#gauge-chart}

A **Medición** muestra el número de registros que cumplen determinados criterios en formato de medición. El indicador de la medición señala al número de registros que cumplen los criterios seleccionados en la vista y la agrupación del informe. No es necesario agrupar los informes para configurar un gráfico de medición.

Para agregar un **Medición** para el informe:

1. Comience a agregar un gráfico al informe, tal como se describe en [Agregar un gráfico a un informe](#add-a-chart-to-a-report).
1. En el **Valores** , seleccione los valores que desea que se muestren en el informe y cómo desea que se resuman. Si selecciona **Recuento de registros**, los valores mostrados son el objeto del informe.

1. En el **Indicadores** , seleccione el grupo que desee incluir en el gráfico. El grupo se representa mediante la línea del indicador del gráfico.\
   Si tiene un Grouping que contiene dos elementos, se muestran dos indicadores en el gráfico.\
   Por ejemplo, si tiene una Agrupación de estado del proyecto y hay dos estados de proyecto (Actual y En espera), el gráfico Medición contiene dos indicadores. Señalarán el número de proyectos que están en ese estado.\
   (Opcional) Seleccione **Total** en el **Indicadores** para mostrar el total de los objetos seleccionados en la variable **Valores** campo .

1. En el **Rango de valores** especifique el rango de valores y el color que representa los valores que se mostrarán en el gráfico Medición.
1. (Opcional) Haga clic en **Añadir otro rango de valores** para agregar rangos de valores adicionales al gráfico.\
   ![](assets/qs-gauge-chart-350x181.png)

1. Haga clic en **Guardar + Cerrar** para guardar el gráfico y el informe.

### Gráfico de burbujas {#bubble-chart}

Puede mostrar hasta tres campos de un objeto en un **Burbujas** gráfico. Esto significa que puede mostrar hasta cuatro puntos de datos en un gráfico de burbujas. Cada entidad con tres campos asociados se muestra como un círculo que expresa dos de los campos dentro de su ubicación dentro de los ejes X e Y. El tercer campo se representa por el tamaño del círculo.

Para agregar un **Burbujas** para el informe:

1. Comience a agregar un gráfico al informe, tal como se describe en [Agregar un gráfico a un informe](#add-a-chart-to-a-report).
1. En el **Eje izquierdo (Y)** , seleccione los valores que desea incluir en el eje Y del gráfico. Los valores proceden de la vista del informe. Especifique cómo desea que se resume la información.
1. En el **Campo de eje inferior (X)**, seleccione los valores que desee incluir en el eje X del gráfico. Los valores proceden de la vista del informe. Especifique cómo desea que se resume la información.

   >[!NOTE]
   >
   >Asegúrese de que tiene al menos una columna que se resume para que este campo esté activo.\
   >Para obtener más información sobre cómo resumir la información en una columna de informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. En el **Tamaño de burbuja** , seleccione los valores que desee representar según el tamaño de las burbujas del gráfico. Los valores proceden de la vista del informe. Especifique cómo desea que se resume la información.

   >[!NOTE]
   >
   >Asegúrese de que tiene al menos una columna que se resume para que este campo esté activo.\
   >Para obtener más información sobre cómo resumir la información en una columna de informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. En el **Burbujas** , seleccione el grupo que desee incluir en el gráfico. La agrupación se representa colocando las burbujas en el gráfico.
1. En el **Color de burbuja** , seleccione el campo que desea que se represente con los colores de las burbujas. La variable **Color de burbuja** puede ser un grupo definido en el informe, pero solo pueden ser campos del objeto seleccionado como **Burbujas**. Por ejemplo, si seleccionó Nombre de tarea, puede agregar Estado de tarea, pero no Estado del proyecto como **Color de burbuja**.\
   ![](assets/qs-bubble-chart-350x103.png)

1. Haga clic en **Guardar + Cerrar** para guardar los cambios en el generador de interfaces.

## Exportación de un gráfico

Puede exportar un gráfico a un archivo .pdf.

Para exportar un gráfico:

1. Haga clic en **Exportar** para exportar el gráfico a .pdf.\
   Se descarga un archivo .pdf en el equipo.

1. Abra el archivo .pdf .\
   El archivo exportado incluye la siguiente información:

   * Imagen del gráfico.
   * Un título que es el nombre del informe.
   * Un nombre de archivo único que es el nombre del informe.
   * Un pie de página con la fecha y hora en que se exportó el informe y el número de página.

## Personalizar colores de gráficos {#customize-chart-colors}

Puede permitir que Workfront seleccione los colores de los elementos del gráfico o personalizarlos mientras agrega un gráfico a los informes. Si el gráfico contiene un único grupo que representa una métrica (por ejemplo, un informe de tareas que muestra la cantidad de tareas agrupadas por fecha de finalización real), cada resultado en el grupo se muestra en el mismo color.

Solo se puede elegir un color para los campos mostrados en la Vista del informe. Puede elegir varios colores (uno para cada opción) para los campos mostrados en la Agrupación del informe.

>[!IMPORTANT]
>
>Para los campos de fecha, solo puede seleccionar un color para los elementos de gráfico.

Para personalizar los colores de los gráficos:

1. Mientras crea un informe, vaya a la **Gráfico** en el Creador de informes.
1. Seleccione un tipo de gráfico para agregarlo al informe.\
   Para obtener más información sobre cómo agregar un gráfico al informe, consulte [Agregar un gráfico a un informe](#add-a-chart-to-a-report).

1. Haga clic en **Colores personalizados** cuando este campo esté disponible.\
   Aparece el cuadro de diálogo Colores personalizados .\
   ![](assets/custom-colors-in-charts-350x286.png)

   >[!NOTE]
   >
   >Puede asociar colores personalizados con cualquier campo que pueda agrupar por y con algunos campos que se pueden mostrar en una vista, incluidos los campos personalizados. Los campos personalizados o las opciones personalizadas de los campos que elija en el cuadro de diálogo Color personalizado distinguen entre mayúsculas y minúsculas.

1. Considere la posibilidad de seleccionar cualquiera de las siguientes opciones:

   * **Utilizar un color**: Todos los elementos del gráfico se mostrarán en el color seleccionado.

      1. Comience a escribir el nombre de una opción del campo seleccionado y, a continuación, seleccione un color. Esta opción se muestra en el color seleccionado del gráfico.
      1. (Opcional) Especifique un valor de color hexadecimal para el color, en lugar de seleccionar uno de los ejemplos de color disponibles\
         O\
         Haga clic en el selector de color que aparece después de hacer clic en el código hexadecimal y seleccione otro color.
   * **Agregar color**: Continúe agregando colores personalizados para todas las demás opciones posibles del campo seleccionado.
   * **Eliminar todo**: Seleccione esta opción para eliminar todos los colores y opciones del campo seleccionado arriba.
   * **Opciones avanzadas**: Seleccione entre las siguientes opciones:

      * **Sin valor**: Seleccione este campo y un color personalizado para mostrar la columna del gráfico que agrupa los elementos &quot;sin valor&quot;. Son elementos que no se pueden agrupar por ninguna de las opciones del campo seleccionado en la agrupación.
      * **Todos los demás valores**: Seleccione este campo y un color personalizado para mostrar todos los demás elementos del gráfico cuyas opciones no están seleccionadas anteriormente.

         >[!NOTE]
         >
         >Los colores que ha utilizado recientemente se muestran en la parte superior del cuadro de diálogo Colores personalizados . Cuando pase el ratón sobre un color que se haya utilizado recientemente, se mostrará el nombre del campo asociado a él.


1. Haga clic en la &quot;x&quot; en la esquina superior derecha de los colores personalizados para cerrar el cuadro de diálogo Colores personalizados . Los colores seleccionados se guardan automáticamente.
1. Haga clic en **Guardar + Cerrar** para guardar el gráfico y ejecutar el informe.

## Eliminación de un gráfico de un informe

Para quitar un gráfico de un informe:

1. Abra el **Gráfico** del creador de informes.
1. Pase el ratón sobre el icono del tipo de gráfico que ha elegido y aparecerá un botón &quot;x&quot; en la esquina superior derecha del icono.
1. Haga clic en la &quot;x&quot; para quitar el gráfico.
1. Haga clic en **Guardar + Cerrar**.

## Limitaciones mientras se trabaja con gráficos

Tenga en cuenta las siguientes limitaciones mientras trabaja con gráficos:

* La variable **Vista previa del gráfico** a la derecha del creador de informes no contiene datos reales del informe. Debe guardar el gráfico y verlo desde el **Gráfico** para ver el gráfico con los datos.

* Algunos elementos de gráfico no se pueden editar:

   * No se puede cambiar el tipo de fuente ni el tamaño de los valores de cada elemento.
   * No se pueden cambiar los nombres de los ejes en el gráfico.

* No se puede editar el pie de ilustración del gráfico.
* Al utilizar campos calculados para las agrupaciones, no se puede hacer clic en los elementos de gráfico.
* La mayor cantidad de puntos de datos que se pueden mostrar en un gráfico es de cuatro, en un gráfico de burbujas. Todos los demás tipos de gráficos muestran dos o un máximo de tres puntos de datos.
