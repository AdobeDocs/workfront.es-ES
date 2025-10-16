---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Informe: Hora presupuestada'
description: 'Informe: Hora presupuestada'
author: Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 72%

---

# Informe: Hora presupuestada

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resource Management and it is super important.) </p>
-->

Si desea compartir información de horas presupuestadas con otros usuarios que no tienen acceso al Planificador de recursos, puede hacerlo generando un informe Hora presupuestada. A continuación, puede compartir el informe con ellos.

>[!IMPORTANT]
>
>Las horas presupuestadas por lo general se actualizan cada hora (con poca frecuencia, puede tardar un máximo de tres horas) en la base de datos de Adobe Workfront. Actualizar el informe no actualiza por fuerza la información horaria que contiene. Puede ver el tiempo transcurrido desde la última actualización en la esquina superior derecha de todos los informes Hora presupuestada. Al actualizar el informe, se actualiza la información que contiene solo cuando ha transcurrido más de una hora desde la última actualización.
>
>![Advertencia de sincronización de tiempo de informe de hora presupuestada](assets/budgeted-hour-report-time-sync-warning-350x74.png)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o solicitud para modificar un filtro </p>
   <p>Estándar o Plan para modificar un informe</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios para modificar un informe</p> <p>Acceso de edición a filtros, vistas y agrupaciones para modificar un filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Generación de un informe Hora presupuestada

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha, o en el icono **Menú principal** ![Líneas del menú principal](assets/lines-main-menu.png) en la esquina superior izquierda, si está disponible, y luego haga clic en **Informes**.

1. Haga clic en **Nuevo informe** > **Más** > **Hora presupuestada**.

   La vista predeterminada se aplica al informe.

1. (Opcional) Para facilitar la lectura del informe, haga clic en **Bud. Horas** columna, luego **Cambiar al modo de texto**, luego haga clic en **Editar modo de texto**.
1. Cambie la línea `valuefield` a `valueexpreesion` e introduzca la expresión de redondeo.

   Esto redondea el número de horas presupuestadas al número de decimales que especifique.

   Para obtener información acerca de cómo redondear un número en Workfront, vea el artículo [Información general sobre expresiones de datos calculados](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. Haga clic en **Listo**.
1. (Opcional) Haga clic en **Agregar columna** para agregar columnas adicionales.
1. (Opcional) Para que el informe sea más fácil de leer, le recomendamos que le añada una agrupación. Sugerimos la siguiente agrupación:

   Haga clic en la pestaña **Agrupaciones** y, después, siga uno o varios de estos procedimientos:

   * Haga clic en **Agregar agrupación** y empiece a escribir &quot;Nombre de proyecto&quot;. A continuación, selecciónelo cuando aparezca en la lista.
   * Haga clic en **Agregar agrupación** y empiece a escribir &quot;Nombre de rol&quot;. A continuación, selecciónelo cuando aparezca en la lista.
   * Haga clic en **Agregar agrupación** y empiece a escribir &quot;Fecha de asignación&quot;, selecciónela cuando aparezca en la lista y, a continuación, seleccione el periodo de tiempo por el que desea agrupar desde el campo **Agrupar fechas por**.

1. (Opcional) Haga clic en **Filtros** para agregar filtros al informe.
1. (Opcional) Haga clic en **Gráfico** para agregar un gráfico al informe.
1. Haga clic en **Guardar + Cerrar**.

## Revisión del informe Hora presupuestada

La siguiente información está disponible en el informe Hora presupuestada de forma predeterminada:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Proyecto </td> 
   <td>Nombre del proyecto asociado a Hora presupuestada.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Función</p> </td> 
   <td>Es el nombre de la función asociada con Hora presupuestada. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Usuario</td> 
   <td>Nombre del usuario asociado a Hora presupuestada.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Fecha de asig</td> 
   <td> <p>Esta es la fecha de asignación. Es el primer día (un domingo) de la semana para el que presupuestó las horas.</p> <p>Sugerencia:  <p>Si una semana abarca dos meses, esto genera dos filas en el informe: una correspondiente al primer día de la semana (el domingo de la semana que es durante el primer mes) y una segunda correspondiente al primer día del segundo mes (y que podría ser cualquier día de la semana).</p> <p>Por ejemplo, si asigna un presupuesto de 8 horas a un usuario para la semana del 30 de junio (domingo) al 6 de julio (sábado), las dos filas muestran una Fecha de asignación del 30 de junio y del 1 de julio.</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Horas presup.</td> 
   <td>Horas presupuestadas asignadas al usuario en el Planificador de recursos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pln. Horas presup.</td> 
   <td>Son las horas presupuestadas asignadas a la función o al proyecto en el Planificador de recursos.</td> 
  </tr> 
 </tbody> 
</table>
