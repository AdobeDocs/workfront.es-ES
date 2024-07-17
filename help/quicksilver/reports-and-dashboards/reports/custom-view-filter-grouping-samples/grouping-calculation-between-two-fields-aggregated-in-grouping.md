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
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# Grouping: muestra el resultado de agregar varios valores calculados en una agrupación

Puede utilizar el modo de texto en una columna para mostrar un cálculo entre dos campos en la vista de un informe o una lista. Cada línea muestra el cálculo para cada objeto en el informe o la lista.

Por ejemplo, puede mostrar la diferencia entre las horas reales y las planificadas en una tercera columna denominada Saldo de trabajo para cada tarea de un informe de tareas. Para obtener más información sobre las expresiones de datos calculados, vea [Información general sobre expresiones de datos calculados](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Puede mostrar el valor agregado de varios elementos de vista calculados en la misma columna de una agrupación agregando un cálculo a la línea `aggregator` de la columna que contiene el valor calculado. Por ejemplo, puede agregar (mostrar la suma de) la cantidad de horas de saldo de trabajo de todas las tareas de la agrupación del informe o de la lista de la columna Saldo de trabajo. Este artículo describe cómo hacerlo.

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

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Mostrar el resultado de agregar varios valores calculados en una agrupación

1. Vaya a un informe de tareas y haga clic en **Acciones de informe** > **Editar**.
1. En la ficha **Agrupaciones**, haga clic en **Agregar agrupación** y empiece a escribir **Nombre del proyecto** en el campo **Agrupar su informe** > **Primero por**; a continuación, selecciónelo cuando se muestre en la lista.

1. En la ficha **Columnas(Vista)**, haga clic en **Agregar columna**, empiece a escribir **Horas planificadas** en el campo **Mostrar en esta columna** y, a continuación, selecciónelo cuando se muestre en la lista.

   >[!TIP]
   >
   >Empiece siempre a añadir tanta información con la interfaz estándar antes de editar la información en el modo de texto. Agregue los campos más cercanos o que contengan la mayor cantidad de información posible para el cálculo que está intentando realizar.

1. En el campo **Resumir esta columna por**, seleccione **Suma** y, a continuación, haga clic en **Listo**.
1. Haga clic en **Cambiar al modo de texto** en la columna que agregó.
1. Pase el ratón sobre el área de modo de texto y haga clic **Haga clic para editar el texto**.
1. Reemplace las líneas `valuefield ` y `aggregator.valuefield` con las líneas resaltadas en el siguiente ejemplo de modo de texto:

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

1. Haga clic en **Guardar+Cerrar**.
