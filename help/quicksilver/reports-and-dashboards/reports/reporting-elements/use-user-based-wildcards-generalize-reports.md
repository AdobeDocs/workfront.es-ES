---
product-area: reporting
navigation-topic: reporting-elements
title: Usar comodines basados en el usuario para generalizar informes
description: Puede generalizar un informe utilizando comodines en lugar de información específica al crear determinados elementos de informes.
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 96%

---

# Usar comodines basados en el usuario para generalizar informes

<!-- Audited: 11/2024 -->

Puede generalizar un informe utilizando comodines en lugar de información específica al crear determinados elementos de informes. Por ejemplo, si desea crear un informe que muestre las tareas asignadas a un usuario específico, puede utilizar el nombre del usuario en el campo Asignado a del filtro. Sin embargo, si desea crear un informe que muestre las tareas asignadas al usuario que ha iniciado sesión, independientemente de quién sea ese usuario, puede utilizar un comodín que indique que cuando alguien vea el informe, muestre información que sólo le concierna a él. De este modo, el informe se genera una vez, pero como se utiliza un comodín en el filtro, produce resultados diferentes cada vez que otro usuario lo lee.

Puede utilizar comodines basados en usuarios al crear los siguientes elementos de informes:

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

Debe crear un informe para poder añadirle una variable comodín.

Para obtener instrucciones sobre cómo crear informes, consulte [Crear un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Pasos a seguir

Para insertar un comodín basado en el usuario en un informe:

1. Vaya a un informe para el que desea insertar un comodín basado en el usuario.
1. Haga clic en **Acciones de informe** y, a continuación, en **Editar**.

1. Haga clic en la pestaña **Filtros**.
1. Haga clic en **Añadir una regla de filtro**.
1. Empiece a escribir el nombre del campo por el que desea filtrar.\
   Debe escribir campos que hagan referencia al objeto de usuario o información sobre los usuarios.
1. Seleccione **Equal** en el menú desplegable de la variable de filtro.

   >[!TIP]
   >
   >Siempre debe seleccionar la variable de filtro **Equal** al trabajar con comodines en Adobe Workfront.

1. En el cuadro **Empiece a escribir el nombre...**, escriba: `$$USER.ID` o `$$USER.name` si desea que el informe muestre información sobre el usuario que inicia sesión, basada en su nombre. Puede insertar otros caracteres comodín que hagan referencia al grupo, equipo, compañía u otra información del usuario que ha iniciado sesión.

   Para obtener una lista completa de los comodines basados en usuarios, consulte [Información general sobre las variables de filtro comodín](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Haga clic en **Guardar + Cerrar**.

## Más información

Consulte también lo siguiente:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Información general sobre las variables del filtro comodín](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Crear o editar filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Información general de los filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Añadir una solicitud a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Usar formato condicional en vistas](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
