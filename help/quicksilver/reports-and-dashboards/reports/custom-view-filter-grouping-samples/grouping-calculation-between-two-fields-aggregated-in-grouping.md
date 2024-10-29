---
content-type: reference
product-area: reporting;projects
keywords: calculadas, acumuladas, avanzadas, vistas
navigation-topic: custom-view-filter-and-grouping-samples
title: "Agrupación: Mostrar el resultado de la agregación de varios valores calculados en una agrupación"
description: Puede utilizar el modo de texto en una columna para mostrar un cálculo entre dos campos en la vista de un informe o una lista. Cada línea muestra el cálculo para cada objeto en el informe o la lista.
author: Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Grouping: muestra el resultado de agregar varios valores calculados en una agrupación

<!--Audited: 10/2024-->

Puede utilizar el modo de texto en una columna para mostrar un cálculo entre dos campos en la vista de un informe o una lista. Cada línea muestra el cálculo para cada objeto en el informe o la lista.

Por ejemplo, puede mostrar la diferencia entre las horas reales y las planificadas en una tercera columna denominada Saldo de trabajo para cada tarea de un informe de tareas. Para obtener más información sobre las expresiones de datos calculados, vea [Información general sobre expresiones de datos calculados](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Puede mostrar el valor agregado de varios elementos de vista calculados en la misma columna de una agrupación agregando un cálculo a la línea `aggregator` de la columna que contiene el valor calculado. Por ejemplo, puede agregar (mostrar la suma de) la cantidad de horas de saldo de trabajo de todas las tareas de la agrupación del informe o de la lista de la columna Saldo de trabajo. Este artículo describe cómo hacerlo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> 
    <p>Nuevo:</p>
   <ul><li><p>Colaborador para modificar un filtro </p></li>
   <li><p>Estándar para modificar un informe</p></li> </ul>

<p>Actual:</p>
   <ul><li><p>Solicitud para modificar un filtro </p></li>
   <li><p>Plan para modificar un informe</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mostrar el resultado de agregar varios valores calculados en una agrupación

1. Vaya a un informe de tareas y haga clic en **Acciones de informe** > **Editar**.
1. En la ficha **Agrupaciones**, haga clic en **Agregar agrupación**, empiece a escribir **Nombre del proyecto** en el campo **Agrupar por** y, a continuación, seleccione **Proyecto > Nombre** cuando se muestre en la lista.

1. En la ficha **Columnas(Vista)**, haga clic en **Agregar columna**, empiece a escribir **Horas planificadas** en el campo **Mostrar en esta columna** y, a continuación, selecciónelo cuando se muestre en la lista.

   >[!TIP]
   >
   >Empiece siempre a añadir tanta información con la interfaz estándar antes de editar la información en el modo de texto. Agregue los campos más cercanos o que contengan la mayor cantidad de información posible para el cálculo que está intentando realizar.

1. En el campo **Resumir esta columna por**, seleccione **Suma**.
1. Haga clic en **Cambiar al modo de texto** en la columna que agregó y, a continuación, haga clic en **Editar modo de texto**.
1. Reemplace el texto del cuadro por el siguiente ejemplo de modo de texto:

   ```
   valueformat=compound
   aggregator.displayformat=minutesAsHoursString
   aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2)
   aggregator.function=SUM
   aggregator.valueformat=val
   aggregator.namekey=workrequired
   linkedname=direct
   textmode=true
   valuefield=workRequired
   namekey=workrequired
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") 
   viewalias=workrequired 
   displayname=Work Balance
   ```

   >[!TIP]
   >
   >Para que el valor agregado de la agrupación muestre la diferencia agregada entre los campos Horas planificadas y Horas reales, escriba la misma ecuación en la línea `aggregator.valuefield`. El `aggregator.displayformat` usado para la columna Horas planificadas convierte los minutos en horas. Dado que el campo Horas planificadas se utilizó como marcador de posición, no es necesario ajustar esta línea.
   >
   >
   >La definición de `minutesAsHoursString` de la línea `aggregator.displayformat` significa que no es necesario dividir cada campo entre 60 como se hizo en `valueexpression` para los resultados. En este(a) `aggregator.valuefield=workRequired` se convierte en: `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.
1. Haga clic en **Listo**.
1. Haga clic en **Guardar+Cerrar**.
