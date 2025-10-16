---
product-area: reporting
navigation-topic: reporting-elements
title: Usar comodines basados en fecha para generalizar informes
description: Puede generalizar un informe utilizando comodines en lugar de información específica al crear determinados elementos de informes.
author: Nolan
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 92%

---

# Usar comodines basados en fecha para generalizar informes

<!-- Audited: 11/2024 -->

Puede generalizar un informe utilizando comodines en lugar de información específica al crear determinados elementos de informes.

Por ejemplo, si desea crear un informe que muestre las tareas que tienen una fecha de inicio planificada específica, puede utilizar el selector de fecha de calendario en un filtro para seleccionar una fecha específica. Sin embargo, si desea crear un informe que muestre las tareas que tienen la fecha de inicio planificada dentro de un periodo de tiempo determinado desde la fecha en que se accede al informe, puede utilizar un comodín que indique que, cuando alguien vea el informe, muestre información correspondiente a un periodo de tiempo relevante para el momento en el que vea el informe.

Por ejemplo, la semana pasada, el año pasado, las próximas dos semanas, etc. De este modo, el informe se genera una vez, pero como se utiliza un comodín en el filtro, genera resultados diferentes cada vez que alguien lo lee, ya que se adapta al día en que se ejecuta el informe.

Puede utilizar comodines basados en la fecha al crear los siguientes elementos de creación informes:

* Filtros
* Solicitudes personalizadas
* Vistas al añadir reglas para columnas

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
   <td role="rowheader">Licencia de Adobe Workfront</strong></td> 
   <td> 
    <p>Estándar</p>
    <p>Plan</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a filtros, vistas y agrupaciones</p> <p>Editar el acceso a los informes, paneles y calendarios para editar los elementos de un informe</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
    <td> <p>Permisos de administración a un informe para editar los elementos de un informe</p> <p>Permisos de administración a una vista o filtro para editarlos</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Debe crear un informe para poder añadirle variables comodín.

Para obtener información sobre cómo crear un informe, consulte [Crear un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Pasos a seguir

Para insertar un comodín basado en la fecha en un informe:

1. Vaya a un informe para el que desea insertar un comodín basado en la fecha.
1. Haga clic en **Acciones de informe** y, a continuación, en **Editar**.
1. Haga clic en la pestaña **Filtros**.
1. Haga clic en **Añadir una regla de filtro**.
1. Empiece a escribir el nombre del campo por el que desea filtrar.\
   Debe escribir campos que hagan referencia a una fecha.
1. Seleccione **Equal** en el menú desplegable de la variable de filtro.

   >[!TIP]
   >
   >Siempre debe seleccionar la variable de filtro **Equal** al trabajar con comodines en Adobe Workfront.

1. Haga clic en el botón de alternancia **Establecer fecha relativa** y, a continuación, en el cuadro de texto que aparece, escriba: `$$TODAY` si desea mostrar información acerca de algo que ocurra el mismo día en que se ejecuta el informe.

   O

   Escriba `$$NOW` si desea mostrar información acerca de algo que ocurra en la misma fecha y hora en que se ejecuta el informe.

   Esta fecha siempre es diferente, ya que cambia con la fecha en la que un usuario ve realmente el informe. Por lo tanto, la información del informe es diferente día a día.

1. (Opcional) Si desea mostrar información que se produce dentro de un periodo de tiempo después de la fecha en la que se ejecuta el informe, escriba `$$TODAY+1w` para mostrar información de la semana siguiente o `$$TODAY+2m` para mostrar información de los próximos dos meses. También puede indicar periodos de tiempo de trimestres, horas, días o años.
1. (Opcional) Si desea mostrar información sobre algo que se produjo dentro de un periodo de tiempo antes de la fecha en la que se ejecuta el informe, escriba `$$TODAY-1w` para mostrar información de la semana anterior o `$$TODAY-2m` para mostrar información de los dos meses anteriores. También puede indicar periodos de tiempo de trimestres, horas, días o años.

   Para obtener una lista completa de los atributos, calificadores y operadores que puede usar en los comodines basados en fecha, vea el artículo [Información general sobre las variables del filtro comodín](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Haga clic en **Guardar + Cerrar**.

## Más información

Consulte también lo siguiente:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Información general sobre las variables del filtro comodín](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Crear o editar filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Añadir una solicitud a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Usar formato condicional en vistas](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
