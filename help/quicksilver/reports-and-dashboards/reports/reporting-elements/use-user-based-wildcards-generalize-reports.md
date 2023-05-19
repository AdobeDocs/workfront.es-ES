---
product-area: reporting
navigation-topic: reporting-elements
title: Utilice comodines basados en usuarios para generalizar informes
description: Puede generalizar un informe utilizando caracteres comodín en lugar de información específica al crear determinados elementos de informe.
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# Utilice comodines basados en usuarios para generalizar informes

Puede generalizar un informe utilizando caracteres comodín en lugar de información específica al crear determinados elementos de informe. Por ejemplo, si desea crear un informe que muestre las tareas asignadas a un usuario específico, puede utilizar el nombre del usuario en el campo Asignado a del filtro. Sin embargo, si desea crear un informe que muestre las tareas asignadas al usuario que ha iniciado sesión, independientemente de quién sea ese usuario, puede utilizar un comodín que indique que cuando alguien ve el informe, muestra información que solo le pertenece a él. De este modo, el informe se genera una vez, pero como se utiliza un comodín en el filtro, produce resultados diferentes cada vez que otro usuario lo lee.

Puede utilizar comodines basados en usuarios al crear los siguientes elementos de informes:

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

Debe crear un informe para poder agregarle una variable comodín.

Para obtener instrucciones sobre la creación de informes, consulte [Creación de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Pasos a seguir

Para insertar un comodín basado en usuario en un informe:

1. Vaya a un informe en el que desee insertar un comodín basado en el usuario.
1. Clic **Acciones de informe**, entonces **Editar**.

1. Haga clic en **Filtros** pestaña.
1. Clic **Agregar una regla de filtro**.
1. Empiece a escribir el nombre del campo por el que desea filtrar.\
   Debe escribir campos que hagan referencia al objeto de usuario o información sobre los usuarios.
1. Seleccionar **Igual** en el menú desplegable de la variable de filtro.

   >[!TIP]
   >
   >Siempre debe seleccionar la variable **Igual** variable de filtro al trabajar con caracteres comodín en Adobe Workfront.

1. En el **Empiece a escribir el nombre...** cuadro, escriba: `$$USER.ID` o `$$USER.name` si desea que el informe muestre información sobre el usuario que inicia sesión, basada en su nombre. Puede insertar otros caracteres comodín que hagan referencia al grupo, equipo, compañía u otra información del usuario que ha iniciado sesión.

   Para obtener una lista completa de los comodines basados en usuarios, consulte [Variables de filtro comodín](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/user-based-wildcard-in-project-filter-350x74.png)

1. Clic **Guardar + Cerrar**.

## Información adicional

Consulte también:

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [Variables de filtro comodín](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Creación o edición de filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Agregar una solicitud a un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Uso de formato condicional en vistas](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
