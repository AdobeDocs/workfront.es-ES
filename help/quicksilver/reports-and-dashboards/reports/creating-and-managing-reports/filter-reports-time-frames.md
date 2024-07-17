---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Filtrado de informes por lapsos de tiempo
description: Puede filtrar un informe por el lapso de tiempo de una fecha que exista en un objeto. Por ejemplo, puede filtrar un informe de horas para un intervalo de tiempo en particular de cuándo se ingresaron las horas.
author: Nolan
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1059'
ht-degree: 4%

---

# Filtrado de informes por lapsos de tiempo

Puede filtrar un informe por el lapso de tiempo de una fecha que exista en un objeto. Por ejemplo, puede filtrar un informe de horas para un intervalo de tiempo en particular de cuándo se ingresaron las horas.

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
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

El informe debe crearse antes de filtrar sus resultados.

Para obtener más información sobre la creación de informes, consulte [Crear un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Filtrado de informes por el lapso de tiempo de una fecha {#filter-a-report-by-the-time-frame-of-a-date}

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) y luego haga clic en **Informes**.

1. Haga clic en **Nuevo informe** y, a continuación, seleccione el tipo de informe que desee.\
   Por ejemplo, seleccione **Informe de horas**.

1. Seleccione la ficha **Filtros**.
1. Haga clic en **Agregar una regla de filtro** y luego seleccione **Fecha de entrada de hora**.\
   ![](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

1. En el siguiente menú desplegable, seleccione cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Igual (distingue mayúsculas y minúsculas)</td> 
      <td>Después de seleccionar este modificador, especifique la fecha en la que se ingresaron las horas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">No es igual a (distingue mayúsculas y minúsculas)</td> 
      <td>Después de seleccionar este modificador, especifique la fecha en la que se ingresaron las horas para excluir esta fecha del informe. El informe muestra las horas registradas en todas las fechas, esperadas para la fecha especificada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nulo</td> 
      <td>Seleccione este modificador para mostrar sólo las horas en las que falta la fecha de entrada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">No es nulo</td> 
      <td>Seleccione este modificador para mostrar sólo las horas en las que la fecha de entrada tiene un valor.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entre</td> 
      <td>Después de seleccionar este modificador, especifique un intervalo de fechas en el que introducir las horas. El informe muestra las horas ingresadas entre las fechas especificadas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Menor que</td> 
      <td>Después de seleccionar este modificador, especifique una fecha antes de la cual se ingresaron las horas. El informe muestra las horas ingresadas antes de la fecha especificada, sin incluir la fecha especificada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Menor o igual a</td> 
      <td>Después de seleccionar este modificador, especifique una fecha antes de la cual se ingresaron las horas. El informe muestra las horas ingresadas antes de la fecha especificada, incluida la fecha especificada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mayor que</td> 
      <td>Después de seleccionar este modificador, especifique una fecha después de la cual se ingresaron las horas. El informe muestra las horas ingresadas después de la fecha especificada, sin incluir la fecha especificada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mayor o igual a</td> 
      <td> <p>Después de seleccionar este modificador, especifique una fecha después de la cual se ingresaron las horas. El informe muestra las horas ingresadas después de la fecha especificada, incluida la fecha especificada.</p> <p>Seleccione cualquiera de los modificadores de lapso de tiempo integrados, tal como se describe en <a href="#built-in-time-frame-modifiers" class="MCXref xref">Modificadores de lapso de tiempo integrados</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Estos modificadores están disponibles para cualquier campo de fecha de un filtro o para una solicitud de datos de cualquier informe.
1. Haga clic en **Guardar + Cerrar**.

## Modificadores de lapso de tiempo integrados {#built-in-time-frame-modifiers}

Adobe Workfront tiene modificadores de lapso de tiempo integrados que se pueden utilizar sin definir una fecha específica. 

Estos modificadores están disponibles para cualquier campo de fecha de un filtro o para una solicitud de datos de cualquier informe. 

Para obtener más información sobre cómo filtrar un informe por un lapso de tiempo asociado a una fecha, consulte  [Filtrar un informe por el lapso de tiempo de una fecha](#filter-a-report-by-the-time-frame-of-a-date).

Por ejemplo, si está generando un informe de horas y desea mostrar las horas ingresadas en un lapso de tiempo específico, puede elegir entre las siguientes opciones de filtro de lapso de tiempo integrado:

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
   <td> <p>Muestra las horas en las que la fecha de entrada es una fecha del trimestre anterior al trimestre actual, donde los trimestres se han definido anteriormente.</p> <p>Nota: Si el administrador de Workfront ha activado y definido trimestres personalizados para el sistema, los filtros integrados para trimestres se sustituyen por la información de trimestre personalizada. Para obtener más información acerca de cómo habilitar trimestres personalizados, vea <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">Habilitar trimestres personalizados para proyectos</a>.</p> </td> 
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
   <td> <p>Muestra las horas en las que la fecha de entrada es una fecha del último año, donde el último año comienza el 1 de enero y finaliza el 31 de diciembre del año anterior al año actual.</p> <p>Nota: No hay ningún período de tiempo integrado para el año fiscal. Puede crear un informe y filtrar la información por fecha utilizando un modificador personalizado para el intervalo de fechas del año fiscal, tal como está definido en su organización. Si desea elegir un lapso de tiempo para un año fiscal en el momento, debe utilizar un mensaje en lugar de un filtro. </p> </td> 
  </tr> 
 </tbody> 
</table>
