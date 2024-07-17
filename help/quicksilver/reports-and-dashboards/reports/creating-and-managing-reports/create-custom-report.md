---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Creación de un informe personalizado
description: Puede proporcionar acceso a la información que su organización necesita en Adobe Workfront creando informes. Puede utilizar cualquiera de los informes integrados disponibles en Workfront o puede crear los informes personalizados desde cero.
author: Nolan
feature: Reports and Dashboards
exl-id: 10c4df37-f09f-4b91-9cfd-3d0c3835bc7b
source-git-commit: 4cab7bed6cb4c25d96e70ccce2ece7f6d156f435
workflow-type: tm+mt
source-wordcount: '1828'
ht-degree: 1%

---


# Creación de un informe personalizado

<!--Audited: 12/2023-->

Puede proporcionar acceso a la información que su organización necesita en Adobe Workfront creando informes. Puede utilizar cualquiera de los informes integrados disponibles en Workfront o puede crear los informes personalizados desde cero.

Para obtener más información sobre los informes integrados, consulte [Usar informes integrados de Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

Para obtener información sobre cómo crear un informe copiándolo, vea [Crear una copia de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

Para obtener más información sobre la creación y administración de informes, incluidas clases, vídeos y tutoriales, consulte la sección Más información en el sitio de Adobe Experience League.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nuevo: estándar </p>
   o
   <p>Actual: plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p><b>NOTA</b></p>
   <p> Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Puede obtener permisos de administración para los informes que cree.</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

+++

## Creación de un informe {#create-a-report}

{{step1-to-reports}}

1. Haga clic en **Nuevo informe** y, a continuación, seleccione el tipo de objeto que desee para el informe.

   Se carga Report Builder.

   Para obtener información específica sobre los informes de objetos disponibles, consulte la sección [Informe sobre objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) en el artículo [Comprender los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   ![](assets/nwe-select-new-report-350x666.png)

   >[!TIP]
   >
   >También puede crear un informe realizando una copia de un informe existente. Para obtener más información, consulte [Crear una copia de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. En Report Builder, añada lo siguiente al informe:

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
      <td> <p>Añadir columnas al informe determina qué información contiene el informe.</p> <p>Para obtener información sobre cómo agregar una columna, consulte <a href="#add-columns-view-to-a-report" class="MCXref xref">Agregar columnas (vista) a un informe</a>.<br></p> </td> 
     </tr> 
     <tr> 
      <td>Agrupaciones</td> 
      <td> <p>Añadir agrupaciones al informe determina la organización del informe.</p> <p>Para obtener información sobre cómo agregar una agrupación, consulte <a href="#add-groupings-to-a-report" class="MCXref xref">Agregar agrupaciones a un informe</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Filtros</td> 
      <td> <p>Añadir reglas de filtro al informe determina la información que se ve en el informe.</p> <p>Para obtener información sobre cómo agregar un filtro, consulte <a href="#add-filters-to-a-report" class="MCXref xref">Agregar filtros a un informe</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Gráfico</td> 
      <td> <p>Agregar un gráfico al informe determina cómo se presenta visualmente la información del informe.</p> <p>Para obtener información sobre cómo agregar un gráfico, consulte <a href="#add-a-chart-to-a-report" class="MCXref xref">Agregar un gráfico a un informe</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. En cualquier momento del proceso de creación del informe, haga clic en **Aplicar** para guardar los cambios.
1. Una vez finalizado, haga clic en **Guardar + Cerrar**.

### Agregar columnas (vista) a un informe {#add-columns-view-to-a-report}

1. Comience a crear un informe como se describe en la sección [Crear un informe](#create-a-report) de este artículo.
1. En Report Builder, seleccione la ficha **Columnas (vista)** para identificar las columnas que aparecerán en el informe.
1. (Opcional) Haga clic en **Aplicar una vista existente** y haga clic en el nombre de una vista en el menú desplegable para usar una vista existente.

   Para obtener más información acerca de cómo crear una vista, vea [Información general sobre vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. (Opcional) Para quitar una columna existente, haga clic en la columna que desee quitar y, a continuación, haga clic en **x** junto al nombre actual en el encabezado de la columna.

1. Para agregar una nueva columna, haga clic en **Agregar columna**.

   O

   Para cambiar una columna existente, haga clic en la columna, haga clic en el icono **Quitar** ![](assets/x-icon-circled.png) a la izquierda del campo actual en el cuadro **Mostrar en este campo de columna** en la esquina superior izquierda de Report Builder, y empiece a escribir un nuevo campo; a continuación, haga clic en él cuando se muestre en la lista.

   Para obtener más información sobre los campos que se ven en las columnas, consulte [Glosario de terminología de Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

   ![](assets/nwe-add-column-typeahead-350x459.png)

1. (Opcional) En el área **Configuración de columna**, seleccione **Ordenar por esta columna** para ordenar los valores de la columna en orden ascendente o alfabético descendente y, a continuación, indique si la lista debe utilizar esta columna como su primer orden.

   Puede tener varios niveles de ordenación en una vista de informe si desea ordenar por el valor de una columna en primer lugar, el valor de una segunda columna en segundo lugar, etc.

   Si varios resultados son idénticos según el primer criterio de ordenación, se ordenan según el orden del segundo criterio de ordenación. Si varios resultados son idénticos según el primer y el segundo criterio de ordenación, se ordenan según el tercer criterio de ordenación, etc.

   >[!NOTE]
   >
   >Si agrega un campo que hace referencia a un objeto que está demasiado alejado del objeto sobre el que realiza el informe, es posible que no pueda ordenar por este campo.\
   >Por ejemplo, un informe de problemas no puede ordenar por el campo Propietario del proyecto porque hace referencia a tres objetos adicionales: Proyecto, Propietario y Nombre. Sin embargo, aún puede agregar este campo a un informe de problemas y ver la información correspondiente.

   <!--outdated: To learn more about cross-object references in reports, see the section "Advanced Reporting Part 1 of 3" in the [Reports and Dashboards Learning Path](https://one.workfront.com/s/learningpath2/workfront-reporting-MC7MZT2BOL2ZC2LMJ4MA3EMHOCNY?tabset-dc70e=2).-->

1. (Opcional) Si está usando agrupaciones y desea resumir (agregar) la información de una columna, haga clic en la lista desplegable **Resumir esta columna por** en el área de **Configuración de columna** y, a continuación, seleccione la opción que desee usar para agregar la información en la columna.

   La información agregada se muestra en la columna de las filas de agrupación.

   ![Resumen agregado sobre agrupaciones](assets/aggregate-summary-displays-on-groupings-2022-350x195.png)

   Para obtener más información sobre cómo resumir los datos de una columna, vea [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

   >[!NOTE]
   >
   >Las siguientes excepciones se aplican a los objetos principales (por ejemplo, las tareas principales) cuando se agregan valores para los siguientes campos en agrupaciones:
   >
   >* Todos los campos de número y moneda excepto Horas reales (por ejemplo, Costo de mano de obra planificado o real, Costo de gasto planificado o real, Costo planificado o real, Horas planificadas) agregan solo los valores de las tareas secundarias y las tareas independientes. No acumulan los valores de las tareas principales o principales de los elementos principales.
   >* Las horas reales acumulan los valores de las tareas principales e independientes; no acumulan los números de las tareas principales o secundarias.
   >* Los campos de datos personalizados para valores numéricos y monetarios acumulan todas las tareas: principales, secundarios, principales de principales y tareas independientes.

   Para obtener más información acerca del uso de agrupaciones en un informe, vea [Información general sobre agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

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
      <td> <p>Seleccione el formato en el que desea que se muestren los valores de los campos de la columna.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar esta columna en panel de control</td> 
      <td> <p>Seleccione esta opción para mostrar esta columna en un panel cuando el informe se muestre en paralelo con otro informe. Cuando esta opción no está seleccionada, esta columna no se muestra al ver el informe en un panel en el que los informes se muestran uno al lado del otro.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Reglas de columna</td> 
      <td> <p>Haga clic en <strong>Agregar una regla para esta columna</strong> para agregar formato condicional a la columna. Después de agregar una regla, puede definir estilos de campo y de texto para ver cómo se muestran los campos que coinciden con esa regla. Haga clic en <strong>Agregar regla</strong> después de haber terminado de definir la regla. Para obtener más información acerca del formato condicional en una vista, vea <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md" class="MCXref xref">Usar formato condicional en vistas</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Aplicar** para aplicar los cambios hasta el momento y seguir editando el informe con las siguientes opciones.

   Haga clic en **Guardar + Cerrar** si ha terminado de editar las columnas del informe y desea guardarlo.

### Adición de agrupaciones a un informe {#add-groupings-to-a-report}

1. Comience a crear un informe como se describe en la sección [Crear un informe](#create-a-report) de este artículo.
1. En Report Builder, seleccione la ficha **Agrupaciones** para identificar cómo desea agrupar los elementos en el informe.
1. Haga clic en **Agregar agrupación** para agregar una nueva agrupación.

   O

   Elija **Aplicar una agrupación existente** para seleccionar una agrupación existente cuando se muestre en la lista.

   ![](assets/nwe-add-grouping-350x230.png)

1. Empiece a escribir el campo que desea agregar como agrupación. Si el campo está disponible, se rellena para cada objeto donde se puede asociar. Haga clic en el nombre del campo para agregarlo a esa agrupación.
1. (Opcional) Si lo desea, puede generar una agrupación en modo de texto haciendo clic en **Cambiar al modo de texto**. Para obtener más información acerca del uso del modo de texto, vea [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

   Para obtener más información sobre cómo crear nuevas agrupaciones, consulte [Información general sobre agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. (Opcional) Seleccione **Contraer esta agrupación de forma predeterminada** si desea que los resultados de esta agrupación se muestren contraídos en lugar de expandidos.

   Esta configuración está deshabilitada de forma predeterminada y los resultados de la agrupación siempre se muestran en una lista expandida.

   >[!TIP]
   >
   >* Cuando ajusta manualmente las agrupaciones al ver una lista, Workfront recuerda su preferencia manual hasta que cierre la sesión. Cuando vuelva a iniciar sesión, la lista se mostrará según esta configuración.
   >* Los resultados de una agrupación siempre se muestran expandidos después de acceder a ellos desde un elemento de gráfico.

1. (Opcional) Haga clic en **Cambiar a agrupación de matriz** para generar una agrupación de matriz y mostrar los resultados en formato de cuadrícula.

   Para obtener más información sobre cómo generar un informe de matriz, consulte [Crear un informe de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Haga clic en **Aplicar** para aplicar los cambios hasta el momento y seguir editando el informe con las siguientes opciones.

   Haga clic en **Guardar + Cerrar** si ha terminado de editar las agrupaciones del informe y desea guardar el informe.

### Adición de filtros a un informe {#add-filters-to-a-report}

1. Comience a crear un informe como se describe en la sección [Crear un informe](#create-a-report) de este artículo.
1. En Report Builder, seleccione la ficha **Filtros** para identificar la cantidad de información que desea que incluya el informe.
1. Haga clic en **Agregar una regla de filtro** para agregar un filtro personalizado.\
   O\
   Elija **Aplicar un filtro existente** para usar un filtro existente.

   ![](assets/nwe-add-a-filter-350x93.png)

1. Si hizo clic en **Agregar una regla de filtro**, empiece a escribir el campo que desea agregar como filtro. Si el campo está disponible, se rellena para cada objeto donde se puede asociar. Haga clic en el nombre del campo para añadirlo a ese filtro.\
   Utilice modificadores de filtro para crear el filtro. Para obtener más información acerca de los modificadores de filtro, vea [Modificadores de filtro y condición](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   Para obtener más información sobre la creación de nuevos filtros, consulte [Resumen de filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Opcional) Puede optar por generar un filtro en modo de texto si hace clic en **Cambiar al modo de texto**.

   Para obtener más información acerca del uso del modo de texto, vea [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

1. Haga clic en **Aplicar** cuando haya terminado de editar los filtros del informe para aplicar los cambios hasta el momento y seguir editando el informe con las siguientes opciones.

   Haga clic en **Guardar + Cerrar** si el informe y desea guardarlo.

### Agregar un gráfico a un informe {#add-a-chart-to-a-report}

1. Comience a crear un informe como se describe en la sección [Crear un informe](#create-a-report) de este artículo.
1. En Report Builder, seleccione la ficha **Gráfico** y, a continuación, seleccione el tipo de gráfico que desee agregar.

   ![](assets/nwe-add-a-chart-350x247.png)

   Para obtener más información sobre cómo crear un gráfico en un informe, consulte [Agregar un gráfico a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. Haga clic en **Aplicar** para aplicar los cambios hasta el momento y seguir editando el informe con las siguientes opciones.

   Haga clic en **Guardar + Cerrar** si ha terminado de editar el informe y desea guardarlo.
