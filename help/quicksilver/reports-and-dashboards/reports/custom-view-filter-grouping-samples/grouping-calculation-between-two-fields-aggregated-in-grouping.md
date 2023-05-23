---
content-type: reference
product-area: reporting;projects
keywords: calculadas, acumuladas, avanzadas, vistas
navigation-topic: custom-view-filter-and-grouping-samples
title: "Agrupación: muestra el resultado de agregar varios valores calculados en una agrupación"
description: Puede utilizar el modo de texto en una columna para mostrar un cálculo entre dos campos en la vista de un informe o una lista. Cada línea muestra el cálculo para cada objeto en el informe o la lista.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# Grouping: muestra el resultado de agregar varios valores calculados en una agrupación

Puede utilizar el modo de texto en una columna para mostrar un cálculo entre dos campos en la vista de un informe o una lista. Cada línea muestra el cálculo para cada objeto en el informe o la lista.

Por ejemplo, puede mostrar la diferencia entre las horas reales y las planificadas en una tercera columna denominada Saldo de trabajo para cada tarea de un informe de tareas. Para obtener más información sobre las expresiones de datos calculados, consulte [Expresiones de datos calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Puede mostrar el valor agregado de varios elementos de vista calculados en la misma columna de una agrupación agregando un cálculo a la variable `aggregator` línea de la columna que contiene el valor calculado. Por ejemplo, puede agregar (mostrar la suma de) la cantidad de horas de saldo de trabajo de todas las tareas de la agrupación del informe o de la lista de la columna Saldo de trabajo. Este artículo describe cómo hacerlo.

## Requisitos de acceso

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
   <td> <p>Solicitud para modificar una agrupación </p>
   <p>Plan para modificar un informe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar una agrupación</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Mostrar el resultado de agregar varios valores calculados en una agrupación

1. Vaya a un informe de tareas y haga clic en **Acciones de informe** > **Editar**.
1. En el **Agrupaciones** pestaña, haga clic en **Agregar agrupación** y empiece a escribir **Nombre de proyecto** en el **Agrupar el informe** > **Primero por** y, a continuación, selecciónelo cuando se muestre en la lista.

1. En el **Columnas (vista)** pestaña, haga clic en **Agregar columna**, y empiece a escribir **Horas planificadas** en el **Mostrar en esta columna** y, a continuación, selecciónelo cuando se muestre en la lista.

   >[!TIP]
   >
   >Empiece siempre a añadir tanta información con la interfaz estándar antes de editar la información en el modo de texto. Agregue los campos más cercanos o que contengan la mayor cantidad de información posible para el cálculo que está intentando realizar.

1. En el **Resumir esta columna por** , seleccione **Sum**, luego haga clic en **Listo**.
1. Clic **Cambiar a modo de texto** en la columna que ha añadido.
1. Pase el ratón sobre el área de modo de texto y haga clic en **Haga clic para editar el texto**.
1. Reemplace el `valuefield ` y el `aggregator.valuefield` líneas con las líneas resaltadas en el siguiente ejemplo de modo de texto:

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
   >Para obtener el valor agregado en la agrupación y mostrar la diferencia agregada entre los campos Horas planificadas y Horas reales, escriba la misma ecuación en la variable `aggregator.valuefield` línea. El `aggregator.displayformat` que se utiliza para la columna Horas planificadas convierte los minutos en horas. Dado que el campo Horas planificadas se utilizó como marcador de posición, no es necesario ajustar esta línea.
   >
   >
   >El `minutesAsHoursString` definición de la `aggregator.displayformat` line significa que no es necesario dividir cada campo por 60, como se hace en la `valueexpression` para obtener los resultados. En este `aggregator.valuefield=workRequired` se convierte en: `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.

1. Clic **Guardar + Cerrar**.
