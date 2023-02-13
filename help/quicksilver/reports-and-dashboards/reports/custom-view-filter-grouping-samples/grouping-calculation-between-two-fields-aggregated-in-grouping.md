---
content-type: reference
product-area: reporting;projects
keywords: calculado,agregados,avanzado,vistas
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Agrupación: mostrar el resultado de agregar varios valores calculados en una agrupación'
description: Se puede utilizar el modo de texto en una columna para mostrar un cálculo entre dos campos en la vista de un informe o una lista. Cada línea muestra el cálculo de cada objeto del informe o la lista.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# Agrupación: mostrar el resultado de agregar varios valores calculados en una agrupación

Se puede utilizar el modo de texto en una columna para mostrar un cálculo entre dos campos en la vista de un informe o una lista. Cada línea muestra el cálculo de cada objeto del informe o la lista.

Por ejemplo, puede mostrar la diferencia entre horas reales y horas planeadas en una tercera columna llamada Balance de trabajo para cada tarea en un informe de tareas. Para obtener más información sobre las expresiones de datos calculadas, consulte [Expresiones de datos calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Puede mostrar el valor agregado de varios elementos de vista calculada en la misma columna de una agrupación añadiendo un cálculo al `aggregator` línea de la columna que contiene el valor calculado. Por ejemplo, se puede acumular (mostrar la suma de) la cantidad de horas de balance de trabajo de todas las tareas de la agrupación del informe o la lista de la columna Balance de trabajo. Este artículo describe cómo hacerlo.

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

## Mostrar el resultado de agregar varios valores calculados en una agrupación

1. Vaya a un informe de tareas y haga clic en **Acciones de informe** > **Editar**.
1. En el **Agrupaciones** , haga clic en **Agregar agrupación** y empiece a escribir **Nombre del proyecto** en el **Agrupar su informe** > **Primero por** y selecciónelo cuando aparezca en la lista.

1. En el **Columnas (Vista)** , haga clic en **Agregar columna** y, a continuación, empiece a escribir **Horas planificadas** en el **Mostrar en esta columna** y selecciónelo cuando aparezca en la lista.

   >[!TIP]
   >
   >Antes de editar información en modo de texto, empiece a agregar siempre la misma información mediante la interfaz de Standard. Añada campos que sean los más cercanos o que contengan la mayor cantidad de información que para el cálculo que está intentando realizar.

1. En el **Resumir esta columna por** campo, seleccione **Sum** y haga clic en **Listo**.
1. Haga clic en **Cambiar al modo de texto** en la columna que ha agregado.
1. Pase el ratón sobre el área del modo de texto y haga clic en **Haga clic para editar texto**.
1. Sustituya el `valuefield ` y `aggregator.valuefield` líneas con las líneas resaltadas en el siguiente ejemplo de modo de texto:

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
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") viewalias=workrequired displayname=Work Balance
   ```

   >[!TIP]
   >
   >Para obtener el valor agregado en la agrupación y mostrar la diferencia agregada entre los campos Horario planeado y Hora real , introduzca la misma ecuación en la variable `aggregator.valuefield` línea. La variable `aggregator.displayformat` se utiliza en la columna Horario planificado para convertir minutos a horas. Dado que el campo Horario planeado se utilizó como marcador de posición, no es necesario ajustar esta línea.
   >
   >
   >La variable `minutesAsHoursString` definición de `aggregator.displayformat` línea significa que no hay necesidad de dividir cada campo por 60, como se hace en la `valueexpression` para los resultados. En este `aggregator.valuefield=workRequired` se convierte en: `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.

1. Haga clic en **Guardar y cerrar**.
