---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Filtrado de informes por lapsos de tiempo
description: Puede filtrar un informe por el lapso de tiempo de una fecha que exista en un objeto. Por ejemplo, puede filtrar un informe de hora para un lapso de tiempo en particular de cuándo se introdujeron las horas.
author: Nolan
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: e8acdf8f7b3859385237e788dfda34ee62ee11d1
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 95%

---

# Filtrado de informes por lapsos de tiempo

<!-- Audited: 11/2024 -->

Puede filtrar un informe por el lapso de tiempo de una fecha que exista en un objeto. Por ejemplo, puede filtrar un informe de hora para un lapso de tiempo en particular de cuándo se introdujeron las horas.

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
   <td> <p>Acceso de Edición a informes, paneles y calendarios</p> <p>Acceso de edición a filtros, vistas y agrupaciones</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p></td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

El informe debe crearse antes de que filtre sus resultados.

Para obtener más información sobre la creación de informes, consulte [Crear un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Filtrado de informes por el lapso de tiempo de una fecha {#filter-a-report-by-the-time-frame-of-a-date}

1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) y luego haga clic en **Informes**.

1. Haga clic en **Nuevo informe** y, a continuación, seleccione el tipo de informe que desee.\
   Por ejemplo, seleccione **Informe de hora**.

1. Seleccione la pestaña **Filtros**.
1. Haga clic en **Agregar regla de filtro** y luego seleccione **Fecha de entrada de hora**.\
   ![Filtrado del informe de horas por intervalo de tiempo](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

1. En el siguiente menú desplegable, seleccione cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Igual (distingue mayúsculas y minúsculas)</td> 
      <td>Después de seleccionar este modificador, especifique la fecha en la que se introdujeron las horas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">No es igual a (distingue mayúsculas y minúsculas)</td> 
      <td>Después de seleccionar este modificador, especifique la fecha en la que se introdujeron las horas para excluir esta fecha del informe. El informe muestra las horas registradas en todas las fechas, excepto en la fecha especificada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nulo</td> 
      <td>Seleccione este modificador para mostrar solo las horas en las que falta la fecha de entrada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">No es nulo</td> 
      <td>Seleccione este modificador para mostrar solo las horas en las que la fecha de entrada tiene un valor.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entre</td> 
      <td>Después de seleccionar este modificador, especifique un intervalo de fechas en el que introducir las horas. El informe muestra las horas introducidas entre las fechas especificadas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Menor que</td> 
      <td>Después de seleccionar este modificador, especifique una fecha antes de la cual se introdujeron las horas. El informe muestra las horas introducidas antes de la fecha especificada, sin incluir la fecha especificada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Menor o igual a</td> 
      <td>Después de seleccionar este modificador, especifique una fecha antes de la cual se introdujeron las horas. El informe muestra las horas introducidas antes de la fecha especificada, incluida la fecha especificada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mayor que</td> 
      <td>Después de seleccionar este modificador, especifique una fecha después de la cual se introdujeron las horas. El informe muestra las horas introducidas después de la fecha especificada, sin incluir la fecha especificada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mayor o igual a</td> 
      <td> <p>Después de seleccionar este modificador, especifique una fecha después de la cual se introdujeron las horas. El informe muestra las horas introducidas después de la fecha especificada, incluida la fecha especificada.</p> <p>Seleccione cualquiera de los modificadores de lapso de tiempo integrados, tal como se describe en <a href="#built-in-time-frame-modifiers" class="MCXref xref">Modificadores de lapso de tiempo integrados</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Estos modificadores están disponibles para cualquier campo de fecha de un filtro o para una solicitud de datos de cualquier informe.
1. Haga clic en **Guardar + Cerrar**.

## Modificadores de lapso de tiempo integrados {#built-in-time-frame-modifiers}

Adobe Workfront tiene modificadores de lapso de tiempo integrados que se pueden utilizar sin definir una fecha específica.

Estos modificadores están disponibles para cualquier campo de fecha de un filtro o para una solicitud de datos de cualquier informe.

Para obtener más información sobre cómo filtrar un informe por un lapso de tiempo asociado a una fecha, consulte la sección anterior [Filtrar un informe por el lapso de tiempo de una fecha](#filter-a-report-by-the-time-frame-of-a-date).

Por ejemplo, si está generando un informe de hora y desea mostrar las horas introducidas en un lapso de tiempo específico, puede elegir entre las siguientes opciones de filtro de lapso de tiempo integrado:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Hoy</td> 
   <td>Muestra las horas cuya fecha de entrada es hoy.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Esta semana</td> 
   <td>Muestra las horas en las que la fecha de entrada es una fecha de la semana actual, donde la semana comienza un domingo y termina un sábado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Próxima semana</td> 
   <td>Muestra las horas en las que la fecha de entrada es una fecha de la semana siguiente a la semana actual, donde la semana comienza un domingo y termina un sábado. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Última semana</td> 
   <td>Muestra las horas en las que la fecha de entrada es una fecha de la semana anterior a la semana actual, en la que la semana comienza un domingo y termina un sábado. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Este mes</td> 
   <td>Muestra las horas en las que la fecha de entrada es una fecha del mes actual.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Próximo mes</td> 
   <td>Muestra las horas en las que la fecha de entrada es una fecha del mes siguiente al mes actual.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Último mes</td> 
   <td>Muestra las horas en las que la fecha de entrada es una fecha del mes anterior al mes actual</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Este trimestre</td> 
   <td> <p>Muestra las horas en las que la fecha de entrada es una fecha del trimestre actual, en las que los trimestres se definen como:</p> 
    <ul> 
     <li>Primer trimestre: del 1 de enero al 30 de marzo</li> 
     <li>Segundo trimestre: del 1 de abril al 30 de junio</li> 
     <li>Tercer trimestre: del 1 de julio al 30 de septiembre</li> 
     <li>Cuarto trimestre: del 1 de octubre al 31 de diciembre</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Próximo trimestre</td> 
   <td>Muestra las horas en las que la fecha de entrada es una fecha del trimestre siguiente al trimestre actual, en el que los trimestres se han definido anteriormente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Último trimestre</td> 
   <td> <p>Muestra las horas en las que la fecha de entrada es una fecha del trimestre anterior al actual, donde los trimestres se han definido anteriormente.</p> <p>Nota: Si el administrador de Workfront ha activado y definido trimestres personalizados para el sistema, los filtros integrados para trimestres se sustituyen por la información de trimestre personalizada. Para obtener más información acerca de cómo habilitar trimestres personalizados, vea <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">Habilitar trimestres personalizados para proyectos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Este año</td> 
   <td>Muestra las horas en las que la fecha de entrada es una fecha del año actual, donde este comienza el 1 de enero y finaliza el 31 de diciembre.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Último año</td> 
   <td>Muestra las horas en las que la fecha de entrada es una fecha del año pasado, en el que el año pasado comienza 12 meses antes de la fecha actual.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Año pasado</td> 
   <td> <p>Muestra las horas en las que la fecha de entrada es una fecha del último año, donde el último año comienza el 1 de enero y finaliza el 31 de diciembre del año anterior al año actual.</p> <p>Nota: No hay ningún período de tiempo integrado para el año fiscal. Puede crear un informe y filtrar la información por fecha utilizando un modificador personalizado para el intervalo de fecha del año fiscal, tal como está definido en su organización. Si desea elegir un lapso de tiempo para un año fiscal en mismo el momento, debe utilizar una indicación en lugar de un filtro. </p> </td> 
  </tr> 
 </tbody> 
</table>
