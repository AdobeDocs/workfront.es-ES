---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Filtrado de informes por intervalos de tiempo
description: Puede filtrar un informe por el lapso de tiempo de una fecha que exista en un objeto. Por ejemplo, puede filtrar un informe de hora para un lapso de tiempo determinado en el que se especificaron las horas.
author: Nolan
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1046'
ht-degree: 4%

---

# Filtrado de informes por intervalos de tiempo

Puede filtrar un informe por el lapso de tiempo de una fecha que exista en un objeto. Por ejemplo, puede filtrar un informe de hora para un lapso de tiempo determinado en el que se especificaron las horas.

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

## Requisitos previos

El informe debe crearse antes de filtrar sus resultados.

Para obtener más información sobre la creación de informes, consulte [Crear un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Filtrado de un informe por el lapso de tiempo de una fecha {#filter-a-report-by-the-time-frame-of-a-date}

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png)y haga clic en **Informes**.

1. Haga clic en **Nuevo informe** y, a continuación, seleccione el tipo de informe que desee.\
   Por ejemplo, seleccione **Informe de hora**.

1. Seleccione el **Filtros** pestaña .
1. Haga clic en **Agregar una regla de filtro** y, a continuación, seleccione **Fecha de entrada de hora**.\
   ![](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

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
      <td>Después de seleccionar este modificador, especifique la fecha en la que se introdujeron las horas para excluir esta fecha del informe. El informe muestra las horas registradas en todas las fechas; espere la fecha especificada.</td> 
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
      <td>Después de seleccionar este modificador, especifique un intervalo de fechas en el que se introdujeron las horas. El informe muestra las horas introducidas entre las fechas especificadas.</td> 
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

1. Estos modificadores están disponibles para cualquier campo de fecha de un filtro o para una solicitud de cualquier informe.
1. Haga clic en **Guardar + Cerrar**.

## Modificadores de lapso de tiempo integrados {#built-in-time-frame-modifiers}

Adobe Workfront tiene modificadores de lapso de tiempo integrados que puede utilizar sin definir una fecha específica. 

Estos modificadores están disponibles para cualquier campo de fecha de un filtro o para una solicitud de cualquier informe. 

Para obtener más información sobre cómo filtrar un informe por un lapso de tiempo asociado con una fecha, consulte  [Filtrado de un informe por el lapso de tiempo de una fecha](#filter-a-report-by-the-time-frame-of-a-date).

Por ejemplo, si está creando un informe de hora y desea mostrar las horas introducidas en un intervalo de tiempo específico, puede elegir entre las siguientes opciones de filtro de intervalo de tiempo integradas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Hoy</td> 
   <td>Muestra las horas en las que la fecha de entrada es hoy.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Esta semana</td> 
   <td>Muestra las horas en las que la fecha de entrada es una fecha de la semana actual, donde la semana comienza un domingo y finaliza un sábado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Próxima semana</td> 
   <td>Muestra las horas en las que la fecha de entrada es una fecha de la semana siguiente a la semana actual, donde la semana comienza un domingo y finaliza un sábado. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Última semana</td> 
   <td>Muestra las horas en las que la fecha de entrada es una fecha de la semana anterior a la semana actual, donde la semana comienza en un domingo y finaliza en un sábado. </td> 
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
   <td> <p>Muestra las horas en las que la fecha de entrada es una fecha del trimestre actual, donde los trimestres se definen como:</p> 
    <ul> 
     <li>Primer trimestre: Del 1 de enero al 30 de marzo</li> 
     <li>Segundo trimestre: Del 1 de abril al 30 de junio</li> 
     <li>Tercer trimestre: Del 1 de julio al 30 de septiembre</li> 
     <li>Cuarto trimestre: Del 1 de octubre al 31 de diciembre</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Próximo trimestre</td> 
   <td>Muestra las horas en las que la fecha de entrada es una fecha del trimestre siguiente al trimestre actual, donde los trimestres están definidos anteriormente.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Último trimestre</td> 
   <td> <p>Muestra las horas en las que la fecha de entrada es una fecha del trimestre anterior al trimestre actual, donde los trimestres se definen más arriba.</p> <p>Nota: Si el administrador de Workfront ha habilitado y definido trimestres personalizados para su sistema, los filtros integrados para trimestres se sustituyen por la información de trimestre personalizada. Para obtener más información sobre cómo activar los trimestres personalizados, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">Habilitar trimestres personalizados para proyectos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Este año</td> 
   <td>Muestra las horas en las que la fecha de entrada es una fecha del año actual, donde el año actual comienza el 1 de enero y finaliza el 31 de diciembre.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Último año</td> 
   <td>Muestra las horas en las que la fecha de entrada es una fecha del año anterior, donde el año anterior comienza 12 meses antes de la fecha actual.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Año pasado</td> 
   <td> <p>Muestra las horas en las que la fecha de entrada es una fecha del último año, donde el último año comienza el 1 de enero y finaliza el 31 de diciembre del año anterior al año actual.</p> <p>Nota: No hay un período de tiempo integrado para el año fiscal. Puede crear un informe y filtrar la información por fecha utilizando un modificador personalizado para el intervalo de fechas del año fiscal, tal como se define en su organización. Si desea elegir un intervalo de tiempo para un año fiscal sobre el terreno, debe utilizar un mensaje en lugar de un filtro. </p> </td> 
  </tr> 
 </tbody> 
</table>
