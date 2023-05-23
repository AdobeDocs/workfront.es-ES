---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Informe: Hora presupuestada"
description: "Informe: Hora presupuestada"
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 1%

---

# Informe: Horas presupuestadas

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resouce Management and it is super important.) </p>
-->

Si desea compartir información de horas presupuestadas con otros usuarios que no tienen acceso al Planificador de recursos, puede hacerlo generando un informe de horas presupuestadas. A continuación, puede compartir el informe con ellos.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This info is also added and drafted in the article "View Budget Hours in a report" in the Resource Planning section. Consider deleting this article?!)</p>
-->

>[!IMPORTANT]
>
>Las horas presupuestadas se actualizan cada hora en la base de datos de Adobe Workfront. Al actualizar el informe no se actualiza necesariamente la información de las horas que contiene. Puede ver el tiempo transcurrido desde la última actualización en la esquina superior derecha de todos los informes de horas presupuestadas. Al actualizar el informe, se actualiza la información que contiene únicamente cuando ha transcurrido más de una hora desde la última actualización.
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)>

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Generar un informe de horas presupuestadas

1. Haga clic en **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha, haga clic en **Informes**.

1. Clic **Nuevo informe > Hora presupuestada**.

   La vista predeterminada se aplica al informe.

1. (Opcional) Para facilitar la lectura del informe, haga clic en el icono **Horas presupuestadas** y luego **Cambiar a modo de texto**, luego cambie la

   ```
   valuefield
   ```

   línea a

   ```
   valueexpreesion
   ```

   e introduzca la expresión de redondeo.

   Esto redondea el número de horas presupuestadas al número de decimales que especifique.

   Para obtener información sobre cómo redondear un número en Workfront, consulte el artículo [Expresiones de datos calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. (Opcional) Haga clic en **Agregar columna** para añadir columnas adicionales.
1. (Opcional) Para que el informe sea más fácil de leer, le recomendamos que le agregue una agrupación. Sugerimos la siguiente agrupación:

   Haga clic en **Agrupaciones** y, a continuación, siga uno o varios de estos procedimientos:

   1. Clic **Agregar agrupación** y empiece a escribir &quot;Nombre del proyecto&quot; y, a continuación, selecciónelo cuando aparezca en la lista.
   1. Clic **Agregar agrupación** y empiece a escribir &quot;Nombre de rol&quot;, luego selecciónelo cuando aparezca en la lista.
   1. Clic **Agregar agrupación** y empiece a escribir **Fecha de asignación**, selecciónelo cuando aparezca en la lista y, a continuación, seleccione el periodo de tiempo por el que desee agrupar en el **Agrupar fechas por** field.

1. (Opcional) Haga clic en **Filtros** para añadir filtros al informe.
1. (Opcional) Haga clic en **Gráfico** para agregar un gráfico al informe.
1. Clic **Guardar + Cerrar**.

## Revisar el informe de horas presupuestadas

La siguiente información está disponible en el informe Hora presupuestada de forma predeterminada:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Proyecto </td> 
   <td>Nombre del proyecto asociado a la hora presupuestada.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Rol</p> </td> 
   <td>Es el nombre de la función asociada con la hora presupuestada. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Usuario</td> 
   <td>Nombre del usuario asociado a la hora presupuestada.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Fecha de asig</td> 
   <td> <p>Fecha de asignación. Es el primer día (un domingo) de la semana para el que presupuestó las horas.</p> <p>Sugerencia:  <p>Si una semana abarca dos meses, esto genera dos filas en el informe: una correspondiente al primer día de la semana (el domingo de la semana que es durante el primer mes) y una segunda correspondiente al primer día del segundo mes (y que podría ser cualquier día de la semana).</p> <p>Por ejemplo, si asigna un presupuesto de 8 horas a un usuario para la semana del 30 de junio (domingo) al 6 de julio (sábado), las dos filas muestran una Fecha de asignación del 30 de junio y del 1 de julio.</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Horas presup.</td> 
   <td>Horas presupuestadas asignadas al usuario en el Planificador de recursos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pln. Horas presup.</td> 
   <td>Son las horas presupuestadas asignadas al rol o al proyecto en el Planificador de recursos.</td> 
  </tr> 
 </tbody> 
</table>
