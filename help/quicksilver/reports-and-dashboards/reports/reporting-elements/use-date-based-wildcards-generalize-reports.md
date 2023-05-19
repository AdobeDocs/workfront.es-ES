---
product-area: reporting
navigation-topic: reporting-elements
title: Utilice comodines basados en fecha para generalizar informes
description: Puede generalizar un informe utilizando caracteres comodín en lugar de información específica al crear determinados elementos de informe.
author: Nolan
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 0%

---

# Utilice comodines basados en fecha para generalizar informes

Puede generalizar un informe utilizando caracteres comodín en lugar de información específica al crear determinados elementos de informe.

Por ejemplo, si desea crear un informe que muestre las tareas que tienen una fecha planificada de inicio específica, puede utilizar el selector de fecha de calendario en un filtro para seleccionar una fecha específica. Sin embargo, si desea crear un informe que muestre las tareas que tienen la fecha planificada de inicio dentro de un intervalo de tiempo determinado desde la fecha en que se accede al informe, puede utilizar un comodín que indique que, cuando alguien ve el informe, muestra información correspondiente a un intervalo de tiempo relevante para el momento en que ve el informe.

Por ejemplo, la semana pasada, el año pasado, las dos semanas siguientes, etc. De este modo, el informe se genera una vez, pero como se utiliza un comodín en el filtro, genera resultados diferentes cada vez que alguien lo lee, ya que se adapta al día en que se ejecuta el informe.

Puede utilizar comodines basados en fecha al crear los siguientes elementos de informes:

* Filtros
* Indicadores personalizados
* Vistas al añadir reglas para columnas

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p>Editar el acceso a los informes, paneles y calendarios para editar los elementos de un informe</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Administración de permisos de un informe para editar los elementos de un informe</p> <p>Administrar permisos a una vista o filtro para editarlos</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Requisitos previos

Debe crear un informe para poder agregarle variables comodín.

Para obtener información sobre cómo crear un informe, consulte [Creación de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Pasos a seguir

Para insertar un comodín basado en la fecha en un informe:

1. Vaya a un informe en el que desee insertar un comodín basado en fecha.
1. Clic **Acciones de informe**, entonces **Editar**.

1. Haga clic en **Filtros** pestaña.
1. Clic **Agregar una regla de filtro**.
1. Empiece a escribir el nombre del campo por el que desea filtrar.\
   Debe escribir campos que hagan referencia a una fecha.
1. Seleccionar **Igual** en el menú desplegable de la variable de filtro.

   >[!TIP]
   >
   >Siempre debe seleccionar la variable **Igual** variable de filtro al trabajar con caracteres comodín en Adobe Workfront.

1. En el **Empiece a escribir el nombre...** cuadro, escriba: `$$TODAY` si desea mostrar información sobre algo que ocurre el mismo día en que se ejecuta el informe.

   O

   Tipo `$$NOW` si desea mostrar información acerca de algo que ocurre en la misma fecha y hora en que se ejecuta el informe.

   Esta fecha siempre es diferente, ya que cambia con la fecha en la que un usuario ve realmente el informe. por lo tanto, la información del informe es diferente día a día.

1. (Opcional) Si desea mostrar información que se produce dentro de un periodo de tiempo después de la fecha en la que se ejecuta el informe, escriba `$$TODAY+1w` para mostrar información en la semana siguiente, o `$$TODAY+2m` para mostrar información en los próximos dos meses. También puede indicar marcos de tiempo para trimestres, horas, días o años.
1. (Opcional) Si desea mostrar información sobre algo que se produjo dentro de un periodo de tiempo antes de la fecha en la que se ejecuta el informe, escriba `$$TODAY-1w` para mostrar información de la semana anterior, o `$$TODAY-2m` para mostrar información de los dos meses anteriores. También puede indicar marcos de tiempo para trimestres, horas, días o años.

   Para obtener una lista completa de los atributos, calificadores y operadores que puede utilizar en los comodines basados en fecha, consulte el artículo [Variables de filtro comodín](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/video-date-based-wildcard-in-task-filter-350x81.png)

1. Clic **Guardar + Cerrar**.

## Información adicional

Consulte también:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Variables de filtro comodín](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Creación o edición de filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Agregar una solicitud a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Uso de formato condicional en vistas](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
