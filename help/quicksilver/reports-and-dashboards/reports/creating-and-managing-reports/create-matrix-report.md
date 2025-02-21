---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Creación de un informe de matriz
description: Los informes de matriz presentan la información de resumen en un formato de tabla agregado, lo que hace más fácil su visualización que si se mostrara en una lista como en un informe tradicional.
author: Nolan
feature: Reports and Dashboards
exl-id: 714f2802-089f-4a41-8205-f397cf474a24
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1091'
ht-degree: 98%

---

# Creación de un informe de matriz

Los informes de matriz presentan la información de resumen en un formato de tabla agregado, lo que hace más fácil su visualización que si se mostrara en una lista como en un informe tradicional.

## Cuándo utilizar un informe de matriz

Puede crear un informe de matriz para cualquier informe que contenga dos o más agrupaciones. Un informe tradicional puede contener hasta tres agrupaciones y un informe de matriz puede contener hasta cuatro agrupaciones.

Por ejemplo, desea crear un informe de horas que muestre las horas registradas durante un período de tres meses y desea que el informe se organice en función de quién introdujo las horas, así como por mes y semana.

![Descripción general de la matriz de informes](assets/report-matrix-overview-350x123.png)

## Visualización de los datos en un informe de matriz

La información del informe de matriz siempre se muestra como un valor numérico. En la mayoría de los casos, es mejor mostrar las columnas que contienen un valor numérico en un informe de matriz (como las horas registradas y el coste real).

Sin embargo, otras columnas (como Estado) se pueden seguir mostrando en el informe de matriz, como se muestra en el siguiente gráfico:\
![Estado de la matriz](assets/report-matrix-status-350x73.png)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
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
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td><p>Acceso de edición a informes, paneles y calendarios</p> <p>Acceso de edición a filtros, vistas y agrupaciones</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p></td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar un informe de matriz

1. Cree un informe tradicional que contenga datos numéricos en el resultado del informe.\
   Para obtener información sobre cómo crear un informe, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Vaya al informe que creó en el paso 1, haga clic en **Acciones de informe** y, a continuación, seleccione **Editar**.

1. (Condicional) Si ya ha creado una vista y desea aplicarla a este informe, haga clic en **Aplicar una vista existente** y, a continuación, seleccione la vista en la lista desplegable.
1. (Condicional) Si desea crear una nueva vista para el informe, complete los siguientes pasos:

   1. Haga clic en la pestaña **Columnas (Vista)** y, a continuación, seleccione una columna que desee resumir en el informe de matriz.
   1. En el área **Configuración de columna**, haga clic en la lista desplegable **Resumir esta columna por** y, a continuación, seleccione una de las opciones disponibles para resumir la información.

      >[!IMPORTANT]
      >
      >Si no se selecciona esta opción, la información de la columna no se muestra correctamente en el informe de matriz.

      ![Matriz resumida](assets/qs-report-matrix-summarized-350x392.png)

   1. Repita este proceso con cada columna de la pestaña Columnas (Vista) y, a continuación, haga clic en **Listo**.

1. Haga clic en la pestaña **Agrupaciones**.
1. (Condicional) Si ya ha creado una agrupación y desea aplicarla a este informe, haga clic en **Aplicar una agrupación existente** y, a continuación, seleccione la agrupación en la lista desplegable.
1. (Condicional) Si desea crear una nueva agrupación de matriz para el informe, complete los siguientes pasos:

   1. Seleccione **Cambiar a agrupación de matriz** en la esquina superior derecha de la interfaz del generador.
   1. En la sección **Agrupaciones de filas**, identifique la agrupación de filas, que establece las agrupaciones horizontales de la tabla.
   1. (Opcional) Para añadir una agrupación de filas adicional, haga clic en **Agregar agrupación de filas secundaria**.
   1. En la sección **Agrupaciones de columnas**, identifique la agrupación de columnas, que establece las agrupaciones verticales de la tabla.
   1. (Opcional) Para añadir una agrupación de columnas adicional, haga clic en **Agregar agrupación de columnas secundaria**.
   1. (Condicional) Si agrega una agrupación por fecha, especifique también si los resultados se agrupan por día, semana, mes, trimestre o año.\
      ![Opciones de agrupación por fecha](assets/qs-grouping-by-date-options-for-matrix-report-350x450.png)

   1. (Condicional) Si ha seleccionado agrupar por fecha y mostrar los resultados por trimestre, por ejemplo, especifique si desea mostrar trimestres sin datos seleccionando la casilla de verificación **Mostrar trimestres sin resultados**.\
      ![Mostrar trimestres sin resultados](assets/qs-show-quarters-with-no-results-on-matrix-report-350x175.png)

      >[!NOTE]
      >
      >El campo **Mostrar trimestres sin resultados** solo está disponible para agrupaciones de matriz y no para agrupaciones estándar.\
      >Solo los trimestres sin datos que se encuentran entre dos trimestres con datos válidos mostrarán cero para los valores de datos en la pestaña matriz. Los trimestres sin datos ubicados al principio y al final del periodo de tiempo seleccionado por el filtro no aparecen en absoluto en la agrupación de matriz. Los trimestres sin resultados no se muestran en una agrupación de la pestaña Detalles del informe.

1. (Opcional y condicional) Haga clic en **Configuración de matriz** y, a continuación, seleccione entre las siguientes opciones:\
   **Mostrar recuentos de registros:** seleccione esta opción para mostrar una fila con el número total de entradas para el campo especificado.\
   **Mostrar columna de valor:** seleccione esta opción para mostrar la siguiente información en la matriz:

   * Recuentos de registros
   * La columna Valor

     >[!NOTE]
     >
     >Esta columna contiene información que describe lo que representan los datos de cada fila.\
     >Las siguientes excepciones se aplican a los objetos principales (por ejemplo, las tareas principales) cuando se añaden valores para los siguientes campos en agrupaciones:
     >
     >   
     >   
     >   * Todos los campos de número y moneda excepto Horas reales (por ejemplo, Coste planificado/real de mano de obra, Coste planificado/real de gastos, Coste planificado/ real, Horas planificadas) acumulan solo los valores de las tareas secundarias y las tareas independientes. No acumulan los valores de las tareas principales o principales de los elementos principales.
     >   * Las horas reales acumulan los valores de las tareas principales e independientes; no acumulan los números de las tareas principales o secundarias.
     >   * Los campos de datos personalizados para valores numéricos y de moneda agregan todas las tareas: principales, secundarias, principales de principales y tareas independientes. Si ha creado el informe de matriz para mostrar las horas planificadas o las horas reales en la columna **Valor**, tenga en cuenta que la información de horas o costes de cualquier objeto principal (como las tareas principales) no se muestra en el informe de matriz. Para ver las horas de los objetos principales, debe consultar la pestaña **Detalles**.
     >   
     >   
     >

   **Reglas condicionales:** configure cualquier regla de formato para los valores agregados.\
   Después de añadir una regla, puede definir estilos de campo y de texto para ver cómo se muestran los campos que coinciden con esa regla. Haga clic en **Añadir regla** después de haber terminado de definir la regla y, a continuación, **Listo** para guardarla.

1. Haga clic en la pestaña **Filtros** para definir la información que se mostrará en el informe.
1. (Condicional) Si ya ha creado un filtro y desea aplicarlo a este informe, haga clic en **Aplicar un filtro existente** y, a continuación, seleccione el filtro en la lista desplegable.
1. (Condicional) Si desea crear un nuevo Filtro para este informe, consulte [Modificadores de filtro y condición](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   and
   <a href="../../../reports-and-dashboards/reports/reporting-elements/advanced-filter-condition-qualifiers.md" class="MCXref xref">Advanced Filter and condition qualifiers </a>
   </MadCap:conditionalText>
   -->

   para obtener información sobre los distintos calificadores que puede utilizar al crear filtros.

1. Haga clic en **Guardar+Cerrar** para guardar y ver el informe de matriz.
