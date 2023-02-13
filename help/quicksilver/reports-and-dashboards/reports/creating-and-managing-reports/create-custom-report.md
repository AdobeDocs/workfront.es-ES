---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Crear un informe personalizado
description: El modo de crear informes le ayuda a proporcionar acceso a la información que su organización necesita en Adobe Workfront. Puede utilizar cualquiera de los informes integrados disponibles en Workfront o crear sus propios informes desde cero.
author: Nolan
feature: Reports and Dashboards
exl-id: 10c4df37-f09f-4b91-9cfd-3d0c3835bc7b
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '1821'
ht-degree: 1%

---


# Crear un informe personalizado

El modo de crear informes le ayuda a proporcionar acceso a la información que su organización necesita en Adobe Workfront. Puede utilizar cualquiera de los informes integrados disponibles en Workfront o crear sus propios informes desde cero.

Para obtener más información sobre los informes integrados, consulte [Uso de los informes integrados de Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md). Para obtener información sobre la creación de un informe copiándolo, consulte [Creación de una copia de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

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
   <td> <p>Obtendrá permisos de administración para el informe que cree</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Crear un informe {#create-a-report}

Para ver un vídeo sobre cómo crear un informe, consulte esta [Crear un informe personalizado](#Walk-thr) más abajo.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha, haga clic en **Informes**.
1. Haga clic en **Nuevo informe** y, a continuación, seleccione el tipo de objeto que desee para el informe.

   Se carga el Creador de informes.

   Para obtener información específica sobre los informes de objeto disponibles, consulte la sección [Informar sobre objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) en el artículo [Explicación de los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   ![](assets/nwe-select-new-report-350x666.png)

   >[!TIP]
   >
   >También puede crear un informe haciendo una copia de un informe existente. Para obtener más información, consulte [Creación de una copia de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. En el Creador de informes, agregue lo siguiente al informe:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Función</th> 
      <th>Descripción</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>Columnas (vista)</td> 
      <td> <p>Añadir columnas al informe determina la información que contiene el informe.</p> <p>Para obtener información sobre cómo añadir una columna, consulte <a href="#add-columns-view-to-a-report" class="MCXref xref">Agregar columnas (vista) a un informe</a>.<br></p> </td> 
     </tr> 
     <tr> 
      <td>Agrupaciones</td> 
      <td> <p>Añadir agrupaciones al informe determina cómo se organiza el informe.</p> <p>Para obtener información sobre cómo añadir una agrupación, consulte <a href="#add-groupings-to-a-report" class="MCXref xref">Añadir agrupaciones a un informe</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Filtros</td> 
      <td> <p>La adición de reglas de filtro al informe determina la información que se ve en el informe.</p> <p>Para obtener información sobre cómo añadir un filtro, consulte <a href="#add-filters-to-a-report" class="MCXref xref">Añadir filtros a un informe</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Gráfico</td> 
      <td> <p>Agregar un gráfico al informe determina cómo se presenta visualmente la información del informe.</p> <p>Para obtener información sobre cómo añadir un gráfico, consulte <a href="#add-a-chart-to-a-report" class="MCXref xref">Agregar un gráfico a un informe</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. En cualquier momento del proceso de creación del informe, haga clic en **Aplicar** para guardar los cambios.
1. Una vez finalizado, haga clic en **Guardar + Cerrar**.

### Agregar columnas (vista) a un informe {#add-columns-view-to-a-report}

1. Comience a crear un informe como se describe en la sección [Crear un informe](#create-a-report) en este artículo.
1. En el Creador de informes, seleccione la opción **Columnas (Vista)** para identificar las columnas que se mostrarán en el informe.
1. (Opcional) Haga clic en **Aplicar una vista existente** para utilizar una vista existente.

   Para obtener más información sobre la creación de una nueva vista, consulte [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Para agregar una columna nueva, haga clic en **Agregar columna**.

   O

   Para cambiar una columna existente, seleccione la columna que desee cambiar y luego haga clic en (x) junto al nombre actual.

1. Comience a escribir el campo que desee añadir. Si el campo está disponible, se rellena para cada objeto al que se puede asociar. Haga clic en el nombre del campo para agregarlo a la columna .

   Para obtener más información sobre los campos que se ven en las columnas, consulte [Glosario de terminología de Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

   ![](assets/nwe-add-column-typeahead-350x459.png)

1. (Opcional) En la **Configuración de columna** área, seleccione **Ordenar por esta columna** para ordenar los valores de la columna de forma ascendente según el orden alfabético descendente, indique si la lista debe utilizar esta columna como su primer orden.

   Puede tener varios niveles de clasificación en una vista de informe si desea clasificarlos primero por el valor de una columna, luego por el valor de una segunda columna, etc.

   Si varios resultados son idénticos según los primeros criterios de clasificación, se ordenan según el segundo criterio de clasificación. Si varios resultados son idénticos según los criterios de clasificación primero y segundo, se ordenan según la tercera clasificación, etc.

   >[!NOTE]
   >
   >Si agrega un campo que hace referencia a un objeto que está demasiado alejado del objeto sobre el que informa, es posible que no pueda ordenarlo por este campo.\
   >Por ejemplo, un informe de problemas no se puede ordenar por el campo Propietario del proyecto porque hace referencia a 3 objetos adicionales: Proyecto, Propietario y Nombre. Sin embargo, puede agregar este campo a un informe de problemas y ver la información correspondiente.\
   >Para obtener más información sobre las referencias entre objetos en los informes, consulte la sección &quot;Informes avanzados, parte 1 de 3&quot; en la sección [Ruta de aprendizaje de los informes y los paneles](https://one.workfront.com/s/learningpath2/workfront-reporting-MC7MZT2BOL2ZC2LMJ4MA3EMHOCNY?tabset-dc70e=2).

1. (Opcional) Si está utilizando agrupaciones y desea resumir (sumar) la información de una columna, haga clic en el botón **Resumir esta columna por** lista desplegable en la **Configuración de columna** y, a continuación, seleccione la opción que desee utilizar para agregar la información en la columna .

   La información agregada se muestra en la columna de las filas de agrupación.

   ![Resumen agregado en agrupaciones](assets/aggregate-summary-displays-on-groupings-2022-350x195.png)

   Para obtener más información sobre el resumen de datos en una columna, consulte [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

   >[!NOTE]
   >
   >Las siguientes excepciones se aplican a los objetos principales (por ejemplo, tareas principales) cuando se agregan valores para los siguientes campos en agrupaciones:
   >
   >* Todos los campos de número y moneda excepto Horario real (por ejemplo, Coste laboral planeado/real, Coste planeado/real, Coste planeado/real, Horario planificado) agregan solamente los valores para las tareas secundarias y las tareas independientes. No acumulan los valores para las tareas principales o los principales de los padres.
   >* Las horas reales agregan los valores para las tareas principales y las tareas independientes; no agregan los números para los elementos principales de las tareas principales o las tareas secundarias.
   >* Los campos de datos personalizados para valores numéricos y monetarios agregan todas las tareas: padres, hijos, padres de padres y tareas independientes.


   Para obtener más información sobre el uso de agrupaciones en un informe, consulte [Información general sobre las agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. (Opcional) Haga clic en **Opciones avanzadas** para especificar la siguiente información para la columna:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etiqueta personalizada de columna</td> 
      <td> <p>Especifique una etiqueta personalizada para la columna. Esta etiqueta reemplaza la etiqueta predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formato de campo</td> 
      <td> <p>Seleccione el formato en el que desea que se muestren los valores para los campos de la columna .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar esta columna en panel</td> 
      <td> <p>Seleccione esta opción para mostrar esta columna en un tablero, cuando el informe se muestre en paralelo con otro informe. Cuando se anula la selección de esta opción, esta columna no se muestra al ver el informe en un tablero en el que los informes se muestran uno al lado del otro.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Reglas de columna</td> 
      <td> <p>Haga clic en <strong>Agregar una regla para esta columna</strong> para agregar formato condicional a la columna. Después de agregar una regla, puede definir los estilos de campo y texto para ver cómo se muestran los campos que coinciden con esa regla. Haga clic en <strong>Agregar regla</strong> una vez que haya terminado de definir la regla. Para obtener más información sobre el formato condicional en una vista, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md" class="MCXref xref">Utilizar el formato condicional en las vistas</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Aplicar** para aplicar los cambios realizados hasta el momento y continuar editando el informe con las siguientes opciones.

   Haga clic en **Guardar + Cerrar** si ha terminado de editar las columnas en el informe y desea guardar el informe.

### Añadir agrupaciones a un informe {#add-groupings-to-a-report}

1. Comience a crear un informe como se describe en la sección [Crear un informe](#create-a-report) en este artículo.
1. En el Creador de informes, seleccione la opción **Agrupaciones** para identificar cómo desea agrupar los elementos en el informe.
1. Haga clic en **Agregar agrupación** para agregar una nueva agrupación.

   O

   Choose **Aplicar una agrupación existente** para seleccionar una agrupación existente
   ![](assets/nwe-add-grouping-350x230.png)

1. Comience a escribir el campo que desee añadir como una agrupación. Si el campo está disponible, se rellena para cada objeto al que se puede asociar. Haga clic en el nombre del campo para agregarlo a esa agrupación.
1. (Opcional) Puede elegir crear una agrupación en modo de texto haciendo clic en **Cambiar al modo de texto**. Para obtener más información sobre el uso del modo de texto, consulte [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

   Para obtener más información sobre la creación de nuevas agrupaciones, consulte [Información general sobre las agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. (Opcional) Seleccione **Contraer esta agrupación de forma predeterminada** si desea que los resultados de esta agrupación se muestren contraídos en lugar de expandidos.

   Esta configuración está desactivada de forma predeterminada y los resultados de la agrupación siempre se muestran en una lista ampliada.

   >[!TIP]
   >
   >* Cuando ajusta las agrupaciones manualmente al ver una lista, Workfront recuerda su preferencia manual hasta que cierre la sesión. Cuando vuelve a iniciar sesión, la lista se muestra según esta configuración.
   >* Los resultados de una agrupación siempre se muestran expandidos después de acceder a ellos desde un elemento de gráfico.


1. (Opcional) Puede optar por crear una agrupación de matriz para mostrar los resultados en formato de cuadrícula.

   Para obtener más información sobre cómo crear un informe de matriz, consulte [Crear un informe de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Haga clic en **Aplicar** para aplicar los cambios realizados hasta el momento y continuar editando el informe con las siguientes opciones.

   Haga clic en **Guardar + Cerrar** si ha terminado de editar las agrupaciones en el informe y desea guardar el informe.

### Añadir filtros a un informe {#add-filters-to-a-report}

1. Comience a crear un informe como se describe en la sección [Crear un informe](#create-a-report) en este artículo.
1. En el Creador de informes, seleccione la opción **Filtros** para identificar la cantidad de información que desea que incluya el informe.
1. Haga clic en **Agregar una regla de filtro** para agregar un filtro personalizado.\
   O\
   Choose **Aplicar un filtro existente** para usar un filtro existente.

   ![](assets/nwe-add-a-filter-350x93.png)

1. Si ha hecho clic **Agregar una regla de filtro**, empiece a escribir el campo que desee añadir como filtro. Si el campo está disponible, se rellena para cada objeto al que se puede asociar. Haga clic en el nombre del campo para agregarlo a ese filtro.\
   Utilice modificadores de filtro para crear el filtro. Para obtener más información sobre los modificadores de filtro, consulte [Modificadores de filtro y condición](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   Para obtener más información sobre la creación de filtros nuevos, consulte [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Puede elegir crear un filtro en modo de texto haciendo clic en **Cambiar al modo de texto**.

   Para obtener más información sobre el uso del modo de texto, consulte [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

1. Haga clic en **Aplicar** cuando haya terminado de editar los filtros en el informe para aplicar los cambios realizados hasta el momento y continúe editando el informe con las siguientes opciones.

   Haga clic en **Guardar + Cerrar** si el informe y desea guardarlo.

### Agregar un gráfico a un informe {#add-a-chart-to-a-report}

1. Comience a crear un informe como se describe en la sección [Crear un informe](#create-a-report) en este artículo.
1. En el Creador de informes, seleccione la opción **Gráfico** y, a continuación, seleccione el tipo de gráfico que desea añadir.

   ![](assets/nwe-add-a-chart-350x247.png)

   Para obtener más información sobre cómo crear un gráfico en un informe, consulte [Agregar un gráfico a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. Haga clic en **Aplicar** para aplicar los cambios realizados hasta el momento y continuar editando el informe con las siguientes opciones.

   Haga clic en **Guardar + Cerrar** si ha terminado de editar el informe y desea guardarlo.
