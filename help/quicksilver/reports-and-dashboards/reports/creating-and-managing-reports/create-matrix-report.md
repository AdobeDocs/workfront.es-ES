---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Crear un informe de matriz
description: Los informes de matriz presentan la información de resumen en un formato de tabla agregada, lo que facilita su visualización que si se mostrara en una lista como en un informe tradicional.
author: Nolan
feature: Reports and Dashboards
exl-id: 714f2802-089f-4a41-8205-f397cf474a24
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1115'
ht-degree: 0%

---

# Crear un informe de matriz

Los informes de matriz presentan la información de resumen en un formato de tabla agregada, lo que facilita su visualización que si se mostrara en una lista como en un informe tradicional.

## Cuándo utilizar un informe de matriz

Puede crear un informe de matriz para cualquier informe que contenga 2 o más agrupamientos. Un informe tradicional puede contener hasta 3 Agrupaciones y un informe de matriz puede contener hasta 4 Agrupaciones.

Por ejemplo, si desea crear un informe de hora que muestre las horas registradas durante un período de 3 meses, y desea que el informe se organice según quién ingresó las horas, así como por mes y semana.

![](assets/report-matrix-overview-350x123.png)

## Cómo se muestran los datos en un informe de matriz

La información del informe de matriz siempre se muestra como un valor numérico. En la mayoría de los casos, las columnas que contienen un valor numérico son mejores para mostrarlas en un informe de matriz (como las horas registradas y el coste real).

Sin embargo, otras columnas (como Estado) se pueden seguir mostrando en el informe de matriz como se muestra en el siguiente gráfico:\
![](assets/report-matrix-status-350x73.png)

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

## Configurar un informe de matriz

1. Cree un informe tradicional que contenga datos numéricos en el resultado del informe.\
   Para obtener información sobre cómo crear un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Vaya al informe que ha creado en el paso 1, haga clic en **Acciones de informe** y, a continuación, seleccione **Editar**.

1. (Condicional) Si ya ha creado una vista y desea aplicarla a este informe, haga clic en **Aplicar una vista existente** y, a continuación, seleccione la opción Ver en la lista desplegable.
1. (Condicional) Si desea crear una nueva vista para el informe, complete los pasos siguientes:

   1. Haga clic en el **Columnas (Vista)** y, a continuación, seleccione una columna que desee resumir en el informe de matriz.
   1. En el **Configuración de columna** , haga clic en el **Resumir esta columna por** lista desplegable y, a continuación, seleccione una de las opciones disponibles para resumir la información.

      >[!IMPORTANT]
      >
      >Si no se selecciona esta opción, la información de la columna no se muestra correctamente en el informe de matriz.

      ![](assets/qs-report-matrix-summarized-350x392.png)

   1. Repita este proceso para cada columna de la ficha Columnas (Ver) y, a continuación, haga clic en **Listo**.

1. Haga clic en el **Agrupaciones** pestaña .
1. (Condicional) Si ya ha creado un grupo y desea aplicarlo a este informe, haga clic en **Aplicar una agrupación existente** y, a continuación, seleccione Grouping en la lista desplegable.
1. (Condicional) Si desea crear un nuevo grupo de matriz para el informe, complete los pasos siguientes:

   1. Select **Cambiar a agrupación en matriz** en la esquina superior derecha de la interfaz del generador.
   1. En el **Agrupaciones de filas** identifique la agrupación de filas, que establece las agrupaciones horizontales de la tabla.
   1. (Opcional) Para agregar una agrupación de filas adicional, haga clic en **Agregar grupo de filas secundario**.
   1. En el **Agrupaciones de columnas** identifique la agrupación de columnas que establecen las agrupaciones verticales de la tabla.
   1. (Opcional) Para agregar una agrupación de columnas adicional, haga clic en **Agregar grupo de columnas secundario**.
   1. (Condicional) Si agrega una agrupación por fecha, especifique también si los resultados se agrupan por día, semana, mes, trimestre o año.\
      ![](assets/qs-grouping-by-date-options-for-matrix-report-350x450.png)

   1. (Condicional) Si seleccionó agrupar por fecha y mostrar los resultados por trimestre, por ejemplo, especifique si desea mostrar trimestres sin datos seleccionando la opción **Mostrar trimestres sin resultados** casilla de verificación.\
      ![](assets/qs-show-quarters-with-no-results-on-matrix-report-350x175.png)

      >[!NOTE]
      >
      >La variable **Mostrar trimestres sin resultados** solo está disponible para agrupaciones de matrices y no para agrupaciones estándar.\
      >Solo los trimestres sin datos ubicados entre dos trimestres con datos válidos mostrarán cero para los valores de datos en la ficha matriz. Los trimestres que no tienen datos ubicados al principio y al final del periodo seleccionado por el filtro no aparecen en la agrupación de matriz. Los trimestres sin resultados no se mostrarán en una agrupación de la pestaña Detalles del informe.

1. (Opcional y condicional) Haga clic en **Configuración de matriz** y, a continuación, seleccione entre las siguientes opciones:\
   **Mostrar recuentos de registros:** Seleccione esta opción para mostrar una fila con el número total de entradas para el campo dado.\
   **Mostrar columna de valor:** Seleccione esta opción para mostrar la siguiente información en la matriz:

   * Recuentos de registros
   * La columna Value

      >[!NOTE]
      >
      >Esta columna contiene información que describe lo que representan los datos de cada fila.\
      >Las siguientes excepciones se aplican a los objetos principales (por ejemplo, tareas principales) cuando se agregan valores para los siguientes campos en agrupaciones:
      >
      >   
      >   
      >   * Todos los campos de número y moneda excepto Horario real (por ejemplo, Coste laboral planeado/real, Coste planeado/real, Coste planeado/real, Horario planificado) agregan solamente los valores para las tareas secundarias y las tareas independientes. No acumulan los valores para las tareas principales o los principales de los padres.
      >   * Las horas reales agregan los valores para las tareas principales y las tareas independientes; no agregan los números para los elementos principales de las tareas principales o las tareas secundarias.
      >   * Los campos de datos personalizados para valores numéricos y monetarios agregan todas las tareas: padres, hijos, padres de padres y tareas independientes. Si ha creado el informe de matriz para mostrar las horas planificadas u horas reales en la variable **Valor** , tenga en cuenta que la información de horas o costes de cualquier objeto principal (como las tareas principales) no se muestra en el informe de matriz. Para ver las horas de los objetos principales, debe ver la variable **Detalles** pestaña .

   **Reglas condicionales:** Configure cualquier regla de formato para los valores agregados.\
   Después de agregar una regla, puede definir los estilos de campo y texto para ver cómo se muestran los campos que coinciden con esa regla. Haga clic en **Agregar regla** una vez que haya terminado de definir la regla, **Listo** para guardar la regla.

1. Haga clic en el **Filtros** para definir qué información se mostrará en el informe.
1. (Condicional) Si ya ha creado un filtro y desea aplicarlo a este informe, haga clic en **Aplicar un filtro existente** y, a continuación, seleccione el Filtro en la lista desplegable.
1. (Condicional) Si desea crear un nuevo filtro para este informe, consulte [Modificadores de filtro y condición](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   and
   <a href="../../../reports-and-dashboards/reports/reporting-elements/advanced-filter-condition-qualifiers.md" class="MCXref xref">Advanced Filter and condition qualifiers </a>
   </MadCap:conditionalText>
   -->

   para obtener información sobre los distintos calificadores que puede utilizar al crear filtros.

1. Haga clic en **Guardar y cerrar** para guardar y ver el informe de matriz.
