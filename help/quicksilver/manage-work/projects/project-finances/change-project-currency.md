---
product-area: projects
navigation-topic: financials
title: Cambiar la moneda del proyecto
description: Como administrador de proyectos, puede configurar un proyecto para que utilice una moneda distinta de la predeterminada para su sistema Adobe Workfront. Esto le permite mostrar la información financiera del proyecto en la moneda deseada al calcular los costes laborales y los ingresos.
author: Alina
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# Cambiar la moneda del proyecto

Como administrador de proyectos, puede configurar un proyecto para que utilice una moneda distinta de la predeterminada para su sistema Adobe Workfront. Esto le permite mostrar la información financiera del proyecto en la moneda deseada al calcular los costes laborales y los ingresos.

Para poder utilizar monedas alternativas, como se describe en esta sección, el administrador de Workfront debe habilitar y configurar primero varias monedas, tal como se describe en el artículo [Configurar tipos de cambio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

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
   <td> <p>Editar acceso a Proyectos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones al cambiar la moneda de un proyecto en Workfront

* No puede cambiar la moneda de un proyecto si hay información financiera en él.
* Las tasas se utilizan para los costos laborales; Los cálculos de ingresos y se utilizan en el futuro para la generación de informes.
* Si no especifica una moneda diferente para un proyecto, Workfront supone que la moneda del proyecto es la moneda predeterminada del sistema. Para obtener información sobre la moneda predeterminada de nivel de sistema, consulte [Configurar tipos de cambio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* De forma predeterminada, todos los usuarios de licencias completas tienen acceso para ver monedas y tipos de cambio. El administrador de Workfront debe conceder acceso administrativo adicional para **Tipos de cambio** para permitir a los usuarios establecer tasas específicas en los proyectos.
* Los tipos de cambio en Workfront no son dinámicos. El valor lo establece un administrador y debe actualizarse cuando se produzcan cambios en los tipos de cambio.
* Cuando crea un informe para reflejar la moneda de un proyecto, de forma predeterminada todos los informes se agrupan por la moneda predeterminada del proyecto. Si crea un informe con varios proyectos que tienen diferentes tipos de cambio, cualquier agrupación aplicada al proyecto reflejará la tasa de cambio predeterminada a nivel del sistema. Para obtener más información, consulte el artículo [Crear informes de datos financieros con tipos de cambio únicos](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

## Configuración de la moneda de un proyecto

1. Vaya al proyecto donde desee cambiar la moneda predeterminada.

   >[!TIP]
   >
   >Asegúrese de que el proyecto no tenga ya información financiera. Por ejemplo, asegúrese de que no haya costos planificados o reales asociados al proyecto.

1. Haga clic en **Detalles del proyecto** en el panel izquierdo y, a continuación, vaya a la **Finanzas** .
1. Haga clic en **Agregar** en el **Moneda** y seleccione la moneda que desea utilizar como moneda predeterminada para el proyecto. Se muestran todas las monedas que el administrador de Workfront ha establecido para la instancia de Workfront.

   ![](assets/currency-on-project-expanded-nwe.png)

1. (Condicional) Si selecciona una moneda que no sea la predeterminada establecida para el sistema Workfront, especifique la tasa para la moneda seleccionada, ya que está relacionada con la moneda que se ha establecido como moneda base en el sistema.
1. Haga clic en **Guardar cambios**.
