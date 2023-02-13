---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Informe: Hora presupuestada'
description: 'Informe: Hora presupuestada'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 1%

---

# Informe: Hora presupuestada

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resouce Management and it is super important.) </p>
-->

Si desea compartir información sobre la hora presupuestada con otros usuarios que no tienen acceso al planificador de recursos, puede hacerlo creando un informe de hora presupuestada. A continuación, puede compartir el informe con ellos.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This info is also added and drafted in the article "View Budget Hours in a report" in the Resource Planning section. Consider deleting this article?!)</p>
-->

>[!IMPORTANT]
>
>Las horas presupuestadas se actualizan cada hora en la base de datos de Adobe Workfront. Al actualizar el informe, no se actualiza necesariamente la información de horas que contiene. Puede ver el tiempo transcurrido desde la última actualización en la esquina superior derecha de cada informe de hora presupuestada. Al actualizar el informe, se actualiza la información que contiene únicamente cuando ha transcurrido más de una hora desde la última actualización.
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)>

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

## Generar un informe de hora presupuestada

1. Haga clic en el **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha, haga clic en **Informes**.

1. Haga clic en **Nuevo informe > Hora presupuestada**.

   La vista predeterminada se aplica al informe.

1. (Opcional) Para facilitar la lectura del informe, haga clic en el **Horas presupuestadas** , luego **Cambiar al modo de texto** y, a continuación, cambie la variable

   ```
   valuefield
   ```

   línea hasta

   ```
   valueexpreesion
   ```

   e introduzca la expresión de redondeo.

   De este modo, se redondea el número de horas presupuestadas a una cantidad de decimales que se especifique.

   Para obtener información sobre cómo redondear un número en Workfront, consulte el artículo [Expresiones de datos calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. (Opcional) Haga clic en **Agregar columna** para agregar columnas adicionales.
1. (Opcional) Para que el informe sea más fácil de leer, le recomendamos que agregue una agrupación a él. Sugerimos la siguiente agrupación:

   Haga clic en el **Agrupaciones** y, a continuación, realice una o varias de las siguientes acciones:

   1. Haga clic en **Agregar agrupación** y empiece a escribir &quot;Nombre del proyecto&quot; y, a continuación, selecciónelo cuando aparezca en la lista.
   1. Haga clic en **Agregar agrupación** y empiece a escribir &quot;Nombre de función de trabajo&quot;, luego selecciónelo cuando aparezca en la lista.
   1. Haga clic en **Agregar agrupación** y empiece a escribir **Fecha de asignación**, selecciónela cuando aparezca en la lista y, a continuación, seleccione el intervalo de tiempo por el que desee agrupar en el **Agrupar fechas por** campo .

1. (Opcional) Haga clic en **Filtros** para agregar filtros al informe.
1. (Opcional) Haga clic en **Gráfico** para agregar un gráfico al informe.
1. Haga clic en **Guardar + Cerrar**.

## Revisar el informe de horas presupuestadas

La siguiente información está disponible en el informe de horas presupuestadas de forma predeterminada:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Proyecto </td> 
   <td>Este es el nombre del proyecto asociado con la hora presupuestada.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Función del trabajo</p> </td> 
   <td>Este es el nombre del rol de trabajo asociado con la hora presupuestada. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Usuario</td> 
   <td>Es el nombre del usuario asociado con la hora presupuestada.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Fecha de asig</td> 
   <td> <p>Esta es la fecha de asignación. Es el primer día (un domingo) de la semana en el que se presupuestaron las horas.</p> <p>Sugerencia:  <p>Si una semana abarca dos meses, se generan dos filas en el informe: uno correspondiente al primer día de la semana (el domingo de la semana que es el primer mes) y otro correspondiente al primer día del segundo mes (y que podría ser cualquier día de la semana).</p> <p>Por ejemplo, si se presupuestan 8 horas para un usuario para la semana del 30 de junio (domingo) al 6 de julio (sábado), las dos filas muestran una fecha de asignación del 30 de junio y el 1 de julio.</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Horas presup.</td> 
   <td>Son las horas presupuestadas asignadas al usuario en el Planificador de recursos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pln. Horas presup.</td> 
   <td>Son las horas presupuestadas asignadas a la función de trabajo o al proyecto en el planificador de recursos.</td> 
  </tr> 
 </tbody> 
</table>
