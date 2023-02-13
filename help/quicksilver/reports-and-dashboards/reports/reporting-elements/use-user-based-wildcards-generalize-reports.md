---
product-area: reporting
navigation-topic: reporting-elements
title: Utilice caracteres comodín basados en el usuario para generalizar informes
description: Puede generalizar un informe utilizando caracteres comodín en lugar de información específica al crear ciertos elementos de informes.
author: Lisa
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# Utilice caracteres comodín basados en el usuario para generalizar informes

Puede generalizar un informe utilizando caracteres comodín en lugar de información específica al crear ciertos elementos de informes. Por ejemplo, si desea crear un informe que muestre las tareas asignadas a un usuario específico, puede utilizar el nombre del usuario en el campo Asignado a del filtro. Sin embargo, si desea crear un informe que muestre las tareas asignadas al usuario que ha iniciado sesión, independientemente de quién sea, puede utilizar un comodín que indique que, cuando alguien vea el informe, muestra la información que pertenece únicamente a él. De este modo, el informe se crea una vez, pero como se utiliza un comodín en el filtro, produce resultados diferentes cada vez que alguien lo lee.

Los comodines basados en el usuario se pueden usar al crear los siguientes elementos de informes:

* Filtros
* Mensajes personalizados
* Vistas al agregar reglas para columnas

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan de Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Editar acceso a filtros, vistas y grupos</p> <p>Editar acceso a informes, tableros y calendarios para editar elementos de informes en un informe</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Administrar permisos en un informe para editar elementos de informes en un informe</p> <p>Administrar permisos para una vista o filtro para editarlos</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Debe crear un informe para poder agregar una variable comodín.

Para obtener instrucciones sobre la creación de informes, consulte [Crear un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Pasos prácticos

Para insertar un comodín basado en el usuario en un informe:

1. Vaya a un informe para el que desee insertar un comodín basado en el usuario.
1. Haga clic en **Acciones de informe**, luego **Editar**.

1. Haga clic en el **Filtros** pestaña .
1. Haga clic en **Agregar una regla de filtro**.
1. Empiece a escribir el nombre del campo por el que desea filtrar.\
   Debe escribir campos que hagan referencia al objeto de usuario o información sobre los usuarios.
1. Select **Igual** en el menú desplegable para la variable de filtro.

   >[!TIP]
   >
   >Siempre debe seleccionar la variable **Igual** cuando se trabaja con caracteres comodín en Adobe Workfront.

1. En el **Empiece a escribir el nombre ...** cuadro, tipo: `$$USER.ID` o `$$USER.name` si desea que el informe muestre información sobre el usuario que inicia sesión en función de su nombre. Puede insertar otros caracteres comodín que hagan referencia al grupo, el equipo, la empresa u otra información del usuario que ha iniciado sesión.

   Para obtener una lista completa de los comodines basados en el usuario, consulte [Variables de filtro comodín](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/user-based-wildcard-in-project-filter-350x74.png)

1. Haga clic en **Guardar + Cerrar**.

## Información adicional

Consulte también:

* [Programa básico de creación de informes](https://one.workfront.com/s/basic-report-creation-program)
* [Variables de filtro comodín](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Crear o editar filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Agregar solicitudes a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Utilizar el formato condicional en las vistas](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
